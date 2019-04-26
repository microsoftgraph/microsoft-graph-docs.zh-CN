---
title: 'workbookRangeView: range'
description: 返回与 rangeView 资源相关联的范围。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: d4a97773f255e08e54be0360fc443f1193884fae
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339552"
---
# <a name="workbookrangeview-range"></a><span data-ttu-id="31cde-103">workbookRangeView: range</span><span class="sxs-lookup"><span data-stu-id="31cde-103">workbookRangeView: range</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31cde-104">返回与 rangeView 资源相关联的范围。</span><span class="sxs-lookup"><span data-stu-id="31cde-104">Return the range associated with the rangeView resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="31cde-105">权限</span><span class="sxs-lookup"><span data-stu-id="31cde-105">Permissions</span></span>
<span data-ttu-id="31cde-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="31cde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="31cde-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="31cde-108">Permission type</span></span>      | <span data-ttu-id="31cde-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="31cde-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31cde-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31cde-110">Delegated (work or school account)</span></span> | <span data-ttu-id="31cde-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31cde-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="31cde-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31cde-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31cde-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="31cde-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="31cde-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="31cde-114">Application</span></span> | <span data-ttu-id="31cde-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="31cde-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="31cde-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31cde-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET me/drive/root/workbook/worksheets/{id}/range(addres={address})/visibleView/range

```
## <a name="request-headers"></a><span data-ttu-id="31cde-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="31cde-117">Request headers</span></span>
| <span data-ttu-id="31cde-118">名称</span><span class="sxs-lookup"><span data-stu-id="31cde-118">Name</span></span>       | <span data-ttu-id="31cde-119">说明</span><span class="sxs-lookup"><span data-stu-id="31cde-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="31cde-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="31cde-120">Authorization</span></span>  | <span data-ttu-id="31cde-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="31cde-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="31cde-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="31cde-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="31cde-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="31cde-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="31cde-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="31cde-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="31cde-127">响应</span><span class="sxs-lookup"><span data-stu-id="31cde-127">Response</span></span>

<span data-ttu-id="31cde-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [workbookRange](../resources/workbookrange.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="31cde-128">If successful, this method returns `200 OK` response code and [workbookRange](../resources/workbookrange.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31cde-129">示例</span><span class="sxs-lookup"><span data-stu-id="31cde-129">Example</span></span>
<span data-ttu-id="31cde-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="31cde-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="31cde-131">请求</span><span class="sxs-lookup"><span data-stu-id="31cde-131">Request</span></span>
<span data-ttu-id="31cde-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="31cde-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_range"
}-->
```http
GET https://graph.microsoft.com/beta/drive/root/workbook/worksheets/{id}/range(addres='A1:Z10')/visibleView/range
```

##### <a name="response"></a><span data-ttu-id="31cde-133">响应</span><span class="sxs-lookup"><span data-stu-id="31cde-133">Response</span></span>
<span data-ttu-id="31cde-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="31cde-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
