---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 发送邀请以访问项目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: cc88297c1848e9b66195f9a07ac96167d096a762
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481207"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="522be-102">发送共享邀请</span><span class="sxs-lookup"><span data-stu-id="522be-102">Send a sharing invitation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="522be-p101">发送 **DriveItem** 的共享邀请。共享邀请为收件人提供权限，也可以选择向收件人发送电子邮件以通知他们项目已共享。</span><span class="sxs-lookup"><span data-stu-id="522be-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="522be-105">权限</span><span class="sxs-lookup"><span data-stu-id="522be-105">Permissions</span></span>

<span data-ttu-id="522be-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="522be-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="522be-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="522be-108">Permission type</span></span>      | <span data-ttu-id="522be-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="522be-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="522be-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="522be-110">Delegated (work or school account)</span></span> | <span data-ttu-id="522be-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="522be-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="522be-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="522be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="522be-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="522be-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="522be-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="522be-114">Application</span></span> | <span data-ttu-id="522be-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="522be-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="522be-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="522be-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="522be-117">请求正文</span><span class="sxs-lookup"><span data-stu-id="522be-117">Request body</span></span>

<span data-ttu-id="522be-118">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="522be-118">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="522be-119">参数</span><span class="sxs-lookup"><span data-stu-id="522be-119">Parameter</span></span>        | <span data-ttu-id="522be-120">类型</span><span class="sxs-lookup"><span data-stu-id="522be-120">Type</span></span>                                            | <span data-ttu-id="522be-121">说明</span><span class="sxs-lookup"><span data-stu-id="522be-121">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="522be-122">recipients</span><span class="sxs-lookup"><span data-stu-id="522be-122">recipients</span></span>       | <span data-ttu-id="522be-123">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="522be-123">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="522be-124">将获得访问权限和共享邀请的收件人的集合。</span><span class="sxs-lookup"><span data-stu-id="522be-124">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="522be-125">message</span><span class="sxs-lookup"><span data-stu-id="522be-125">message</span></span>          | <span data-ttu-id="522be-126">String</span><span class="sxs-lookup"><span data-stu-id="522be-126">String</span></span>                                          | <span data-ttu-id="522be-p103">共享邀请中包含的纯文本格式的邮件。最大长度为 2000 个字符。</span><span class="sxs-lookup"><span data-stu-id="522be-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="522be-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="522be-129">requireSignIn</span></span>    | <span data-ttu-id="522be-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="522be-130">Boolean</span></span>                                         | <span data-ttu-id="522be-131">指定邀请的收件人要查看共享项目的登录位置。</span><span class="sxs-lookup"><span data-stu-id="522be-131">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="522be-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="522be-132">sendInvitation</span></span>   | <span data-ttu-id="522be-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="522be-133">Boolean</span></span>                                         | <span data-ttu-id="522be-134">指定是否生成电子邮件或帖子 (false)，或是否仅创建权限 (true)。</span><span class="sxs-lookup"><span data-stu-id="522be-134">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="522be-135">roles</span><span class="sxs-lookup"><span data-stu-id="522be-135">roles</span></span>            | <span data-ttu-id="522be-136">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="522be-136">Collection(String)</span></span>                              | <span data-ttu-id="522be-137">指定授予共享邀请收件人的角色。</span><span class="sxs-lookup"><span data-stu-id="522be-137">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="example"></a><span data-ttu-id="522be-138">示例</span><span class="sxs-lookup"><span data-stu-id="522be-138">Example</span></span>

<span data-ttu-id="522be-139">本示例向电子邮件地址为“ryan@contoso.org”的用户发送共享邀请，其中包含关于协作文件的讯息。</span><span class="sxs-lookup"><span data-stu-id="522be-139">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="522be-140">此邀请授予 Ryan 对该文件的读写访问权限。</span><span class="sxs-lookup"><span data-stu-id="522be-140">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="522be-141">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="522be-141">HTTP Request</span></span>

<span data-ttu-id="522be-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [permission](../resources/permission.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="522be-142">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

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
  "roles": [ "write" ]
}
```

### <a name="response"></a><span data-ttu-id="522be-143">响应</span><span class="sxs-lookup"><span data-stu-id="522be-143">Response</span></span>

<span data-ttu-id="522be-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="522be-144">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="522be-145">注解</span><span class="sxs-lookup"><span data-stu-id="522be-145">Remarks</span></span>

* <span data-ttu-id="522be-146">具有 `personal` **driveType**（OneDrive 个人版）的[驱动器](../resources/drive.md)无法创建或修改根 DriveItem 上的权限。</span><span class="sxs-lookup"><span data-stu-id="522be-146">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="522be-147">如需可用角色的列表，请参阅[角色枚举](../resources/permission.md#roles-enumeration-values)。</span><span class="sxs-lookup"><span data-stu-id="522be-147">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="522be-148">错误响应</span><span class="sxs-lookup"><span data-stu-id="522be-148">Error Responses</span></span>

<span data-ttu-id="522be-149">请参阅[错误响应][error-response]主题，详细了解错误返回方式。</span><span class="sxs-lookup"><span data-stu-id="522be-149">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-invite.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
