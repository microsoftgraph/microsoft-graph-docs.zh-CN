---
title: 更新警报
description: 在任何集成的解决方案中更新可编辑的 alert 属性，以保持各个解决方案之间同步警报状态和分配。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: c2e16affa5bc6906dd16e1f063dc875b950842d2
ms.sourcegitcommit: 2a601cffdb8df375b2ee32a1f35b8f71e0ffd04f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2020
ms.locfileid: "41023024"
---
# <a name="update-alert"></a><span data-ttu-id="591ed-103">更新警报</span><span class="sxs-lookup"><span data-stu-id="591ed-103">Update alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="591ed-104">在任何集成的解决方案中更新可编辑的**alert**属性，以保持各个解决方案之间同步警报状态和分配。</span><span class="sxs-lookup"><span data-stu-id="591ed-104">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="591ed-105">此方法更新任何包含所引用警报 ID 的记录的解决方案。</span><span class="sxs-lookup"><span data-stu-id="591ed-105">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="591ed-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="591ed-106">Permissions</span></span>

<span data-ttu-id="591ed-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="591ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="591ed-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="591ed-109">Permission type</span></span>      | <span data-ttu-id="591ed-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="591ed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="591ed-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="591ed-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="591ed-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="591ed-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="591ed-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="591ed-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="591ed-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="591ed-114">Not supported.</span></span>  |
|<span data-ttu-id="591ed-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="591ed-115">Application</span></span> | <span data-ttu-id="591ed-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="591ed-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="591ed-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="591ed-117">HTTP request</span></span>

> <span data-ttu-id="591ed-118">**注意：** 您必须将**警报**ID 作为参数和 vendorInformation （包含`provider`和`vendor`使用此方法）包括在内。</span><span class="sxs-lookup"><span data-stu-id="591ed-118">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="591ed-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="591ed-119">Request headers</span></span>

| <span data-ttu-id="591ed-120">名称</span><span class="sxs-lookup"><span data-stu-id="591ed-120">Name</span></span>       | <span data-ttu-id="591ed-121">说明</span><span class="sxs-lookup"><span data-stu-id="591ed-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="591ed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="591ed-122">Authorization</span></span>  | <span data-ttu-id="591ed-123">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="591ed-123">Bearer {code}.</span></span> <span data-ttu-id="591ed-124">必需。</span><span class="sxs-lookup"><span data-stu-id="591ed-124">Required.</span></span>|
|<span data-ttu-id="591ed-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="591ed-125">Prefer</span></span> | <span data-ttu-id="591ed-126">返回 = 表示。</span><span class="sxs-lookup"><span data-stu-id="591ed-126">return=representation.</span></span> <span data-ttu-id="591ed-127">可选。</span><span class="sxs-lookup"><span data-stu-id="591ed-127">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="591ed-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="591ed-128">Request body</span></span>

