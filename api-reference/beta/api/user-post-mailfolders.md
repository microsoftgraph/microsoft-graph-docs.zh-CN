---
title: 创建 MailFolder
description: 使用此 API 在用户邮箱的根文件夹中新建邮件文件夹。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b4a339338063c4aa511a41eac4342b376d8bc1e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974061"
---
# <a name="create-mailfolder"></a><span data-ttu-id="9868c-103">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="9868c-103">Create MailFolder</span></span>

> <span data-ttu-id="9868c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9868c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9868c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9868c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9868c-106">使用此 API 在用户邮箱的根文件夹中新建邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="9868c-106">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="9868c-107">权限</span><span class="sxs-lookup"><span data-stu-id="9868c-107">Permissions</span></span>
<span data-ttu-id="9868c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9868c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9868c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9868c-110">Permission type</span></span>      | <span data-ttu-id="9868c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9868c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9868c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9868c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9868c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9868c-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9868c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9868c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9868c-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9868c-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="9868c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9868c-116">Application</span></span> | <span data-ttu-id="9868c-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9868c-117">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9868c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9868c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="9868c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9868c-119">Request headers</span></span>
| <span data-ttu-id="9868c-120">标头</span><span class="sxs-lookup"><span data-stu-id="9868c-120">Header</span></span>       | <span data-ttu-id="9868c-121">值</span><span class="sxs-lookup"><span data-stu-id="9868c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9868c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9868c-122">Authorization</span></span>  | <span data-ttu-id="9868c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9868c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9868c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9868c-125">Content-Type</span></span>  | <span data-ttu-id="9868c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9868c-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9868c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9868c-127">Request body</span></span>
<span data-ttu-id="9868c-p104">在请求正文中，提供具有以下参数的 JSON 对象。**displayName** 是 [MailFolder](../resources/mailfolder.md) 对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="9868c-p104">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="9868c-130">参数</span><span class="sxs-lookup"><span data-stu-id="9868c-130">Parameter</span></span>    | <span data-ttu-id="9868c-131">类型</span><span class="sxs-lookup"><span data-stu-id="9868c-131">Type</span></span>   |<span data-ttu-id="9868c-132">说明</span><span class="sxs-lookup"><span data-stu-id="9868c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9868c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9868c-133">displayName</span></span>|<span data-ttu-id="9868c-134">String</span><span class="sxs-lookup"><span data-stu-id="9868c-134">String</span></span>|<span data-ttu-id="9868c-135">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9868c-135">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="9868c-136">响应</span><span class="sxs-lookup"><span data-stu-id="9868c-136">Response</span></span>

<span data-ttu-id="9868c-137">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9868c-137">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9868c-138">示例</span><span class="sxs-lookup"><span data-stu-id="9868c-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9868c-139">请求</span><span class="sxs-lookup"><span data-stu-id="9868c-139">Request</span></span>
<span data-ttu-id="9868c-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9868c-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="9868c-141">响应</span><span class="sxs-lookup"><span data-stu-id="9868c-141">Response</span></span>
<span data-ttu-id="9868c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9868c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 179

{
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create MailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
