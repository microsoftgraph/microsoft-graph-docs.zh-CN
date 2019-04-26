---
title: 创建 bookingCustomer
description: 创建新的 bookingCustomer 对象。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0825681905c309ce889a12cbb49e051e0612ab38
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322468"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="8935c-103">创建 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="8935c-103">Create bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8935c-104">创建新的[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8935c-104">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8935c-105">权限</span><span class="sxs-lookup"><span data-stu-id="8935c-105">Permissions</span></span>
<span data-ttu-id="8935c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8935c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8935c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8935c-108">Permission type</span></span>      | <span data-ttu-id="8935c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8935c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8935c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8935c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="8935c-111">BookingsAppointment, 全部, 全部登记, 全部, 预订。 all</span><span class="sxs-lookup"><span data-stu-id="8935c-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="8935c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8935c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8935c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8935c-113">Not supported.</span></span>   |
|<span data-ttu-id="8935c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8935c-114">Application</span></span> | <span data-ttu-id="8935c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8935c-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8935c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8935c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="8935c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8935c-117">Request headers</span></span>
| <span data-ttu-id="8935c-118">名称</span><span class="sxs-lookup"><span data-stu-id="8935c-118">Name</span></span>       | <span data-ttu-id="8935c-119">说明</span><span class="sxs-lookup"><span data-stu-id="8935c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8935c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8935c-120">Authorization</span></span>  | <span data-ttu-id="8935c-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8935c-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8935c-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="8935c-122">Request body</span></span>
<span data-ttu-id="8935c-123">在请求正文中, 提供[bookingCustomer](../resources/bookingcustomer.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8935c-123">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="8935c-124">响应</span><span class="sxs-lookup"><span data-stu-id="8935c-124">Response</span></span>
<span data-ttu-id="8935c-125">如果成功, 此方法在`201, Created`响应正文中返回响应代码和[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8935c-125">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8935c-126">示例</span><span class="sxs-lookup"><span data-stu-id="8935c-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8935c-127">请求</span><span class="sxs-lookup"><span data-stu-id="8935c-127">Request</span></span>
<span data-ttu-id="8935c-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8935c-128">The following is an example of the request.</span></span>
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
<span data-ttu-id="8935c-129">在请求正文中, 提供[bookingCustomer](../resources/bookingcustomer.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8935c-129">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8935c-130">响应</span><span class="sxs-lookup"><span data-stu-id="8935c-130">Response</span></span>
<span data-ttu-id="8935c-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8935c-131">The following is an example of the response.</span></span> <span data-ttu-id="8935c-132">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8935c-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8935c-133">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8935c-133">All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
