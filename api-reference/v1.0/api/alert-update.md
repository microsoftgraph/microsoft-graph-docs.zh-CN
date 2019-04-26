---
title: 更新警报
description: 在任何集成的解决方案中更新可编辑的**alert**属性, 以保持各个解决方案之间同步警报状态和分配。 此方法更新任何包含所引用警报 ID 的记录的解决方案。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 42bc945dde726466439802350796d628ee438e22
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32551506"
---
# <a name="update-alert"></a><span data-ttu-id="6786e-104">更新警报</span><span class="sxs-lookup"><span data-stu-id="6786e-104">Update alert</span></span>

<span data-ttu-id="6786e-105">在任何集成的解决方案中更新可编辑的**alert**属性, 以保持各个解决方案之间同步警报状态和分配。</span><span class="sxs-lookup"><span data-stu-id="6786e-105">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="6786e-106">此方法更新任何包含所引用警报 ID 的记录的解决方案。</span><span class="sxs-lookup"><span data-stu-id="6786e-106">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="6786e-107">权限</span><span class="sxs-lookup"><span data-stu-id="6786e-107">Permissions</span></span>

<span data-ttu-id="6786e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6786e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6786e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6786e-110">Permission type</span></span>                        | <span data-ttu-id="6786e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6786e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="6786e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6786e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6786e-113">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6786e-113">SecurityEvents.ReadWrite.All</span></span>        |
| <span data-ttu-id="6786e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6786e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6786e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6786e-115">Not supported.</span></span>                      |
| <span data-ttu-id="6786e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6786e-116">Application</span></span>                            | <span data-ttu-id="6786e-117">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6786e-117">SecurityEvents.ReadWrite.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="6786e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6786e-118">HTTP request</span></span>

> <span data-ttu-id="6786e-119">**注意:** 您必须将**警报**ID 作为参数和 vendorInformation (包含`provider`和`vendor`使用此方法) 包括在内。</span><span class="sxs-lookup"><span data-stu-id="6786e-119">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="6786e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6786e-120">Request headers</span></span>

| <span data-ttu-id="6786e-121">名称</span><span class="sxs-lookup"><span data-stu-id="6786e-121">Name</span></span>          | <span data-ttu-id="6786e-122">说明</span><span class="sxs-lookup"><span data-stu-id="6786e-122">Description</span></span>              |
|:--------------|:-------------------------|
| <span data-ttu-id="6786e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6786e-123">Authorization</span></span> | <span data-ttu-id="6786e-124">持有者 {代码}。</span><span class="sxs-lookup"><span data-stu-id="6786e-124">Bearer {code}.</span></span> <span data-ttu-id="6786e-125">必需。</span><span class="sxs-lookup"><span data-stu-id="6786e-125">Required.</span></span> |
| <span data-ttu-id="6786e-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="6786e-126">Prefer</span></span>        | <span data-ttu-id="6786e-127">return = 表示形式</span><span class="sxs-lookup"><span data-stu-id="6786e-127">return=representation</span></span>    |

## <a name="request-body"></a><span data-ttu-id="6786e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6786e-128">Request body</span></span>

