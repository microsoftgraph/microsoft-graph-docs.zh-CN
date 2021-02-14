---
author: JeremyKelley
ms.date: 09/10/2017
title: 发送访问项目的邀请
localization_priority: Normal
ms.prod: sharepoint
description: 发送 driveItem 的共享邀请。
doc_type: apiPageType
ms.openlocfilehash: e514fbd3b8f79d3696f894a6b15ad55055137b70
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240288"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="84b4f-103">发送共享邀请</span><span class="sxs-lookup"><span data-stu-id="84b4f-103">Send a sharing invitation</span></span>

<span data-ttu-id="84b4f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84b4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="84b4f-105">发送 **driveItem** 的共享邀请。</span><span class="sxs-lookup"><span data-stu-id="84b4f-105">Sends a sharing invitation for a **driveItem**.</span></span>
<span data-ttu-id="84b4f-106">共享邀请向收件人提供权限，并选择性地向其发送带[共享链接][]的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="84b4f-106">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="84b4f-107">权限</span><span class="sxs-lookup"><span data-stu-id="84b4f-107">Permissions</span></span>

<span data-ttu-id="84b4f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84b4f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84b4f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="84b4f-110">Permission type</span></span>      | <span data-ttu-id="84b4f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="84b4f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84b4f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84b4f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="84b4f-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84b4f-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="84b4f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84b4f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84b4f-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84b4f-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="84b4f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="84b4f-116">Application</span></span> | <span data-ttu-id="84b4f-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84b4f-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84b4f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84b4f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="84b4f-119">请求正文</span><span class="sxs-lookup"><span data-stu-id="84b4f-119">Request body</span></span>

<span data-ttu-id="84b4f-120">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="84b4f-120">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

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

| <span data-ttu-id="84b4f-121">参数</span><span class="sxs-lookup"><span data-stu-id="84b4f-121">Parameter</span></span>        | <span data-ttu-id="84b4f-122">类型</span><span class="sxs-lookup"><span data-stu-id="84b4f-122">Type</span></span>                           | <span data-ttu-id="84b4f-123">说明</span><span class="sxs-lookup"><span data-stu-id="84b4f-123">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="84b4f-124">recipients</span><span class="sxs-lookup"><span data-stu-id="84b4f-124">recipients</span></span>       | <span data-ttu-id="84b4f-125">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="84b4f-125">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="84b4f-126">将获得访问权限和共享邀请的收件人的集合。</span><span class="sxs-lookup"><span data-stu-id="84b4f-126">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="84b4f-127">message</span><span class="sxs-lookup"><span data-stu-id="84b4f-127">message</span></span>          | <span data-ttu-id="84b4f-128">String</span><span class="sxs-lookup"><span data-stu-id="84b4f-128">String</span></span>                         | <span data-ttu-id="84b4f-p103">共享邀请中包含的纯文本格式的邮件。最大长度为 2000 个字符。</span><span class="sxs-lookup"><span data-stu-id="84b4f-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="84b4f-131">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="84b4f-131">requireSignIn</span></span>    | <span data-ttu-id="84b4f-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b4f-132">Boolean</span></span>                        | <span data-ttu-id="84b4f-133">指定邀请的收件人是否需要登录才能查看共享项。</span><span class="sxs-lookup"><span data-stu-id="84b4f-133">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="84b4f-134">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="84b4f-134">sendInvitation</span></span>   | <span data-ttu-id="84b4f-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="84b4f-135">Boolean</span></span>                        | <span data-ttu-id="84b4f-136">如果为 true，则向收件人发送[共享链接][]。</span><span class="sxs-lookup"><span data-stu-id="84b4f-136">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="84b4f-137">否则，直接授予权限，而不发送通知。</span><span class="sxs-lookup"><span data-stu-id="84b4f-137">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="84b4f-138">角色</span><span class="sxs-lookup"><span data-stu-id="84b4f-138">roles</span></span>            | <span data-ttu-id="84b4f-139">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="84b4f-139">Collection(String)</span></span>             | <span data-ttu-id="84b4f-140">指定要授予共享邀请收件人的角色。</span><span class="sxs-lookup"><span data-stu-id="84b4f-140">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>
| <span data-ttu-id="84b4f-141">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="84b4f-141">expirationDateTime</span></span> | <span data-ttu-id="84b4f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84b4f-142">DateTimeOffset</span></span>                       | <span data-ttu-id="84b4f-143">指定权限过期后的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="84b4f-143">Specify the DateTime after which the permission expires.</span></span> <span data-ttu-id="84b4f-144">在 OneDrive for Business、SharePoint 和高级个人 OneDrive 帐户上可用。</span><span class="sxs-lookup"><span data-stu-id="84b4f-144">Available on OneDrive for Business, SharePoint, and premium personal OneDrive accounts.</span></span>
| <span data-ttu-id="84b4f-145">密码</span><span class="sxs-lookup"><span data-stu-id="84b4f-145">password</span></span>           | <span data-ttu-id="84b4f-146">String</span><span class="sxs-lookup"><span data-stu-id="84b4f-146">String</span></span>                         | <span data-ttu-id="84b4f-147">创建者在邀请上设置的密码。</span><span class="sxs-lookup"><span data-stu-id="84b4f-147">The password set on the invite by the creator.</span></span> <span data-ttu-id="84b4f-148">可选，仅 OneDrive 个人。</span><span class="sxs-lookup"><span data-stu-id="84b4f-148">Optional and OneDrive Personal only.</span></span>

