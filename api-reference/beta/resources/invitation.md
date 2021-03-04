---
title: 邀请资源类型
description: 表示用于将外部用户添加到组织的邀请。
localization_priority: Normal
author: elisolMS
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5f132f1fb79c9f74df636b4684f6d42cdbe5bdc7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443004"
---
# <a name="invitation-resource-type"></a><span data-ttu-id="7c0af-103">邀请资源类型</span><span class="sxs-lookup"><span data-stu-id="7c0af-103">invitation resource type</span></span>

<span data-ttu-id="7c0af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c0af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c0af-105">表示用于将外部用户添加到组织的邀请。</span><span class="sxs-lookup"><span data-stu-id="7c0af-105">Represents an invitation that is used to add external users to an organization.</span></span> 

<span data-ttu-id="7c0af-106">邀请进程使用以下流程：</span><span class="sxs-lookup"><span data-stu-id="7c0af-106">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="7c0af-107">创建邀请</span><span class="sxs-lookup"><span data-stu-id="7c0af-107">An invitation is created</span></span>
* <span data-ttu-id="7c0af-108">将邀请发送至邀请的用户（包含邀请链接）</span><span class="sxs-lookup"><span data-stu-id="7c0af-108">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="7c0af-109">邀请的用户单击邀请链接、登录并兑现邀请和创建用户实体表示邀请的用户完成操作</span><span class="sxs-lookup"><span data-stu-id="7c0af-109">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="7c0af-110">兑现完成后，将用户重定向至指定页面</span><span class="sxs-lookup"><span data-stu-id="7c0af-110">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="7c0af-p101">创建邀请会在响应中返回兑现 URL (*inviteRedeemUrl*)。通过将 *sendInvitationMessage* 设置为 true，创建邀请 API 可以自动向邀请的用户发送包含兑现 URL 的电子邮件。还可以自定义要发送至邀请的用户的邮件。反之，如果想要通过一些其他的方法发送兑现 URL，则可以将 *sendInvitationMessage* 设置为 false，然后使用响应中的兑现 URL 创建自己的通信。目前没有可以执行兑现进程的 API。邀请的用户必须单击在上述步骤中的通信中发送的 *inviteRedeemUrl* 链接，并在浏览器中进行交互式兑现流程。完成后，邀请的用户即成为组织中的外部用户。</span><span class="sxs-lookup"><span data-stu-id="7c0af-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>

>[!NOTE]
><span data-ttu-id="7c0af-118">使用作为邀请请求的一部分创建的外部用户资源上的 [](user.md)**externalUserState** 和 **externalUserStateChangeDateTime** 属性跟踪邀请状态。</span><span class="sxs-lookup"><span data-stu-id="7c0af-118">The invitation status is tracked using the **externalUserState** and the **externalUserStateChangeDateTime** properties on the external [user](user.md) resource created as part of the invitation request.</span></span>

