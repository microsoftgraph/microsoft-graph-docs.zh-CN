---
title: 更新警报
description: 更新任何集成解决方案中的可编辑警报属性，使警报状态和分配在解决方案之间保持同步。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 3af60a66413f605fc62ef550bb8c20448cc65c8d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048174"
---
# <a name="update-alert"></a><span data-ttu-id="84413-103">更新警报</span><span class="sxs-lookup"><span data-stu-id="84413-103">Update alert</span></span>

<span data-ttu-id="84413-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84413-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84413-105">更新任何集成 **解决方案** 中的可编辑警报属性，使警报状态和分配在解决方案之间保持同步。</span><span class="sxs-lookup"><span data-stu-id="84413-105">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="84413-106">此方法更新具有引用警报 ID 记录的任何解决方案。</span><span class="sxs-lookup"><span data-stu-id="84413-106">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="84413-107">权限</span><span class="sxs-lookup"><span data-stu-id="84413-107">Permissions</span></span>

<span data-ttu-id="84413-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84413-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84413-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="84413-110">Permission type</span></span>      | <span data-ttu-id="84413-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="84413-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84413-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84413-112">Delegated (work or school account)</span></span> |   <span data-ttu-id="84413-113">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84413-113">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="84413-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84413-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="84413-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="84413-115">Not supported.</span></span>  |
|<span data-ttu-id="84413-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="84413-116">Application</span></span> | <span data-ttu-id="84413-117">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84413-117">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="84413-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84413-118">HTTP request</span></span>

> <span data-ttu-id="84413-119">**注意：** 必须使用此方法 **将警报** ID 作为参数和 vendorInformation 包含 和 `provider` `vendor` 。</span><span class="sxs-lookup"><span data-stu-id="84413-119">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="84413-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="84413-120">Request headers</span></span>

| <span data-ttu-id="84413-121">名称</span><span class="sxs-lookup"><span data-stu-id="84413-121">Name</span></span>       | <span data-ttu-id="84413-122">说明</span><span class="sxs-lookup"><span data-stu-id="84413-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="84413-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84413-123">Authorization</span></span>  | <span data-ttu-id="84413-124">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="84413-124">Bearer {code}.</span></span> <span data-ttu-id="84413-125">必需。</span><span class="sxs-lookup"><span data-stu-id="84413-125">Required.</span></span>|
|<span data-ttu-id="84413-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="84413-126">Prefer</span></span> | <span data-ttu-id="84413-127">return=representation。</span><span class="sxs-lookup"><span data-stu-id="84413-127">return=representation.</span></span> <span data-ttu-id="84413-128">可选。</span><span class="sxs-lookup"><span data-stu-id="84413-128">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84413-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="84413-129">Request body</span></span>

