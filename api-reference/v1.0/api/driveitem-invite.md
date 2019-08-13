---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 发送邀请以访问项目
localization_priority: Normal
ms.prod: sharepoint
description: 发送 DriveItem 的共享邀请。
doc_type: apiPageType
ms.openlocfilehash: 47aa7e49875d4d07ebc8b80a0f86c5939aea13ec
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36375042"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="1d772-103">发送共享邀请</span><span class="sxs-lookup"><span data-stu-id="1d772-103">Send a sharing invitation</span></span>

<span data-ttu-id="1d772-104">发送 **DriveItem** 的共享邀请。</span><span class="sxs-lookup"><span data-stu-id="1d772-104">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="1d772-105">共享邀请向收件人提供权限, 并根据需要向其发送带有[共享链接][]的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="1d772-105">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="1d772-106">权限</span><span class="sxs-lookup"><span data-stu-id="1d772-106">Permissions</span></span>

<span data-ttu-id="1d772-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1d772-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d772-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1d772-109">Permission type</span></span>      | <span data-ttu-id="1d772-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1d772-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d772-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1d772-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1d772-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d772-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1d772-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1d772-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d772-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d772-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1d772-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1d772-115">Application</span></span> | <span data-ttu-id="1d772-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d772-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d772-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d772-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="1d772-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="1d772-118">Request body</span></span>

<span data-ttu-id="1d772-119">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1d772-119">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="1d772-120">参数</span><span class="sxs-lookup"><span data-stu-id="1d772-120">Parameter</span></span>        | <span data-ttu-id="1d772-121">类型</span><span class="sxs-lookup"><span data-stu-id="1d772-121">Type</span></span>                           | <span data-ttu-id="1d772-122">说明</span><span class="sxs-lookup"><span data-stu-id="1d772-122">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="1d772-123">recipients</span><span class="sxs-lookup"><span data-stu-id="1d772-123">recipients</span></span>       | <span data-ttu-id="1d772-124">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="1d772-124">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="1d772-125">将获得访问权限和共享邀请的收件人的集合。</span><span class="sxs-lookup"><span data-stu-id="1d772-125">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="1d772-126">message</span><span class="sxs-lookup"><span data-stu-id="1d772-126">message</span></span>          | <span data-ttu-id="1d772-127">String</span><span class="sxs-lookup"><span data-stu-id="1d772-127">String</span></span>                         | <span data-ttu-id="1d772-p103">共享邀请中包含的纯文本格式的邮件。最大长度为 2000 个字符。</span><span class="sxs-lookup"><span data-stu-id="1d772-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="1d772-130">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="1d772-130">requireSignIn</span></span>    | <span data-ttu-id="1d772-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d772-131">Boolean</span></span>                        | <span data-ttu-id="1d772-132">指定是否需要邀请收件人登录才能查看共享项目。</span><span class="sxs-lookup"><span data-stu-id="1d772-132">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="1d772-133">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="1d772-133">sendInvitation</span></span>   | <span data-ttu-id="1d772-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d772-134">Boolean</span></span>                        | <span data-ttu-id="1d772-135">如果为 true, 则会向收件人发送[共享链接][]。</span><span class="sxs-lookup"><span data-stu-id="1d772-135">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="1d772-136">否则, 将直接授予权限, 而不发送通知。</span><span class="sxs-lookup"><span data-stu-id="1d772-136">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="1d772-137">roles</span><span class="sxs-lookup"><span data-stu-id="1d772-137">roles</span></span>            | <span data-ttu-id="1d772-138">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="1d772-138">Collection(String)</span></span>             | <span data-ttu-id="1d772-139">指定要向共享邀请的收件人授予的角色。</span><span class="sxs-lookup"><span data-stu-id="1d772-139">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="1d772-140">示例</span><span class="sxs-lookup"><span data-stu-id="1d772-140">Example</span></span>

<span data-ttu-id="1d772-141">本示例向电子邮件地址为 "ryan@contoso.com" 的用户发送共享邀请, 并发送一封邮件, 其中包含有关正在合作的文件的消息。</span><span class="sxs-lookup"><span data-stu-id="1d772-141">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="1d772-142">此邀请授予 Ryan 对该文件的读写访问权限。</span><span class="sxs-lookup"><span data-stu-id="1d772-142">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="1d772-143">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1d772-143">HTTP Request</span></span>

<span data-ttu-id="1d772-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [permission](../resources/permission.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="1d772-144">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1d772-145">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1d772-145">HTTP</span></span>](#tab/http)
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
  "roles": [ "write" ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1d772-146">C#</span><span class="sxs-lookup"><span data-stu-id="1d772-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1d772-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d772-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1d772-148">目标-C</span><span class="sxs-lookup"><span data-stu-id="1d772-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="1d772-149">Java</span><span class="sxs-lookup"><span data-stu-id="1d772-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1d772-150">响应</span><span class="sxs-lookup"><span data-stu-id="1d772-150">Response</span></span>

<span data-ttu-id="1d772-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1d772-151">Here is an example of the response.</span></span>

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
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="1d772-152">备注</span><span class="sxs-lookup"><span data-stu-id="1d772-152">Remarks</span></span>

* <span data-ttu-id="1d772-153">具有 `personal` **driveType**（OneDrive 个人版）的[驱动器](../resources/drive.md)无法创建或修改根 DriveItem 上的权限。</span><span class="sxs-lookup"><span data-stu-id="1d772-153">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="1d772-154">如需可用角色的列表，请参阅[角色枚举](../resources/permission.md#roles-enumeration)。</span><span class="sxs-lookup"><span data-stu-id="1d772-154">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="1d772-155">错误响应</span><span class="sxs-lookup"><span data-stu-id="1d772-155">Error Responses</span></span>

<span data-ttu-id="1d772-156">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="1d772-156">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


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
