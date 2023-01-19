## Cross Site Scripting Automation in Burp Suite 
#### <em>Extentions: AutoRepeater and Logger++</em>


## AutoRepeater Replacement Configuration
 
1) Replace All Params Value with Canary:

    ```
    Type: Request Param Value
    Match: .*
    Replace: /1'"(){}<Charlie>:;/
    Witch: Replace All
    Regex Match: Enabled
    ```
2) You can Add lot of Replecment Payloads AutoRepeater ;)

## Logger++ Filter For AutoRepeater Response Charlie Reflection

    Response.Body CONTAINS "<Charlie>"
    

<h4><em>Happy Hunting ;) </em><h4>