<span data-ttu-id="84413-130">在请求正文中，提供应更新的相关字段值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84413-130">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="84413-131">正文 **必须** 包含具有 有效 和 字段的 **vendorInformation** `provider` `vendor` 属性。</span><span class="sxs-lookup"><span data-stu-id="84413-131">The body **must** contain the **vendorInformation** property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="84413-132">下表列出了可以针对警报进行更新的字段。</span><span class="sxs-lookup"><span data-stu-id="84413-132">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="84413-133">请求正文中不包含的现有属性的值不会更改。</span><span class="sxs-lookup"><span data-stu-id="84413-133">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="84413-134">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="84413-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="84413-135">属性</span><span class="sxs-lookup"><span data-stu-id="84413-135">Property</span></span>   | <span data-ttu-id="84413-136">类型</span><span class="sxs-lookup"><span data-stu-id="84413-136">Type</span></span> |<span data-ttu-id="84413-137">说明</span><span class="sxs-lookup"><span data-stu-id="84413-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84413-138">assignedTo</span><span class="sxs-lookup"><span data-stu-id="84413-138">assignedTo</span></span>|<span data-ttu-id="84413-139">String</span><span class="sxs-lookup"><span data-stu-id="84413-139">String</span></span>|<span data-ttu-id="84413-140">分配警报的分析员的姓名，用于会审、调查或修正。</span><span class="sxs-lookup"><span data-stu-id="84413-140">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="84413-141">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="84413-141">closedDateTime</span></span>|<span data-ttu-id="84413-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84413-142">DateTimeOffset</span></span>|<span data-ttu-id="84413-143">警报关闭的时间。</span><span class="sxs-lookup"><span data-stu-id="84413-143">Time at which the alert was closed.</span></span> <span data-ttu-id="84413-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="84413-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="84413-145">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="84413-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="84413-146">comments</span><span class="sxs-lookup"><span data-stu-id="84413-146">comments</span></span>|<span data-ttu-id="84413-147">字符串集合</span><span class="sxs-lookup"><span data-stu-id="84413-147">String collection</span></span>|<span data-ttu-id="84413-148">针对客户警报管理的警报 (分析员) 。</span><span class="sxs-lookup"><span data-stu-id="84413-148">Analyst comments on the alert (for customer alert management).</span></span> <span data-ttu-id="84413-149">此方法只能使用下列值更新 comments 字段 `Closed in IPC` `Closed in MCAS` ：、。</span><span class="sxs-lookup"><span data-stu-id="84413-149">This method can update the comments field with the following values only: `Closed in IPC`, `Closed in MCAS`.</span></span>|
|<span data-ttu-id="84413-150">反馈</span><span class="sxs-lookup"><span data-stu-id="84413-150">feedback</span></span>|<span data-ttu-id="84413-151">alertFeedback 枚举</span><span class="sxs-lookup"><span data-stu-id="84413-151">alertFeedback enum</span></span>|<span data-ttu-id="84413-152">分析师对警报的反馈。</span><span class="sxs-lookup"><span data-stu-id="84413-152">Analyst feedback on the alert.</span></span> <span data-ttu-id="84413-153">可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。</span><span class="sxs-lookup"><span data-stu-id="84413-153">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="84413-154">状态</span><span class="sxs-lookup"><span data-stu-id="84413-154">status</span></span>|<span data-ttu-id="84413-155">alertStatus 枚举</span><span class="sxs-lookup"><span data-stu-id="84413-155">alertStatus enum</span></span>|<span data-ttu-id="84413-156">警报生命周期状态 (阶段) 。</span><span class="sxs-lookup"><span data-stu-id="84413-156">Alert life cycle status (stage).</span></span> <span data-ttu-id="84413-157">可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。</span><span class="sxs-lookup"><span data-stu-id="84413-157">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="84413-158">tags</span><span class="sxs-lookup"><span data-stu-id="84413-158">tags</span></span>|<span data-ttu-id="84413-159">字符串集合</span><span class="sxs-lookup"><span data-stu-id="84413-159">String collection</span></span>|<span data-ttu-id="84413-160">可应用于警报并可以作为筛选器条件的用户可定义标签 (例如，"HVA"、"SAW) "</span><span class="sxs-lookup"><span data-stu-id="84413-160">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="84413-161">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="84413-161">vendorInformation</span></span> |[<span data-ttu-id="84413-162">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="84413-162">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="84413-163">包含有关安全产品/服务供应商、提供程序和子提供程序的详细信息的复杂类型（例如，供应商 = Microsoft；提供程序 = Windows Defender ATP；子提供程序 = AppLocker）。</span><span class="sxs-lookup"><span data-stu-id="84413-163">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="84413-164">**提供程序和供应商字段是必需的。**</span><span class="sxs-lookup"><span data-stu-id="84413-164">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="84413-165">响应</span><span class="sxs-lookup"><span data-stu-id="84413-165">Response</span></span>

<span data-ttu-id="84413-166">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="84413-166">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="84413-167">如果使用可选请求标头，则该方法在响应正文中返回 响应 `200 OK` 代码和更新的 [alert](../resources/alert.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="84413-167">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="84413-168">示例</span><span class="sxs-lookup"><span data-stu-id="84413-168">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="84413-169">示例 1：不带 Prefer 标头的请求</span><span class="sxs-lookup"><span data-stu-id="84413-169">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="84413-170">请求</span><span class="sxs-lookup"><span data-stu-id="84413-170">Request</span></span>

<span data-ttu-id="84413-171">下面是一个没有 标头的请求 `Prefer` 示例。</span><span class="sxs-lookup"><span data-stu-id="84413-171">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="http"></a>[<span data-ttu-id="84413-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="84413-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_alert_1"
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
# <a name="c"></a>[<span data-ttu-id="84413-173">C#</span><span class="sxs-lookup"><span data-stu-id="84413-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84413-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84413-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84413-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84413-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84413-176">Java</span><span class="sxs-lookup"><span data-stu-id="84413-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="84413-177">响应</span><span class="sxs-lookup"><span data-stu-id="84413-177">Response</span></span>

<span data-ttu-id="84413-178">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="84413-178">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="84413-179">示例 2：具有 Prefer 标头的请求</span><span class="sxs-lookup"><span data-stu-id="84413-179">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="84413-180">请求</span><span class="sxs-lookup"><span data-stu-id="84413-180">Request</span></span>

<span data-ttu-id="84413-181">以下示例显示包含请求标头 `Prefer` 的请求。</span><span class="sxs-lookup"><span data-stu-id="84413-181">The following example shows a request that includes the `Prefer` request header.</span></span>


# <a name="http"></a>[<span data-ttu-id="84413-182">HTTP</span><span class="sxs-lookup"><span data-stu-id="84413-182">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_alert_2"
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
# <a name="c"></a>[<span data-ttu-id="84413-183">C#</span><span class="sxs-lookup"><span data-stu-id="84413-183">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-alert-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="84413-184">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84413-184">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-alert-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84413-185">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84413-185">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-alert-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84413-186">Java</span><span class="sxs-lookup"><span data-stu-id="84413-186">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-alert-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="84413-187">响应</span><span class="sxs-lookup"><span data-stu-id="84413-187">Response</span></span>

<span data-ttu-id="84413-188">下面是使用可选请求标头 `Prefer: return=representation` 时的响应示例。</span><span class="sxs-lookup"><span data-stu-id="84413-188">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="84413-189">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="84413-189">**Note:** The response object shown here might be shortened for readability.</span></span>
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


