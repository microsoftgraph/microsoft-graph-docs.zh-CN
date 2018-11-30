---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 发送访问项的邀请
ms.openlocfilehash: db089fcd0a3f948d8e43f366a4e6674c2505fa2d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008590"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="5c5f8-102">发送共享邀请</span><span class="sxs-lookup"><span data-stu-id="5c5f8-102">Send a sharing invitation</span></span>

<span data-ttu-id="5c5f8-103">为**DriveItem**发送共享邀请。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-103">Sends a sharing invitation for a **DriveItem**.</span></span>
<span data-ttu-id="5c5f8-104">共享邀请提供给收件人的权限，并 （可选） 将其发送电子邮件与[共享链接][]。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-104">A sharing invitation provides permissions to the recipients and optionally sends them an email with a [sharing link][].</span></span>

## <a name="permissions"></a><span data-ttu-id="5c5f8-105">权限</span><span class="sxs-lookup"><span data-stu-id="5c5f8-105">Permissions</span></span>

<span data-ttu-id="5c5f8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c5f8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c5f8-108">Permission type</span></span>      | <span data-ttu-id="5c5f8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c5f8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c5f8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c5f8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5c5f8-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5f8-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c5f8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c5f8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c5f8-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5f8-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5c5f8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c5f8-114">Application</span></span> | <span data-ttu-id="5c5f8-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5f8-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c5f8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c5f8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="5c5f8-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c5f8-117">Request body</span></span>

<span data-ttu-id="5c5f8-118">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-118">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="5c5f8-119">参数</span><span class="sxs-lookup"><span data-stu-id="5c5f8-119">Parameter</span></span>        | <span data-ttu-id="5c5f8-120">类型</span><span class="sxs-lookup"><span data-stu-id="5c5f8-120">Type</span></span>                           | <span data-ttu-id="5c5f8-121">说明</span><span class="sxs-lookup"><span data-stu-id="5c5f8-121">Description</span></span>
|:-----------------|:-------------------------------|:-------------------------
| <span data-ttu-id="5c5f8-122">recipients</span><span class="sxs-lookup"><span data-stu-id="5c5f8-122">recipients</span></span>       | <span data-ttu-id="5c5f8-123">Collection([DriveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="5c5f8-123">Collection([DriveRecipient][])</span></span> | <span data-ttu-id="5c5f8-124">将获得访问权限和共享邀请的收件人的集合。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-124">A collection of recipients who will receive access and the sharing invitation.</span></span>
| <span data-ttu-id="5c5f8-125">message</span><span class="sxs-lookup"><span data-stu-id="5c5f8-125">message</span></span>          | <span data-ttu-id="5c5f8-126">字符串</span><span class="sxs-lookup"><span data-stu-id="5c5f8-126">String</span></span>                         | <span data-ttu-id="5c5f8-p103">共享邀请中包含的纯文本格式的邮件。最大长度为 2000 个字符。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>
| <span data-ttu-id="5c5f8-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="5c5f8-129">requireSignIn</span></span>    | <span data-ttu-id="5c5f8-130">布尔</span><span class="sxs-lookup"><span data-stu-id="5c5f8-130">Boolean</span></span>                        | <span data-ttu-id="5c5f8-131">指定是否需要邀请的收件人来登录以查看共享的项目。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-131">Specifies whether the recipient of the invitation is required to sign-in to view the shared item.</span></span>
| <span data-ttu-id="5c5f8-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="5c5f8-132">sendInvitation</span></span>   | <span data-ttu-id="5c5f8-133">布尔</span><span class="sxs-lookup"><span data-stu-id="5c5f8-133">Boolean</span></span>                        | <span data-ttu-id="5c5f8-134">如果为 true，则[共享链接][]发送给收件人。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-134">If true, a [sharing link][] is sent to the recipient.</span></span> <span data-ttu-id="5c5f8-135">否则，直接而发送通知不授予权限。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-135">Otherwise, a permission is granted directly without sending a notification.</span></span>
| <span data-ttu-id="5c5f8-136">roles</span><span class="sxs-lookup"><span data-stu-id="5c5f8-136">roles</span></span>            | <span data-ttu-id="5c5f8-137">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="5c5f8-137">Collection(String)</span></span>             | <span data-ttu-id="5c5f8-138">指定要授予共享邀请的收件人的角色。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-138">Specify the roles that are to be granted to the recipients of the sharing invitation.</span></span>

## <a name="example"></a><span data-ttu-id="5c5f8-139">示例</span><span class="sxs-lookup"><span data-stu-id="5c5f8-139">Example</span></span>

<span data-ttu-id="5c5f8-140">本示例将对电子邮件地址"ryan@contoso.com"一条消息的用户共享邀请发送关于合作完成了文件。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-140">This example sends a sharing invitation to a user with email address "ryan@contoso.com" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="5c5f8-141">此邀请授予 Ryan 对该文件的读写访问权限。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-141">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="5c5f8-142">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c5f8-142">HTTP Request</span></span>

<span data-ttu-id="5c5f8-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [permission](../resources/permission.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-143">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

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

### <a name="response"></a><span data-ttu-id="5c5f8-144">响应</span><span class="sxs-lookup"><span data-stu-id="5c5f8-144">Response</span></span>

<span data-ttu-id="5c5f8-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-145">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="5c5f8-146">备注</span><span class="sxs-lookup"><span data-stu-id="5c5f8-146">Remarks</span></span>

* <span data-ttu-id="5c5f8-147">具有 `personal` **driveType**（OneDrive 个人版）的[驱动器](../resources/drive.md)无法创建或修改根 DriveItem 上的权限。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-147">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="5c5f8-148">如需可用角色的列表，请参阅[角色枚举](../resources/permission.md#roles-enumeration)。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-148">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="5c5f8-149">错误响应</span><span class="sxs-lookup"><span data-stu-id="5c5f8-149">Error Responses</span></span>

<span data-ttu-id="5c5f8-150">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="5c5f8-150">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[共享链接]: ../resources/permission.md#sharing-links
[sharing link]: ../resources/permission.md#sharing-links

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
