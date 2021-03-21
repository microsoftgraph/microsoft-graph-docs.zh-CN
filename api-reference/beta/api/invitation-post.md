---
title: 创建邀请
description: 使用该 API 创建新的邀请。 邀请会将外部用户添加至组织。
localization_priority: Normal
author: Sammak
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a74643bbc75de77f68f5084310d739a1ffceccfa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954629"
---
# <a name="create-invitation"></a><span data-ttu-id="74c5a-104">创建邀请</span><span class="sxs-lookup"><span data-stu-id="74c5a-104">Create invitation</span></span>

<span data-ttu-id="74c5a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74c5a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74c5a-p102">使用该 API 创建新的[邀请](../resources/invitation.md)。邀请将外部用户添加至组织。</span><span class="sxs-lookup"><span data-stu-id="74c5a-p102">Use this API to create a new [invitation](../resources/invitation.md). Invitation adds an external user to the organization.</span></span>

<span data-ttu-id="74c5a-108">创建新的邀请时，有多个选项可供使用：</span><span class="sxs-lookup"><span data-stu-id="74c5a-108">When creating a new invitation you have several options available:</span></span>

1. <span data-ttu-id="74c5a-p103">创建邀请后，Microsoft Graph 可以自动向邀请的用户直接发送邀请电子邮件，或者你的应用可以使用创建响应中返回的 *inviteRedeemUrl* 创建自己的邀请（通过你所选择的通信机制）并发送给邀请的用户。如果决定让 Microsoft Graph 自动发送邀请电子邮件，则你可以使用 [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md) 控制电子邮件的内容和语言。</span><span class="sxs-lookup"><span data-stu-id="74c5a-p103">On invitation creation, Microsoft Graph can automatically send an invitation email directly to the invited user, or your app can use the *inviteRedeemUrl* returned in the creation response to craft your own invitation (through your communication mechanism of choice) to the invited user. If you decide to have Microsoft Graph send an invitation email automatically, you can control the content and language of the email using [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span></span>
2. <span data-ttu-id="74c5a-p104">邀请用户后，会创建用户实体（userType 为“来宾”）并且现在可以使用它来控制对资源的访问。受邀请的用户必须完成兑换过程才能访问其获得邀请的任意资源。</span><span class="sxs-lookup"><span data-stu-id="74c5a-p104">When the user is invited, a user entity (of userType Guest) is created and can now be used to control access to resources. The invited user has to go through the redemption process to access any resources he has been invited to.</span></span>

## <a name="permissions"></a><span data-ttu-id="74c5a-113">权限</span><span class="sxs-lookup"><span data-stu-id="74c5a-113">Permissions</span></span>
<span data-ttu-id="74c5a-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74c5a-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="74c5a-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="74c5a-116">Permission type</span></span>      | <span data-ttu-id="74c5a-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74c5a-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="74c5a-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74c5a-118">Delegated (work or school account)</span></span> | <span data-ttu-id="74c5a-119">User.Invite.All、User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74c5a-119">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="74c5a-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74c5a-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74c5a-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="74c5a-121">Not supported.</span></span>    |
|<span data-ttu-id="74c5a-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="74c5a-122">Application</span></span> | <span data-ttu-id="74c5a-123">User.Invite.All、User.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74c5a-123">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="74c5a-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74c5a-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
## <a name="request-headers"></a><span data-ttu-id="74c5a-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="74c5a-125">Request headers</span></span>
| <span data-ttu-id="74c5a-126">标头</span><span class="sxs-lookup"><span data-stu-id="74c5a-126">Header</span></span>       | <span data-ttu-id="74c5a-127">值</span><span class="sxs-lookup"><span data-stu-id="74c5a-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="74c5a-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="74c5a-128">Authorization</span></span>  | <span data-ttu-id="74c5a-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="74c5a-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="74c5a-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="74c5a-131">Content-Type</span></span>  | <span data-ttu-id="74c5a-132">application/json</span><span class="sxs-lookup"><span data-stu-id="74c5a-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="74c5a-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="74c5a-133">Request body</span></span>
<span data-ttu-id="74c5a-134">在请求正文中，提供 [invitation](../resources/invitation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74c5a-134">In the request body, supply a JSON representation of an [invitation](../resources/invitation.md) object.</span></span>

<span data-ttu-id="74c5a-135">下表显示创建邀请时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="74c5a-135">The following table shows the properties that are required when you create a invitation.</span></span>

| <span data-ttu-id="74c5a-136">参数</span><span class="sxs-lookup"><span data-stu-id="74c5a-136">Parameter</span></span> | <span data-ttu-id="74c5a-137">类型</span><span class="sxs-lookup"><span data-stu-id="74c5a-137">Type</span></span> | <span data-ttu-id="74c5a-138">说明</span><span class="sxs-lookup"><span data-stu-id="74c5a-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74c5a-139">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="74c5a-139">invitedUserEmailAddress</span></span> |<span data-ttu-id="74c5a-140">string</span><span class="sxs-lookup"><span data-stu-id="74c5a-140">string</span></span> | <span data-ttu-id="74c5a-141">你要邀请的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="74c5a-141">The email address of the user you are inviting.</span></span>|
|<span data-ttu-id="74c5a-142">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="74c5a-142">inviteRedirectUrl</span></span> |<span data-ttu-id="74c5a-143">string</span><span class="sxs-lookup"><span data-stu-id="74c5a-143">string</span></span> |<span data-ttu-id="74c5a-144">兑现后用户将被重定向至的 URL。</span><span class="sxs-lookup"><span data-stu-id="74c5a-144">The URL that the user will be redirected to after redemption.</span></span>|

## <a name="response"></a><span data-ttu-id="74c5a-145">响应</span><span class="sxs-lookup"><span data-stu-id="74c5a-145">Response</span></span>

<span data-ttu-id="74c5a-146">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [invitation](../resources/invitation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74c5a-146">If successful, this method returns `201 Created` response code and [invitation](../resources/invitation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74c5a-147">示例</span><span class="sxs-lookup"><span data-stu-id="74c5a-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="74c5a-148">请求</span><span class="sxs-lookup"><span data-stu-id="74c5a-148">Request</span></span>
<span data-ttu-id="74c5a-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="74c5a-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="74c5a-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="74c5a-150">HTTP</span></span>](#tab/http)
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
  "inviteRedirectUrl": "https://myapp.contoso.com"
}
```
# <a name="c"></a>[<span data-ttu-id="74c5a-151">C#</span><span class="sxs-lookup"><span data-stu-id="74c5a-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-invitation-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="74c5a-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74c5a-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-invitation-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="74c5a-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74c5a-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-invitation-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="74c5a-154">Java</span><span class="sxs-lookup"><span data-stu-id="74c5a-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-invitation-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="74c5a-155">响应</span><span class="sxs-lookup"><span data-stu-id="74c5a-155">Response</span></span>
<span data-ttu-id="74c5a-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="74c5a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "inviteRedirectUrl": "https://myapp.contoso.com/",
  "status": "Completed",
  "invitedUser":  [ {  "id": "243b1de4-ad9f-421c-a933-d55305fb165d" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


