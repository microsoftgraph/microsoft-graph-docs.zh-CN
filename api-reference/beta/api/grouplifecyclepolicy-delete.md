---
title: 删除 groupLifecyclePolicy
description: 删除 groupLifecyclePolicy。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c78e59c010e9c449af665d0b67abb0efcad0d3cc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527785"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="1f400-103">删除 groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="1f400-103">Delete groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f400-104">删除 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="1f400-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1f400-105">权限</span><span class="sxs-lookup"><span data-stu-id="1f400-105">Permissions</span></span>

<span data-ttu-id="1f400-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f400-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f400-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f400-108">Permission type</span></span>      | <span data-ttu-id="1f400-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1f400-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f400-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f400-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1f400-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f400-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="1f400-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f400-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f400-113">不支持</span><span class="sxs-lookup"><span data-stu-id="1f400-113">Not supported</span></span> |
|<span data-ttu-id="1f400-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f400-114">Application</span></span> | <span data-ttu-id="1f400-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f400-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f400-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f400-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="1f400-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f400-117">Request headers</span></span>

| <span data-ttu-id="1f400-118">名称</span><span class="sxs-lookup"><span data-stu-id="1f400-118">Name</span></span> | <span data-ttu-id="1f400-119">说明</span><span class="sxs-lookup"><span data-stu-id="1f400-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="1f400-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f400-120">Authorization</span></span> | <span data-ttu-id="1f400-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1f400-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1f400-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f400-123">Content-Type</span></span>  | <span data-ttu-id="1f400-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1f400-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f400-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f400-125">Request body</span></span>
<span data-ttu-id="1f400-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1f400-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1f400-127">响应</span><span class="sxs-lookup"><span data-stu-id="1f400-127">Response</span></span>

<span data-ttu-id="1f400-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1f400-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f400-130">示例</span><span class="sxs-lookup"><span data-stu-id="1f400-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1f400-131">请求</span><span class="sxs-lookup"><span data-stu-id="1f400-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/beta/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="1f400-132">响应</span><span class="sxs-lookup"><span data-stu-id="1f400-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/grouplifecyclepolicy-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
