---
title: 'workbookRangeView: range'
description: 返回与 rangeView 资源相关联的范围。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 04d43dff5dc108eef64971e2bf4be9c454ddf2ae
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970779"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="f8745-103">workbookRangeView: range</span><span class="sxs-lookup"><span data-stu-id="f8745-103">workbookRangeView: range</span></span>

<span data-ttu-id="f8745-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8745-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8745-105">返回与 rangeView 资源相关联的范围。</span><span class="sxs-lookup"><span data-stu-id="f8745-105">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8745-106">权限</span><span class="sxs-lookup"><span data-stu-id="f8745-106">Permissions</span></span>
<span data-ttu-id="f8745-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8745-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f8745-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8745-109">Permission type</span></span>      | <span data-ttu-id="f8745-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8745-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8745-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8745-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f8745-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8745-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f8745-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8745-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8745-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8745-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="f8745-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8745-115">Application</span></span> | <span data-ttu-id="f8745-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8745-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8745-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8745-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="f8745-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8745-118">Request headers</span></span>
| <span data-ttu-id="f8745-119">名称</span><span class="sxs-lookup"><span data-stu-id="f8745-119">Name</span></span>       | <span data-ttu-id="f8745-120">说明</span><span class="sxs-lookup"><span data-stu-id="f8745-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f8745-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8745-121">Authorization</span></span>  | <span data-ttu-id="f8745-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8745-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f8745-124">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="f8745-124">Workbook-Session-Id</span></span>  | <span data-ttu-id="f8745-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="f8745-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8745-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8745-127">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f8745-128">响应</span><span class="sxs-lookup"><span data-stu-id="f8745-128">Response</span></span>

<span data-ttu-id="f8745-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f8745-129">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8745-130">示例</span><span class="sxs-lookup"><span data-stu-id="f8745-130">Example</span></span>
<span data-ttu-id="f8745-131">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f8745-131">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f8745-132">请求</span><span class="sxs-lookup"><span data-stu-id="f8745-132">Request</span></span>
<span data-ttu-id="f8745-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8745-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f8745-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8745-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(address='A1:Z10')/visibleView/range
```
# <a name="c"></a>[<span data-ttu-id="f8745-135">C#</span><span class="sxs-lookup"><span data-stu-id="f8745-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbookrangeview-range-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8745-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8745-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbookrangeview-range-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8745-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8745-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbookrangeview-range-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8745-138">Java</span><span class="sxs-lookup"><span data-stu-id="f8745-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbookrangeview-range-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f8745-139">响应</span><span class="sxs-lookup"><span data-stu-id="f8745-139">Response</span></span>
<span data-ttu-id="f8745-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8745-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```