## <a name="example"></a><span data-ttu-id="84b4f-149">示例</span><span class="sxs-lookup"><span data-stu-id="84b4f-149">Example</span></span>

<span data-ttu-id="84b4f-150">本示例向电子邮件地址为“ryan@contoso.com”的用户发送共享邀请，其中包含关于协作文件的讯息。</span><span class="sxs-lookup"><span data-stu-id="84b4f-150">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="84b4f-151">此邀请授予 Ryan 对该文件的读写访问权限。</span><span class="sxs-lookup"><span data-stu-id="84b4f-151">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="84b4f-152">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84b4f-152">HTTP request</span></span>

<span data-ttu-id="84b4f-153">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [permission](../resources/permission.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="84b4f-153">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="http"></a>[<span data-ttu-id="84b4f-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="84b4f-154">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.com"
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
# <a name="c"></a>[<span data-ttu-id="84b4f-155">C#</span><span class="sxs-lookup"><span data-stu-id="84b4f-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84b4f-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84b4f-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84b4f-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84b4f-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84b4f-158">Java</span><span class="sxs-lookup"><span data-stu-id="84b4f-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="84b4f-159">响应</span><span class="sxs-lookup"><span data-stu-id="84b4f-159">Response</span></span>

<span data-ttu-id="84b4f-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="84b4f-160">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="84b4f-161">备注</span><span class="sxs-lookup"><span data-stu-id="84b4f-161">Remarks</span></span>

* <span data-ttu-id="84b4f-162">**driveType** 为 `personal` 的 [Drives](../resources/drive.md)（OneDrive 个人版）无法创建或修改根 DriveItem 上的权限。</span><span class="sxs-lookup"><span data-stu-id="84b4f-162">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="84b4f-163">有关可用角色的列表，请参阅 [角色属性值](../resources/permission.md#roles-property-values)。</span><span class="sxs-lookup"><span data-stu-id="84b4f-163">For a list of available roles, see [roles property values](../resources/permission.md#roles-property-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="84b4f-164">错误响应</span><span class="sxs-lookup"><span data-stu-id="84b4f-164">Error responses</span></span>

<span data-ttu-id="84b4f-165">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="84b4f-165">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[共享链接]: ../resources/permission.md#sharing-links
[sharing link]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
  ]
} -->

