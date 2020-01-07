---
title: 获取 offerShiftRequest
description: 检索 offerShiftRequest 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 48fa2dc104dc609192232a4f173b314134829fb5
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952151"
---
# <a name="get-offershiftrequest"></a><span data-ttu-id="0b7ae-103">获取 offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="0b7ae-103">Get offerShiftRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b7ae-104">检索[offerShiftRequest](../resources/offershiftrequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0b7ae-104">Retrieve the properties and relationships of an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b7ae-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="0b7ae-105">Permissions</span></span>

<span data-ttu-id="0b7ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b7ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b7ae-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b7ae-108">Permission type</span></span>                        | <span data-ttu-id="0b7ae-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b7ae-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0b7ae-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b7ae-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b7ae-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b7ae-111">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="0b7ae-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b7ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b7ae-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b7ae-113">Not supported.</span></span> |
| <span data-ttu-id="0b7ae-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b7ae-114">Application</span></span>                            | <span data-ttu-id="0b7ae-115">Schedule. All *、schedule、all*</span><span class="sxs-lookup"><span data-stu-id="0b7ae-115">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="0b7ae-116">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="0b7ae-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="0b7ae-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b7ae-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/schedule/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b7ae-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0b7ae-118">Optional query parameters</span></span>

<span data-ttu-id="0b7ae-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0b7ae-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0b7ae-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0b7ae-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b7ae-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b7ae-121">Request headers</span></span>

| <span data-ttu-id="0b7ae-122">名称</span><span class="sxs-lookup"><span data-stu-id="0b7ae-122">Name</span></span>      |<span data-ttu-id="0b7ae-123">说明</span><span class="sxs-lookup"><span data-stu-id="0b7ae-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0b7ae-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b7ae-124">Authorization</span></span> | <span data-ttu-id="0b7ae-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b7ae-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b7ae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b7ae-127">Request body</span></span>

<span data-ttu-id="0b7ae-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b7ae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b7ae-129">响应</span><span class="sxs-lookup"><span data-stu-id="0b7ae-129">Response</span></span>

<span data-ttu-id="0b7ae-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[offerShiftRequest](../resources/offershiftrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0b7ae-130">If successful, this method returns a `200 OK` response code and the requested [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b7ae-131">示例</span><span class="sxs-lookup"><span data-stu-id="0b7ae-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0b7ae-132">请求</span><span class="sxs-lookup"><span data-stu-id="0b7ae-132">Request</span></span>

<span data-ttu-id="0b7ae-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b7ae-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```http
GET https://graph.microsoft.com/beta/teams/schedule/offerShiftRequests
```

### <a name="response"></a><span data-ttu-id="0b7ae-134">响应</span><span class="sxs-lookup"><span data-stu-id="0b7ae-134">Response</span></span>

<span data-ttu-id="0b7ae-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b7ae-135">The following is an example of the response.</span></span>

> <span data-ttu-id="0b7ae-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0b7ae-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "recipientActionMessage": "recipientActionMessage-value",
  "recipientActionDateTime": "datetime-value",
  "senderShiftId": "senderShiftId-value",
  "recipientUserId": "recipientUserId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get offerShiftRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
