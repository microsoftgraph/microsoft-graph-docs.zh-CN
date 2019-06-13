---
title: 邀请资源类型
description: 表示用于向组织添加外部用户的邀请。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bb0979954421a9b0fe1d5b119e7f060843380a06
ms.sourcegitcommit: 8aaf10f7c11d1bf481e9acac19884346dbd44cb8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/13/2019
ms.locfileid: "34914663"
---
# <a name="invitation-resource-type"></a><span data-ttu-id="ab071-103">邀请资源类型</span><span class="sxs-lookup"><span data-stu-id="ab071-103">invitation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab071-104">表示用于向组织添加外部用户的邀请。</span><span class="sxs-lookup"><span data-stu-id="ab071-104">Represents an invitation that is used to add external users to an organization.</span></span> 

<span data-ttu-id="ab071-105">邀请进程使用以下流程：</span><span class="sxs-lookup"><span data-stu-id="ab071-105">The invitation process uses the following flow:</span></span>

* <span data-ttu-id="ab071-106">创建邀请</span><span class="sxs-lookup"><span data-stu-id="ab071-106">An invitation is created</span></span>
* <span data-ttu-id="ab071-107">将邀请发送至邀请的用户（包含邀请链接）</span><span class="sxs-lookup"><span data-stu-id="ab071-107">An invitation is sent to the invited user (containing an invitation link)</span></span>
* <span data-ttu-id="ab071-108">邀请的用户单击邀请链接、登录并兑现邀请和创建用户实体表示邀请的用户完成操作</span><span class="sxs-lookup"><span data-stu-id="ab071-108">The invited user clicks on the invitation link, signs in and redeems the invitation and creation of the user entity representing the invited user completes</span></span>
* <span data-ttu-id="ab071-109">兑现完成后，将用户重定向至指定页面</span><span class="sxs-lookup"><span data-stu-id="ab071-109">The user is redirected to a specific page after redemption completes</span></span>

<span data-ttu-id="ab071-p101">创建邀请会在响应中返回兑现 URL (*inviteRedeemUrl*)。通过将 *sendInvitationMessage* 设置为 true，创建邀请 API 可以自动向邀请的用户发送包含兑现 URL 的电子邮件。还可以自定义要发送至邀请的用户的邮件。反之，如果想要通过一些其他的方法发送兑现 URL，则可以将 *sendInvitationMessage* 设置为 false，然后使用响应中的兑现 URL 创建自己的通信。目前没有可以执行兑现进程的 API。邀请的用户必须单击在上述步骤中的通信中发送的 *inviteRedeemUrl* 链接，并在浏览器中进行交互式兑现流程。完成后，邀请的用户即成为组织中的外部用户。</span><span class="sxs-lookup"><span data-stu-id="ab071-p101">Creating an invitation will return a redemption URL in the response (*inviteRedeemUrl*). The create invitation API can automatically send an email containing the redemption URL to the invited user, by setting the *sendInvitationMessage* to true. You can also customize the message that will be sent to the invited user. Instead, if you wish to send the redemption URL through some other means, you can set the *sendInvitationMessage* to false and use the redeem URL from the response to craft your own communication. Currently, there is no API to perform the redemption process. The invited user has to click on the *inviteRedeemUrl* link sent in the communication in the step above, and go through the interactive redemption process in a browser. Once completed, the invited user becomes an external user in the organization.</span></span>


