---
title: 获取 swapShiftsChangeRequest
description: 检索 swapShiftsChangeRequest 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5203f7902a5c25683e173c4647b7cb776655e05c
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951750"
---
# <a name="get-swapshiftschangerequest"></a><span data-ttu-id="017bb-103">获取 swapShiftsChangeRequest</span><span class="sxs-lookup"><span data-stu-id="017bb-103">Get swapShiftsChangeRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="017bb-104">检索[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="017bb-104">Retrieve the properties and relationships of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="017bb-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="017bb-105">Permissions</span></span>

<span data-ttu-id="017bb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="017bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="017bb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="017bb-108">Permission type</span></span>                        | <span data-ttu-id="017bb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="017bb-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="017bb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="017bb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="017bb-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="017bb-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="017bb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="017bb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="017bb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="017bb-113">Not supported.</span></span> |
| <span data-ttu-id="017bb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="017bb-114">Application</span></span> | <span data-ttu-id="017bb-115">Schedule. All *、schedule、all*</span><span class="sxs-lookup"><span data-stu-id="017bb-115">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="017bb-116">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="017bb-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="017bb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="017bb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/swapShiftsChangeRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="017bb-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="017bb-118">Optional query parameters</span></span>

<span data-ttu-id="017bb-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="017bb-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="017bb-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="017bb-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="017bb-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="017bb-121">Request headers</span></span>

| <span data-ttu-id="017bb-122">名称</span><span class="sxs-lookup"><span data-stu-id="017bb-122">Name</span></span>      |<span data-ttu-id="017bb-123">说明</span><span class="sxs-lookup"><span data-stu-id="017bb-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="017bb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="017bb-124">Authorization</span></span> | <span data-ttu-id="017bb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="017bb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="017bb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="017bb-127">Request body</span></span>

<span data-ttu-id="017bb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="017bb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="017bb-129">响应</span><span class="sxs-lookup"><span data-stu-id="017bb-129">Response</span></span>

<span data-ttu-id="017bb-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="017bb-130">If successful, this method returns a `200 OK` response code and the requested [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="017bb-131">示例</span><span class="sxs-lookup"><span data-stu-id="017bb-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="017bb-132">请求</span><span class="sxs-lookup"><span data-stu-id="017bb-132">Request</span></span>

<span data-ttu-id="017bb-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="017bb-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_swapshiftschangerequest"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests/{swapShiftsChangeRequestId}
```

### <a name="response"></a><span data-ttu-id="017bb-134">响应</span><span class="sxs-lookup"><span data-stu-id="017bb-134">Response</span></span>

<span data-ttu-id="017bb-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="017bb-135">The following is an example of the response.</span></span>

> <span data-ttu-id="017bb-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="017bb-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "0b87dd20-d5ed-4764-9c3e-cfc8516def09",
    "senderShiftId": "5ad10161-6524-4c7c-9beb-4e8677ba2f6d",
    "recipientShiftId": "e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c",
    "assignedTo": "manager",
    "state": "approved",
    "senderUserId": "3fe0bc21-1398-4fd9-9713-52511b434c1e",
    "senderDateTime": "2019-05-01T10:00:00Z",
    "senderMessage": "I can't make my shift, any chance we can swap?",
    "recipientUserId": "567c8ea5-9e32-422a-a663-8270201699cd",
    "recipientActionDateTime": "2019-05-01T11:00:00Z",
    "recipientActionMessage": "Sure!",
    "managerUserId": "fdcc8d43-7f83-438a-9ab1-098e8f2a95ff",
    "managerActionDateTime": "2019-05-01T12:00:00Z",
    "managerActionMessage": "Approved!"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get swapShiftsChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
