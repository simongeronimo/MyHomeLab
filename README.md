My objective was to have a VPN so I can remote access to my laptop at home from any other available computer.

I tried to do it on my own with what I've learned but I got into some weird issues not letting me access the wg0.conf file in the correct path inside the pod.

Then I changed my deployment file to match the one on this post https://medium.com/@s.hameedakmal/wireguard-vpn-in-a-kubernetes-cluster-e306fdc69731. Then it looked like it was working fine I was able to get to the peer user config files and run the command wg on the pod and see the list of peers.

When I tried to apply that peer config file on my laptop, it looked like I joined a vpn but I wasn't able to access the internet.

When I tried to apply it to the computer I was running the cluster, it took down all my cloudflare tunnels and I had to restart all the cloudflare pods.

I wasn't able to see the last handshake info inside the pod as the post suggested with any of my tries.

Changing the approach to tackle this problem wiith a cloud-based solution.
