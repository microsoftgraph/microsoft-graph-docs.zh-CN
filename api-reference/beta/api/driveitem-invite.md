---
author: JeremyKelley
description: 发送 DriveItem 的共享邀请。
ms.date: 09/10/2017
title: 发送访问项目的邀请
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 00252b35b786d467848ed417d9a80dab2b165bc7
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473446"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="c99bd-103">发送共享邀请</span><span class="sxs-lookup"><span data-stu-id="c99bd-103">Send a sharing invitation</span></span>

<span data-ttu-id="c99bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c99bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c99bd-p101">发送 **DriveItem** 的共享邀请。共享邀请为收件人提供权限，也可以选择向收件人发送电子邮件以通知他们项目已共享。</span><span class="sxs-lookup"><span data-stu-id="c99bd-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="c99bd-107">权限</span><span class="sxs-lookup"><span data-stu-id="c99bd-107">Permissions</span></span>

<span data-ttu-id="c99bd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c99bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c99bd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c99bd-110">Permission type</span></span>      | <span data-ttu-id="c99bd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c99bd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c99bd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c99bd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c99bd-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c99bd-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c99bd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c99bd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c99bd-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c99bd-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c99bd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c99bd-116">Application</span></span> | <span data-ttu-id="c99bd-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c99bd-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c99bd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c99bd-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="c99bd-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="c99bd-119">Request body</span></span>

<span data-ttu-id="c99bd-120">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c99bd-120">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="c99bd-121">参数</span><span class="sxs-lookup"><span data-stu-id="c99bd-121">Parameter</span></span>        | <span data-ttu-id="c99bd-122">类型</span><span class="sxs-lookup"><span data-stu-id="c99bd-122">Type</span></span>                                            | <span data-ttu-id="c99bd-123">说明</span><span class="sxs-lookup"><span data-stu-id="c99bd-123">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c99bd-124">recipients</span><span class="sxs-lookup"><span data-stu-id="c99bd-124">recipients</span></span>       | <span data-ttu-id="c99bd-125">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="c99bd-125">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="c99bd-126">将获得访问权限和共享邀请的收件人的集合。</span><span class="sxs-lookup"><span data-stu-id="c99bd-126">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="c99bd-127">message</span><span class="sxs-lookup"><span data-stu-id="c99bd-127">message</span></span>          | <span data-ttu-id="c99bd-128">String</span><span class="sxs-lookup"><span data-stu-id="c99bd-128">String</span></span>                                          | <span data-ttu-id="c99bd-p103">共享邀请中包含的纯文本格式的邮件。最大长度为 2000 个字符。</span><span class="sxs-lookup"><span data-stu-id="c99bd-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="c99bd-131">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="c99bd-131">requireSignIn</span></span>    | <span data-ttu-id="c99bd-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99bd-132">Boolean</span></span>                                         | <span data-ttu-id="c99bd-133">指定邀请的收件人要查看共享项目的登录位置。</span><span class="sxs-lookup"><span data-stu-id="c99bd-133">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="c99bd-134">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="c99bd-134">sendInvitation</span></span>   | <span data-ttu-id="c99bd-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="c99bd-135">Boolean</span></span>                                         | <span data-ttu-id="c99bd-136">指定是否生成电子邮件或帖子 (false)，或是否仅创建权限 (true)。</span><span class="sxs-lookup"><span data-stu-id="c99bd-136">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="c99bd-137">角色</span><span class="sxs-lookup"><span data-stu-id="c99bd-137">roles</span></span>            | <span data-ttu-id="c99bd-138">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="c99bd-138">Collection(String)</span></span>                              | <span data-ttu-id="c99bd-139">指定授予共享邀请收件人的角色。</span><span class="sxs-lookup"><span data-stu-id="c99bd-139">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |
| <span data-ttu-id="c99bd-140">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c99bd-140">expirationDateTime</span></span> | <span data-ttu-id="c99bd-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c99bd-141">DateTimeOffset</span></span>                       | <span data-ttu-id="c99bd-142">指定权限过期后的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c99bd-142">Specify the DateTime after which the permission expires.</span></span> <span data-ttu-id="c99bd-143">在 OneDrive for Business、SharePoint 和高级个人 OneDrive 帐户上可用。</span><span class="sxs-lookup"><span data-stu-id="c99bd-143">Available on OneDrive for Business, SharePoint, and premium personal OneDrive accounts.</span></span>
| <span data-ttu-id="c99bd-144">密码</span><span class="sxs-lookup"><span data-stu-id="c99bd-144">password</span></span>           | <span data-ttu-id="c99bd-145">String</span><span class="sxs-lookup"><span data-stu-id="c99bd-145">String</span></span>                         | <span data-ttu-id="c99bd-146">创建者在邀请上设置的密码。</span><span class="sxs-lookup"><span data-stu-id="c99bd-146">The password set on the invite by the creator.</span></span> <span data-ttu-id="c99bd-147">可选，仅 OneDrive 个人</span><span class="sxs-lookup"><span data-stu-id="c99bd-147">Optional and OneDrive Personal only</span></span>

