---
author: JeremyKelley
description: 发送 DriveItem 的共享邀请。
ms.date: 09/10/2017
title: 发送邀请以访问项目
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0344a4b6b663aa5a2a0cc03a470907bb48f63f9f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416728"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="676bf-103">发送共享邀请</span><span class="sxs-lookup"><span data-stu-id="676bf-103">Send a sharing invitation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="676bf-p101">发送 **DriveItem** 的共享邀请。共享邀请为收件人提供权限，也可以选择向收件人发送电子邮件以通知他们项目已共享。</span><span class="sxs-lookup"><span data-stu-id="676bf-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="676bf-106">权限</span><span class="sxs-lookup"><span data-stu-id="676bf-106">Permissions</span></span>

<span data-ttu-id="676bf-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="676bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="676bf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="676bf-109">Permission type</span></span>      | <span data-ttu-id="676bf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="676bf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="676bf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="676bf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="676bf-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="676bf-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="676bf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="676bf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="676bf-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="676bf-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="676bf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="676bf-115">Application</span></span> | <span data-ttu-id="676bf-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="676bf-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="676bf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="676bf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="676bf-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="676bf-118">Request body</span></span>

<span data-ttu-id="676bf-119">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="676bf-119">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite" } -->

```json
{
  "requireSignIn": false,
  "sendInvitation": false,
  "roles": [ "read | write"],
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" },
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "message": "string"
}
```

| <span data-ttu-id="676bf-120">参数</span><span class="sxs-lookup"><span data-stu-id="676bf-120">Parameter</span></span>        | <span data-ttu-id="676bf-121">类型</span><span class="sxs-lookup"><span data-stu-id="676bf-121">Type</span></span>                                            | <span data-ttu-id="676bf-122">说明</span><span class="sxs-lookup"><span data-stu-id="676bf-122">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="676bf-123">recipients</span><span class="sxs-lookup"><span data-stu-id="676bf-123">recipients</span></span>       | <span data-ttu-id="676bf-124">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="676bf-124">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="676bf-125">将获得访问权限和共享邀请的收件人的集合。</span><span class="sxs-lookup"><span data-stu-id="676bf-125">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="676bf-126">message</span><span class="sxs-lookup"><span data-stu-id="676bf-126">message</span></span>          | <span data-ttu-id="676bf-127">String</span><span class="sxs-lookup"><span data-stu-id="676bf-127">String</span></span>                                          | <span data-ttu-id="676bf-p103">共享邀请中包含的纯文本格式的邮件。最大长度为 2000 个字符。</span><span class="sxs-lookup"><span data-stu-id="676bf-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="676bf-130">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="676bf-130">requireSignIn</span></span>    | <span data-ttu-id="676bf-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="676bf-131">Boolean</span></span>                                         | <span data-ttu-id="676bf-132">指定邀请的收件人要查看共享项目的登录位置。</span><span class="sxs-lookup"><span data-stu-id="676bf-132">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="676bf-133">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="676bf-133">sendInvitation</span></span>   | <span data-ttu-id="676bf-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="676bf-134">Boolean</span></span>                                         | <span data-ttu-id="676bf-135">指定是否生成电子邮件或帖子 (false)，或是否仅创建权限 (true)。</span><span class="sxs-lookup"><span data-stu-id="676bf-135">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="676bf-136">roles</span><span class="sxs-lookup"><span data-stu-id="676bf-136">roles</span></span>            | <span data-ttu-id="676bf-137">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="676bf-137">Collection(String)</span></span>                              | <span data-ttu-id="676bf-138">指定授予共享邀请收件人的角色。</span><span class="sxs-lookup"><span data-stu-id="676bf-138">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |
| <span data-ttu-id="676bf-139">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="676bf-139">expirationDateTime</span></span> | <span data-ttu-id="676bf-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="676bf-140">DateTimeOffset</span></span>                       | <span data-ttu-id="676bf-141">指定权限将在其后过期的日期时间。</span><span class="sxs-lookup"><span data-stu-id="676bf-141">Specify the DateTime after which the permission expires.</span></span> <span data-ttu-id="676bf-142">在 OneDrive for business、SharePoint 和 premium 个人 OneDrive 帐户上可用。</span><span class="sxs-lookup"><span data-stu-id="676bf-142">Available on OneDrive for Business, SharePoint, and premium personal OneDrive accounts.</span></span>
| <span data-ttu-id="676bf-143">密码</span><span class="sxs-lookup"><span data-stu-id="676bf-143">password</span></span>           | <span data-ttu-id="676bf-144">String</span><span class="sxs-lookup"><span data-stu-id="676bf-144">String</span></span>                         | <span data-ttu-id="676bf-145">由创建者在邀请上设置的密码。</span><span class="sxs-lookup"><span data-stu-id="676bf-145">The password set on the invite by the creator.</span></span> <span data-ttu-id="676bf-146">可选和 OneDrive 仅个人版</span><span class="sxs-lookup"><span data-stu-id="676bf-146">Optional and OneDrive Personal only</span></span>

