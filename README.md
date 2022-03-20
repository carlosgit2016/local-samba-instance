## Sambda

Samba is an Open Source / Free Software suite that has, since 1992, provided file and print services to all manner of SMB/CIFS clients, including the numerous versions of Microsoft Windows operating systems. Samba is freely available under the GNU General Public License.

The Samba project is a member of the Software Freedom Conservancy.

### Setting up a shared FS for guests
- Execute docker-compose up -d in the root level

It will spin up a samba instance with a simple shared location named `shared`, for accessing using a Windows machine map a new location using `NET USE M: \\nameserver\shared` where `M` is the mapped letter and `nameserver` is the name of the host running this container in the network or local place