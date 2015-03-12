.. _manual-configuration-options-label:

Full configuration options
==========================


.. code-block:: erlang

    [{carotene, [
        %%
        % Port Carotene listens to
        %%
        {port, 8081}
    
        %%
        % Enable presence
        %%
    
        %, {presence, true}
    
        %%
        % Restrict HTTP API access to an IP
        %%
    
        %, {restrict_api_access_to, {127, 0, 0, 1}}
    
        %%
        % URL of your backend, where messages from subscribed_channels
        % will be POSTed
        %%
    
        %, {subscribe_url, "http://myserver.com/carotene-consume"}
        %, {subscribed_channels, ["chat"]}
    
        %%
        % Authentication URL
        %%
    
        %, {authenticate_url, "http://myserver.com/carotene-auth"}
    
    
        %%
        % Authorization levels
        %%
    
        %, {publish_authorization, [
        %    {level, ask},
        %    {authorization_url, "http://myserver.com/authorize-publish-carotene"}
        %]}
        %, {subscribe_authorization, [
        %    {level, anonymous}
        %]}
    
        %%
        % Back broker, where messages are republished
        %%
    
        %, {broker, redis}
    
        %%
        % Nodes in cluster, including this one
        %%
    
        %, {nodes_in_cluster, ['carotene@localhost', 'carotene2@localhost']}
    
        %%
        % SSL configuration options. Certificates and key locations
        %%
    
        %, {ssl, [
        %    {cacertfile, "/etc/cacertfile.crt"},
        %    {certfile, "/etc/server.crt"},
        %    {keyfile, "/etc/server.key"}
        %    ]}
    ]}].

