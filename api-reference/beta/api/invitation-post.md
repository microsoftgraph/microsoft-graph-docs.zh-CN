---
title: 创建邀请
description: 使用该 API 创建新的邀请。 邀请会将外部用户添加至组织。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e30c6fed6fc485b9c305b0b0e8e082b7ca1833c5
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656809"
---
# <a name="create-invitation"></a><span data-ttu-id="673be-104">创建邀请</span><span class="sxs-lookup"><span data-stu-id="673be-104">Create invitation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="673be-p102">使用该 API 创建新的[邀请](../resources/invitation.md)。邀请将外部用户添加至组织。</span><span class="sxs-lookup"><span data-stu-id="673be-p102">Use this API to create a new [invitation](../resources/invitation.md). Invitation adds an external user to the organization.</span></span>

<span data-ttu-id="673be-107">创建新的邀请时，有多个选项可供使用：</span><span class="sxs-lookup"><span data-stu-id="673be-107">When creating a new invitation you have several options available:</span></span>

1. <span data-ttu-id="673be-p103">创建邀请后，Microsoft Graph 可以自动向邀请的用户直接发送邀请电子邮件，或者你的应用可以使用创建响应中返回的 *inviteRedeemUrl* 创建自己的邀请（通过你所选择的通信机制）并发送给邀请的用户。如果决定让 Microsoft Graph 自动发送邀请电子邮件，则你可以使用 [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md) 控制电子邮件的内容和语言。</span><span class="sxs-lookup"><span data-stu-id="673be-p103">On invitation creation, Microsoft Graph can automatically send an invitation email directly to the invited user, or your app can use the *inviteRedeemUrl* returned in the creation response to craft your own invitation (through your communication mechanism of choice) to the invited user. If you decide to have Microsoft Graph send an invitation email automatically, you can control the content and language of the email using [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span></span>
2. <span data-ttu-id="673be-p104">邀请用户后，会创建用户实体（userType 为“来宾”）并且现在可以使用它来控制对资源的访问。受邀请的用户必须完成兑换过程才能访问其获得邀请的任意资源。</span><span class="sxs-lookup"><span data-stu-id="673be-p104">When the user is invited, a user entity (of userType Guest) is created and can now be used to control access to resources. The invited user has to go through the redemption process to access any resources he has been invited to.</span></span>

## <a name="permissions"></a><span data-ttu-id="673be-112">权限</span><span class="sxs-lookup"><span data-stu-id="673be-112">Permissions</span></span>
<span data-ttu-id="673be-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="673be-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="673be-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="673be-115">Permission type</span></span>      | <span data-ttu-id="673be-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="673be-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="673be-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="673be-117">Delegated (work or school account)</span></span> | <span data-ttu-id="673be-118">User.Invite.All、User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="673be-118">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="673be-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="673be-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="673be-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="673be-120">Not supported.</span></span>    |
|<span data-ttu-id="673be-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="673be-121">Application</span></span> | <span data-ttu-id="673be-122">User.Invite.All、User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="673be-122">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="673be-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="673be-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
## <a name="request-headers"></a><span data-ttu-id="673be-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="673be-124">Request headers</span></span>
| <span data-ttu-id="673be-125">标头</span><span class="sxs-lookup"><span data-stu-id="673be-125">Header</span></span>       | <span data-ttu-id="673be-126">值</span><span class="sxs-lookup"><span data-stu-id="673be-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="673be-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="673be-127">Authorization</span></span>  | <span data-ttu-id="673be-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="673be-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="673be-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="673be-130">Content-Type</span></span>  | <span data-ttu-id="673be-131">application/json</span><span class="sxs-lookup"><span data-stu-id="673be-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="673be-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="673be-132">Request body</span></span>
<span data-ttu-id="673be-133">在请求正文中，提供 [invitation](../resources/invitation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="673be-133">In the request body, supply a JSON representation of an [invitation](../resources/invitation.md) object.</span></span>

<span data-ttu-id="673be-134">下表显示创建邀请时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="673be-134">The following table shows the properties that are required when you create a invitation.</span></span>

| <span data-ttu-id="673be-135">参数</span><span class="sxs-lookup"><span data-stu-id="673be-135">Parameter</span></span> | <span data-ttu-id="673be-136">类型</span><span class="sxs-lookup"><span data-stu-id="673be-136">Type</span></span> | <span data-ttu-id="673be-137">说明</span><span class="sxs-lookup"><span data-stu-id="673be-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="673be-138">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="673be-138">invitedUserEmailAddress</span></span> |<span data-ttu-id="673be-139">string</span><span class="sxs-lookup"><span data-stu-id="673be-139">string</span></span> | <span data-ttu-id="673be-140">你要邀请的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="673be-140">The email address of the user you are inviting.</span></span>|
|<span data-ttu-id="673be-141">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="673be-141">inviteRedirectUrl</span></span> |<span data-ttu-id="673be-142">string</span><span class="sxs-lookup"><span data-stu-id="673be-142">string</span></span> |<span data-ttu-id="673be-143">兑现后用户将被重定向至的 URL。</span><span class="sxs-lookup"><span data-stu-id="673be-143">The URL that the user will be redirected to after redemption.</span></span>|

## <a name="response"></a><span data-ttu-id="673be-144">响应</span><span class="sxs-lookup"><span data-stu-id="673be-144">Response</span></span>

<span data-ttu-id="673be-145">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [invitation](../resources/invitation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="673be-145">If successful, this method returns `201 Created` response code and [invitation](../resources/invitation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="673be-146">示例</span><span class="sxs-lookup"><span data-stu-id="673be-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="673be-147">请求</span><span class="sxs-lookup"><span data-stu-id="673be-147">Request</span></span>
<span data-ttu-id="673be-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="673be-148">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_invitation_post"
}-->
```http
POST https://graph.microsoft.com/beta/invitations
Content-type: application/json
Content-length: 551

{
  "invitedUserEmailAddress": "yyy@test.com",
  "inviteRedirectUrl": "https://myapp.com"
}
```

##### <a name="response"></a><span data-ttu-id="673be-149">响应</span><span class="sxs-lookup"><span data-stu-id="673be-149">Response</span></span>
<span data-ttu-id="673be-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="673be-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invitation"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 551

{
  "id": "7b92124c-9fa9-406f-8b8e-225df8376ba9",
  "inviteRedeemUrl": "https://invitations.microsoft.com/redeem/?tenant=04dcc6ab-388a-4559-b527-fbec656300ea&user=7b92124c-9fa9-406f-8b8e-225df8376ba9&ticket=VV9dmiExBsfRIVNFjb9ITj9VXAd07Ypv4gTg%2f8PiuJs%3d&lc=1033&ver=2.0",
  "invitedUserDisplayName": "yyy",
  "invitedUserEmailAddress": "yyy@test.com",
  "sendInvitationMessage": false,
  "invitedUserMessageInfo": {
     "messageLanguage": null,
     "ccRecipients": [
          {
             "emailAddress": {
                 "name": null,
                 "address": null
              }
          }
     ],
     "customizedMessageBody": null
  },
  "inviteRedirectUrl": "https://myapp.com/",
  "status": "Completed",
  "invitedUser":  [ {  "id": "243b1de4-ad9f-421c-a933-d55305fb165d" } ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="673be-153">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="673be-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="673be-154">C#</span><span class="sxs-lookup"><span data-stu-id="673be-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_invitation_post-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="673be-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="673be-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_invitation_post-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/invitation-post.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/invitation-post.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
