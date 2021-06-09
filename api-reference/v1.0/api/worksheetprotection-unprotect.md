---
title: 'WorksheetProtection: unprotect'
description: 解除工作表保护
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 273f841a4fc05d78dece7ab26f233eb28c314a88
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813025"
---
# <a name="worksheetprotection-unprotect"></a><span data-ttu-id="c62cb-103">WorksheetProtection: unprotect</span><span class="sxs-lookup"><span data-stu-id="c62cb-103">WorksheetProtection: unprotect</span></span>

<span data-ttu-id="c62cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c62cb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c62cb-105">解除工作表保护</span><span class="sxs-lookup"><span data-stu-id="c62cb-105">Unprotect a worksheet</span></span>
## <a name="permissions"></a><span data-ttu-id="c62cb-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c62cb-106">Permissions</span></span>
<span data-ttu-id="c62cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c62cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c62cb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c62cb-109">Permission type</span></span>      | <span data-ttu-id="c62cb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c62cb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c62cb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c62cb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c62cb-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c62cb-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c62cb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c62cb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c62cb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c62cb-114">Not supported.</span></span>    |
|<span data-ttu-id="c62cb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c62cb-115">Application</span></span> | <span data-ttu-id="c62cb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c62cb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c62cb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c62cb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/protection/unprotect

```
## <a name="request-headers"></a><span data-ttu-id="c62cb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c62cb-118">Request headers</span></span>
| <span data-ttu-id="c62cb-119">名称</span><span class="sxs-lookup"><span data-stu-id="c62cb-119">Name</span></span>       | <span data-ttu-id="c62cb-120">说明</span><span class="sxs-lookup"><span data-stu-id="c62cb-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c62cb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c62cb-121">Authorization</span></span>  | <span data-ttu-id="c62cb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c62cb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c62cb-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c62cb-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="c62cb-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="c62cb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c62cb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c62cb-127">Request body</span></span>
<span data-ttu-id="c62cb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c62cb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c62cb-129">响应</span><span class="sxs-lookup"><span data-stu-id="c62cb-129">Response</span></span>

<span data-ttu-id="c62cb-p104">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c62cb-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c62cb-132">示例</span><span class="sxs-lookup"><span data-stu-id="c62cb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c62cb-133">请求</span><span class="sxs-lookup"><span data-stu-id="c62cb-133">Request</span></span>
<span data-ttu-id="c62cb-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c62cb-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "worksheetprotection_unprotect"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect
```


### <a name="response"></a><span data-ttu-id="c62cb-135">响应</span><span class="sxs-lookup"><span data-stu-id="c62cb-135">Response</span></span>
<span data-ttu-id="c62cb-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c62cb-136">The following is an example of the response.</span></span> 
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
  "description": "WorksheetProtection: unprotect",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