## <a name="methods"></a><span data-ttu-id="7c0af-119">Methods</span><span class="sxs-lookup"><span data-stu-id="7c0af-119">Methods</span></span>
| <span data-ttu-id="7c0af-120">方法</span><span class="sxs-lookup"><span data-stu-id="7c0af-120">Method</span></span>       | <span data-ttu-id="7c0af-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="7c0af-121">Return Type</span></span>  |<span data-ttu-id="7c0af-122">说明</span><span class="sxs-lookup"><span data-stu-id="7c0af-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7c0af-123">创建邀请</span><span class="sxs-lookup"><span data-stu-id="7c0af-123">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="7c0af-124">邀请</span><span class="sxs-lookup"><span data-stu-id="7c0af-124">invitation</span></span> | <span data-ttu-id="7c0af-125">写入 invitation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7c0af-125">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7c0af-126">属性</span><span class="sxs-lookup"><span data-stu-id="7c0af-126">Properties</span></span>
| <span data-ttu-id="7c0af-127">属性</span><span class="sxs-lookup"><span data-stu-id="7c0af-127">Property</span></span>     | <span data-ttu-id="7c0af-128">类型</span><span class="sxs-lookup"><span data-stu-id="7c0af-128">Type</span></span>   |<span data-ttu-id="7c0af-129">说明</span><span class="sxs-lookup"><span data-stu-id="7c0af-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c0af-130">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="7c0af-130">invitedUserDisplayName</span></span>|<span data-ttu-id="7c0af-131">String</span><span class="sxs-lookup"><span data-stu-id="7c0af-131">String</span></span>|<span data-ttu-id="7c0af-132">被邀请的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7c0af-132">The display name of the user being invited.</span></span>|
|<span data-ttu-id="7c0af-133">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="7c0af-133">invitedUserEmailAddress</span></span>|<span data-ttu-id="7c0af-134">String</span><span class="sxs-lookup"><span data-stu-id="7c0af-134">String</span></span>|<span data-ttu-id="7c0af-135">被邀请的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="7c0af-135">The email address of the user being invited.</span></span> <span data-ttu-id="7c0af-136">必需。</span><span class="sxs-lookup"><span data-stu-id="7c0af-136">Required.</span></span> <span data-ttu-id="7c0af-137">电子邮件地址中不允许使用以下特殊字符：</span><span class="sxs-lookup"><span data-stu-id="7c0af-137">The following special characters are not permitted in the email address:</span></span><br><ul><li><span data-ttu-id="7c0af-138">波形符 (~)</span><span class="sxs-lookup"><span data-stu-id="7c0af-138">Tilde (~)</span></span></li><li><span data-ttu-id="7c0af-139">感叹号 (`!`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-139">Exclamation point (`!`)</span></span></li><li><span data-ttu-id="7c0af-140">@ 符号 (`@`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-140">At sign (`@`)</span></span></li><li><span data-ttu-id="7c0af-141">井号 (`#`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-141">Number sign (`#`)</span></span></li><li><span data-ttu-id="7c0af-142">美元符号 (`$`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-142">Dollar sign (`$`)</span></span></li><li><span data-ttu-id="7c0af-143">百分号 (`%`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-143">Percent (`%`)</span></span></li><li><span data-ttu-id="7c0af-144">扬抑符 (`^`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-144">Circumflex (`^`)</span></span></li><li><span data-ttu-id="7c0af-145">与号 (`&`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-145">Ampersand (`&`)</span></span></li><li><span data-ttu-id="7c0af-146">星号 (`*`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-146">Asterisk (`*`)</span></span></li><li><span data-ttu-id="7c0af-147">圆括号 (`( )`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-147">Parentheses (`( )`)</span></span></li><li><span data-ttu-id="7c0af-148">连字符 (`-`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-148">Hyphen (`-`)</span></span></li><li><span data-ttu-id="7c0af-149">加号 (`+`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-149">Plus sign (`+`)</span></span></li><li><span data-ttu-id="7c0af-150">等号 (`=`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-150">Equal sign (`=`)</span></span></li><li><span data-ttu-id="7c0af-151">方括号 (`[ ]`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-151">Brackets (`[ ]`)</span></span></li><li><span data-ttu-id="7c0af-152">大括号 (`{ }`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-152">Braces (`{ }`)</span></span></li><li><span data-ttu-id="7c0af-153">反斜杠 (`\`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-153">Backslash (`\`)</span></span></li><li><span data-ttu-id="7c0af-154">斜杠符号 (`/`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-154">Slash mark (`/`)</span></span></li><li><span data-ttu-id="7c0af-155">竖线 (`|`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-155">Pipe (`|`)</span></span></li><li><span data-ttu-id="7c0af-156">分号 (`;`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-156">Semicolon (`;`)</span></span></li><li><span data-ttu-id="7c0af-157">冒号 (`:`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-157">Colon (`:`)</span></span></li><li><span data-ttu-id="7c0af-158">引号 (`"`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-158">Quotation marks (`"`)</span></span></li><li><span data-ttu-id="7c0af-159">尖括号 (`< >`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-159">Angle brackets (`< >`)</span></span></li><li><span data-ttu-id="7c0af-160">问号 (`?`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-160">Question mark (`?`)</span></span></li><li><span data-ttu-id="7c0af-161">逗号 (`,`)</span><span class="sxs-lookup"><span data-stu-id="7c0af-161">Comma (`,`)</span></span></li></ul><br><span data-ttu-id="7c0af-162">但是，存在下列例外情况：</span><span class="sxs-lookup"><span data-stu-id="7c0af-162">However, the following exceptions apply:</span></span><br><ul><li><span data-ttu-id="7c0af-163">允许在用户名中的任何位置使用句点 (`.`) 或连字符 (`-`)，但名称的开头或结尾除外。</span><span class="sxs-lookup"><span data-stu-id="7c0af-163">A period (`.`) or a hyphen (`-`) is permitted anywhere in the user name, except at the beginning or end of the name.</span></span></li><li><span data-ttu-id="7c0af-164">允许在用户名中的任何位置使用下划线 (`_`)。</span><span class="sxs-lookup"><span data-stu-id="7c0af-164">An underscore (`_`) is permitted anywhere in the user name.</span></span> <span data-ttu-id="7c0af-165">这包括名称的开头或结尾。</span><span class="sxs-lookup"><span data-stu-id="7c0af-165">This includes at the beginning or end of the name.</span></span></li></ul>|
|<span data-ttu-id="7c0af-166">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="7c0af-166">invitedUserMessageInfo</span></span>|[<span data-ttu-id="7c0af-167">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="7c0af-167">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="7c0af-168">要发送至邀请用户的邮件的其他配置，其中包括自定义邮件文本、语言和抄送收件人列表。</span><span class="sxs-lookup"><span data-stu-id="7c0af-168">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="7c0af-169">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="7c0af-169">sendInvitationMessage</span></span>|<span data-ttu-id="7c0af-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c0af-170">Boolean</span></span>|<span data-ttu-id="7c0af-p104">指示电子邮件是否应发送至邀请的用户。默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="7c0af-p104">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="7c0af-173">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="7c0af-173">inviteRedirectUrl</span></span>|<span data-ttu-id="7c0af-174">String</span><span class="sxs-lookup"><span data-stu-id="7c0af-174">String</span></span>|<span data-ttu-id="7c0af-p105">兑现邀请后，用户应被重定向至的 URL。必填。</span><span class="sxs-lookup"><span data-stu-id="7c0af-p105">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="7c0af-177">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="7c0af-177">inviteRedeemUrl</span></span>|<span data-ttu-id="7c0af-178">String</span><span class="sxs-lookup"><span data-stu-id="7c0af-178">String</span></span>|<span data-ttu-id="7c0af-179">用户可用于兑换邀请的 URL。</span><span class="sxs-lookup"><span data-stu-id="7c0af-179">The URL the user can use to redeem their invitation.</span></span> <span data-ttu-id="7c0af-180">只读。</span><span class="sxs-lookup"><span data-stu-id="7c0af-180">Read-only.</span></span>|
|<span data-ttu-id="7c0af-181">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="7c0af-181">invitedUserType</span></span>|<span data-ttu-id="7c0af-182">String</span><span class="sxs-lookup"><span data-stu-id="7c0af-182">String</span></span>|<span data-ttu-id="7c0af-p107">被邀请的用户的 userType。默认情况下，此值为“来宾”。如果你是公司管理员，则可以以“成员”身份进行邀请。</span><span class="sxs-lookup"><span data-stu-id="7c0af-p107">The userType of the user being invited. By default, this is Guest. You can invite as Member if you're are company administrator.</span></span> |
|<span data-ttu-id="7c0af-186">status</span><span class="sxs-lookup"><span data-stu-id="7c0af-186">status</span></span>|<span data-ttu-id="7c0af-187">字符串</span><span class="sxs-lookup"><span data-stu-id="7c0af-187">String</span></span>|<span data-ttu-id="7c0af-p108">邀请的状态。可能的值：PendingAcceptance、Completed、InProgress 和 Error</span><span class="sxs-lookup"><span data-stu-id="7c0af-p108">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c0af-190">关系</span><span class="sxs-lookup"><span data-stu-id="7c0af-190">Relationships</span></span>
| <span data-ttu-id="7c0af-191">关系</span><span class="sxs-lookup"><span data-stu-id="7c0af-191">Relationship</span></span> | <span data-ttu-id="7c0af-192">类型</span><span class="sxs-lookup"><span data-stu-id="7c0af-192">Type</span></span>   |<span data-ttu-id="7c0af-193">说明</span><span class="sxs-lookup"><span data-stu-id="7c0af-193">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c0af-194">invitedUser</span><span class="sxs-lookup"><span data-stu-id="7c0af-194">invitedUser</span></span>|[<span data-ttu-id="7c0af-195">user</span><span class="sxs-lookup"><span data-stu-id="7c0af-195">user</span></span>](user.md)|<span data-ttu-id="7c0af-p109">创建为邀请创建进程组成部分的用户。只读</span><span class="sxs-lookup"><span data-stu-id="7c0af-p109">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c0af-198">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c0af-198">JSON representation</span></span>
<span data-ttu-id="7c0af-199">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c0af-199">Here is a JSON representation of the resource</span></span>

<!-- 
{ 
    "blockType": "resource",
    "keyProperty":"id",
    "@odata.type": "microsoft.graph.invitation", 
    "optionalProperties": [
        "invitedUser"
     ],
    "baseType": "microsoft.graph.entity"
} 
-->
```json
{
  "id": "string",
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
<!--
{
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


