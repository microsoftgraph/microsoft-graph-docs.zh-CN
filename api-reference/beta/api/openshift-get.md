---
title: 获取 openShift
description: 检索 openshift 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5ed57daa9e191427699a35ce2cbe27ff282461b6
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895610"
---
# <a name="get-openshift"></a><span data-ttu-id="d3f47-103">获取 openShift</span><span class="sxs-lookup"><span data-stu-id="d3f47-103">Get openShift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3f47-104">检索[openshift](../resources/openshift.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d3f47-104">Retrieve the properties and relationships of an [openshift](../resources/openshift.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3f47-105">权限</span><span class="sxs-lookup"><span data-stu-id="d3f47-105">Permissions</span></span>

<span data-ttu-id="d3f47-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3f47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3f47-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3f47-108">Permission type</span></span>                        | <span data-ttu-id="d3f47-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3f47-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d3f47-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3f47-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3f47-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3f47-111">Group.Read.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="d3f47-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3f47-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3f47-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3f47-113">Not supported.</span></span> |
| <span data-ttu-id="d3f47-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3f47-114">Application</span></span>                            | <span data-ttu-id="d3f47-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3f47-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3f47-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3f47-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/schedule/openShifts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3f47-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d3f47-117">Optional query parameters</span></span>

<span data-ttu-id="d3f47-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d3f47-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d3f47-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="d3f47-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d3f47-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3f47-120">Request headers</span></span>

| <span data-ttu-id="d3f47-121">名称</span><span class="sxs-lookup"><span data-stu-id="d3f47-121">Name</span></span>      |<span data-ttu-id="d3f47-122">说明</span><span class="sxs-lookup"><span data-stu-id="d3f47-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d3f47-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3f47-123">Authorization</span></span> | <span data-ttu-id="d3f47-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d3f47-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3f47-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3f47-126">Request body</span></span>

<span data-ttu-id="d3f47-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d3f47-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3f47-128">响应</span><span class="sxs-lookup"><span data-stu-id="d3f47-128">Response</span></span>

<span data-ttu-id="d3f47-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[openShift](../resources/openshift.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d3f47-129">If successful, this method returns a `200 OK` response code and the requested [openShift](../resources/openshift.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3f47-130">示例</span><span class="sxs-lookup"><span data-stu-id="d3f47-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3f47-131">请求</span><span class="sxs-lookup"><span data-stu-id="d3f47-131">Request</span></span>

<span data-ttu-id="d3f47-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d3f47-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_openshift"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/schedule/openShifts
```

### <a name="response"></a><span data-ttu-id="d3f47-133">响应</span><span class="sxs-lookup"><span data-stu-id="d3f47-133">Response</span></span>

<span data-ttu-id="d3f47-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d3f47-134">The following is an example of the response.</span></span>

> <span data-ttu-id="d3f47-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d3f47-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "sharedOpenShift": {
    "openSlotCount": 99
  },
  "draftOpenShift": {
    "openSlotCount": 99
  },
  "schedulingGroupId": "schedulingGroupId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get openShift",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
