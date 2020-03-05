---
title: 获取 openShiftChangeRequest
description: 检索 openShiftChangeRequest 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6a2f7e9f55afc566590a847fe8542ae062b182cb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456368"
---
# <a name="get-openshiftchangerequest"></a><span data-ttu-id="beac7-103">获取 openShiftChangeRequest</span><span class="sxs-lookup"><span data-stu-id="beac7-103">Get openShiftChangeRequest</span></span>

<span data-ttu-id="beac7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="beac7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="beac7-105">检索[openShiftChangeRequest](../resources/openshiftchangerequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="beac7-105">Retrieve the properties and relationships of an [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="beac7-106">权限</span><span class="sxs-lookup"><span data-stu-id="beac7-106">Permissions</span></span>

<span data-ttu-id="beac7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="beac7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="beac7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="beac7-109">Permission type</span></span>                        | <span data-ttu-id="beac7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="beac7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="beac7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="beac7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="beac7-112">Group. 全部，Group。 Read. All</span><span class="sxs-lookup"><span data-stu-id="beac7-112">Group.ReadWrite.All, Group.Read.All</span></span> |
| <span data-ttu-id="beac7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="beac7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="beac7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="beac7-114">Not supported.</span></span> |
| <span data-ttu-id="beac7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="beac7-115">Application</span></span>                            | <span data-ttu-id="beac7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="beac7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="beac7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="beac7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShiftsChangeRequests/{openShiftsChangeRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="beac7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="beac7-118">Optional query parameters</span></span>

<span data-ttu-id="beac7-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="beac7-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="beac7-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="beac7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="beac7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="beac7-121">Request headers</span></span>

| <span data-ttu-id="beac7-122">名称</span><span class="sxs-lookup"><span data-stu-id="beac7-122">Name</span></span>      |<span data-ttu-id="beac7-123">说明</span><span class="sxs-lookup"><span data-stu-id="beac7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="beac7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="beac7-124">Authorization</span></span> | <span data-ttu-id="beac7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="beac7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="beac7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="beac7-127">Request body</span></span>

<span data-ttu-id="beac7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="beac7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="beac7-129">响应</span><span class="sxs-lookup"><span data-stu-id="beac7-129">Response</span></span>

<span data-ttu-id="beac7-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[openShiftChangeRequest](../resources/openshiftchangerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="beac7-130">If successful, this method returns a `200 OK` response code and the requested [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="beac7-131">示例</span><span class="sxs-lookup"><span data-stu-id="beac7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="beac7-132">请求</span><span class="sxs-lookup"><span data-stu-id="beac7-132">Request</span></span>

<span data-ttu-id="beac7-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="beac7-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_openshiftchangerequest"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftsChangeRequests/SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09
```

### <a name="response"></a><span data-ttu-id="beac7-134">响应</span><span class="sxs-lookup"><span data-stu-id="beac7-134">Response</span></span>

<span data-ttu-id="beac7-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="beac7-135">The following is an example of the response.</span></span>

> <span data-ttu-id="beac7-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="beac7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShiftChangeRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "SREQ_0b87dd20-d5ed-4764-9c3e-cfc8516def09",
  "openShiftId": "577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "assignedTo": "manager",
  "state": "pending",
  "senderUserId": "3fe0bc21-1398-4fd9-9713-52511b434c1e",
  "senderDateTime": "2019-05-01T10:00:00Z",
  "senderMessage": "Can I take this shift?",
  "managerUserId": null,
  "managerActionDateTime": null,
  "managerActionMessage": null,
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get openShiftChangeRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
