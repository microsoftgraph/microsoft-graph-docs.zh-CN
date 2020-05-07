---
title: 获取 timeOffRequest
description: 检索 timeOffRequest 对象的属性和关系。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7b1f20f71db24e39b5e129cc958f1e0ed182a570
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154288"
---
# <a name="get-timeoffrequest"></a><span data-ttu-id="44c30-103">获取 timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="44c30-103">Get timeOffRequest</span></span>

<span data-ttu-id="44c30-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44c30-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="44c30-105">检索[timeoffrequest](../resources/timeoffrequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="44c30-105">Retrieve the properties and relationships of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="44c30-106">权限</span><span class="sxs-lookup"><span data-stu-id="44c30-106">Permissions</span></span>

<span data-ttu-id="44c30-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="44c30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44c30-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="44c30-109">Permission type</span></span>                        | <span data-ttu-id="44c30-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="44c30-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="44c30-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="44c30-111">Delegated (work or school account)</span></span> | <span data-ttu-id="44c30-112">请参阅 all、Group、Group. all、Schedule、Group、Group。所有</span><span class="sxs-lookup"><span data-stu-id="44c30-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="44c30-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="44c30-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44c30-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="44c30-114">Not supported.</span></span>    |
|<span data-ttu-id="44c30-115">Application</span><span class="sxs-lookup"><span data-stu-id="44c30-115">Application</span></span> | <span data-ttu-id="44c30-116">Schedule. All、Schedule、All</span><span class="sxs-lookup"><span data-stu-id="44c30-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="44c30-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="44c30-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="44c30-118">全局管理员可以访问他们不是其成员的组。</span><span class="sxs-lookup"><span data-stu-id="44c30-118">Global admins can access groups that they are not a member of.</span></span> <span data-ttu-id="44c30-119">目前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="44c30-119">currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="44c30-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="44c30-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="44c30-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="44c30-121">Optional query parameters</span></span>

<span data-ttu-id="44c30-122">此方法不支持 OData 查询参数来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="44c30-122">This method does not support OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="44c30-123">请求头</span><span class="sxs-lookup"><span data-stu-id="44c30-123">Request headers</span></span>

| <span data-ttu-id="44c30-124">名称</span><span class="sxs-lookup"><span data-stu-id="44c30-124">Name</span></span>      |<span data-ttu-id="44c30-125">说明</span><span class="sxs-lookup"><span data-stu-id="44c30-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="44c30-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="44c30-126">Authorization</span></span> | <span data-ttu-id="44c30-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="44c30-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="44c30-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="44c30-129">Request body</span></span>

<span data-ttu-id="44c30-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="44c30-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44c30-131">响应</span><span class="sxs-lookup"><span data-stu-id="44c30-131">Response</span></span>

<span data-ttu-id="44c30-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[timeOffRequest](../resources/timeoffrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="44c30-132">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="44c30-133">示例</span><span class="sxs-lookup"><span data-stu-id="44c30-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="44c30-134">请求</span><span class="sxs-lookup"><span data-stu-id="44c30-134">Request</span></span>

<span data-ttu-id="44c30-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="44c30-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
---


### <a name="response"></a><span data-ttu-id="44c30-136">响应</span><span class="sxs-lookup"><span data-stu-id="44c30-136">Response</span></span>

<span data-ttu-id="44c30-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="44c30-137">The following is an example of the response.</span></span>

> <span data-ttu-id="44c30-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="44c30-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "startDateTime": "datetime-value",
  "endDateTime": "datetime-value",
  "timeOffReasonId": "timeOffReasonId-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
