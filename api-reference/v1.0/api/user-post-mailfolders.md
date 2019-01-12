---
title: 创建 MailFolder
description: 使用此 API 在用户邮箱的根文件夹中新建邮件文件夹。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a1d67351469b197781c98028052ad7d1cae3bc92
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974943"
---
# <a name="create-mailfolder"></a><span data-ttu-id="65ce8-103">创建 MailFolder</span><span class="sxs-lookup"><span data-stu-id="65ce8-103">Create MailFolder</span></span>

<span data-ttu-id="65ce8-104">使用此 API 在用户邮箱的根文件夹中新建邮件文件夹。</span><span class="sxs-lookup"><span data-stu-id="65ce8-104">Use this API to create a new mail folder in the root folder of the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="65ce8-105">权限</span><span class="sxs-lookup"><span data-stu-id="65ce8-105">Permissions</span></span>
<span data-ttu-id="65ce8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65ce8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65ce8-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="65ce8-108">Permission type</span></span>      | <span data-ttu-id="65ce8-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65ce8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65ce8-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65ce8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="65ce8-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65ce8-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="65ce8-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65ce8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65ce8-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65ce8-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="65ce8-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="65ce8-114">Application</span></span> | <span data-ttu-id="65ce8-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="65ce8-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="65ce8-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65ce8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/mailFolders
```
## <a name="request-headers"></a><span data-ttu-id="65ce8-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="65ce8-117">Request headers</span></span>
| <span data-ttu-id="65ce8-118">标头</span><span class="sxs-lookup"><span data-stu-id="65ce8-118">Header</span></span>       | <span data-ttu-id="65ce8-119">值</span><span class="sxs-lookup"><span data-stu-id="65ce8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="65ce8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="65ce8-120">Authorization</span></span>  | <span data-ttu-id="65ce8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65ce8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="65ce8-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65ce8-123">Content-Type</span></span>  | <span data-ttu-id="65ce8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="65ce8-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="65ce8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="65ce8-125">Request body</span></span>
<span data-ttu-id="65ce8-p103">在请求正文中，提供具有以下参数的 JSON 对象。**displayName** 是 [MailFolder](../resources/mailfolder.md) 对象的唯一可写属性。</span><span class="sxs-lookup"><span data-stu-id="65ce8-p103">In the request body, provide a JSON object with the following parameters. **displayName** is the only writable property for a [MailFolder](../resources/mailfolder.md) object.</span></span>

| <span data-ttu-id="65ce8-128">参数</span><span class="sxs-lookup"><span data-stu-id="65ce8-128">Parameter</span></span>    | <span data-ttu-id="65ce8-129">类型</span><span class="sxs-lookup"><span data-stu-id="65ce8-129">Type</span></span>   |<span data-ttu-id="65ce8-130">说明</span><span class="sxs-lookup"><span data-stu-id="65ce8-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65ce8-131">displayName</span><span class="sxs-lookup"><span data-stu-id="65ce8-131">displayName</span></span>|<span data-ttu-id="65ce8-132">String</span><span class="sxs-lookup"><span data-stu-id="65ce8-132">String</span></span>|<span data-ttu-id="65ce8-133">新文件夹的显示名称。</span><span class="sxs-lookup"><span data-stu-id="65ce8-133">The display name of the new folder.</span></span>|

## <a name="response"></a><span data-ttu-id="65ce8-134">响应</span><span class="sxs-lookup"><span data-stu-id="65ce8-134">Response</span></span>

<span data-ttu-id="65ce8-135">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [MailFolder](../resources/mailfolder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65ce8-135">If successful, this method returns `201 Created` response code and a [MailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65ce8-136">示例</span><span class="sxs-lookup"><span data-stu-id="65ce8-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="65ce8-137">请求</span><span class="sxs-lookup"><span data-stu-id="65ce8-137">Request</span></span>
<span data-ttu-id="65ce8-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65ce8-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_mailfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value"
}
```

##### <a name="response"></a><span data-ttu-id="65ce8-139">响应</span><span class="sxs-lookup"><span data-stu-id="65ce8-139">Response</span></span>
<span data-ttu-id="65ce8-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65ce8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
