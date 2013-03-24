Nginx Reverse Proxy access controlled by Apigee Gateway

This is an Ngina reverse proxy configuration that uses a Lua script to check
an Apigee Gateway URL before allowing the proxy url to be accessed.

This will allow a local Nginx proxy to still use Apigee key management, rate
limiting, and analytics without having the traffic proxied through the Apigee
gateway. Useful in situations where one wants to control internal API traffic
using Apigee's cloud services.

Requirements:

OpenResty
LuaSocket
