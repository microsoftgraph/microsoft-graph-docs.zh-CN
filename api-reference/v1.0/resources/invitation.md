---
title: 邀请资源类型
description: 表示用于将外部用户添加到组织的邀请。
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 29dcf476dc7d26f87c04a6fd8d075c4ed0d77bd5
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062551"
---
# <a name="invitation-resource-type"></a><span data-ttu-id="e31f2-103">邀请资源类型</span><span class="sxs-lookup"><span data-stu-id="e31f2-103">invitation resource type</span></span>

<span data-ttu-id="e31f2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e31f2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e31f2-105">表示用于将外部用户添加到组织的邀请。</span><span class="sxs-lookup"><span data-stu-id="e31f2-105">Represents an invitation that is used to add external users to an organization.</span></span> 

<span data-ttu-id="e31f2-106">邀请进程使用以下流程：</span><span class="sxs-lookup"><span data-stu-id="e31f2-106">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="e31f2-107">创建邀请</span><span class="sxs-lookup"><span data-stu-id="e31f2-107">An invitation is created</span></span>
* <span data-ttu-id="e31f2-108">将邀请发送至邀请的用户（包含邀请链接）</span><span class="sxs-lookup"><span data-stu-id="e31f2-108">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="e31f2-109">邀请的用户单击邀请链接、登录并兑现邀请和创建用户实体表示邀请的用户完成操作</span><span class="sxs-lookup"><span data-stu-id="e31f2-109">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="e31f2-110">兑现完成后，将用户重定向至指定页面</span><span class="sxs-lookup"><span data-stu-id="e31f2-110">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="e31f2-p101">创建邀请会在响应中返回兑现 URL (*inviteRedeemUrl*)。通过将 *sendInvitationMessage* 设置为 true，创建邀请 API 可以自动向邀请的用户发送包含兑现 URL 的电子邮件。还可以自定义要发送至邀请的用户的邮件。反之，如果想要通过一些其他的方法发送兑现 URL，则可以将 *sendInvitationMessage* 设置为 false，然后使用响应中的兑现 URL 创建自己的通信。目前没有可以执行兑现进程的 API。邀请的用户必须单击在上述步骤中的通信中发送的 *inviteRedeemUrl* 链接，并在浏览器中进行交互式兑现流程。完成后，邀请的用户即成为组织中的外部用户。</span><span class="sxs-lookup"><span data-stu-id="e31f2-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>


