---
title: 'Filter: clear'
description: 清除给定列上的筛选器。
localization_priority: Normal
ms.openlocfilehash: 4296101bc660e10060a984e5bebfccef6d454a2a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324813"
---
# <a name="filter-clear"></a><span data-ttu-id="e6835-103">Filter: clear</span><span class="sxs-lookup"><span data-stu-id="e6835-103">Filter: clear</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6835-104">清除给定列上的筛选器。</span><span class="sxs-lookup"><span data-stu-id="e6835-104">Clear the filter on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="e6835-105">权限</span><span class="sxs-lookup"><span data-stu-id="e6835-105">Permissions</span></span>
<span data-ttu-id="e6835-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6835-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6835-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6835-108">Permission type</span></span>      | <span data-ttu-id="e6835-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6835-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6835-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6835-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e6835-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6835-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e6835-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6835-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6835-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6835-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="e6835-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6835-114">Application</span></span> | <span data-ttu-id="e6835-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6835-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6835-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6835-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/clear

```
## <a name="request-headers"></a><span data-ttu-id="e6835-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6835-117">Request headers</span></span>
| <span data-ttu-id="e6835-118">名称</span><span class="sxs-lookup"><span data-stu-id="e6835-118">Name</span></span>       | <span data-ttu-id="e6835-119">说明</span><span class="sxs-lookup"><span data-stu-id="e6835-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e6835-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6835-120">Authorization</span></span>  | <span data-ttu-id="e6835-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6835-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6835-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6835-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="e6835-124">响应</span><span class="sxs-lookup"><span data-stu-id="e6835-124">Response</span></span>

<span data-ttu-id="e6835-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e6835-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6835-127">示例</span><span class="sxs-lookup"><span data-stu-id="e6835-127">Example</span></span>
<span data-ttu-id="e6835-128">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e6835-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e6835-129">请求</span><span class="sxs-lookup"><span data-stu-id="e6835-129">Request</span></span>
<span data-ttu-id="e6835-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6835-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "filter_clear"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/clear
```

##### <a name="response"></a><span data-ttu-id="e6835-131">响应</span><span class="sxs-lookup"><span data-stu-id="e6835-131">Response</span></span>
<span data-ttu-id="e6835-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e6835-132">Here is an example of the response.</span></span> 
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
<!--
{
  "type": "#page.annotation",
  "description": "Filter: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
