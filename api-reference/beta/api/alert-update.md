---
title: 更新警报
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8b8e21334d9a94d6a41c1e283959bd6473c11e1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990616"
---
# <a name="update-alert"></a><span data-ttu-id="1c336-104">更新警报</span><span class="sxs-lookup"><span data-stu-id="1c336-104">Update alert</span></span>

 > <span data-ttu-id="1c336-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1c336-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c336-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1c336-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1c336-107">更新在任何集成的解决方案，以使警报状态和分配保持同步跨解决方案的可编辑**通知**属性。</span><span class="sxs-lookup"><span data-stu-id="1c336-107">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="1c336-108">此方法将更新的任何解决方案都有一个记录引用的警报 id。</span><span class="sxs-lookup"><span data-stu-id="1c336-108">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c336-109">权限</span><span class="sxs-lookup"><span data-stu-id="1c336-109">Permissions</span></span>

<span data-ttu-id="1c336-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c336-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c336-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c336-112">Permission type</span></span>      | <span data-ttu-id="1c336-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c336-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c336-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c336-114">Delegated (work or school account)</span></span> |   <span data-ttu-id="1c336-115">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c336-115">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="1c336-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c336-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1c336-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c336-117">Not supported.</span></span>  |
|<span data-ttu-id="1c336-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c336-118">Application</span></span> | <span data-ttu-id="1c336-119">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c336-119">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c336-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c336-120">HTTP request</span></span>

> <span data-ttu-id="1c336-121">**注意：** 您必须为参数和 vendorInformation 包含包括的**警报**ID`provider`和`vendor`使用此方法。</span><span class="sxs-lookup"><span data-stu-id="1c336-121">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="1c336-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c336-122">Request headers</span></span>

| <span data-ttu-id="1c336-123">名称</span><span class="sxs-lookup"><span data-stu-id="1c336-123">Name</span></span>       | <span data-ttu-id="1c336-124">说明</span><span class="sxs-lookup"><span data-stu-id="1c336-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1c336-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c336-125">Authorization</span></span>  | <span data-ttu-id="1c336-p105">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c336-p105">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="1c336-128">Prefer</span><span class="sxs-lookup"><span data-stu-id="1c336-128">Prefer</span></span> | <span data-ttu-id="1c336-129">返回 = 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c336-129">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c336-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c336-130">Request body</span></span>