## <a name="methods"></a><span data-ttu-id="ab071-117">方法</span><span class="sxs-lookup"><span data-stu-id="ab071-117">Methods</span></span>
| <span data-ttu-id="ab071-118">方法</span><span class="sxs-lookup"><span data-stu-id="ab071-118">Method</span></span>       | <span data-ttu-id="ab071-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="ab071-119">Return Type</span></span>  |<span data-ttu-id="ab071-120">说明</span><span class="sxs-lookup"><span data-stu-id="ab071-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ab071-121">创建邀请</span><span class="sxs-lookup"><span data-stu-id="ab071-121">Create invitation</span></span>](../api/invitation-post.md) | <span data-ttu-id="ab071-122">邀请</span><span class="sxs-lookup"><span data-stu-id="ab071-122">invitation</span></span> | <span data-ttu-id="ab071-123">写入 invitation 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ab071-123">Write properties and relationships of invitation object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ab071-124">属性</span><span class="sxs-lookup"><span data-stu-id="ab071-124">Properties</span></span>
| <span data-ttu-id="ab071-125">属性</span><span class="sxs-lookup"><span data-stu-id="ab071-125">Property</span></span>     | <span data-ttu-id="ab071-126">类型</span><span class="sxs-lookup"><span data-stu-id="ab071-126">Type</span></span>   |<span data-ttu-id="ab071-127">说明</span><span class="sxs-lookup"><span data-stu-id="ab071-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab071-128">invitedUserDisplayName</span><span class="sxs-lookup"><span data-stu-id="ab071-128">invitedUserDisplayName</span></span>|<span data-ttu-id="ab071-129">String</span><span class="sxs-lookup"><span data-stu-id="ab071-129">String</span></span>|<span data-ttu-id="ab071-130">被邀请的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ab071-130">The display name of the user being invited.</span></span>|
|<span data-ttu-id="ab071-131">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="ab071-131">invitedUserEmailAddress</span></span>|<span data-ttu-id="ab071-132">String</span><span class="sxs-lookup"><span data-stu-id="ab071-132">String</span></span>|<span data-ttu-id="ab071-p102">被邀请的用户的电子邮件地址。必填。</span><span class="sxs-lookup"><span data-stu-id="ab071-p102">The email address of the user being invited. Required.</span></span>|
|<span data-ttu-id="ab071-135">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="ab071-135">invitedUserMessageInfo</span></span>|[<span data-ttu-id="ab071-136">invitedUserMessageInfo</span><span class="sxs-lookup"><span data-stu-id="ab071-136">invitedUserMessageInfo</span></span>](invitedusermessageinfo.md)|<span data-ttu-id="ab071-137">要发送至邀请用户的邮件的其他配置，其中包括自定义邮件文本、语言和抄送收件人列表。</span><span class="sxs-lookup"><span data-stu-id="ab071-137">Additional configuration for the message being sent to the invited user, including customizing message text, language and cc recipient list.</span></span>|
|<span data-ttu-id="ab071-138">sendInvitationMessage</span><span class="sxs-lookup"><span data-stu-id="ab071-138">sendInvitationMessage</span></span>|<span data-ttu-id="ab071-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab071-139">Boolean</span></span>|<span data-ttu-id="ab071-p103">指示电子邮件是否应发送至邀请的用户。默认值为 false。</span><span class="sxs-lookup"><span data-stu-id="ab071-p103">Indicates whether an email should be sent to the user being invited or not. The default is false.</span></span>|
|<span data-ttu-id="ab071-142">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="ab071-142">inviteRedirectUrl</span></span>|<span data-ttu-id="ab071-143">String</span><span class="sxs-lookup"><span data-stu-id="ab071-143">String</span></span>|<span data-ttu-id="ab071-p104">兑现邀请后，用户应被重定向至的 URL。必填。</span><span class="sxs-lookup"><span data-stu-id="ab071-p104">The URL user should be redirected to once the invitation is redeemed. Required.</span></span>|
|<span data-ttu-id="ab071-146">inviteRedeemUrl</span><span class="sxs-lookup"><span data-stu-id="ab071-146">inviteRedeemUrl</span></span>|<span data-ttu-id="ab071-147">String</span><span class="sxs-lookup"><span data-stu-id="ab071-147">String</span></span>|<span data-ttu-id="ab071-p105">用户可用于兑现邀请的 URL。只读</span><span class="sxs-lookup"><span data-stu-id="ab071-p105">The URL user can use to redeem his invitation. Read-Only</span></span>|
|<span data-ttu-id="ab071-150">invitedUserType</span><span class="sxs-lookup"><span data-stu-id="ab071-150">invitedUserType</span></span>|<span data-ttu-id="ab071-151">String</span><span class="sxs-lookup"><span data-stu-id="ab071-151">String</span></span>|<span data-ttu-id="ab071-p106">被邀请的用户的 userType。默认情况下，此值为“来宾”。如果你是公司管理员，则可以以“成员”身份进行邀请。</span><span class="sxs-lookup"><span data-stu-id="ab071-p106">The userType of the user being invited. By default, this is Guest. You can invite as Member if you're are company administrator.</span></span> |
|<span data-ttu-id="ab071-155">状态</span><span class="sxs-lookup"><span data-stu-id="ab071-155">status</span></span>|<span data-ttu-id="ab071-156">字符串</span><span class="sxs-lookup"><span data-stu-id="ab071-156">String</span></span>|<span data-ttu-id="ab071-p107">邀请的状态。可能的值：PendingAcceptance、Completed、InProgress 和 Error</span><span class="sxs-lookup"><span data-stu-id="ab071-p107">The status of the invitation. Possible values: PendingAcceptance, Completed, InProgress, and Error</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab071-159">关系</span><span class="sxs-lookup"><span data-stu-id="ab071-159">Relationships</span></span>
| <span data-ttu-id="ab071-160">关系</span><span class="sxs-lookup"><span data-stu-id="ab071-160">Relationship</span></span> | <span data-ttu-id="ab071-161">类型</span><span class="sxs-lookup"><span data-stu-id="ab071-161">Type</span></span>   |<span data-ttu-id="ab071-162">说明</span><span class="sxs-lookup"><span data-stu-id="ab071-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ab071-163">invitedUser</span><span class="sxs-lookup"><span data-stu-id="ab071-163">invitedUser</span></span>|[<span data-ttu-id="ab071-164">user</span><span class="sxs-lookup"><span data-stu-id="ab071-164">user</span></span>](user.md)|<span data-ttu-id="ab071-p108">创建为邀请创建进程组成部分的用户。只读</span><span class="sxs-lookup"><span data-stu-id="ab071-p108">The user created as part of the invitation creation. Read-Only</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab071-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab071-167">JSON representation</span></span>
<span data-ttu-id="ab071-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab071-168">Here is a JSON representation of the resource</span></span>

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
