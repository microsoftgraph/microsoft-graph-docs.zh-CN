---
title: 更新 timeoffrequest
description: 更新 timeoffrequest 对象的属性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4e961a197620f27de11397952c2d868dcec848c3
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895580"
---
# <a name="update-timeoffrequest"></a><span data-ttu-id="ac99b-103">更新 timeoffrequest</span><span class="sxs-lookup"><span data-stu-id="ac99b-103">Update timeoffrequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac99b-104">更新[timeoffrequest](../resources/timeoffrequest.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ac99b-104">Update the properties of [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac99b-105">权限</span><span class="sxs-lookup"><span data-stu-id="ac99b-105">Permissions</span></span>

<span data-ttu-id="ac99b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac99b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ac99b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac99b-108">Permission type</span></span>                        | <span data-ttu-id="ac99b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac99b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ac99b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac99b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ac99b-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac99b-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="ac99b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac99b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac99b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac99b-113">Not supported.</span></span> |
| <span data-ttu-id="ac99b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac99b-114">Application</span></span>                            | <span data-ttu-id="ac99b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac99b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac99b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac99b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/timeOffRequests
```

## <a name="request-headers"></a><span data-ttu-id="ac99b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac99b-117">Request headers</span></span>

| <span data-ttu-id="ac99b-118">名称</span><span class="sxs-lookup"><span data-stu-id="ac99b-118">Name</span></span>       | <span data-ttu-id="ac99b-119">说明</span><span class="sxs-lookup"><span data-stu-id="ac99b-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ac99b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac99b-120">Authorization</span></span> | <span data-ttu-id="ac99b-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="ac99b-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac99b-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac99b-122">Request body</span></span>

<span data-ttu-id="ac99b-123">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="ac99b-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ac99b-124">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="ac99b-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ac99b-125">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ac99b-125">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ac99b-126">属性</span><span class="sxs-lookup"><span data-stu-id="ac99b-126">Property</span></span>     | <span data-ttu-id="ac99b-127">类型</span><span class="sxs-lookup"><span data-stu-id="ac99b-127">Type</span></span>        | <span data-ttu-id="ac99b-128">说明</span><span class="sxs-lookup"><span data-stu-id="ac99b-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ac99b-129">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ac99b-129">endDateTime</span></span>|<span data-ttu-id="ac99b-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac99b-130">DateTimeOffset</span></span>|<span data-ttu-id="ac99b-131">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ac99b-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ac99b-132">例如，2014年1月1日午夜 UTC 将如下所示： ' 2014-01-01T00：00： 00Z '</span><span class="sxs-lookup"><span data-stu-id="ac99b-132">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="ac99b-133">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ac99b-133">startDateTime</span></span>|<span data-ttu-id="ac99b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac99b-134">DateTimeOffset</span></span>|<span data-ttu-id="ac99b-135">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ac99b-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ac99b-136">例如，2014年1月1日午夜 UTC 将如下所示： ' 2014-01-01T00：00： 00Z '</span><span class="sxs-lookup"><span data-stu-id="ac99b-136">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="ac99b-137">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="ac99b-137">timeOffReasonId</span></span>|<span data-ttu-id="ac99b-138">字符串</span><span class="sxs-lookup"><span data-stu-id="ac99b-138">String</span></span>|<span data-ttu-id="ac99b-139">请求的时间关的原因。</span><span class="sxs-lookup"><span data-stu-id="ac99b-139">Reason for the requested time off.</span></span>|

## <a name="response"></a><span data-ttu-id="ac99b-140">响应</span><span class="sxs-lookup"><span data-stu-id="ac99b-140">Response</span></span>

<span data-ttu-id="ac99b-141">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[timeOffRequest](../resources/timeoffrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ac99b-141">If successful, this method returns a `200 OK` response code and an updated [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ac99b-142">示例</span><span class="sxs-lookup"><span data-stu-id="ac99b-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ac99b-143">请求</span><span class="sxs-lookup"><span data-stu-id="ac99b-143">Request</span></span>

<span data-ttu-id="ac99b-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ac99b-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_timeoffrequest"
}-->

```http
PATCH https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests
Content-type: application/json

{
  "startDateTime": "datetime-value",
  "endDateTime": "datetime-value",
  "timeOffReasonId": "timeOffReasonId-value"
}
```

### <a name="response"></a><span data-ttu-id="ac99b-145">响应</span><span class="sxs-lookup"><span data-stu-id="ac99b-145">Response</span></span>

<span data-ttu-id="ac99b-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ac99b-146">The following is an example of the response.</span></span>

> <span data-ttu-id="ac99b-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ac99b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Update timeoffrequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->