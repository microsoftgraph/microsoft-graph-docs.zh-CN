---
title: 邀请资源类型
description: 表示用于将外部用户添加到组织的邀请。
localization_priority: Priority
author: Sammak
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ff977732b4d0894767f06ccfcf03451a8cc77f61
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941363"
---
# <a name="invitation-resource-type"></a><span data-ttu-id="54e05-103">邀请资源类型</span><span class="sxs-lookup"><span data-stu-id="54e05-103">invitation resource type</span></span>

<span data-ttu-id="54e05-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54e05-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="54e05-105">表示用于将外部用户添加到组织的邀请。</span><span class="sxs-lookup"><span data-stu-id="54e05-105">Represents an invitation that is used to add external users to an organization.</span></span> 

<span data-ttu-id="54e05-106">邀请进程使用以下流程：</span><span class="sxs-lookup"><span data-stu-id="54e05-106">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="54e05-107">创建邀请</span><span class="sxs-lookup"><span data-stu-id="54e05-107">An invitation is created</span></span>
* <span data-ttu-id="54e05-108">将邀请发送至邀请的用户（包含邀请链接）</span><span class="sxs-lookup"><span data-stu-id="54e05-108">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="54e05-109">邀请的用户单击邀请链接、登录并兑现邀请和创建用户实体表示邀请的用户完成操作</span><span class="sxs-lookup"><span data-stu-id="54e05-109">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="54e05-110">兑现完成后，将用户重定向至指定页面</span><span class="sxs-lookup"><span data-stu-id="54e05-110">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="54e05-p101">创建邀请会在响应中返回兑现 URL (*inviteRedeemUrl*)。通过将 *sendInvitationMessage* 设置为 true，创建邀请 API 可以自动向邀请的用户发送包含兑现 URL 的电子邮件。还可以自定义要发送至邀请的用户的邮件。反之，如果想要通过一些其他的方法发送兑现 URL，则可以将 *sendInvitationMessage* 设置为 false，然后使用响应中的兑现 URL 创建自己的通信。目前没有可以执行兑现进程的 API。邀请的用户必须单击在上述步骤中的通信中发送的 *inviteRedeemUrl* 链接，并在浏览器中进行交互式兑现流程。完成后，邀请的用户即成为组织中的外部用户。</span><span class="sxs-lookup"><span data-stu-id="54e05-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>