<span data-ttu-id="6786e-129">在请求正文中, 提供应更新的相关字段的值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6786e-129">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6786e-130">正文**必须**包含具有有效`vendorInformation` `provider`和`vendor`字段的属性。</span><span class="sxs-lookup"><span data-stu-id="6786e-130">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="6786e-131">下表列出了可以为警报更新的字段。</span><span class="sxs-lookup"><span data-stu-id="6786e-131">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="6786e-132">未包含在请求正文中的现有属性的值不会更改。</span><span class="sxs-lookup"><span data-stu-id="6786e-132">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="6786e-133">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="6786e-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6786e-134">属性</span><span class="sxs-lookup"><span data-stu-id="6786e-134">Property</span></span>          | <span data-ttu-id="6786e-135">类型</span><span class="sxs-lookup"><span data-stu-id="6786e-135">Type</span></span>                                                                   | <span data-ttu-id="6786e-136">说明</span><span class="sxs-lookup"><span data-stu-id="6786e-136">Description</span></span> |
|:------------------|:-----------------------------------------------------------------------|:--|
| <span data-ttu-id="6786e-137">assignedTo</span><span class="sxs-lookup"><span data-stu-id="6786e-137">assignedTo</span></span>        | <span data-ttu-id="6786e-138">String</span><span class="sxs-lookup"><span data-stu-id="6786e-138">String</span></span>                                                                 | <span data-ttu-id="6786e-139">为会审、调查或修正分配了警报的分析师的名称。</span><span class="sxs-lookup"><span data-stu-id="6786e-139">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span> |
| <span data-ttu-id="6786e-140">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="6786e-140">closedDateTime</span></span>    | <span data-ttu-id="6786e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6786e-141">DateTimeOffset</span></span>                                                         | <span data-ttu-id="6786e-142">警报关闭的时间。</span><span class="sxs-lookup"><span data-stu-id="6786e-142">Time at which the alert was closed.</span></span> <span data-ttu-id="6786e-143">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="6786e-143">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6786e-144">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="6786e-144">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
| <span data-ttu-id="6786e-145">comments</span><span class="sxs-lookup"><span data-stu-id="6786e-145">comments</span></span>          | <span data-ttu-id="6786e-146">String collection</span><span class="sxs-lookup"><span data-stu-id="6786e-146">String collection</span></span>                                                      | <span data-ttu-id="6786e-147">通知的分析师注释 (针对客户通知管理)。</span><span class="sxs-lookup"><span data-stu-id="6786e-147">Analyst comments on the alert (for customer alert management).</span></span> |
| <span data-ttu-id="6786e-148">征求</span><span class="sxs-lookup"><span data-stu-id="6786e-148">feedback</span></span>          | <span data-ttu-id="6786e-149">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="6786e-149">alertFeedback</span></span>                                                          | <span data-ttu-id="6786e-150">通知的分析师反馈。</span><span class="sxs-lookup"><span data-stu-id="6786e-150">Analyst feedback on the alert.</span></span> <span data-ttu-id="6786e-151">可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。</span><span class="sxs-lookup"><span data-stu-id="6786e-151">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span> |
| <span data-ttu-id="6786e-152">状态</span><span class="sxs-lookup"><span data-stu-id="6786e-152">status</span></span>            | <span data-ttu-id="6786e-153">alertStatus</span><span class="sxs-lookup"><span data-stu-id="6786e-153">alertStatus</span></span>                                                            | <span data-ttu-id="6786e-154">警报生命周期状态 (阶段)。</span><span class="sxs-lookup"><span data-stu-id="6786e-154">Alert life cycle status (stage).</span></span> <span data-ttu-id="6786e-155">可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。</span><span class="sxs-lookup"><span data-stu-id="6786e-155">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span> |
| <span data-ttu-id="6786e-156">tags</span><span class="sxs-lookup"><span data-stu-id="6786e-156">tags</span></span>              | <span data-ttu-id="6786e-157">String 集合</span><span class="sxs-lookup"><span data-stu-id="6786e-157">String collection</span></span>                                                      | <span data-ttu-id="6786e-158">可应用于警报并可用作筛选条件的用户定义的标签 (例如, "HVA"、"锯")。</span><span class="sxs-lookup"><span data-stu-id="6786e-158">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span> |
| <span data-ttu-id="6786e-159">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="6786e-159">vendorInformation</span></span> | [<span data-ttu-id="6786e-160">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="6786e-160">securityVendorInformation</span></span>](../resources/securityvendorinformation.md) | <span data-ttu-id="6786e-161">包含有关安全产品/服务供应商、提供程序和 subprovider 的详细信息的复杂类型 (例如, 供应商 = Microsoft; provider = Windows Defender ATP; subprovider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="6786e-161">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="6786e-162">**提供程序和供应商字段是必需的。**</span><span class="sxs-lookup"><span data-stu-id="6786e-162">**Provider and vendor fields are required.**</span></span> |

## <a name="response"></a><span data-ttu-id="6786e-163">响应</span><span class="sxs-lookup"><span data-stu-id="6786e-163">Response</span></span>

<span data-ttu-id="6786e-164">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6786e-164">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="6786e-165">如果使用可选的请求标头, 则该方法将`200 OK`在响应正文中返回响应代码和更新的[alert](../resources/alert.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6786e-165">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6786e-166">示例</span><span class="sxs-lookup"><span data-stu-id="6786e-166">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="6786e-167">示例 1: 不带首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="6786e-167">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="6786e-168">请求</span><span class="sxs-lookup"><span data-stu-id="6786e-168">Request</span></span>

<span data-ttu-id="6786e-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6786e-169">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="6786e-170">响应</span><span class="sxs-lookup"><span data-stu-id="6786e-170">Response</span></span>

<span data-ttu-id="6786e-171">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="6786e-171">The following is an example of a successful response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="6786e-172">示例 2: 具有首选标头的请求</span><span class="sxs-lookup"><span data-stu-id="6786e-172">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="6786e-173">请求</span><span class="sxs-lookup"><span data-stu-id="6786e-173">Request</span></span>

<span data-ttu-id="6786e-174">下面的示例演示包含`Prefer`请求标头的请求。</span><span class="sxs-lookup"><span data-stu-id="6786e-174">The following example shows a request that includes the `Prefer` request header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_alert"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/security/alerts/{alert_id}
Content-type: application/json
Prefer: return=representation

{
  "assignedTo": "String",
  "closedDateTime": "String (timestamp)",
  "comments": [
    "String"
  ],
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "provider": "String",
    "vendor": "String"
  }
}
```

#### <a name="response"></a><span data-ttu-id="6786e-175">响应</span><span class="sxs-lookup"><span data-stu-id="6786e-175">Response</span></span>

<span data-ttu-id="6786e-176">以下是使用可选`Prefer: return=representation`请求标头时响应的示例。</span><span class="sxs-lookup"><span data-stu-id="6786e-176">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

> <span data-ttu-id="6786e-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6786e-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update alert",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
