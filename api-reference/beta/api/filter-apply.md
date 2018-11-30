---
title: 'Filter: apply'
description: 在给定列中应用给定的筛选条件。
ms.openlocfilehash: e799b4e4b5f94664e9420e810075205691e1bd96
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041354"
---
# <a name="filter-apply"></a><span data-ttu-id="73205-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="73205-103">Filter: apply</span></span>

> <span data-ttu-id="73205-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="73205-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73205-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="73205-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="73205-106">在给定列中应用给定的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="73205-106">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="73205-107">权限</span><span class="sxs-lookup"><span data-stu-id="73205-107">Permissions</span></span>
<span data-ttu-id="73205-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73205-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73205-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="73205-110">Permission type</span></span>      | <span data-ttu-id="73205-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73205-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73205-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73205-112">Delegated (work or school account)</span></span> | <span data-ttu-id="73205-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73205-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="73205-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73205-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73205-115">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73205-115">Files.ReadWrite</span></span>    |
|<span data-ttu-id="73205-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="73205-116">Application</span></span> | <span data-ttu-id="73205-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="73205-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73205-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73205-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="73205-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="73205-119">Request headers</span></span>
| <span data-ttu-id="73205-120">名称</span><span class="sxs-lookup"><span data-stu-id="73205-120">Name</span></span>       | <span data-ttu-id="73205-121">说明</span><span class="sxs-lookup"><span data-stu-id="73205-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="73205-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73205-122">Authorization</span></span>  | <span data-ttu-id="73205-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73205-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73205-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="73205-125">Request body</span></span>
<span data-ttu-id="73205-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="73205-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="73205-127">参数</span><span class="sxs-lookup"><span data-stu-id="73205-127">Parameter</span></span>    | <span data-ttu-id="73205-128">类型</span><span class="sxs-lookup"><span data-stu-id="73205-128">Type</span></span>   |<span data-ttu-id="73205-129">说明</span><span class="sxs-lookup"><span data-stu-id="73205-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73205-130">条件</span><span class="sxs-lookup"><span data-stu-id="73205-130">criteria</span></span>|<span data-ttu-id="73205-131">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="73205-131">FilterCriteria</span></span>|<span data-ttu-id="73205-132">要应用的条件。</span><span class="sxs-lookup"><span data-stu-id="73205-132">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="73205-133">响应</span><span class="sxs-lookup"><span data-stu-id="73205-133">Response</span></span>

<span data-ttu-id="73205-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="73205-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73205-136">示例</span><span class="sxs-lookup"><span data-stu-id="73205-136">Example</span></span>
<span data-ttu-id="73205-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="73205-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="73205-138">请求</span><span class="sxs-lookup"><span data-stu-id="73205-138">Request</span></span>
<span data-ttu-id="73205-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73205-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
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

##### <a name="response"></a><span data-ttu-id="73205-140">响应</span><span class="sxs-lookup"><span data-stu-id="73205-140">Response</span></span>
<span data-ttu-id="73205-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="73205-141">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
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