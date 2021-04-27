---
title: 在组上创建目录设置
description: 使用此 API 为组创建新的目录设置。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4204478494dc02bb2013e95c6952f9b2bef166af
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041174"
---
# <a name="create-a-directory-setting-on-groups"></a><span data-ttu-id="e0859-103">在组上创建目录设置</span><span class="sxs-lookup"><span data-stu-id="e0859-103">Create a directory setting on groups</span></span>

<span data-ttu-id="e0859-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0859-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0859-105">使用此 API 为组创建新的目录设置。</span><span class="sxs-lookup"><span data-stu-id="e0859-105">Use this API to create a new directory setting for the group.</span></span>
## <a name="permissions"></a><span data-ttu-id="e0859-106">权限</span><span class="sxs-lookup"><span data-stu-id="e0859-106">Permissions</span></span>
<span data-ttu-id="e0859-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0859-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0859-109">Permission type</span></span>      | <span data-ttu-id="e0859-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0859-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0859-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0859-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e0859-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e0859-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e0859-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0859-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0859-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0859-114">Not supported.</span></span>    |
|<span data-ttu-id="e0859-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0859-115">Application</span></span> | <span data-ttu-id="e0859-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0859-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0859-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0859-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/settings
```
## <a name="request-headers"></a><span data-ttu-id="e0859-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0859-118">Request headers</span></span>
| <span data-ttu-id="e0859-119">名称</span><span class="sxs-lookup"><span data-stu-id="e0859-119">Name</span></span>       | <span data-ttu-id="e0859-120">说明</span><span class="sxs-lookup"><span data-stu-id="e0859-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e0859-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0859-121">Authorization</span></span>  | <span data-ttu-id="e0859-122">持有者 <token>。</span><span class="sxs-lookup"><span data-stu-id="e0859-122">Bearer <token>.</span></span> <span data-ttu-id="e0859-123">必需</span><span class="sxs-lookup"><span data-stu-id="e0859-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0859-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0859-124">Request body</span></span>
<span data-ttu-id="e0859-125">在请求正文中，提供 [directorySetting](../resources/directorysetting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0859-125">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e0859-126">响应</span><span class="sxs-lookup"><span data-stu-id="e0859-126">Response</span></span>

<span data-ttu-id="e0859-127">如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和 [directorySetting](../resources/directorysetting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0859-127">If successful, this method returns `201 Created` response code and [directorySetting](../resources/directorysetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0859-128">示例</span><span class="sxs-lookup"><span data-stu-id="e0859-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0859-129">请求</span><span class="sxs-lookup"><span data-stu-id="e0859-129">Request</span></span>
<span data-ttu-id="e0859-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0859-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0859-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0859-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/settings
Content-type: application/json
Content-length: 222

{
  "directorySetting": {
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="e0859-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0859-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directorysetting-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="e0859-133">C#</span><span class="sxs-lookup"><span data-stu-id="e0859-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directorysetting-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="e0859-134">在请求正文中，提供 [directorySetting](../resources/directorysetting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0859-134">In the request body, supply a JSON representation of [directorySetting](../resources/directorysetting.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e0859-135">响应</span><span class="sxs-lookup"><span data-stu-id="e0859-135">Response</span></span>
<span data-ttu-id="e0859-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e0859-136">Here is an example of the response.</span></span> <span data-ttu-id="e0859-137">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e0859-137">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "directorySetting": {
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