<span data-ttu-id="1c336-131">在请求正文中，提供应更新的相关字段的值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c336-131">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1c336-132">**必须**正文包含`vendorInformation`属性与有效`provider`和`vendor`字段。</span><span class="sxs-lookup"><span data-stu-id="1c336-132">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="1c336-133">下表列出了可更新的通知的字段。</span><span class="sxs-lookup"><span data-stu-id="1c336-133">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="1c336-134">不包含在请求正文中的现有属性的值不会更改。</span><span class="sxs-lookup"><span data-stu-id="1c336-134">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="1c336-135">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1c336-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1c336-136">属性</span><span class="sxs-lookup"><span data-stu-id="1c336-136">Property</span></span>   | <span data-ttu-id="1c336-137">类型</span><span class="sxs-lookup"><span data-stu-id="1c336-137">Type</span></span> |<span data-ttu-id="1c336-138">说明</span><span class="sxs-lookup"><span data-stu-id="1c336-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c336-139">assignedTo</span><span class="sxs-lookup"><span data-stu-id="1c336-139">assignedTo</span></span>|<span data-ttu-id="1c336-140">字符串</span><span class="sxs-lookup"><span data-stu-id="1c336-140">String</span></span>|<span data-ttu-id="1c336-141">分析师通知的名称分配给进行会审、 调查或修复。</span><span class="sxs-lookup"><span data-stu-id="1c336-141">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="1c336-142">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c336-142">closedDateTime</span></span>|<span data-ttu-id="1c336-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c336-143">DateTimeOffset</span></span>|<span data-ttu-id="1c336-144">通知关闭的时间。</span><span class="sxs-lookup"><span data-stu-id="1c336-144">Time at which the alert was closed.</span></span> <span data-ttu-id="1c336-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1c336-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1c336-146">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="1c336-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="1c336-147">comments</span><span class="sxs-lookup"><span data-stu-id="1c336-147">comments</span></span>|<span data-ttu-id="1c336-148">String 集合</span><span class="sxs-lookup"><span data-stu-id="1c336-148">String collection</span></span>|<span data-ttu-id="1c336-149">分析师评论的警报 （客户警报管理）。</span><span class="sxs-lookup"><span data-stu-id="1c336-149">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="1c336-150">反馈</span><span class="sxs-lookup"><span data-stu-id="1c336-150">feedback</span></span>|<span data-ttu-id="1c336-151">alertFeedback 枚举</span><span class="sxs-lookup"><span data-stu-id="1c336-151">alertFeedback enum</span></span>|<span data-ttu-id="1c336-152">分析师通知上的反馈。</span><span class="sxs-lookup"><span data-stu-id="1c336-152">Analyst feedback on the alert.</span></span> <span data-ttu-id="1c336-153">可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。</span><span class="sxs-lookup"><span data-stu-id="1c336-153">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="1c336-154">status</span><span class="sxs-lookup"><span data-stu-id="1c336-154">status</span></span>|<span data-ttu-id="1c336-155">alertStatus 枚举</span><span class="sxs-lookup"><span data-stu-id="1c336-155">alertStatus enum</span></span>|<span data-ttu-id="1c336-156">警报生命周期状态 （阶段）。</span><span class="sxs-lookup"><span data-stu-id="1c336-156">Alert lifecycle status (stage).</span></span> <span data-ttu-id="1c336-157">可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。</span><span class="sxs-lookup"><span data-stu-id="1c336-157">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="1c336-158">标记前添加的标记</span><span class="sxs-lookup"><span data-stu-id="1c336-158">tags</span></span>|<span data-ttu-id="1c336-159">String 集合</span><span class="sxs-lookup"><span data-stu-id="1c336-159">String collection</span></span>|<span data-ttu-id="1c336-160">可以应用于通知和可以充当筛选条件 (例如，"HVA"，"看到) 的用户可定义标签。</span><span class="sxs-lookup"><span data-stu-id="1c336-160">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="1c336-161">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="1c336-161">vendorInformation</span></span> |[<span data-ttu-id="1c336-162">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="1c336-162">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="1c336-163">包含有关安全产品/服务供应商、 提供商和 subprovider 的详细信息的复杂类型 (例如，供应商 = Microsoft; 提供程序 = Windows Defender ATP; subProvider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="1c336-163">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="1c336-164">**提供程序和供应商字段是必需的。**</span><span class="sxs-lookup"><span data-stu-id="1c336-164">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="1c336-165">响应</span><span class="sxs-lookup"><span data-stu-id="1c336-165">Response</span></span>

<span data-ttu-id="1c336-166">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1c336-166">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="1c336-167">如果使用可选请求标头，则该方法返回`200 OK`响应代码和响应正文中的更新的[通知](../resources/alert.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1c336-167">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="1c336-168">示例 1</span><span class="sxs-lookup"><span data-stu-id="1c336-168">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="1c336-169">请求</span><span class="sxs-lookup"><span data-stu-id="1c336-169">Request</span></span>

<span data-ttu-id="1c336-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1c336-170">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1c336-171">响应</span><span class="sxs-lookup"><span data-stu-id="1c336-171">Response</span></span>

<span data-ttu-id="1c336-172">以下是响应的成功的示例。</span><span class="sxs-lookup"><span data-stu-id="1c336-172">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="1c336-173">示例 2</span><span class="sxs-lookup"><span data-stu-id="1c336-173">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="1c336-174">请求</span><span class="sxs-lookup"><span data-stu-id="1c336-174">Request</span></span>

<span data-ttu-id="1c336-175">下面的示例演示包含的请求，`Prefer`请求标头。</span><span class="sxs-lookup"><span data-stu-id="1c336-175">The following example shows a request that includes the `Prefer` request header.</span></span>

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

### <a name="response"></a><span data-ttu-id="1c336-176">响应</span><span class="sxs-lookup"><span data-stu-id="1c336-176">Response</span></span>

<span data-ttu-id="1c336-177">下面是响应的示例时可选`Prefer: return=representation`使用请求标头。</span><span class="sxs-lookup"><span data-stu-id="1c336-177">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="1c336-p111">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1c336-p111">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
