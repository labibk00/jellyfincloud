# jellyfincloud  *Work in Progress*
## Intro
Idea behind this repo is to layout a basic architecture for setting up Jellyfin + Sonarr + Radarr in the cloud with very low-powered VMs and cheap cloud storage. This example uses Oracle Free Tier VMs + Google Drive.

## High-Level Diagram
![abcd (1)](https://github.com/labibk00/jellyfincloud/assets/73773981/3e920d1e-43bb-46d2-9b83-06307f4652b8)

*Note: This diagram is not meant to be perfect; rather it serves as a nice logical overview for when you're setting things up and get overwhelmed (I sure did!).*

VM1 exists for everything other than hosting Jellyfin, and VM2 exists for just that. The reason behind this is write operations on the remotely mounted Google Drive via rclone can slow the whole system down.
