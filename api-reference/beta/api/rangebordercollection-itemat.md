---
title: 'RangeBorderCollection: ItemAt'
description: 使用其索引获取 border 对象
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: f0308049046cd91484d996d2e3de84b007c89223
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546183"
---
# <a name="rangebordercollection-itemat"></a><span data-ttu-id="d217b-103">RangeBorderCollection: ItemAt</span><span class="sxs-lookup"><span data-stu-id="d217b-103">RangeBorderCollection: ItemAt</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d217b-104">使用其索引获取 border 对象</span><span class="sxs-lookup"><span data-stu-id="d217b-104">Gets a border object using its index</span></span>
## <a name="permissions"></a><span data-ttu-id="d217b-105">权限</span><span class="sxs-lookup"><span data-stu-id="d217b-105">Permissions</span></span>
<span data-ttu-id="d217b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d217b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d217b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d217b-108">Permission type</span></span>      | <span data-ttu-id="d217b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d217b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d217b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d217b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d217b-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d217b-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d217b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d217b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d217b-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d217b-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d217b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d217b-114">Application</span></span> | <span data-ttu-id="d217b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d217b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d217b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d217b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/borders/ItemAt
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/borders/ItemAt
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/borders/ItemAt

```
## <a name="request-headers"></a><span data-ttu-id="d217b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d217b-117">Request headers</span></span>
| <span data-ttu-id="d217b-118">名称</span><span class="sxs-lookup"><span data-stu-id="d217b-118">Name</span></span>       | <span data-ttu-id="d217b-119">说明</span><span class="sxs-lookup"><span data-stu-id="d217b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d217b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d217b-120">Authorization</span></span>  | <span data-ttu-id="d217b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d217b-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d217b-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d217b-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="d217b-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="d217b-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d217b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d217b-126">Request body</span></span>
<span data-ttu-id="d217b-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d217b-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d217b-128">参数</span><span class="sxs-lookup"><span data-stu-id="d217b-128">Parameter</span></span>    | <span data-ttu-id="d217b-129">类型</span><span class="sxs-lookup"><span data-stu-id="d217b-129">Type</span></span>   |<span data-ttu-id="d217b-130">说明</span><span class="sxs-lookup"><span data-stu-id="d217b-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d217b-131">index</span><span class="sxs-lookup"><span data-stu-id="d217b-131">index</span></span>|<span data-ttu-id="d217b-132">number</span><span class="sxs-lookup"><span data-stu-id="d217b-132">number</span></span>|<span data-ttu-id="d217b-p104">要检索的对象的索引值。从零开始编制索引。</span><span class="sxs-lookup"><span data-stu-id="d217b-p104">Index value of the object to be retrieved. Zero-indexed.</span></span>|

## <a name="response"></a><span data-ttu-id="d217b-135">响应</span><span class="sxs-lookup"><span data-stu-id="d217b-135">Response</span></span>

<span data-ttu-id="d217b-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [RangeBorder](../resources/rangeborder.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d217b-136">If successful, this method returns `200 OK` response code and [RangeBorder](../resources/rangeborder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d217b-137">示例</span><span class="sxs-lookup"><span data-stu-id="d217b-137">Example</span></span>
<span data-ttu-id="d217b-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d217b-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d217b-139">请求</span><span class="sxs-lookup"><span data-stu-id="d217b-139">Request</span></span>
<span data-ttu-id="d217b-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d217b-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangebordercollection_itemat"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)/range/format/borders/ItemAt
Content-type: application/json
Content-length: 20

{
  "index": {
  }
}
```

##### <a name="response"></a><span data-ttu-id="d217b-141">响应</span><span class="sxs-lookup"><span data-stu-id="d217b-141">Response</span></span>
<span data-ttu-id="d217b-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d217b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeBorder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 136

{
  "id": "id-value",
  "color": "color-value",
  "style": "style-value",
  "sideIndex": "sideIndex-value",
  "weight": "weight-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "RangeBorderCollection: ItemAt",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/rangebordercollection-itemat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