## <a name="methods"></a><span data-ttu-id="54e05-118">方法</span><span class="sxs-lookup"><span data-stu-id="54e05-118">Methods</span></span>
| <span data-ttu-id="54e05-119">方法</span><span class="sxs-lookup"><span data-stu-id="54e05-119">Method</span></span>       | <span data-ttu-id="54e05-120">返回类型</span><span class="sxs-lookup"><span data-stu-id="54e05-120">Return Type</span></span>  |<span data-ttu-id="54e05-121">说明</span><span class="sxs-lookup"><span data-stu-id="54e05-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="54e05-122">创建邀请</span><span class="sxs-lookup"><span data-stu-id="54e05-122">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="54e05-123">邀请</span><span class="sxs-lookup"><span data-stu-id="54e05-123">invitation</span></span> | <span data-ttu-id="54e05-124">写入 invitation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="54e05-124">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="54e05-125">属性</span><span class="sxs-lookup"><span data-stu-id="54e05-125">Properties</span></span>
| <span data-ttu-id="54e05-126">属性</span><span class="sxs-lookup"><span data-stu-id="54e05-126">Property</span></span>     | <span data-ttu-id="54e05-127">类型</span><span class="sxs-lookup"><span data-stu-id="54e05-127">Type</span></span>   |<span data-ttu-id="54e05-128">说明</span><span class="sxs-lookup"><span data-stu-id="54e05-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54e05-129">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="54e05-129">invitedUserDisplayName</span></span>|<span data-ttu-id="54e05-130">String</span><span class="sxs-lookup"><span data-stu-id="54e05-130">String</span></span>|<span data-ttu-id="54e05-131">被邀请的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="54e05-131">The display name of the user being invited.</span></span>|
|<span data-ttu-id="54e05-132">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="54e05-132">invitedUserEmailAddress</span></span>|<span data-ttu-id="54e05-133">String</span><span class="sxs-lookup"><span data-stu-id="54e05-133">String</span></span>|<span data-ttu-id="54e05-134">被邀请的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="54e05-134">The email address of the user being invited.</span></span> <span data-ttu-id="54e05-135">必需。</span><span class="sxs-lookup"><span data-stu-id="54e05-135">Required.</span></span> <span data-ttu-id="54e05-136">电子邮件地址中不允许使用以下特殊字符：</span><span class="sxs-lookup"><span data-stu-id="54e05-136">The following special characters are not permitted in the email address:</span></span><br><ul><li><span data-ttu-id="54e05-137">波形符 (~)</span><span class="sxs-lookup"><span data-stu-id="54e05-137">Tilde (~)</span></span></li><li><span data-ttu-id="54e05-138">感叹号 (`!`)</span><span class="sxs-lookup"><span data-stu-id="54e05-138">Exclamation point (`!`)</span></span></li><li><span data-ttu-id="54e05-139">井号 (`#`)</span><span class="sxs-lookup"><span data-stu-id="54e05-139">Number sign (`#`)</span></span></li><li><span data-ttu-id="54e05-140">美元符号 (`$`)</span><span class="sxs-lookup"><span data-stu-id="54e05-140">Dollar sign (`$`)</span></span></li><li><span data-ttu-id="54e05-141">百分号 (`%`)</span><span class="sxs-lookup"><span data-stu-id="54e05-141">Percent (`%`)</span></span></li><li><span data-ttu-id="54e05-142">扬抑符 (`^`)</span><span class="sxs-lookup"><span data-stu-id="54e05-142">Circumflex (`^`)</span></span></li><li><span data-ttu-id="54e05-143">与号 (`&`)</span><span class="sxs-lookup"><span data-stu-id="54e05-143">Ampersand (`&`)</span></span></li><li><span data-ttu-id="54e05-144">星号 (`*`)</span><span class="sxs-lookup"><span data-stu-id="54e05-144">Asterisk (`*`)</span></span></li><li><span data-ttu-id="54e05-145">圆括号 (`( )`)</span><span class="sxs-lookup"><span data-stu-id="54e05-145">Parentheses (`( )`)</span></span></li><li><span data-ttu-id="54e05-146">加号 (`+`)</span><span class="sxs-lookup"><span data-stu-id="54e05-146">Plus sign (`+`)</span></span></li><li><span data-ttu-id="54e05-147">等号 (`=`)</span><span class="sxs-lookup"><span data-stu-id="54e05-147">Equal sign (`=`)</span></span></li><li><span data-ttu-id="54e05-148">方括号 (`[ ]`)</span><span class="sxs-lookup"><span data-stu-id="54e05-148">Brackets (`[ ]`)</span></span></li><li><span data-ttu-id="54e05-149">大括号 (`{ }`)</span><span class="sxs-lookup"><span data-stu-id="54e05-149">Braces (`{ }`)</span></span></li><li><span data-ttu-id="54e05-150">反斜杠 (`\`)</span><span class="sxs-lookup"><span data-stu-id="54e05-150">Backslash (`\`)</span></span></li><li><span data-ttu-id="54e05-151">斜杠符号 (`/`)</span><span class="sxs-lookup"><span data-stu-id="54e05-151">Slash mark (`/`)</span></span></li><li><span data-ttu-id="54e05-152">竖线 (`\|`)</span><span class="sxs-lookup"><span data-stu-id="54e05-152">Pipe (`\|`)</span></span></li><li><span data-ttu-id="54e05-153">分号 (`;`)</span><span class="sxs-lookup"><span data-stu-id="54e05-153">Semicolon (`;`)</span></span></li><li><span data-ttu-id="54e05-154">冒号 (`:`)</span><span class="sxs-lookup"><span data-stu-id="54e05-154">Colon (`:`)</span></span></li><li><span data-ttu-id="54e05-155">引号 (`"`)</span><span class="sxs-lookup"><span data-stu-id="54e05-155">Quotation marks (`"`)</span></span></li><li><span data-ttu-id="54e05-156">尖括号 (`< >`)</span><span class="sxs-lookup"><span data-stu-id="54e05-156">Angle brackets (`< >`)</span></span></li><li><span data-ttu-id="54e05-157">问号 (`?`)</span><span class="sxs-lookup"><span data-stu-id="54e05-157">Question mark (`?`)</span></span></li><li><span data-ttu-id="54e05-158">逗号 (`,`)</span><span class="sxs-lookup"><span data-stu-id="54e05-158">Comma (`,`)</span></span></li></ul><br><span data-ttu-id="54e05-159">但是，存在下列例外情况：</span><span class="sxs-lookup"><span data-stu-id="54e05-159">However, the following exceptions apply:</span></span><br><ul><li><span data-ttu-id="54e05-160">允许在用户名中的任何位置使用句点 (`.`) 或连字符 (`-`)，但名称的开头或结尾除外。</span><span class="sxs-lookup"><span data-stu-id="54e05-160">A period (`.`) or a hyphen (`-`) is permitted anywhere in the user name, except at the beginning or end of the name.</span></span></li><li><span data-ttu-id="54e05-161">允许在用户名中的任何位置使用下划线 (`_`)。</span><span class="sxs-lookup"><span data-stu-id="54e05-161">An underscore (`_`) is permitted anywhere in the user name.</span></span> <span data-ttu-id="54e05-162">这包括名称的开头或结尾。</span><span class="sxs-lookup"><span data-stu-id="54e05-162">This includes at the beginning or end of the name.</span></span></li></ul>|
|<span data-ttu-id="54e05-163">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="54e05-163">invitedUserMessageInfo</span></span>|[<span data-ttu-id="54e05-164">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="54e05-164">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="54e05-165">要发送至邀请用户的邮件的其他配置，其中包括自定义邮件文本、语言和抄送收件人列表。</span><span class="sxs-lookup"><span data-stu-id="54e05-165">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="54e05-166">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="54e05-166">sendInvitationMessage</span></span>|<span data-ttu-id="54e05-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="54e05-167">Boolean</span></span>|<span data-ttu-id="54e05-p104">指示电子邮件是否应发送至邀请的用户。默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="54e05-p104">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="54e05-170">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="54e05-170">inviteRedirectUrl</span></span>|<span data-ttu-id="54e05-171">String</span><span class="sxs-lookup"><span data-stu-id="54e05-171">String</span></span>|<span data-ttu-id="54e05-p105">用户在兑现邀请后会被重定向至该 URL。必填。</span><span class="sxs-lookup"><span data-stu-id="54e05-p105">The URL the user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="54e05-174">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="54e05-174">inviteRedeemUrl</span></span>|<span data-ttu-id="54e05-175">String</span><span class="sxs-lookup"><span data-stu-id="54e05-175">String</span></span>|<span data-ttu-id="54e05-p106">用户用于兑现邀请的 URL。只读</span><span class="sxs-lookup"><span data-stu-id="54e05-p106">The URL the user can use to redeem their invitation. Read-only</span></span>|<span data-ttu-id="54e05-178">.</span><span class="sxs-lookup"><span data-stu-id="54e05-178">.</span></span>
|<span data-ttu-id="54e05-179">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="54e05-179">invitedUserType</span></span>|<span data-ttu-id="54e05-180">String</span><span class="sxs-lookup"><span data-stu-id="54e05-180">String</span></span>|<span data-ttu-id="54e05-181">被邀请的用户的 userType。</span><span class="sxs-lookup"><span data-stu-id="54e05-181">The userType of the user being invited.</span></span> <span data-ttu-id="54e05-182">默认情况下，此操作为 `Guest`。</span><span class="sxs-lookup"><span data-stu-id="54e05-182">By default, this is `Guest`.</span></span> <span data-ttu-id="54e05-183">如果您是公司管理员， `Member` 邀请作为管理员。</span><span class="sxs-lookup"><span data-stu-id="54e05-183">You can invite as `Member` if you are a company administrator.</span></span> |
|<span data-ttu-id="54e05-184">状态</span><span class="sxs-lookup"><span data-stu-id="54e05-184">status</span></span>|<span data-ttu-id="54e05-185">String</span><span class="sxs-lookup"><span data-stu-id="54e05-185">String</span></span>|<span data-ttu-id="54e05-186">邀请的状态。</span><span class="sxs-lookup"><span data-stu-id="54e05-186">The status of the invitation.</span></span> <span data-ttu-id="54e05-187">可能的值为： `PendingAcceptance`、 `Completed`、 `InProgress`和 `Error`</span><span class="sxs-lookup"><span data-stu-id="54e05-187">Possible values are: `PendingAcceptance`, `Completed`, `InProgress`, and `Error`</span></span>|

## <a name="relationships"></a><span data-ttu-id="54e05-188">关系</span><span class="sxs-lookup"><span data-stu-id="54e05-188">Relationships</span></span>
| <span data-ttu-id="54e05-189">关系</span><span class="sxs-lookup"><span data-stu-id="54e05-189">Relationship</span></span> | <span data-ttu-id="54e05-190">类型</span><span class="sxs-lookup"><span data-stu-id="54e05-190">Type</span></span>   |<span data-ttu-id="54e05-191">说明</span><span class="sxs-lookup"><span data-stu-id="54e05-191">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54e05-192">invitedUser</span><span class="sxs-lookup"><span data-stu-id="54e05-192">invitedUser</span></span>|[<span data-ttu-id="54e05-193">用户</span><span class="sxs-lookup"><span data-stu-id="54e05-193">User</span></span>](user.md)|<span data-ttu-id="54e05-p109">创建为邀请创建进程组成部分的用户。只读</span><span class="sxs-lookup"><span data-stu-id="54e05-p109">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54e05-196">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54e05-196">JSON representation</span></span>
<span data-ttu-id="54e05-197">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54e05-197">Here is a JSON representation of the resource</span></span>

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