## <a name="example"></a><span data-ttu-id="676bf-147">示例</span><span class="sxs-lookup"><span data-stu-id="676bf-147">Example</span></span>

<span data-ttu-id="676bf-148">本示例向电子邮件地址为“ryan@contoso.org”的用户发送共享邀请，其中包含关于协作文件的讯息。</span><span class="sxs-lookup"><span data-stu-id="676bf-148">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="676bf-149">此邀请授予 Ryan 对该文件的读写访问权限。</span><span class="sxs-lookup"><span data-stu-id="676bf-149">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="676bf-150">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="676bf-150">HTTP request</span></span>

<span data-ttu-id="676bf-151">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [permission](../resources/permission.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="676bf-151">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="676bf-152">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="676bf-152">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ],
  "password": "password123",
  "expirationDateTime": "2018-07-15T14:00:00.000Z"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="676bf-153">C#</span><span class="sxs-lookup"><span data-stu-id="676bf-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="676bf-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="676bf-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="676bf-155">目标-C</span><span class="sxs-lookup"><span data-stu-id="676bf-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="676bf-156">响应</span><span class="sxs-lookup"><span data-stu-id="676bf-156">Response</span></span>

<span data-ttu-id="676bf-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="676bf-157">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "hasPassword": true,
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="partial-success-response"></a><span data-ttu-id="676bf-158">部分成功响应</span><span class="sxs-lookup"><span data-stu-id="676bf-158">Partial success response</span></span>

<span data-ttu-id="676bf-159">当邀请多个收件人时, 通知可能会成功, 其他人也会失败。</span><span class="sxs-lookup"><span data-stu-id="676bf-159">When inviting multiple recipients, it's possible for the notification to succeed for some and fail for others.</span></span>
<span data-ttu-id="676bf-160">在这种情况下, 服务将返回 HTTP 状态代码为207的部分成功响应。</span><span class="sxs-lookup"><span data-stu-id="676bf-160">In this case, the service returns a partial success response with an HTTP status code of 207.</span></span>
<span data-ttu-id="676bf-161">当返回部分成功时, 每个失败的收件人的响应将包含`error`一个对象, 其中包含有关出错的信息以及如何修复。</span><span class="sxs-lookup"><span data-stu-id="676bf-161">When partial success is returned, the response for each failed recipient will contain an `error` object with information about what went wrong and how to fix it.</span></span>