<span data-ttu-id="591ed-129">在请求正文中，提供应更新的相关字段的值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="591ed-129">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="591ed-130">正文**必须**包含具有有效\*\*\*\* `provider`和`vendor`字段的 vendorInformation 属性。</span><span class="sxs-lookup"><span data-stu-id="591ed-130">The body **must** contain the **vendorInformation** property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="591ed-131">下表列出了可以为警报更新的字段。</span><span class="sxs-lookup"><span data-stu-id="591ed-131">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="591ed-132">未包含在请求正文中的现有属性的值不会更改。</span><span class="sxs-lookup"><span data-stu-id="591ed-132">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="591ed-133">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="591ed-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="591ed-134">属性</span><span class="sxs-lookup"><span data-stu-id="591ed-134">Property</span></span>   | <span data-ttu-id="591ed-135">类型</span><span class="sxs-lookup"><span data-stu-id="591ed-135">Type</span></span> |<span data-ttu-id="591ed-136">Description</span><span class="sxs-lookup"><span data-stu-id="591ed-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="591ed-137">assignedTo</span><span class="sxs-lookup"><span data-stu-id="591ed-137">assignedTo</span></span>|<span data-ttu-id="591ed-138">String</span><span class="sxs-lookup"><span data-stu-id="591ed-138">String</span></span>|<span data-ttu-id="591ed-139">为会审、调查或修正分配了警报的分析师的名称。</span><span class="sxs-lookup"><span data-stu-id="591ed-139">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="591ed-140">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="591ed-140">closedDateTime</span></span>|<span data-ttu-id="591ed-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="591ed-141">DateTimeOffset</span></span>|<span data-ttu-id="591ed-142">警报关闭的时间。</span><span class="sxs-lookup"><span data-stu-id="591ed-142">Time at which the alert was closed.</span></span> <span data-ttu-id="591ed-143">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="591ed-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="591ed-144">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="591ed-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="591ed-145">comments</span><span class="sxs-lookup"><span data-stu-id="591ed-145">comments</span></span>|<span data-ttu-id="591ed-146">字符串集合</span><span class="sxs-lookup"><span data-stu-id="591ed-146">String collection</span></span>|<span data-ttu-id="591ed-147">通知的分析师注释（针对客户通知管理）。</span><span class="sxs-lookup"><span data-stu-id="591ed-147">Analyst comments on the alert (for customer alert management).</span></span> <span data-ttu-id="591ed-148">此方法仅可使用以下值更新 "注释" 字段： `Closed in IPC`、 `Closed in MCAS`。</span><span class="sxs-lookup"><span data-stu-id="591ed-148">This method can update the comments field with the following values only: `Closed in IPC`, `Closed in MCAS`.</span></span>|
|<span data-ttu-id="591ed-149">反馈</span><span class="sxs-lookup"><span data-stu-id="591ed-149">feedback</span></span>|<span data-ttu-id="591ed-150">alertFeedback 枚举</span><span class="sxs-lookup"><span data-stu-id="591ed-150">alertFeedback enum</span></span>|<span data-ttu-id="591ed-151">分析师对警报的反馈。</span><span class="sxs-lookup"><span data-stu-id="591ed-151">Analyst feedback on the alert.</span></span> <span data-ttu-id="591ed-152">可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。</span><span class="sxs-lookup"><span data-stu-id="591ed-152">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="591ed-153">状态</span><span class="sxs-lookup"><span data-stu-id="591ed-153">status</span></span>|<span data-ttu-id="591ed-154">alertStatus 枚举</span><span class="sxs-lookup"><span data-stu-id="591ed-154">alertStatus enum</span></span>|<span data-ttu-id="591ed-155">警报生命周期状态（阶段）。</span><span class="sxs-lookup"><span data-stu-id="591ed-155">Alert life cycle status (stage).</span></span> <span data-ttu-id="591ed-156">可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。</span><span class="sxs-lookup"><span data-stu-id="591ed-156">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="591ed-157">tags</span><span class="sxs-lookup"><span data-stu-id="591ed-157">tags</span></span>|<span data-ttu-id="591ed-158">String 集合</span><span class="sxs-lookup"><span data-stu-id="591ed-158">String collection</span></span>|<span data-ttu-id="591ed-159">可应用于警报并可用作筛选条件的用户定义的标签（例如，"HVA"、"锯"）。</span><span class="sxs-lookup"><span data-stu-id="591ed-159">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="591ed-160">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="591ed-160">vendorInformation</span></span> |[<span data-ttu-id="591ed-161">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="591ed-161">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="591ed-162">包含有关安全产品/服务供应商、提供程序和子提供程序的详细信息的复杂类型（例如，供应商 = Microsoft；提供程序 = Windows Defender ATP；子提供程序 = AppLocker）。</span><span class="sxs-lookup"><span data-stu-id="591ed-162">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="591ed-163">**提供程序和供应商字段是必需的。**</span><span class="sxs-lookup"><span data-stu-id="591ed-163">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="591ed-164">响应</span><span class="sxs-lookup"><span data-stu-id="591ed-164">Response</span></span>

<span data-ttu-id="591ed-165">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="591ed-165">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="591ed-166">如果使用可选的请求标头，则该方法将`200 OK`在响应正文中返回响应代码和更新的[alert](../resources/alert.md)对象。</span><span class="sxs-lookup"><span data-stu-id="591ed-166">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="591ed-167">示例</span><span class="sxs-lookup"><span data-stu-id="591ed-167">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="591ed-168">示例1：不带首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="591ed-168">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="591ed-169">请求</span><span class="sxs-lookup"><span data-stu-id="591ed-169">Request</span></span>

<span data-ttu-id="591ed-170">以下是不带`Prefer`标头的请求示例。</span><span class="sxs-lookup"><span data-stu-id="591ed-170">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="591ed-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="591ed-171">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="591ed-172">C#</span><span class="sxs-lookup"><span data-stu-id="591ed-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="591ed-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="591ed-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="591ed-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="591ed-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="591ed-175">响应</span><span class="sxs-lookup"><span data-stu-id="591ed-175">Response</span></span>

<span data-ttu-id="591ed-176">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="591ed-176">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="591ed-177">示例2：具有首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="591ed-177">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="591ed-178">请求</span><span class="sxs-lookup"><span data-stu-id="591ed-178">Request</span></span>

<span data-ttu-id="591ed-179">下面的示例演示包含`Prefer`请求标头的请求。</span><span class="sxs-lookup"><span data-stu-id="591ed-179">The following example shows a request that includes the `Prefer` request header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="591ed-180">响应</span><span class="sxs-lookup"><span data-stu-id="591ed-180">Response</span></span>

<span data-ttu-id="591ed-181">以下是使用可选`Prefer: return=representation`请求标头时响应的示例。</span><span class="sxs-lookup"><span data-stu-id="591ed-181">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="591ed-p111">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="591ed-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
