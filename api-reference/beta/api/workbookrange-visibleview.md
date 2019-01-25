---
title: 'workbookRange: visibleView'
description: 要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅权限。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: b7ddea5635f8cf90e448d15223b5de51b0138f21
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525386"
---
# <a name="workbookrange-visibleview"></a><span data-ttu-id="18c19-104">workbookRange: visibleView</span><span class="sxs-lookup"><span data-stu-id="18c19-104">workbookRange: visibleView</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="permissions"></a><span data-ttu-id="18c19-105">权限</span><span class="sxs-lookup"><span data-stu-id="18c19-105">Permissions</span></span>
<span data-ttu-id="18c19-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18c19-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18c19-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="18c19-108">Permission type</span></span>      | <span data-ttu-id="18c19-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18c19-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18c19-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18c19-110">Delegated (work or school account)</span></span> | <span data-ttu-id="18c19-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18c19-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="18c19-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18c19-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18c19-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18c19-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="18c19-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="18c19-114">Application</span></span> | <span data-ttu-id="18c19-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="18c19-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18c19-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18c19-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/drive/root/workbook/worksheets/{id}/range(address={address})/visibleView
```
## <a name="request-headers"></a><span data-ttu-id="18c19-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="18c19-117">Request headers</span></span>
| <span data-ttu-id="18c19-118">名称</span><span class="sxs-lookup"><span data-stu-id="18c19-118">Name</span></span>       | <span data-ttu-id="18c19-119">说明</span><span class="sxs-lookup"><span data-stu-id="18c19-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="18c19-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="18c19-120">Authorization</span></span>  | <span data-ttu-id="18c19-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18c19-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="18c19-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="18c19-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="18c19-p104">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="18c19-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="18c19-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="18c19-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="18c19-127">响应</span><span class="sxs-lookup"><span data-stu-id="18c19-127">Response</span></span>

<span data-ttu-id="18c19-128">如果成功，此方法在响应正文中返回 `200 OK`响应代码和 [workbookRangeView](../resources/workbookrangeview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18c19-128">If successful, this method returns `200 OK` response code and [workbookRangeView](../resources/workbookrangeview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18c19-129">示例</span><span class="sxs-lookup"><span data-stu-id="18c19-129">Example</span></span>
<span data-ttu-id="18c19-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="18c19-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="18c19-131">请求</span><span class="sxs-lookup"><span data-stu-id="18c19-131">Request</span></span>
<span data-ttu-id="18c19-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18c19-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_visibleview"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView
```

##### <a name="response"></a><span data-ttu-id="18c19-133">响应</span><span class="sxs-lookup"><span data-stu-id="18c19-133">Response</span></span>
<span data-ttu-id="18c19-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="18c19-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeView"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

{
  "cellAddresses": "cellAddresses-value",
  "columnCount": 99,
  "formulas": "formulas-value",
  "formulasLocal": "formulasLocal-value",
  "formulasR1C1": "formulasR1C1-value",
  "index": 99
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/workbookrange-visibleview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
