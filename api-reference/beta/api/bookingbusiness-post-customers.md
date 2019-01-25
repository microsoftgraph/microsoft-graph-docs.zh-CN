---
title: 创建 bookingCustomer
description: 创建新的 bookingCustomer 对象。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 4557d65edf4727659fdae94599c0796fc940ed1d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523958"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="f4cb5-103">创建 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="f4cb5-103">Create bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4cb5-104">创建新的[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f4cb5-104">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f4cb5-105">权限</span><span class="sxs-lookup"><span data-stu-id="f4cb5-105">Permissions</span></span>
<span data-ttu-id="f4cb5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4cb5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4cb5-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4cb5-108">Permission type</span></span>      | <span data-ttu-id="f4cb5-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4cb5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4cb5-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4cb5-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f4cb5-111">BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All，Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="f4cb5-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f4cb5-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4cb5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4cb5-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4cb5-113">Not supported.</span></span>   |
|<span data-ttu-id="f4cb5-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4cb5-114">Application</span></span> | <span data-ttu-id="f4cb5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4cb5-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f4cb5-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4cb5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="f4cb5-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4cb5-117">Request headers</span></span>
| <span data-ttu-id="f4cb5-118">名称</span><span class="sxs-lookup"><span data-stu-id="f4cb5-118">Name</span></span>       | <span data-ttu-id="f4cb5-119">说明</span><span class="sxs-lookup"><span data-stu-id="f4cb5-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f4cb5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4cb5-120">Authorization</span></span>  | <span data-ttu-id="f4cb5-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f4cb5-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4cb5-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4cb5-122">Request body</span></span>
<span data-ttu-id="f4cb5-123">在请求正文中，提供[bookingCustomer](../resources/bookingcustomer.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4cb5-123">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="f4cb5-124">响应</span><span class="sxs-lookup"><span data-stu-id="f4cb5-124">Response</span></span>
<span data-ttu-id="f4cb5-125">如果成功，此方法返回`201, Created`响应正文中的响应代码和[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f4cb5-125">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4cb5-126">示例</span><span class="sxs-lookup"><span data-stu-id="f4cb5-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f4cb5-127">请求</span><span class="sxs-lookup"><span data-stu-id="f4cb5-127">Request</span></span>
<span data-ttu-id="f4cb5-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f4cb5-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingcustomer_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers

Content-type: application/json

{
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```
<span data-ttu-id="f4cb5-129">在请求正文中，提供[bookingCustomer](../resources/bookingcustomer.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4cb5-129">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f4cb5-130">响应</span><span class="sxs-lookup"><span data-stu-id="f4cb5-130">Response</span></span>
<span data-ttu-id="f4cb5-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f4cb5-131">The following is an example of the response.</span></span> <span data-ttu-id="f4cb5-132">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f4cb5-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f4cb5-133">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4cb5-133">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "36038f36-634e-44e4-9415-d7d59c2347aa",
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-post-customers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
