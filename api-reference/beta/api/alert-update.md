---
title: 更新警报
description: 在任何集成的解决方案中更新可编辑的 alert 属性, 以保持各个解决方案之间同步警报状态和分配。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8b1fec6bfca2ce116bc35c4a7c8a115418b15012
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459218"
---
# <a name="update-alert"></a><span data-ttu-id="a0123-103">更新警报</span><span class="sxs-lookup"><span data-stu-id="a0123-103">Update alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0123-104">在任何集成的解决方案中更新可编辑的**alert**属性, 以保持各个解决方案之间同步警报状态和分配。</span><span class="sxs-lookup"><span data-stu-id="a0123-104">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="a0123-105">此方法更新任何包含所引用警报 ID 的记录的解决方案。</span><span class="sxs-lookup"><span data-stu-id="a0123-105">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0123-106">权限</span><span class="sxs-lookup"><span data-stu-id="a0123-106">Permissions</span></span>

<span data-ttu-id="a0123-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0123-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0123-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0123-109">Permission type</span></span>      | <span data-ttu-id="a0123-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0123-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0123-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0123-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="a0123-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0123-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="a0123-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0123-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a0123-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0123-114">Not supported.</span></span>  |
|<span data-ttu-id="a0123-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0123-115">Application</span></span> | <span data-ttu-id="a0123-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0123-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a0123-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0123-117">HTTP request</span></span>

> <span data-ttu-id="a0123-118">**注意:** 您必须将**警报**ID 作为参数和 vendorInformation (包含`provider`和`vendor`使用此方法) 包括在内。</span><span class="sxs-lookup"><span data-stu-id="a0123-118">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="a0123-119">请求头</span><span class="sxs-lookup"><span data-stu-id="a0123-119">Request headers</span></span>

| <span data-ttu-id="a0123-120">名称</span><span class="sxs-lookup"><span data-stu-id="a0123-120">Name</span></span>       | <span data-ttu-id="a0123-121">说明</span><span class="sxs-lookup"><span data-stu-id="a0123-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a0123-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0123-122">Authorization</span></span>  | <span data-ttu-id="a0123-123">持有者 {代码}。</span><span class="sxs-lookup"><span data-stu-id="a0123-123">Bearer {code}.</span></span> <span data-ttu-id="a0123-124">必需。</span><span class="sxs-lookup"><span data-stu-id="a0123-124">Required.</span></span>|
|<span data-ttu-id="a0123-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="a0123-125">Prefer</span></span> | <span data-ttu-id="a0123-126">return = 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0123-126">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="a0123-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0123-127">Request body</span></span>

