---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 发送邀请以访问项目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ab9f23961733a37082f48c111974c2116462aeee
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445420"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="295d5-102">发送共享邀请</span><span class="sxs-lookup"><span data-stu-id="295d5-102">Send a sharing invitation</span></span>

<span data-ttu-id="295d5-103">发送 **DriveItem** 的共享邀请。</span><span class="sxs-lookup"><span data-stu-id="295d5-103">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="295d5-104">共享邀请向收件人提供权限, 并根据需要向其发送带有[共享链接][]的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="295d5-104">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="295d5-105">权限</span><span class="sxs-lookup"><span data-stu-id="295d5-105">Permissions</span></span>

<span data-ttu-id="295d5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="295d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="295d5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="295d5-108">Permission type</span></span>      | <span data-ttu-id="295d5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="295d5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="295d5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="295d5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="295d5-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="295d5-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="295d5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="295d5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="295d5-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="295d5-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="295d5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="295d5-114">Application</span></span> | <span data-ttu-id="295d5-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="295d5-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="295d5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="295d5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="295d5-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="295d5-117">Request body</span></span>

<span data-ttu-id="295d5-118">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="295d5-118">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="295d5-119">参数</span><span class="sxs-lookup"><span data-stu-id="295d5-119">Parameter</span></span>        | <span data-ttu-id="295d5-120">类型</span><span class="sxs-lookup"><span data-stu-id="295d5-120">Type</span></span>                           | <span data-ttu-id="295d5-121">说明</span><span class="sxs-lookup"><span data-stu-id="295d5-121">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="295d5-122">recipients</span><span class="sxs-lookup"><span data-stu-id="295d5-122">recipients</span></span>       | <span data-ttu-id="295d5-123">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="295d5-123">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="295d5-124">将获得访问权限和共享邀请的收件人的集合。</span><span class="sxs-lookup"><span data-stu-id="295d5-124">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="295d5-125">message</span><span class="sxs-lookup"><span data-stu-id="295d5-125">message</span></span>          | <span data-ttu-id="295d5-126">String</span><span class="sxs-lookup"><span data-stu-id="295d5-126">String</span></span>                         | <span data-ttu-id="295d5-p103">共享邀请中包含的纯文本格式的邮件。最大长度为 2000 个字符。</span><span class="sxs-lookup"><span data-stu-id="295d5-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="295d5-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="295d5-129">requireSignIn</span></span>    | <span data-ttu-id="295d5-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="295d5-130">Boolean</span></span>                        | <span data-ttu-id="295d5-131">指定是否需要邀请收件人登录才能查看共享项目。</span><span class="sxs-lookup"><span data-stu-id="295d5-131">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="295d5-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="295d5-132">sendInvitation</span></span>   | <span data-ttu-id="295d5-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="295d5-133">Boolean</span></span>                        | <span data-ttu-id="295d5-134">如果为 true, 则会向收件人发送[共享链接][]。</span><span class="sxs-lookup"><span data-stu-id="295d5-134">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="295d5-135">否则, 将直接授予权限, 而不发送通知。</span><span class="sxs-lookup"><span data-stu-id="295d5-135">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="295d5-136">roles</span><span class="sxs-lookup"><span data-stu-id="295d5-136">roles</span></span>            | <span data-ttu-id="295d5-137">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="295d5-137">Collection(String)</span></span>             | <span data-ttu-id="295d5-138">指定要向共享邀请的收件人授予的角色。</span><span class="sxs-lookup"><span data-stu-id="295d5-138">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="295d5-139">示例</span><span class="sxs-lookup"><span data-stu-id="295d5-139">Example</span></span>

<span data-ttu-id="295d5-140">本示例向电子邮件地址为 "ryan@contoso.com" 的用户发送共享邀请, 并发送一封邮件, 其中包含有关正在合作的文件的消息。</span><span class="sxs-lookup"><span data-stu-id="295d5-140">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="295d5-141">此邀请授予 Ryan 对该文件的读写访问权限。</span><span class="sxs-lookup"><span data-stu-id="295d5-141">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="295d5-142">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="295d5-142">HTTP Request</span></span>

<span data-ttu-id="295d5-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [permission](../resources/permission.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="295d5-143">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="295d5-144">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="295d5-144">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="295d5-145">C#</span><span class="sxs-lookup"><span data-stu-id="295d5-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="295d5-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="295d5-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="295d5-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="295d5-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="295d5-148">响应</span><span class="sxs-lookup"><span data-stu-id="295d5-148">Response</span></span>

<span data-ttu-id="295d5-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="295d5-149">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="295d5-150">备注</span><span class="sxs-lookup"><span data-stu-id="295d5-150">Remarks</span></span>

* <span data-ttu-id="295d5-151">具有 `personal` **driveType**（OneDrive 个人版）的[驱动器](../resources/drive.md)无法创建或修改根 DriveItem 上的权限。</span><span class="sxs-lookup"><span data-stu-id="295d5-151">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="295d5-152">如需可用角色的列表，请参阅[角色枚举](../resources/permission.md#roles-enumeration)。</span><span class="sxs-lookup"><span data-stu-id="295d5-152">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="295d5-153">错误响应</span><span class="sxs-lookup"><span data-stu-id="295d5-153">Error Responses</span></span>

<span data-ttu-id="295d5-154">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="295d5-154">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


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