## <a name="example"></a><span data-ttu-id="c99bd-148">示例</span><span class="sxs-lookup"><span data-stu-id="c99bd-148">Example</span></span>

<span data-ttu-id="c99bd-149">本示例向电子邮件地址为“ryan@contoso.org”的用户发送共享邀请，其中包含关于协作文件的讯息。</span><span class="sxs-lookup"><span data-stu-id="c99bd-149">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="c99bd-150">此邀请授予 Ryan 对该文件的读写访问权限。</span><span class="sxs-lookup"><span data-stu-id="c99bd-150">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="c99bd-151">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c99bd-151">HTTP request</span></span>

<span data-ttu-id="c99bd-152">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [permission](../resources/permission.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="c99bd-152">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="http"></a>[<span data-ttu-id="c99bd-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="c99bd-153">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c99bd-154">C#</span><span class="sxs-lookup"><span data-stu-id="c99bd-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c99bd-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c99bd-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c99bd-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c99bd-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c99bd-157">Java</span><span class="sxs-lookup"><span data-stu-id="c99bd-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c99bd-158">响应</span><span class="sxs-lookup"><span data-stu-id="c99bd-158">Response</span></span>

<span data-ttu-id="c99bd-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c99bd-159">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
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
### <a name="partial-success-response"></a><span data-ttu-id="c99bd-160">部分成功响应</span><span class="sxs-lookup"><span data-stu-id="c99bd-160">Partial success response</span></span>

<span data-ttu-id="c99bd-161">邀请多个收件人时，某些收件人的通知可能会成功，而其他收件人可能会失败。</span><span class="sxs-lookup"><span data-stu-id="c99bd-161">When inviting multiple recipients, it's possible for the notification to succeed for some and fail for others.</span></span>
<span data-ttu-id="c99bd-162">在这种情况下，服务返回 HTTP 状态代码为 207 的部分成功响应。</span><span class="sxs-lookup"><span data-stu-id="c99bd-162">In this case, the service returns a partial success response with an HTTP status code of 207.</span></span>
<span data-ttu-id="c99bd-163">返回部分成功后，每个失败收件人的响应将包含一个对象，其中包含有关出错内容以及如何 `error` 修复它的信息。</span><span class="sxs-lookup"><span data-stu-id="c99bd-163">When partial success is returned, the response for each failed recipient will contain an `error` object with information about what went wrong and how to fix it.</span></span>

<span data-ttu-id="c99bd-164">下面是部分响应的示例。</span><span class="sxs-lookup"><span data-stu-id="c99bd-164">Here is an example of the partial response.</span></span>  

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
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
### <a name="sendnotification-errors"></a><span data-ttu-id="c99bd-165">SendNotification 错误</span><span class="sxs-lookup"><span data-stu-id="c99bd-165">SendNotification errors</span></span>
<span data-ttu-id="c99bd-166">下面是应用在发送通知失败时在嵌套对象中 `innererror` 可能遇到的一些其他错误。</span><span class="sxs-lookup"><span data-stu-id="c99bd-166">The following are some additional errors that your app might encounter within the nested `innererror` objects when sending notification fails.</span></span> <span data-ttu-id="c99bd-167">应用不需要处理它们。</span><span class="sxs-lookup"><span data-stu-id="c99bd-167">Apps are not required to handle these.</span></span>

| <span data-ttu-id="c99bd-168">代码</span><span class="sxs-lookup"><span data-stu-id="c99bd-168">Code</span></span>                           | <span data-ttu-id="c99bd-169">说明</span><span class="sxs-lookup"><span data-stu-id="c99bd-169">Description</span></span>
|:-------------------------------|:--------------------------------------------------------------------------------------
| <span data-ttu-id="c99bd-170">accountVerificationRequired</span><span class="sxs-lookup"><span data-stu-id="c99bd-170">accountVerificationRequired</span></span>    | <span data-ttu-id="c99bd-171">若要取消阻止发送通知，需要帐户验证。</span><span class="sxs-lookup"><span data-stu-id="c99bd-171">Account verification is required to unblock sending notifications.</span></span>
| <span data-ttu-id="c99bd-172">hipCheckRequired</span><span class="sxs-lookup"><span data-stu-id="c99bd-172">hipCheckRequired</span></span>               | <span data-ttu-id="c99bd-173">需要解决 HIP (主机入侵防护) 阻止发送通知。</span><span class="sxs-lookup"><span data-stu-id="c99bd-173">Need to solve HIP (Host Intrusion Prevention) check to unblock sending notifications.</span></span>
| <span data-ttu-id="c99bd-174">exchangeInvalidUser</span><span class="sxs-lookup"><span data-stu-id="c99bd-174">exchangeInvalidUser</span></span>            | <span data-ttu-id="c99bd-175">未找到当前用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="c99bd-175">Current user's mailbox was not found.</span></span>
| <span data-ttu-id="c99bd-176">exchangeOutOfMailboxQuota</span><span class="sxs-lookup"><span data-stu-id="c99bd-176">exchangeOutOfMailboxQuota</span></span>      | <span data-ttu-id="c99bd-177">超出配额。</span><span class="sxs-lookup"><span data-stu-id="c99bd-177">Out of quota.</span></span>
| <span data-ttu-id="c99bd-178">exchangeMaxRecipients</span><span class="sxs-lookup"><span data-stu-id="c99bd-178">exchangeMaxRecipients</span></span>          | <span data-ttu-id="c99bd-179">超出了可以同时发送通知的最大收件人数。</span><span class="sxs-lookup"><span data-stu-id="c99bd-179">Exceeded maximum number of recipients that can be sent notifications at the same time.</span></span>

><span data-ttu-id="c99bd-180">**注意：** 该服务可以添加新的错误代码或随时停止返回旧的错误代码。</span><span class="sxs-lookup"><span data-stu-id="c99bd-180">**Note:** The service can add new error codes or stop returning old ones at any time.</span></span>

## <a name="remarks"></a><span data-ttu-id="c99bd-181">备注</span><span class="sxs-lookup"><span data-stu-id="c99bd-181">Remarks</span></span>

* <span data-ttu-id="c99bd-182">**driveType** 为 `personal` 的 [Drives](../resources/drive.md)（OneDrive 个人版）无法创建或修改根 DriveItem 上的权限。</span><span class="sxs-lookup"><span data-stu-id="c99bd-182">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="c99bd-183">有关可用角色的列表，请参阅 [角色属性值](../resources/permission.md#roles-property-values)。</span><span class="sxs-lookup"><span data-stu-id="c99bd-183">For a list of available roles, see [roles property values](../resources/permission.md#roles-property-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="c99bd-184">错误响应</span><span class="sxs-lookup"><span data-stu-id="c99bd-184">Error responses</span></span>

<span data-ttu-id="c99bd-185">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="c99bd-185">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


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


