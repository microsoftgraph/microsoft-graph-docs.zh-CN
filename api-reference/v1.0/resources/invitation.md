# <a name="invitation-manager"></a><span data-ttu-id="1419f-101">邀请管理器</span><span class="sxs-lookup"><span data-stu-id="1419f-101">invitation manager</span></span>

<span data-ttu-id="1419f-102">使用邀请管理器来创建一个邀请，以将外部用户添加到组织。</span><span class="sxs-lookup"><span data-stu-id="1419f-102">Use the invitation manager to create an invite, in order to add an external user to the organization.</span></span> 

<span data-ttu-id="1419f-103">邀请进程使用以下流程：</span><span class="sxs-lookup"><span data-stu-id="1419f-103">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="1419f-104">创建邀请</span><span class="sxs-lookup"><span data-stu-id="1419f-104">An invitation is created</span></span>
* <span data-ttu-id="1419f-105">将邀请发送至邀请的用户（包含邀请链接）</span><span class="sxs-lookup"><span data-stu-id="1419f-105">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="1419f-106">邀请的用户单击邀请链接、登录并兑现邀请和创建用户实体表示邀请的用户完成操作</span><span class="sxs-lookup"><span data-stu-id="1419f-106">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="1419f-107">兑现完成后，将用户重定向至指定页面</span><span class="sxs-lookup"><span data-stu-id="1419f-107">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="1419f-p101">创建邀请会在响应中返回兑现 URL (*inviteRedeemUrl*)。通过将 *sendInvitationMessage* 设置为 true，创建邀请 API 可以自动向邀请的用户发送包含兑现 URL 的电子邮件。还可以自定义要发送至邀请的用户的邮件。反之，如果想要通过一些其他的方法发送兑现 URL，则可以将 *sendInvitationMessage* 设置为 false，然后使用响应中的兑现 URL 创建自己的通信。目前没有可以执行兑现进程的 API。邀请的用户必须单击在上述步骤中的通信中发送的 *inviteRedeemUrl* 链接，并在浏览器中进行交互式兑现流程。完成后，邀请的用户即成为组织中的外部用户。</span><span class="sxs-lookup"><span data-stu-id="1419f-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>


