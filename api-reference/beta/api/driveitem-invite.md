---
author: JeremyKelley
description: 发送 DriveItem 的共享邀请。
ms.date: 09/10/2017
title: 发送邀请以访问项目
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: fdcae44f4d9be14fee4d9da81a96cc9c063ab061
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982023"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="ba48c-103">发送共享邀请</span><span class="sxs-lookup"><span data-stu-id="ba48c-103">Send a sharing invitation</span></span>

<span data-ttu-id="ba48c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba48c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba48c-p101">发送 **DriveItem** 的共享邀请。共享邀请为收件人提供权限，也可以选择向收件人发送电子邮件以通知他们项目已共享。</span><span class="sxs-lookup"><span data-stu-id="ba48c-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba48c-107">权限</span><span class="sxs-lookup"><span data-stu-id="ba48c-107">Permissions</span></span>

<span data-ttu-id="ba48c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ba48c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba48c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba48c-110">Permission type</span></span>      | <span data-ttu-id="ba48c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba48c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba48c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba48c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ba48c-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba48c-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba48c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba48c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba48c-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba48c-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba48c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba48c-116">Application</span></span> | <span data-ttu-id="ba48c-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba48c-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba48c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba48c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="ba48c-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba48c-119">Request body</span></span>

<span data-ttu-id="ba48c-120">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ba48c-120">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="ba48c-121">参数</span><span class="sxs-lookup"><span data-stu-id="ba48c-121">Parameter</span></span>        | <span data-ttu-id="ba48c-122">类型</span><span class="sxs-lookup"><span data-stu-id="ba48c-122">Type</span></span>                                            | <span data-ttu-id="ba48c-123">说明</span><span class="sxs-lookup"><span data-stu-id="ba48c-123">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ba48c-124">recipients</span><span class="sxs-lookup"><span data-stu-id="ba48c-124">recipients</span></span>       | <span data-ttu-id="ba48c-125">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="ba48c-125">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="ba48c-126">将获得访问权限和共享邀请的收件人的集合。</span><span class="sxs-lookup"><span data-stu-id="ba48c-126">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="ba48c-127">message</span><span class="sxs-lookup"><span data-stu-id="ba48c-127">message</span></span>          | <span data-ttu-id="ba48c-128">String</span><span class="sxs-lookup"><span data-stu-id="ba48c-128">String</span></span>                                          | <span data-ttu-id="ba48c-p103">共享邀请中包含的纯文本格式的邮件。最大长度为 2000 个字符。</span><span class="sxs-lookup"><span data-stu-id="ba48c-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="ba48c-131">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="ba48c-131">requireSignIn</span></span>    | <span data-ttu-id="ba48c-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba48c-132">Boolean</span></span>                                         | <span data-ttu-id="ba48c-133">指定邀请的收件人要查看共享项目的登录位置。</span><span class="sxs-lookup"><span data-stu-id="ba48c-133">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="ba48c-134">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="ba48c-134">sendInvitation</span></span>   | <span data-ttu-id="ba48c-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba48c-135">Boolean</span></span>                                         | <span data-ttu-id="ba48c-136">指定是否生成电子邮件或帖子 (false)，或是否仅创建权限 (true)。</span><span class="sxs-lookup"><span data-stu-id="ba48c-136">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="ba48c-137">角色</span><span class="sxs-lookup"><span data-stu-id="ba48c-137">roles</span></span>            | <span data-ttu-id="ba48c-138">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="ba48c-138">Collection(String)</span></span>                              | <span data-ttu-id="ba48c-139">指定授予共享邀请收件人的角色。</span><span class="sxs-lookup"><span data-stu-id="ba48c-139">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |
| <span data-ttu-id="ba48c-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ba48c-140">expirationDateTime</span></span> | <span data-ttu-id="ba48c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba48c-141">DateTimeOffset</span></span>                       | <span data-ttu-id="ba48c-142">指定权限将在其后过期的日期时间。</span><span class="sxs-lookup"><span data-stu-id="ba48c-142">Specify the DateTime after which the permission expires.</span></span> <span data-ttu-id="ba48c-143">在 OneDrive for business、SharePoint 和 premium 个人 OneDrive 帐户上可用。</span><span class="sxs-lookup"><span data-stu-id="ba48c-143">Available on OneDrive for Business, SharePoint, and premium personal OneDrive accounts.</span></span>
| <span data-ttu-id="ba48c-144">密码</span><span class="sxs-lookup"><span data-stu-id="ba48c-144">password</span></span>           | <span data-ttu-id="ba48c-145">String</span><span class="sxs-lookup"><span data-stu-id="ba48c-145">String</span></span>                         | <span data-ttu-id="ba48c-146">由创建者在邀请上设置的密码。</span><span class="sxs-lookup"><span data-stu-id="ba48c-146">The password set on the invite by the creator.</span></span> <span data-ttu-id="ba48c-147">可选和 OneDrive 仅个人版</span><span class="sxs-lookup"><span data-stu-id="ba48c-147">Optional and OneDrive Personal only</span></span>

