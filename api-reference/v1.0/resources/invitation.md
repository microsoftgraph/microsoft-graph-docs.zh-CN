<span data-ttu-id="df9de-p108">创建为邀请创建进程组成部分的用户。只读</span><span class="sxs-lookup"><span data-stu-id="df9de-p108">The user created as part of the invitation creation. Read-Only</span></span>|创建为邀请创建进程组成部分的用户。只读|

## <span data-ttu-id="df9de-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df9de-165">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="df9de-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df9de-166">Here is a JSON representation of the resource</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.invitations" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",

  "invitedUser": [{"@odata.type": "microsoft.graph.user"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
