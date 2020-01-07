---
title: 创建 offerShiftRequest
description: 创建 offerShiftRequest 的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3c7eeb1fbe68e41465b5a55150e72c694dad059d
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952123"
---
# <a name="create-offershiftrequest"></a><span data-ttu-id="c7aa1-103">创建 offerShiftRequest</span><span class="sxs-lookup"><span data-stu-id="c7aa1-103">Create offerShiftRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7aa1-104">创建[offerShiftRequest](../resources/offershiftrequest.md)的实例。</span><span class="sxs-lookup"><span data-stu-id="c7aa1-104">Create an instance of an [offerShiftRequest](../resources/offershiftrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c7aa1-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="c7aa1-105">Permissions</span></span>

<span data-ttu-id="c7aa1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7aa1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7aa1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7aa1-108">Permission type</span></span>                        | <span data-ttu-id="c7aa1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7aa1-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c7aa1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7aa1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7aa1-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7aa1-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c7aa1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7aa1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7aa1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7aa1-113">Not supported.</span></span> |
| <span data-ttu-id="c7aa1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7aa1-114">Application</span></span>                            | <span data-ttu-id="c7aa1-115">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="c7aa1-115">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="c7aa1-116">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="c7aa1-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="c7aa1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7aa1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/offerShiftRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7aa1-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c7aa1-118">Optional query parameters</span></span>

<span data-ttu-id="c7aa1-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c7aa1-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c7aa1-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c7aa1-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7aa1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7aa1-121">Request headers</span></span>

| <span data-ttu-id="c7aa1-122">名称</span><span class="sxs-lookup"><span data-stu-id="c7aa1-122">Name</span></span>      |<span data-ttu-id="c7aa1-123">说明</span><span class="sxs-lookup"><span data-stu-id="c7aa1-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7aa1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7aa1-124">Authorization</span></span> | <span data-ttu-id="c7aa1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7aa1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7aa1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7aa1-127">Request body</span></span>
<span data-ttu-id="c7aa1-128">在此方法的请求正文中提供新的[offershiftrequest](../resources/offershiftrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c7aa1-128">Provide the new [offershiftrequest](../resources/offershiftrequest.md) object in the request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7aa1-129">响应</span><span class="sxs-lookup"><span data-stu-id="c7aa1-129">Response</span></span>

<span data-ttu-id="c7aa1-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[offerShiftRequest](../resources/offershiftrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c7aa1-130">If successful, this method returns a `200 OK` response code and an [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7aa1-131">示例</span><span class="sxs-lookup"><span data-stu-id="c7aa1-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c7aa1-132">请求</span><span class="sxs-lookup"><span data-stu-id="c7aa1-132">Request</span></span>

<span data-ttu-id="c7aa1-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c7aa1-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}-->

```http
POST https://graph.microsoft.com/beta/teams/788b75d2-a911-48c0-a5e2-dc98480457e3/schedule/offershiftrequests
Authorization: Bearer {token}
Content-type: application/json

{
  "senderShiftId": "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
  "senderMessage": "Having a family emergency, could you take this shift for me?",
  "recipientUserId": "fe278b61-21ac-4872-8b41-1962bbb98e3c"
}
```

### <a name="response"></a><span data-ttu-id="c7aa1-134">响应</span><span class="sxs-lookup"><span data-stu-id="c7aa1-134">Response</span></span>

<span data-ttu-id="c7aa1-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c7aa1-135">The following is an example of the response.</span></span>

> <span data-ttu-id="c7aa1-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c7aa1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.etag": "\"4000ee23-0000-0700-0000-5d1415f60000\"",
  "id": "SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09",
  "createdDateTime": "2019-09-27T01:01:04.566Z",
  "lastModifiedDateTime": "2019-09-28T01:03:48.874Z",
  "assignedTo": "recipient",
  "state": "pending",
  "senderDateTime": "2019-09-27T01:01:04.566",
  "senderMessage": "Having a family emergency, could you take this shift for me?",
  "senderUserId": "a4704dd0-3f4c-4f2c-9bb5-8cc575703f30",
  "managerActionDateTime": null,
  "managerActionMessage": null,
  "managerUserId": null,
  "recipientActionDateTime": null,
  "recipientActionMessage": null,
  "senderShiftId": "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29",
  "recipientUserId": "fe278b61-21ac-4872-8b41-1962bbb98e3c",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "fe278b61-21ac-4872-8b41-1962bbb98e3c",
      "displayName": "Employee 1"
    }
  }
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