## <a name="example"></a><span data-ttu-id="ba48c-148">示例</span><span class="sxs-lookup"><span data-stu-id="ba48c-148">Example</span></span>

<span data-ttu-id="ba48c-149">本示例向电子邮件地址为“ryan@contoso.org”的用户发送共享邀请，其中包含关于协作文件的讯息。</span><span class="sxs-lookup"><span data-stu-id="ba48c-149">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="ba48c-150">此邀请授予 Ryan 对该文件的读写访问权限。</span><span class="sxs-lookup"><span data-stu-id="ba48c-150">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="ba48c-151">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba48c-151">HTTP request</span></span>

<span data-ttu-id="ba48c-152">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [permission](../resources/permission.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="ba48c-152">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="http"></a>[<span data-ttu-id="ba48c-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba48c-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="ba48c-154">C#</span><span class="sxs-lookup"><span data-stu-id="ba48c-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ba48c-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba48c-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ba48c-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba48c-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ba48c-157">响应</span><span class="sxs-lookup"><span data-stu-id="ba48c-157">Response</span></span>

<span data-ttu-id="ba48c-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ba48c-158">Here is an example of the response.</span></span>

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
### <a name="partial-success-response"></a><span data-ttu-id="ba48c-159">部分成功响应</span><span class="sxs-lookup"><span data-stu-id="ba48c-159">Partial success response</span></span>

<span data-ttu-id="ba48c-160">当邀请多个收件人时，通知可能会成功，其他人也会失败。</span><span class="sxs-lookup"><span data-stu-id="ba48c-160">When inviting multiple recipients, it's possible for the notification to succeed for some and fail for others.</span></span>
<span data-ttu-id="ba48c-161">在这种情况下，服务将返回 HTTP 状态代码为207的部分成功响应。</span><span class="sxs-lookup"><span data-stu-id="ba48c-161">In this case, the service returns a partial success response with an HTTP status code of 207.</span></span>
<span data-ttu-id="ba48c-162">当返回部分成功时，每个失败的收件人的响应将包含一个对象，其中包含有关出错的 `error` 信息以及如何修复。</span><span class="sxs-lookup"><span data-stu-id="ba48c-162">When partial success is returned, the response for each failed recipient will contain an `error` object with information about what went wrong and how to fix it.</span></span>

<span data-ttu-id="ba48c-163">下面的示例展示了部分响应。</span><span class="sxs-lookup"><span data-stu-id="ba48c-163">Here is an example of the partial response.</span></span>  

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
### <a name="sendnotification-errors"></a><span data-ttu-id="ba48c-164">SendNotification 错误</span><span class="sxs-lookup"><span data-stu-id="ba48c-164">SendNotification errors</span></span>
<span data-ttu-id="ba48c-165">以下是在 `innererror` 发送通知失败时，应用可能会在嵌套的对象中遇到的一些其他错误。</span><span class="sxs-lookup"><span data-stu-id="ba48c-165">The following are some additional errors that your app might encounter within the nested `innererror` objects when sending notification fails.</span></span> <span data-ttu-id="ba48c-166">应用程序不需要处理这些。</span><span class="sxs-lookup"><span data-stu-id="ba48c-166">Apps are not required to handle these.</span></span>

| <span data-ttu-id="ba48c-167">代码</span><span class="sxs-lookup"><span data-stu-id="ba48c-167">Code</span></span>                           | <span data-ttu-id="ba48c-168">说明</span><span class="sxs-lookup"><span data-stu-id="ba48c-168">Description</span></span>
|:-------------------------------|:--------------------------------------------------------------------------------------
| <span data-ttu-id="ba48c-169">accountVerificationRequired</span><span class="sxs-lookup"><span data-stu-id="ba48c-169">accountVerificationRequired</span></span>    | <span data-ttu-id="ba48c-170">若要取消阻止发送通知，需要进行帐户验证。</span><span class="sxs-lookup"><span data-stu-id="ba48c-170">Account verification is required to unblock sending notifications.</span></span>
| <span data-ttu-id="ba48c-171">hipCheckRequired</span><span class="sxs-lookup"><span data-stu-id="ba48c-171">hipCheckRequired</span></span>               | <span data-ttu-id="ba48c-172">需要解决 HIP (主机入侵防护) 检查以取消阻止发送通知。</span><span class="sxs-lookup"><span data-stu-id="ba48c-172">Need to solve HIP (Host Intrusion Prevention) check to unblock sending notifications.</span></span>
| <span data-ttu-id="ba48c-173">exchangeInvalidUser</span><span class="sxs-lookup"><span data-stu-id="ba48c-173">exchangeInvalidUser</span></span>            | <span data-ttu-id="ba48c-174">找不到当前用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="ba48c-174">Current user's mailbox was not found.</span></span>
| <span data-ttu-id="ba48c-175">exchangeOutOfMailboxQuota</span><span class="sxs-lookup"><span data-stu-id="ba48c-175">exchangeOutOfMailboxQuota</span></span>      | <span data-ttu-id="ba48c-176">配额不足。</span><span class="sxs-lookup"><span data-stu-id="ba48c-176">Out of quota.</span></span>
| <span data-ttu-id="ba48c-177">exchangeMaxRecipients</span><span class="sxs-lookup"><span data-stu-id="ba48c-177">exchangeMaxRecipients</span></span>          | <span data-ttu-id="ba48c-178">超过了可以同时发送通知的收件人的最大数量。</span><span class="sxs-lookup"><span data-stu-id="ba48c-178">Exceeded maximum number of recipients that can be sent notifications at the same time.</span></span>

><span data-ttu-id="ba48c-179">**注意：** 服务可随时添加新的错误代码或停止返回旧的错误代码。</span><span class="sxs-lookup"><span data-stu-id="ba48c-179">**Note:** The service can add new error codes or stop returning old ones at any time.</span></span>

## <a name="remarks"></a><span data-ttu-id="ba48c-180">备注</span><span class="sxs-lookup"><span data-stu-id="ba48c-180">Remarks</span></span>

* <span data-ttu-id="ba48c-181">**driveType** 为 `personal` 的 [Drives](../resources/drive.md)（OneDrive 个人版）无法创建或修改根 DriveItem 上的权限。</span><span class="sxs-lookup"><span data-stu-id="ba48c-181">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="ba48c-182">有关可用角色的列表，请参阅 [roles 属性值](../resources/permission.md#roles-property-values)。</span><span class="sxs-lookup"><span data-stu-id="ba48c-182">For a list of available roles, see [roles property values](../resources/permission.md#roles-property-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="ba48c-183">错误响应</span><span class="sxs-lookup"><span data-stu-id="ba48c-183">Error responses</span></span>

<span data-ttu-id="ba48c-184">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="ba48c-184">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


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


