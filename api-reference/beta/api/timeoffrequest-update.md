---
title: 更新 timeoffrequest
description: 更新 timeoffrequest 对象的属性。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2197e0e4e2f9c78337a6d5ae06d6c1e106f77afa
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863527"
---
# <a name="update-timeoffrequest"></a><span data-ttu-id="9747a-103">更新 timeoffrequest</span><span class="sxs-lookup"><span data-stu-id="9747a-103">Update timeoffrequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9747a-104">更新[timeoffrequest](../resources/timeoffrequest.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9747a-104">Update the properties of a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9747a-105">权限</span><span class="sxs-lookup"><span data-stu-id="9747a-105">Permissions</span></span>

<span data-ttu-id="9747a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9747a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9747a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9747a-108">Permission type</span></span>                        | <span data-ttu-id="9747a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9747a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9747a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9747a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9747a-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9747a-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="9747a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9747a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9747a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9747a-113">Not supported.</span></span> |
|<span data-ttu-id="9747a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9747a-114">Application</span></span> | <span data-ttu-id="9747a-115">计划的所有写。 \*</span><span class="sxs-lookup"><span data-stu-id="9747a-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="9747a-116">\***重要说明：** 应用程序权限当前仅在专用预览中，不可供公众使用。</span><span class="sxs-lookup"><span data-stu-id="9747a-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="9747a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9747a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /teams/{id}/schedule/timeOffRequests
```

## <a name="request-headers"></a><span data-ttu-id="9747a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9747a-118">Request headers</span></span>

| <span data-ttu-id="9747a-119">名称</span><span class="sxs-lookup"><span data-stu-id="9747a-119">Name</span></span>       | <span data-ttu-id="9747a-120">说明</span><span class="sxs-lookup"><span data-stu-id="9747a-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9747a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9747a-121">Authorization</span></span> | <span data-ttu-id="9747a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9747a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9747a-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="9747a-124">Content-type</span></span> | <span data-ttu-id="9747a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="9747a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9747a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9747a-127">Request body</span></span>

<span data-ttu-id="9747a-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="9747a-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9747a-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="9747a-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9747a-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9747a-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9747a-131">属性</span><span class="sxs-lookup"><span data-stu-id="9747a-131">Property</span></span>     | <span data-ttu-id="9747a-132">类型</span><span class="sxs-lookup"><span data-stu-id="9747a-132">Type</span></span>        | <span data-ttu-id="9747a-133">说明</span><span class="sxs-lookup"><span data-stu-id="9747a-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9747a-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9747a-134">endDateTime</span></span>|<span data-ttu-id="9747a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9747a-135">DateTimeOffset</span></span>|<span data-ttu-id="9747a-136">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="9747a-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9747a-137">例如，2014年1月1日午夜 UTC 将如下所示： ' 2014-01-01T00：00： 00Z '</span><span class="sxs-lookup"><span data-stu-id="9747a-137">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="9747a-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9747a-138">startDateTime</span></span>|<span data-ttu-id="9747a-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9747a-139">DateTimeOffset</span></span>|<span data-ttu-id="9747a-140">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="9747a-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9747a-141">例如，2014年1月1日午夜 UTC 将如下所示： ' 2014-01-01T00：00： 00Z '</span><span class="sxs-lookup"><span data-stu-id="9747a-141">For example, midnight UTC on Jan 1, 2014 would look like this: \`'2014-01-01T00:00:00Z'</span></span>|
|<span data-ttu-id="9747a-142">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="9747a-142">timeOffReasonId</span></span>|<span data-ttu-id="9747a-143">String</span><span class="sxs-lookup"><span data-stu-id="9747a-143">String</span></span>|<span data-ttu-id="9747a-144">请求的时间关的原因。</span><span class="sxs-lookup"><span data-stu-id="9747a-144">Reason for the requested time off.</span></span>|

## <a name="response"></a><span data-ttu-id="9747a-145">响应</span><span class="sxs-lookup"><span data-stu-id="9747a-145">Response</span></span>

<span data-ttu-id="9747a-146">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[timeOffRequest](../resources/timeoffrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9747a-146">If successful, this method returns a `200 OK` response code and an updated [timeOffRequest](../resources/timeoffrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9747a-147">示例</span><span class="sxs-lookup"><span data-stu-id="9747a-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9747a-148">请求</span><span class="sxs-lookup"><span data-stu-id="9747a-148">Request</span></span>

<span data-ttu-id="9747a-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9747a-149">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9747a-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="9747a-150">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9747a-151">C#</span><span class="sxs-lookup"><span data-stu-id="9747a-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9747a-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9747a-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9747a-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9747a-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9747a-154">响应</span><span class="sxs-lookup"><span data-stu-id="9747a-154">Response</span></span>

<span data-ttu-id="9747a-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9747a-155">The following is an example of the response.</span></span>

> <span data-ttu-id="9747a-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9747a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
