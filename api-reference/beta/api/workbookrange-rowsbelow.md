---
title: 'workbookRange: rowsBelow'
description: 获取给定范围下方的一定数量的行。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 42d53ce3aa9d26c7c499b19af3d5330259786520
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535963"
---
# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="214ef-103">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="214ef-103">workbookRange: rowsBelow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="214ef-104">获取给定范围下方的一定数量的行。</span><span class="sxs-lookup"><span data-stu-id="214ef-104">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="214ef-105">权限</span><span class="sxs-lookup"><span data-stu-id="214ef-105">Permissions</span></span>
<span data-ttu-id="214ef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="214ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="214ef-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="214ef-108">Permission type</span></span>      | <span data-ttu-id="214ef-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="214ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="214ef-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="214ef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="214ef-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="214ef-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="214ef-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="214ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="214ef-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="214ef-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="214ef-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="214ef-114">Application</span></span> | <span data-ttu-id="214ef-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="214ef-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="214ef-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="214ef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="214ef-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="214ef-117">Function parameters</span></span>

| <span data-ttu-id="214ef-118">参数</span><span class="sxs-lookup"><span data-stu-id="214ef-118">Parameter</span></span>    | <span data-ttu-id="214ef-119">类型</span><span class="sxs-lookup"><span data-stu-id="214ef-119">Type</span></span>   |<span data-ttu-id="214ef-120">说明</span><span class="sxs-lookup"><span data-stu-id="214ef-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="214ef-121">count</span><span class="sxs-lookup"><span data-stu-id="214ef-121">count</span></span>|<span data-ttu-id="214ef-122">Int32</span><span class="sxs-lookup"><span data-stu-id="214ef-122">Int32</span></span>|<span data-ttu-id="214ef-p102">可选。生成的范围中要包含的行数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="214ef-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="214ef-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="214ef-128">Request headers</span></span>
| <span data-ttu-id="214ef-129">名称</span><span class="sxs-lookup"><span data-stu-id="214ef-129">Name</span></span>       | <span data-ttu-id="214ef-130">说明</span><span class="sxs-lookup"><span data-stu-id="214ef-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="214ef-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="214ef-131">Authorization</span></span>  | <span data-ttu-id="214ef-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="214ef-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="214ef-134">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="214ef-134">Workbook-Session-Id</span></span>  | <span data-ttu-id="214ef-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="214ef-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="214ef-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="214ef-137">Request body</span></span>
<span data-ttu-id="214ef-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="214ef-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="214ef-139">响应</span><span class="sxs-lookup"><span data-stu-id="214ef-139">Response</span></span>

<span data-ttu-id="214ef-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="214ef-140">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="214ef-141">示例</span><span class="sxs-lookup"><span data-stu-id="214ef-141">Example</span></span>
<span data-ttu-id="214ef-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="214ef-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="214ef-143">请求</span><span class="sxs-lookup"><span data-stu-id="214ef-143">Request</span></span>
<span data-ttu-id="214ef-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="214ef-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsBelow"
}-->
```http
POST https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="214ef-145">响应</span><span class="sxs-lookup"><span data-stu-id="214ef-145">Response</span></span>
<span data-ttu-id="214ef-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="214ef-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrange-rowsbelow.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
