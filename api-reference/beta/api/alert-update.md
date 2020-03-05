---
title: 更新警报
description: 在任何集成的解决方案中更新可编辑的 alert 属性，以保持各个解决方案之间同步警报状态和分配。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 963440a7d8d2c6035660a1cc831b474dbab68ee0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441612"
---
# <a name="update-alert"></a><span data-ttu-id="02f0d-103">更新警报</span><span class="sxs-lookup"><span data-stu-id="02f0d-103">Update alert</span></span>

<span data-ttu-id="02f0d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="02f0d-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02f0d-105">在任何集成的解决方案中更新可编辑的**alert**属性，以保持各个解决方案之间同步警报状态和分配。</span><span class="sxs-lookup"><span data-stu-id="02f0d-105">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="02f0d-106">此方法更新任何包含所引用警报 ID 的记录的解决方案。</span><span class="sxs-lookup"><span data-stu-id="02f0d-106">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="02f0d-107">权限</span><span class="sxs-lookup"><span data-stu-id="02f0d-107">Permissions</span></span>

<span data-ttu-id="02f0d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02f0d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02f0d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="02f0d-110">Permission type</span></span>      | <span data-ttu-id="02f0d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="02f0d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02f0d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02f0d-112">Delegated (work or school account)</span></span> |   <span data-ttu-id="02f0d-113">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02f0d-113">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="02f0d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02f0d-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="02f0d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="02f0d-115">Not supported.</span></span>  |
|<span data-ttu-id="02f0d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="02f0d-116">Application</span></span> | <span data-ttu-id="02f0d-117">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02f0d-117">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02f0d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02f0d-118">HTTP request</span></span>

> <span data-ttu-id="02f0d-119">**注意：** 您必须将**警报**ID 作为参数和 vendorInformation （包含`provider`和`vendor`使用此方法）包括在内。</span><span class="sxs-lookup"><span data-stu-id="02f0d-119">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="02f0d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="02f0d-120">Request headers</span></span>

| <span data-ttu-id="02f0d-121">名称</span><span class="sxs-lookup"><span data-stu-id="02f0d-121">Name</span></span>       | <span data-ttu-id="02f0d-122">说明</span><span class="sxs-lookup"><span data-stu-id="02f0d-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="02f0d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="02f0d-123">Authorization</span></span>  | <span data-ttu-id="02f0d-124">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="02f0d-124">Bearer {code}.</span></span> <span data-ttu-id="02f0d-125">必需。</span><span class="sxs-lookup"><span data-stu-id="02f0d-125">Required.</span></span>|
|<span data-ttu-id="02f0d-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="02f0d-126">Prefer</span></span> | <span data-ttu-id="02f0d-127">返回 = 表示。</span><span class="sxs-lookup"><span data-stu-id="02f0d-127">return=representation.</span></span> <span data-ttu-id="02f0d-128">可选。</span><span class="sxs-lookup"><span data-stu-id="02f0d-128">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02f0d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="02f0d-129">Request body</span></span>