<span data-ttu-id="a0123-128">在请求正文中, 提供应更新的相关字段的值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0123-128">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a0123-129">正文**必须**包含具有有效`vendorInformation` `provider`和`vendor`字段的属性。</span><span class="sxs-lookup"><span data-stu-id="a0123-129">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="a0123-130">下表列出了可以为警报更新的字段。</span><span class="sxs-lookup"><span data-stu-id="a0123-130">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="a0123-131">未包含在请求正文中的现有属性的值不会更改。</span><span class="sxs-lookup"><span data-stu-id="a0123-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="a0123-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a0123-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a0123-133">属性</span><span class="sxs-lookup"><span data-stu-id="a0123-133">Property</span></span>   | <span data-ttu-id="a0123-134">类型</span><span class="sxs-lookup"><span data-stu-id="a0123-134">Type</span></span> |<span data-ttu-id="a0123-135">说明</span><span class="sxs-lookup"><span data-stu-id="a0123-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a0123-136">assignedTo</span><span class="sxs-lookup"><span data-stu-id="a0123-136">assignedTo</span></span>|<span data-ttu-id="a0123-137">String</span><span class="sxs-lookup"><span data-stu-id="a0123-137">String</span></span>|<span data-ttu-id="a0123-138">为会审、调查或修正分配了警报的分析师的名称。</span><span class="sxs-lookup"><span data-stu-id="a0123-138">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="a0123-139">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0123-139">closedDateTime</span></span>|<span data-ttu-id="a0123-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0123-140">DateTimeOffset</span></span>|<span data-ttu-id="a0123-141">警报关闭的时间。</span><span class="sxs-lookup"><span data-stu-id="a0123-141">Time at which the alert was closed.</span></span> <span data-ttu-id="a0123-142">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="a0123-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a0123-143">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="a0123-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a0123-144">comments</span><span class="sxs-lookup"><span data-stu-id="a0123-144">comments</span></span>|<span data-ttu-id="a0123-145">String collection</span><span class="sxs-lookup"><span data-stu-id="a0123-145">String collection</span></span>|<span data-ttu-id="a0123-146">通知的分析师注释 (针对客户通知管理)。</span><span class="sxs-lookup"><span data-stu-id="a0123-146">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="a0123-147">征求</span><span class="sxs-lookup"><span data-stu-id="a0123-147">feedback</span></span>|<span data-ttu-id="a0123-148">alertFeedback 枚举</span><span class="sxs-lookup"><span data-stu-id="a0123-148">alertFeedback enum</span></span>|<span data-ttu-id="a0123-149">通知的分析师反馈。</span><span class="sxs-lookup"><span data-stu-id="a0123-149">Analyst feedback on the alert.</span></span> <span data-ttu-id="a0123-150">可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。</span><span class="sxs-lookup"><span data-stu-id="a0123-150">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="a0123-151">status</span><span class="sxs-lookup"><span data-stu-id="a0123-151">status</span></span>|<span data-ttu-id="a0123-152">alertStatus 枚举</span><span class="sxs-lookup"><span data-stu-id="a0123-152">alertStatus enum</span></span>|<span data-ttu-id="a0123-153">警报生命周期状态 (阶段)。</span><span class="sxs-lookup"><span data-stu-id="a0123-153">Alert life cycle status (stage).</span></span> <span data-ttu-id="a0123-154">可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。</span><span class="sxs-lookup"><span data-stu-id="a0123-154">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="a0123-155">tags</span><span class="sxs-lookup"><span data-stu-id="a0123-155">tags</span></span>|<span data-ttu-id="a0123-156">String 集合</span><span class="sxs-lookup"><span data-stu-id="a0123-156">String collection</span></span>|<span data-ttu-id="a0123-157">可应用于警报并可用作筛选条件的用户定义的标签 (例如, "HVA"、"锯")。</span><span class="sxs-lookup"><span data-stu-id="a0123-157">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="a0123-158">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="a0123-158">vendorInformation</span></span> |[<span data-ttu-id="a0123-159">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="a0123-159">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="a0123-160">包含有关安全产品/服务供应商、提供程序和 subprovider 的详细信息的复杂类型 (例如, 供应商 = Microsoft; provider = Windows Defender ATP; subprovider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="a0123-160">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="a0123-161">**提供程序和供应商字段是必需的。**</span><span class="sxs-lookup"><span data-stu-id="a0123-161">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="a0123-162">响应</span><span class="sxs-lookup"><span data-stu-id="a0123-162">Response</span></span>

<span data-ttu-id="a0123-163">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a0123-163">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="a0123-164">如果使用可选的请求标头, 则该方法将`200 OK`在响应正文中返回响应代码和更新的[alert](../resources/alert.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a0123-164">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0123-165">示例</span><span class="sxs-lookup"><span data-stu-id="a0123-165">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="a0123-166">示例 1: 不带首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="a0123-166">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="a0123-167">请求</span><span class="sxs-lookup"><span data-stu-id="a0123-167">Request</span></span>

<span data-ttu-id="a0123-168">以下是不带`Prefer`标头的请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0123-168">The following is an example of the request without the `Prefer` header.</span></span>
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

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="a0123-169">响应</span><span class="sxs-lookup"><span data-stu-id="a0123-169">Response</span></span>

<span data-ttu-id="a0123-170">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="a0123-170">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="a0123-171">示例 2: 具有首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="a0123-171">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="a0123-172">请求</span><span class="sxs-lookup"><span data-stu-id="a0123-172">Request</span></span>

<span data-ttu-id="a0123-173">下面的示例演示包含`Prefer`请求标头的请求。</span><span class="sxs-lookup"><span data-stu-id="a0123-173">The following example shows a request that includes the `Prefer` request header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="a0123-174">响应</span><span class="sxs-lookup"><span data-stu-id="a0123-174">Response</span></span>

<span data-ttu-id="a0123-175">以下是使用可选`Prefer: return=representation`请求标头时响应的示例。</span><span class="sxs-lookup"><span data-stu-id="a0123-175">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="a0123-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a0123-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/alert-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
