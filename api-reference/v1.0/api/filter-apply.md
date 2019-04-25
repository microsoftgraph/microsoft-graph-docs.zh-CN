---
title: 'Filter: apply'
description: 在给定列中应用给定的筛选条件。
localization_priority: Normal
ms.openlocfilehash: e7223c1b3d7cd75356c459f366c1a230eeb06e59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524258"
---
# <a name="filter-apply"></a><span data-ttu-id="1a11a-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="1a11a-103">Filter: apply</span></span>

<span data-ttu-id="1a11a-104">在给定列中应用给定的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="1a11a-104">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a11a-105">权限</span><span class="sxs-lookup"><span data-stu-id="1a11a-105">Permissions</span></span>
<span data-ttu-id="1a11a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a11a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a11a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a11a-108">Permission type</span></span>      | <span data-ttu-id="1a11a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a11a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a11a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a11a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a11a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1a11a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="1a11a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a11a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a11a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a11a-113">Not supported.</span></span>    |
|<span data-ttu-id="1a11a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a11a-114">Application</span></span> | <span data-ttu-id="1a11a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a11a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a11a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a11a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="1a11a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a11a-117">Request headers</span></span>
| <span data-ttu-id="1a11a-118">名称</span><span class="sxs-lookup"><span data-stu-id="1a11a-118">Name</span></span>       | <span data-ttu-id="1a11a-119">说明</span><span class="sxs-lookup"><span data-stu-id="1a11a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1a11a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a11a-120">Authorization</span></span>  | <span data-ttu-id="1a11a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a11a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a11a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a11a-123">Request body</span></span>
<span data-ttu-id="1a11a-124">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1a11a-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1a11a-125">参数</span><span class="sxs-lookup"><span data-stu-id="1a11a-125">Parameter</span></span>    | <span data-ttu-id="1a11a-126">类型</span><span class="sxs-lookup"><span data-stu-id="1a11a-126">Type</span></span>   |<span data-ttu-id="1a11a-127">说明</span><span class="sxs-lookup"><span data-stu-id="1a11a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a11a-128">条件</span><span class="sxs-lookup"><span data-stu-id="1a11a-128">criteria</span></span>|<span data-ttu-id="1a11a-129">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="1a11a-129">WorkbookFilterCriteria</span></span>|<span data-ttu-id="1a11a-130">要应用的条件。</span><span class="sxs-lookup"><span data-stu-id="1a11a-130">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="1a11a-131">响应</span><span class="sxs-lookup"><span data-stu-id="1a11a-131">Response</span></span>

<span data-ttu-id="1a11a-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1a11a-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a11a-134">示例</span><span class="sxs-lookup"><span data-stu-id="1a11a-134">Example</span></span>
<span data-ttu-id="1a11a-135">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1a11a-135">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1a11a-136">请求</span><span class="sxs-lookup"><span data-stu-id="1a11a-136">Request</span></span>
<span data-ttu-id="1a11a-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a11a-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```

##### <a name="response"></a><span data-ttu-id="1a11a-138">响应</span><span class="sxs-lookup"><span data-stu-id="1a11a-138">Response</span></span>
<span data-ttu-id="1a11a-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1a11a-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
