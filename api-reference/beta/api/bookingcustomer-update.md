---
title: 更新 bookingcustomer
description: 更新 bookingCustomer 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 90de81666335c1825e1d134f9b898ee4b6561664
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461729"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="cfcc3-103">更新 bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="cfcc3-103">Update bookingcustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfcc3-104">更新[bookingCustomer](../resources/bookingcustomer.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cfcc3-104">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cfcc3-105">权限</span><span class="sxs-lookup"><span data-stu-id="cfcc3-105">Permissions</span></span>
<span data-ttu-id="cfcc3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cfcc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfcc3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cfcc3-108">Permission type</span></span>      | <span data-ttu-id="cfcc3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cfcc3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfcc3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cfcc3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cfcc3-111">BookingsAppointment, 全部, 全部登记, 全部, 预订。 all</span><span class="sxs-lookup"><span data-stu-id="cfcc3-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="cfcc3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cfcc3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfcc3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfcc3-113">Not supported.</span></span>   |
|<span data-ttu-id="cfcc3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cfcc3-114">Application</span></span> | <span data-ttu-id="cfcc3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cfcc3-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="cfcc3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cfcc3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="cfcc3-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="cfcc3-117">Optional request headers</span></span>
| <span data-ttu-id="cfcc3-118">名称</span><span class="sxs-lookup"><span data-stu-id="cfcc3-118">Name</span></span>       | <span data-ttu-id="cfcc3-119">说明</span><span class="sxs-lookup"><span data-stu-id="cfcc3-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cfcc3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfcc3-120">Authorization</span></span>  | <span data-ttu-id="cfcc3-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="cfcc3-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfcc3-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="cfcc3-122">Request body</span></span>
<span data-ttu-id="cfcc3-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="cfcc3-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cfcc3-126">属性</span><span class="sxs-lookup"><span data-stu-id="cfcc3-126">Property</span></span>     | <span data-ttu-id="cfcc3-127">类型</span><span class="sxs-lookup"><span data-stu-id="cfcc3-127">Type</span></span>   |<span data-ttu-id="cfcc3-128">说明</span><span class="sxs-lookup"><span data-stu-id="cfcc3-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cfcc3-129">displayName</span><span class="sxs-lookup"><span data-stu-id="cfcc3-129">displayName</span></span>|<span data-ttu-id="cfcc3-130">String</span><span class="sxs-lookup"><span data-stu-id="cfcc3-130">String</span></span>|<span data-ttu-id="cfcc3-131">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="cfcc3-131">The name of the customer.</span></span>|
|<span data-ttu-id="cfcc3-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="cfcc3-132">emailAddress</span></span>|<span data-ttu-id="cfcc3-133">String</span><span class="sxs-lookup"><span data-stu-id="cfcc3-133">String</span></span>|<span data-ttu-id="cfcc3-134">客户的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="cfcc3-134">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="cfcc3-135">响应</span><span class="sxs-lookup"><span data-stu-id="cfcc3-135">Response</span></span>
<span data-ttu-id="cfcc3-136">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cfcc3-136">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cfcc3-137">示例</span><span class="sxs-lookup"><span data-stu-id="cfcc3-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cfcc3-138">请求</span><span class="sxs-lookup"><span data-stu-id="cfcc3-138">Request</span></span>
<span data-ttu-id="cfcc3-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cfcc3-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingcustomer"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
Content-type: application/json

{
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```
##### <a name="response"></a><span data-ttu-id="cfcc3-140">响应</span><span class="sxs-lookup"><span data-stu-id="cfcc3-140">Response</span></span>
<span data-ttu-id="cfcc3-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cfcc3-141">The following is an example of the response.</span></span> <span data-ttu-id="cfcc3-142">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cfcc3-142">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cfcc3-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cfcc3-143">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingcustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingcustomer-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