## <a name="methods"></a><span data-ttu-id="1419f-115">方法</span><span class="sxs-lookup"><span data-stu-id="1419f-115">Methods</span></span>
| <span data-ttu-id="1419f-116">方法</span><span class="sxs-lookup"><span data-stu-id="1419f-116">Method</span></span>       | <span data-ttu-id="1419f-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="1419f-117">Return Type</span></span>  |<span data-ttu-id="1419f-118">说明</span><span class="sxs-lookup"><span data-stu-id="1419f-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1419f-119">创建邀请</span><span class="sxs-lookup"><span data-stu-id="1419f-119">Create invitation</span></span>](../api/invitation_post.md) | <span data-ttu-id="1419f-120">邀请</span><span class="sxs-lookup"><span data-stu-id="1419f-120">invitation</span></span> | <span data-ttu-id="1419f-121">写入 invitation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1419f-121">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1419f-122">属性</span><span class="sxs-lookup"><span data-stu-id="1419f-122">Properties</span></span>
| <span data-ttu-id="1419f-123">属性</span><span class="sxs-lookup"><span data-stu-id="1419f-123">Property</span></span>     | <span data-ttu-id="1419f-124">类型</span><span class="sxs-lookup"><span data-stu-id="1419f-124">Type</span></span>   |<span data-ttu-id="1419f-125">说明</span><span class="sxs-lookup"><span data-stu-id="1419f-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1419f-126">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="1419f-126">invitedUserDisplayName</span></span>|<span data-ttu-id="1419f-127">String</span><span class="sxs-lookup"><span data-stu-id="1419f-127">String</span></span>|<span data-ttu-id="1419f-128">被邀请的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1419f-128">The display name of the user being invited.</span></span>|
|<span data-ttu-id="1419f-129">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="1419f-129">invitedUserEmailAddress</span></span>|<span data-ttu-id="1419f-130">String</span><span class="sxs-lookup"><span data-stu-id="1419f-130">String</span></span>|<span data-ttu-id="1419f-p102">被邀请的用户的电子邮件地址。必填。</span><span class="sxs-lookup"><span data-stu-id="1419f-p102">The email address of the user being invited. Required.</span></span>|
|<span data-ttu-id="1419f-133">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="1419f-133">invitedUserMessageInfo</span></span>|[<span data-ttu-id="1419f-134">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="1419f-134">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="1419f-135">要发送至邀请用户的邮件的其他配置，其中包括自定义邮件文本、语言和抄送收件人列表。</span><span class="sxs-lookup"><span data-stu-id="1419f-135">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="1419f-136">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="1419f-136">sendInvitationMessage</span></span>|<span data-ttu-id="1419f-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="1419f-137">Boolean</span></span>|<span data-ttu-id="1419f-p103">指示电子邮件是否应发送至邀请的用户。默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="1419f-p103">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="1419f-140">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="1419f-140">inviteRedirectUrl</span></span>|<span data-ttu-id="1419f-141">String</span><span class="sxs-lookup"><span data-stu-id="1419f-141">String</span></span>|<span data-ttu-id="1419f-p104">兑现邀请后，用户应被重定向至的 URL。必填。</span><span class="sxs-lookup"><span data-stu-id="1419f-p104">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="1419f-144">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="1419f-144">inviteRedeemUrl</span></span>|<span data-ttu-id="1419f-145">String</span><span class="sxs-lookup"><span data-stu-id="1419f-145">String</span></span>|<span data-ttu-id="1419f-p105">用户可用于兑现邀请的 URL。只读</span><span class="sxs-lookup"><span data-stu-id="1419f-p105">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="1419f-148">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="1419f-148">invitedUserType</span></span>|<span data-ttu-id="1419f-149">String</span><span class="sxs-lookup"><span data-stu-id="1419f-149">String</span></span>|<span data-ttu-id="1419f-150">被邀请的用户的 userType。</span><span class="sxs-lookup"><span data-stu-id="1419f-150">The userType of the user being invited.</span></span> <span data-ttu-id="1419f-151">默认情况下，此值为“来宾”。</span><span class="sxs-lookup"><span data-stu-id="1419f-151">By default, this is Guest.</span></span> <span data-ttu-id="1419f-152">如果你是公司管理员，则可以以“成员”身份进行邀请。</span><span class="sxs-lookup"><span data-stu-id="1419f-152">You can invite as Member if you are a company administrator.</span></span> |
|<span data-ttu-id="1419f-153">状态</span><span class="sxs-lookup"><span data-stu-id="1419f-153">status</span></span>|<span data-ttu-id="1419f-154">String</span><span class="sxs-lookup"><span data-stu-id="1419f-154">String</span></span>|<span data-ttu-id="1419f-p107">邀请的状态。可能的值：PendingAcceptance、Completed、InProgress 和 Error</span><span class="sxs-lookup"><span data-stu-id="1419f-p107">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="1419f-157">关系</span><span class="sxs-lookup"><span data-stu-id="1419f-157">Relationships</span></span>
| <span data-ttu-id="1419f-158">关系</span><span class="sxs-lookup"><span data-stu-id="1419f-158">Relationship</span></span> | <span data-ttu-id="1419f-159">类型</span><span class="sxs-lookup"><span data-stu-id="1419f-159">Type</span></span>   |<span data-ttu-id="1419f-160">说明</span><span class="sxs-lookup"><span data-stu-id="1419f-160">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1419f-161">invitedUser</span><span class="sxs-lookup"><span data-stu-id="1419f-161">invitedUser</span></span>|[<span data-ttu-id="1419f-162">用户</span><span class="sxs-lookup"><span data-stu-id="1419f-162">User</span></span>](user.md)|<span data-ttu-id="1419f-p108">创建为邀请创建进程组成部分的用户。只读</span><span class="sxs-lookup"><span data-stu-id="1419f-p108">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1419f-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1419f-165">JSON representation</span></span>
<span data-ttu-id="1419f-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1419f-166">Here is a JSON representation of the resource</span></span>

<!-- { "blockType": "resource", "baseType": "microsoft.graph.entity", "@odata.type": "microsoft.graph.invitation" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",
  "invitedUser": {"@odata.type": "microsoft.graph.user"},
  "invitedUserType": "string"
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