<span data-ttu-id="02f0d-130">在请求正文中，提供应更新的相关字段的值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02f0d-130">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="02f0d-131">正文**必须**包含具有有效\*\*\*\* `provider`和`vendor`字段的 vendorInformation 属性。</span><span class="sxs-lookup"><span data-stu-id="02f0d-131">The body **must** contain the **vendorInformation** property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="02f0d-132">下表列出了可以为警报更新的字段。</span><span class="sxs-lookup"><span data-stu-id="02f0d-132">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="02f0d-133">未包含在请求正文中的现有属性的值不会更改。</span><span class="sxs-lookup"><span data-stu-id="02f0d-133">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="02f0d-134">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="02f0d-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="02f0d-135">属性</span><span class="sxs-lookup"><span data-stu-id="02f0d-135">Property</span></span>   | <span data-ttu-id="02f0d-136">类型</span><span class="sxs-lookup"><span data-stu-id="02f0d-136">Type</span></span> |<span data-ttu-id="02f0d-137">说明</span><span class="sxs-lookup"><span data-stu-id="02f0d-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02f0d-138">assignedTo</span><span class="sxs-lookup"><span data-stu-id="02f0d-138">assignedTo</span></span>|<span data-ttu-id="02f0d-139">String</span><span class="sxs-lookup"><span data-stu-id="02f0d-139">String</span></span>|<span data-ttu-id="02f0d-140">为会审、调查或修正分配了警报的分析师的名称。</span><span class="sxs-lookup"><span data-stu-id="02f0d-140">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="02f0d-141">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="02f0d-141">closedDateTime</span></span>|<span data-ttu-id="02f0d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02f0d-142">DateTimeOffset</span></span>|<span data-ttu-id="02f0d-143">警报关闭的时间。</span><span class="sxs-lookup"><span data-stu-id="02f0d-143">Time at which the alert was closed.</span></span> <span data-ttu-id="02f0d-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="02f0d-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="02f0d-145">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="02f0d-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="02f0d-146">comments</span><span class="sxs-lookup"><span data-stu-id="02f0d-146">comments</span></span>|<span data-ttu-id="02f0d-147">字符串集合</span><span class="sxs-lookup"><span data-stu-id="02f0d-147">String collection</span></span>|<span data-ttu-id="02f0d-148">通知的分析师注释（针对客户通知管理）。</span><span class="sxs-lookup"><span data-stu-id="02f0d-148">Analyst comments on the alert (for customer alert management).</span></span> <span data-ttu-id="02f0d-149">此方法仅可使用以下值更新 "注释" 字段： `Closed in IPC`、 `Closed in MCAS`。</span><span class="sxs-lookup"><span data-stu-id="02f0d-149">This method can update the comments field with the following values only: `Closed in IPC`, `Closed in MCAS`.</span></span>|
|<span data-ttu-id="02f0d-150">反馈</span><span class="sxs-lookup"><span data-stu-id="02f0d-150">feedback</span></span>|<span data-ttu-id="02f0d-151">alertFeedback 枚举</span><span class="sxs-lookup"><span data-stu-id="02f0d-151">alertFeedback enum</span></span>|<span data-ttu-id="02f0d-152">分析师对警报的反馈。</span><span class="sxs-lookup"><span data-stu-id="02f0d-152">Analyst feedback on the alert.</span></span> <span data-ttu-id="02f0d-153">可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。</span><span class="sxs-lookup"><span data-stu-id="02f0d-153">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="02f0d-154">status</span><span class="sxs-lookup"><span data-stu-id="02f0d-154">status</span></span>|<span data-ttu-id="02f0d-155">alertStatus 枚举</span><span class="sxs-lookup"><span data-stu-id="02f0d-155">alertStatus enum</span></span>|<span data-ttu-id="02f0d-156">警报生命周期状态（阶段）。</span><span class="sxs-lookup"><span data-stu-id="02f0d-156">Alert life cycle status (stage).</span></span> <span data-ttu-id="02f0d-157">可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。</span><span class="sxs-lookup"><span data-stu-id="02f0d-157">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="02f0d-158">标记</span><span class="sxs-lookup"><span data-stu-id="02f0d-158">tags</span></span>|<span data-ttu-id="02f0d-159">String 集合</span><span class="sxs-lookup"><span data-stu-id="02f0d-159">String collection</span></span>|<span data-ttu-id="02f0d-160">可应用于警报并可用作筛选条件的用户定义的标签（例如，"HVA"、"锯"）。</span><span class="sxs-lookup"><span data-stu-id="02f0d-160">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="02f0d-161">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="02f0d-161">vendorInformation</span></span> |[<span data-ttu-id="02f0d-162">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="02f0d-162">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="02f0d-163">包含有关安全产品/服务供应商、提供程序和子提供程序的详细信息的复杂类型（例如，供应商 = Microsoft；提供程序 = Windows Defender ATP；子提供程序 = AppLocker）。</span><span class="sxs-lookup"><span data-stu-id="02f0d-163">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="02f0d-164">**提供程序和供应商字段是必需的。**</span><span class="sxs-lookup"><span data-stu-id="02f0d-164">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="02f0d-165">响应</span><span class="sxs-lookup"><span data-stu-id="02f0d-165">Response</span></span>

<span data-ttu-id="02f0d-166">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="02f0d-166">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="02f0d-167">如果使用可选的请求标头，则该方法将`200 OK`在响应正文中返回响应代码和更新的[alert](../resources/alert.md)对象。</span><span class="sxs-lookup"><span data-stu-id="02f0d-167">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02f0d-168">示例</span><span class="sxs-lookup"><span data-stu-id="02f0d-168">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="02f0d-169">示例1：不带首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="02f0d-169">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="02f0d-170">请求</span><span class="sxs-lookup"><span data-stu-id="02f0d-170">Request</span></span>

<span data-ttu-id="02f0d-171">以下是不带`Prefer`标头的请求示例。</span><span class="sxs-lookup"><span data-stu-id="02f0d-171">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="http"></a>[<span data-ttu-id="02f0d-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="02f0d-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="02f0d-173">C#</span><span class="sxs-lookup"><span data-stu-id="02f0d-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02f0d-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02f0d-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02f0d-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02f0d-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="02f0d-176">响应</span><span class="sxs-lookup"><span data-stu-id="02f0d-176">Response</span></span>

<span data-ttu-id="02f0d-177">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="02f0d-177">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="02f0d-178">示例2：具有首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="02f0d-178">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="02f0d-179">请求</span><span class="sxs-lookup"><span data-stu-id="02f0d-179">Request</span></span>

<span data-ttu-id="02f0d-180">下面的示例演示包含`Prefer`请求标头的请求。</span><span class="sxs-lookup"><span data-stu-id="02f0d-180">The following example shows a request that includes the `Prefer` request header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": ["String"],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "vendorInformation":
    {
      "provider": "String",
      "vendor": "String"
    }
}
```

#### <a name="response"></a><span data-ttu-id="02f0d-181">响应</span><span class="sxs-lookup"><span data-stu-id="02f0d-181">Response</span></span>

<span data-ttu-id="02f0d-182">以下是使用可选`Prefer: return=representation`请求标头时响应的示例。</span><span class="sxs-lookup"><span data-stu-id="02f0d-182">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="02f0d-p111">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="02f0d-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "activityGroupName": "activityGroupName-value",
  "assignedTo": "assignedTo-value",
  "azureSubscriptionId": "azureSubscriptionId-value",
  "azureTenantId": "azureTenantId-value",
  "category": "category-value",
  "closedDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