<span data-ttu-id="676bf-162">下面的示例展示了部分响应。</span><span class="sxs-lookup"><span data-stu-id="676bf-162">Here is an example of the partial response.</span></span>  

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 207 Multi-Status
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "John Adams",
          "id": "5D8CA5D0-FFF8-4A97-B0A6-8F5AEA339681"
        }
      },
      "id": "1EFG7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "adams@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "error": {
        "code":"notAllowed",
        "message":"Account verification needed to unblock sending emails.",
        "localizedMessage": "Kontobestätigung erforderlich, um das Senden von E-Mails zu entsperren.",
        "fixItUrl":"http://g.live.com/8SESkydrive/VerifyAccount",
        "innererror":{  
          "code":"accountVerificationRequired" 
        }
      }
    },
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ],
      "expirationDateTime": "2018-07-15T14:00:00.000Z"
    }
  ]
}
```
### <a name="sendnotification-errors"></a><span data-ttu-id="676bf-163">SendNotification 错误</span><span class="sxs-lookup"><span data-stu-id="676bf-163">SendNotification errors</span></span>
<span data-ttu-id="676bf-164">以下是在发送通知失败时, 应用可能会在嵌套`innererror`的对象中遇到的一些其他错误。</span><span class="sxs-lookup"><span data-stu-id="676bf-164">The following are some additional errors that your app might encounter within the nested `innererror` objects when sending notification fails.</span></span> <span data-ttu-id="676bf-165">应用程序不需要处理这些。</span><span class="sxs-lookup"><span data-stu-id="676bf-165">Apps are not required to handle these.</span></span>

| <span data-ttu-id="676bf-166">代码</span><span class="sxs-lookup"><span data-stu-id="676bf-166">Code</span></span>                           | <span data-ttu-id="676bf-167">说明</span><span class="sxs-lookup"><span data-stu-id="676bf-167">Description</span></span>
|:-------------------------------|:--------------------------------------------------------------------------------------
| <span data-ttu-id="676bf-168">accountVerificationRequired</span><span class="sxs-lookup"><span data-stu-id="676bf-168">accountVerificationRequired</span></span>    | <span data-ttu-id="676bf-169">若要取消阻止发送通知, 需要进行帐户验证。</span><span class="sxs-lookup"><span data-stu-id="676bf-169">Account verification is required to unblock sending notifications.</span></span>
| <span data-ttu-id="676bf-170">hipCheckRequired</span><span class="sxs-lookup"><span data-stu-id="676bf-170">hipCheckRequired</span></span>               | <span data-ttu-id="676bf-171">需要解决 HIP (主机入侵防护) 检查以取消阻止发送通知。</span><span class="sxs-lookup"><span data-stu-id="676bf-171">Need to solve HIP (Host Intrusion Prevention) check to unblock sending notifications.</span></span>
| <span data-ttu-id="676bf-172">exchangeInvalidUser</span><span class="sxs-lookup"><span data-stu-id="676bf-172">exchangeInvalidUser</span></span>            | <span data-ttu-id="676bf-173">找不到当前用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="676bf-173">Current user's mailbox was not found.</span></span>
| <span data-ttu-id="676bf-174">exchangeOutOfMailboxQuota</span><span class="sxs-lookup"><span data-stu-id="676bf-174">exchangeOutOfMailboxQuota</span></span>      | <span data-ttu-id="676bf-175">配额不足。</span><span class="sxs-lookup"><span data-stu-id="676bf-175">Out of quota.</span></span>
| <span data-ttu-id="676bf-176">exchangeMaxRecipients</span><span class="sxs-lookup"><span data-stu-id="676bf-176">exchangeMaxRecipients</span></span>          | <span data-ttu-id="676bf-177">超过了可以同时发送通知的收件人的最大数量。</span><span class="sxs-lookup"><span data-stu-id="676bf-177">Exceeded maximum number of recipients that can be sent notifications at the same time.</span></span>

><span data-ttu-id="676bf-178">**注意:** 服务可随时添加新的错误代码或停止返回旧的错误代码。</span><span class="sxs-lookup"><span data-stu-id="676bf-178">**Note:** The service can add new error codes or stop returning old ones at any time.</span></span>

## <a name="remarks"></a><span data-ttu-id="676bf-179">注解</span><span class="sxs-lookup"><span data-stu-id="676bf-179">Remarks</span></span>

* <span data-ttu-id="676bf-180">具有 `personal` **driveType**（OneDrive 个人版）的[驱动器](../resources/drive.md)无法创建或修改根 DriveItem 上的权限。</span><span class="sxs-lookup"><span data-stu-id="676bf-180">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="676bf-181">如需可用角色的列表，请参阅[角色枚举](../resources/permission.md#roles-enumeration-values)。</span><span class="sxs-lookup"><span data-stu-id="676bf-181">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="676bf-182">错误响应</span><span class="sxs-lookup"><span data-stu-id="676bf-182">Error responses</span></span>

<span data-ttu-id="676bf-183">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="676bf-183">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
  ]
}
-->
