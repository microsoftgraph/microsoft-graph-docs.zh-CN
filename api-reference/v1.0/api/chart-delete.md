---
title: 'Chart: delete'
description: 删除 chart 对象。
author: lumine2008
ms.openlocfilehash: 27fa3372b3d9594de4ba80b4c3a6bf6dc7334202
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305332"
---
# <a name="chart-delete"></a><span data-ttu-id="44b51-103">Chart: delete</span><span class="sxs-lookup"><span data-stu-id="44b51-103">Chart: delete</span></span>

<span data-ttu-id="44b51-104">删除 chart 对象。</span><span class="sxs-lookup"><span data-stu-id="44b51-104">Deletes the chart object.</span></span>
## <a name="permissions"></a><span data-ttu-id="44b51-105">权限</span><span class="sxs-lookup"><span data-stu-id="44b51-105">Permissions</span></span>
<span data-ttu-id="44b51-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44b51-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44b51-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="44b51-108">Permission type</span></span>      | <span data-ttu-id="44b51-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44b51-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44b51-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44b51-110">Delegated (work or school account)</span></span> | <span data-ttu-id="44b51-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44b51-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="44b51-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44b51-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44b51-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="44b51-113">Not supported.</span></span>    |
|<span data-ttu-id="44b51-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="44b51-114">Application</span></span> | <span data-ttu-id="44b51-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="44b51-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44b51-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44b51-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/{id|name}/charts/{name}/delete

```
## <a name="request-headers"></a><span data-ttu-id="44b51-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="44b51-117">Request headers</span></span>
| <span data-ttu-id="44b51-118">Name</span><span class="sxs-lookup"><span data-stu-id="44b51-118">Name</span></span>       | <span data-ttu-id="44b51-119">说明</span><span class="sxs-lookup"><span data-stu-id="44b51-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="44b51-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="44b51-120">Authorization</span></span>  | <span data-ttu-id="44b51-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="44b51-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="44b51-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="44b51-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="44b51-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="44b51-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44b51-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="44b51-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="44b51-127">响应</span><span class="sxs-lookup"><span data-stu-id="44b51-127">Response</span></span>

<span data-ttu-id="44b51-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="44b51-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44b51-130">示例</span><span class="sxs-lookup"><span data-stu-id="44b51-130">Example</span></span>
<span data-ttu-id="44b51-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="44b51-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="44b51-132">请求</span><span class="sxs-lookup"><span data-stu-id="44b51-132">Request</span></span>
<span data-ttu-id="44b51-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="44b51-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "chart_delete"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/delete
```

##### <a name="response"></a><span data-ttu-id="44b51-134">响应</span><span class="sxs-lookup"><span data-stu-id="44b51-134">Response</span></span>
<span data-ttu-id="44b51-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="44b51-135">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart: delete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->