## <a name="methods"></a><span data-ttu-id="e31f2-118">方法</span><span class="sxs-lookup"><span data-stu-id="e31f2-118">Methods</span></span>
| <span data-ttu-id="e31f2-119">方法</span><span class="sxs-lookup"><span data-stu-id="e31f2-119">Method</span></span>       | <span data-ttu-id="e31f2-120">返回类型</span><span class="sxs-lookup"><span data-stu-id="e31f2-120">Return Type</span></span>  |<span data-ttu-id="e31f2-121">说明</span><span class="sxs-lookup"><span data-stu-id="e31f2-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e31f2-122">创建邀请</span><span class="sxs-lookup"><span data-stu-id="e31f2-122">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="e31f2-123">邀请</span><span class="sxs-lookup"><span data-stu-id="e31f2-123">invitation</span></span> | <span data-ttu-id="e31f2-124">写入 invitation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e31f2-124">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e31f2-125">属性</span><span class="sxs-lookup"><span data-stu-id="e31f2-125">Properties</span></span>
| <span data-ttu-id="e31f2-126">属性</span><span class="sxs-lookup"><span data-stu-id="e31f2-126">Property</span></span>     | <span data-ttu-id="e31f2-127">类型</span><span class="sxs-lookup"><span data-stu-id="e31f2-127">Type</span></span>   |<span data-ttu-id="e31f2-128">说明</span><span class="sxs-lookup"><span data-stu-id="e31f2-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e31f2-129">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="e31f2-129">invitedUserDisplayName</span></span>|<span data-ttu-id="e31f2-130">String</span><span class="sxs-lookup"><span data-stu-id="e31f2-130">String</span></span>|<span data-ttu-id="e31f2-131">被邀请的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e31f2-131">The display name of the user being invited.</span></span>|
|<span data-ttu-id="e31f2-132">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e31f2-132">invitedUserEmailAddress</span></span>|<span data-ttu-id="e31f2-133">String</span><span class="sxs-lookup"><span data-stu-id="e31f2-133">String</span></span>|<span data-ttu-id="e31f2-134">被邀请的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="e31f2-134">The email address of the user being invited.</span></span> <span data-ttu-id="e31f2-135">必需。</span><span class="sxs-lookup"><span data-stu-id="e31f2-135">Required.</span></span> <span data-ttu-id="e31f2-136">电子邮件地址中不允许使用以下特殊字符：</span><span class="sxs-lookup"><span data-stu-id="e31f2-136">The following special characters are not permitted in the email address:</span></span><br><ul><li><span data-ttu-id="e31f2-137">波形符 (~)</span><span class="sxs-lookup"><span data-stu-id="e31f2-137">Tilde (~)</span></span></li><li><span data-ttu-id="e31f2-138">感叹号 (`!`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-138">Exclamation point (`!`)</span></span></li><li><span data-ttu-id="e31f2-139">井号 (`#`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-139">Number sign (`#`)</span></span></li><li><span data-ttu-id="e31f2-140">美元符号 (`$`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-140">Dollar sign (`$`)</span></span></li><li><span data-ttu-id="e31f2-141">百分号 (`%`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-141">Percent (`%`)</span></span></li><li><span data-ttu-id="e31f2-142">扬抑符 (`^`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-142">Circumflex (`^`)</span></span></li><li><span data-ttu-id="e31f2-143">与号 (`&`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-143">Ampersand (`&`)</span></span></li><li><span data-ttu-id="e31f2-144">星号 (`*`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-144">Asterisk (`*`)</span></span></li><li><span data-ttu-id="e31f2-145">圆括号 (`( )`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-145">Parentheses (`( )`)</span></span></li><li><span data-ttu-id="e31f2-146">加号 (`+`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-146">Plus sign (`+`)</span></span></li><li><span data-ttu-id="e31f2-147">等号 (`=`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-147">Equal sign (`=`)</span></span></li><li><span data-ttu-id="e31f2-148">方括号 (`[ ]`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-148">Brackets (`[ ]`)</span></span></li><li><span data-ttu-id="e31f2-149">大括号 (`{ }`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-149">Braces (`{ }`)</span></span></li><li><span data-ttu-id="e31f2-150">反斜杠 (`\`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-150">Backslash (`\`)</span></span></li><li><span data-ttu-id="e31f2-151">斜杠符号 (`/`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-151">Slash mark (`/`)</span></span></li><li><span data-ttu-id="e31f2-152">竖线 (`\|`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-152">Pipe (`\|`)</span></span></li><li><span data-ttu-id="e31f2-153">分号 (`;`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-153">Semicolon (`;`)</span></span></li><li><span data-ttu-id="e31f2-154">冒号 (`:`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-154">Colon (`:`)</span></span></li><li><span data-ttu-id="e31f2-155">引号 (`"`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-155">Quotation marks (`"`)</span></span></li><li><span data-ttu-id="e31f2-156">尖括号 (`< >`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-156">Angle brackets (`< >`)</span></span></li><li><span data-ttu-id="e31f2-157">问号 (`?`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-157">Question mark (`?`)</span></span></li><li><span data-ttu-id="e31f2-158">逗号 (`,`)</span><span class="sxs-lookup"><span data-stu-id="e31f2-158">Comma (`,`)</span></span></li></ul><br><span data-ttu-id="e31f2-159">但是，存在下列例外情况：</span><span class="sxs-lookup"><span data-stu-id="e31f2-159">However, the following exceptions apply:</span></span><br><ul><li><span data-ttu-id="e31f2-160">允许在用户名中的任何位置使用句点 (`.`) 或连字符 (`-`)，但名称的开头或结尾除外。</span><span class="sxs-lookup"><span data-stu-id="e31f2-160">A period (`.`) or a hyphen (`-`) is permitted anywhere in the user name, except at the beginning or end of the name.</span></span></li><li><span data-ttu-id="e31f2-161">允许在用户名中的任何位置使用下划线 (`_`)。</span><span class="sxs-lookup"><span data-stu-id="e31f2-161">An underscore (`_`) is permitted anywhere in the user name.</span></span> <span data-ttu-id="e31f2-162">这包括名称的开头或结尾。</span><span class="sxs-lookup"><span data-stu-id="e31f2-162">This includes at the beginning or end of the name.</span></span></li></ul>|
|<span data-ttu-id="e31f2-163">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="e31f2-163">invitedUserMessageInfo</span></span>|[<span data-ttu-id="e31f2-164">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="e31f2-164">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="e31f2-165">要发送至邀请用户的邮件的其他配置，其中包括自定义邮件文本、语言和抄送收件人列表。</span><span class="sxs-lookup"><span data-stu-id="e31f2-165">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="e31f2-166">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="e31f2-166">sendInvitationMessage</span></span>|<span data-ttu-id="e31f2-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="e31f2-167">Boolean</span></span>|<span data-ttu-id="e31f2-p104">指示电子邮件是否应发送至邀请的用户。默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="e31f2-p104">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="e31f2-170">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="e31f2-170">inviteRedirectUrl</span></span>|<span data-ttu-id="e31f2-171">String</span><span class="sxs-lookup"><span data-stu-id="e31f2-171">String</span></span>|<span data-ttu-id="e31f2-p105">兑现邀请后，用户应被重定向至的 URL。必填。</span><span class="sxs-lookup"><span data-stu-id="e31f2-p105">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="e31f2-174">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="e31f2-174">inviteRedeemUrl</span></span>|<span data-ttu-id="e31f2-175">String</span><span class="sxs-lookup"><span data-stu-id="e31f2-175">String</span></span>|<span data-ttu-id="e31f2-p106">用户可用于兑现邀请的 URL。只读</span><span class="sxs-lookup"><span data-stu-id="e31f2-p106">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="e31f2-178">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="e31f2-178">invitedUserType</span></span>|<span data-ttu-id="e31f2-179">String</span><span class="sxs-lookup"><span data-stu-id="e31f2-179">String</span></span>|<span data-ttu-id="e31f2-180">被邀请的用户的 userType。</span><span class="sxs-lookup"><span data-stu-id="e31f2-180">The userType of the user being invited.</span></span> <span data-ttu-id="e31f2-181">默认情况下，此值为“来宾”。</span><span class="sxs-lookup"><span data-stu-id="e31f2-181">By default, this is Guest.</span></span> <span data-ttu-id="e31f2-182">如果你是公司管理员，则可以以“成员”身份进行邀请。</span><span class="sxs-lookup"><span data-stu-id="e31f2-182">You can invite as Member if you are a company administrator.</span></span> |
|<span data-ttu-id="e31f2-183">状态</span><span class="sxs-lookup"><span data-stu-id="e31f2-183">status</span></span>|<span data-ttu-id="e31f2-184">字符串</span><span class="sxs-lookup"><span data-stu-id="e31f2-184">String</span></span>|<span data-ttu-id="e31f2-p108">邀请的状态。可能的值：PendingAcceptance、Completed、InProgress 和 Error</span><span class="sxs-lookup"><span data-stu-id="e31f2-p108">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="e31f2-187">关系</span><span class="sxs-lookup"><span data-stu-id="e31f2-187">Relationships</span></span>
| <span data-ttu-id="e31f2-188">关系</span><span class="sxs-lookup"><span data-stu-id="e31f2-188">Relationship</span></span> | <span data-ttu-id="e31f2-189">类型</span><span class="sxs-lookup"><span data-stu-id="e31f2-189">Type</span></span>   |<span data-ttu-id="e31f2-190">说明</span><span class="sxs-lookup"><span data-stu-id="e31f2-190">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e31f2-191">invitedUser</span><span class="sxs-lookup"><span data-stu-id="e31f2-191">invitedUser</span></span>|[<span data-ttu-id="e31f2-192">用户</span><span class="sxs-lookup"><span data-stu-id="e31f2-192">User</span></span>](user.md)|<span data-ttu-id="e31f2-p109">创建为邀请创建进程组成部分的用户。只读</span><span class="sxs-lookup"><span data-stu-id="e31f2-p109">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e31f2-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e31f2-195">JSON representation</span></span>
<span data-ttu-id="e31f2-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e31f2-196">Here is a JSON representation of the resource</span></span>

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
