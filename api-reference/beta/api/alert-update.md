---
title: 更新警报
description: 更新在任何集成的解决方案，以使警报状态和分配保持同步跨解决方案可编辑的警报属性。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: fc0bc88dad83024d3da2d6f2adf3f16288719cb2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517412"
---
# <a name="update-alert"></a><span data-ttu-id="8a5e2-103">更新警报</span><span class="sxs-lookup"><span data-stu-id="8a5e2-103">Update alert</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a5e2-104">更新在任何集成的解决方案，以使警报状态和分配保持同步跨解决方案的可编辑**通知**属性。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-104">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="8a5e2-105">此方法将更新的任何解决方案都有一个记录引用的警报 id。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-105">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a5e2-106">权限</span><span class="sxs-lookup"><span data-stu-id="8a5e2-106">Permissions</span></span>

<span data-ttu-id="8a5e2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a5e2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a5e2-109">Permission type</span></span>      | <span data-ttu-id="8a5e2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a5e2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a5e2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a5e2-111">Delegated (work or school account)</span></span> |   <span data-ttu-id="8a5e2-112">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a5e2-112">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="8a5e2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a5e2-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8a5e2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-114">Not supported.</span></span>  |
|<span data-ttu-id="8a5e2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a5e2-115">Application</span></span> | <span data-ttu-id="8a5e2-116">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a5e2-116">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a5e2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a5e2-117">HTTP request</span></span>

> <span data-ttu-id="8a5e2-118">**注意：** 您必须为参数和 vendorInformation 包含包括的**警报**ID`provider`和`vendor`使用此方法。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-118">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="8a5e2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8a5e2-119">Request headers</span></span>

| <span data-ttu-id="8a5e2-120">名称</span><span class="sxs-lookup"><span data-stu-id="8a5e2-120">Name</span></span>       | <span data-ttu-id="8a5e2-121">说明</span><span class="sxs-lookup"><span data-stu-id="8a5e2-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8a5e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a5e2-122">Authorization</span></span>  | <span data-ttu-id="8a5e2-p103">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-p103">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="8a5e2-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="8a5e2-125">Prefer</span></span> | <span data-ttu-id="8a5e2-126">返回 = 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a5e2-126">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="8a5e2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a5e2-127">Request body</span></span>

<span data-ttu-id="8a5e2-128">在请求正文中，提供应更新的相关字段的值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-128">In the request body, supply a JSON representation of the values for relevant fields that should be updated.</span></span> <span data-ttu-id="8a5e2-129">**必须**正文包含`vendorInformation`属性与有效`provider`和`vendor`字段。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-129">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="8a5e2-130">下表列出了可更新的通知的字段。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-130">The following table lists the fields that can be updated for an alert.</span></span> <span data-ttu-id="8a5e2-131">不包含在请求正文中的现有属性的值不会更改。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-131">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="8a5e2-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8a5e2-133">属性</span><span class="sxs-lookup"><span data-stu-id="8a5e2-133">Property</span></span>   | <span data-ttu-id="8a5e2-134">类型</span><span class="sxs-lookup"><span data-stu-id="8a5e2-134">Type</span></span> |<span data-ttu-id="8a5e2-135">说明</span><span class="sxs-lookup"><span data-stu-id="8a5e2-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a5e2-136">AssignedTo</span><span class="sxs-lookup"><span data-stu-id="8a5e2-136">assignedTo</span></span>|<span data-ttu-id="8a5e2-137">String</span><span class="sxs-lookup"><span data-stu-id="8a5e2-137">String</span></span>|<span data-ttu-id="8a5e2-138">分析师通知的名称分配给进行会审、 调查或修复。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-138">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="8a5e2-139">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a5e2-139">closedDateTime</span></span>|<span data-ttu-id="8a5e2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a5e2-140">DateTimeOffset</span></span>|<span data-ttu-id="8a5e2-141">通知关闭的时间。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-141">Time at which the alert was closed.</span></span> <span data-ttu-id="8a5e2-142">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8a5e2-143">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="8a5e2-144">comments</span><span class="sxs-lookup"><span data-stu-id="8a5e2-144">comments</span></span>|<span data-ttu-id="8a5e2-145">String 集合</span><span class="sxs-lookup"><span data-stu-id="8a5e2-145">String collection</span></span>|<span data-ttu-id="8a5e2-146">分析师评论的警报 （客户警报管理）。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-146">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="8a5e2-147">反馈</span><span class="sxs-lookup"><span data-stu-id="8a5e2-147">feedback</span></span>|<span data-ttu-id="8a5e2-148">alertFeedback 枚举</span><span class="sxs-lookup"><span data-stu-id="8a5e2-148">alertFeedback enum</span></span>|<span data-ttu-id="8a5e2-149">分析师通知上的反馈。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-149">Analyst feedback on the alert.</span></span> <span data-ttu-id="8a5e2-150">可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-150">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="8a5e2-151">status</span><span class="sxs-lookup"><span data-stu-id="8a5e2-151">status</span></span>|<span data-ttu-id="8a5e2-152">alertStatus 枚举</span><span class="sxs-lookup"><span data-stu-id="8a5e2-152">alertStatus enum</span></span>|<span data-ttu-id="8a5e2-153">警报生命周期状态 （阶段）。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-153">Alert lifecycle status (stage).</span></span> <span data-ttu-id="8a5e2-154">可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-154">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="8a5e2-155">标记</span><span class="sxs-lookup"><span data-stu-id="8a5e2-155">tags</span></span>|<span data-ttu-id="8a5e2-156">String 集合</span><span class="sxs-lookup"><span data-stu-id="8a5e2-156">String collection</span></span>|<span data-ttu-id="8a5e2-157">可以应用于通知和可以充当筛选条件 (例如，"HVA"，"看到) 的用户可定义标签。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-157">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="8a5e2-158">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="8a5e2-158">vendorInformation</span></span> |[<span data-ttu-id="8a5e2-159">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="8a5e2-159">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="8a5e2-160">包含有关安全产品/服务供应商、 提供商和 subprovider 的详细信息的复杂类型 (例如，供应商 = Microsoft; 提供程序 = Windows Defender ATP; subProvider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-160">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="8a5e2-161">**提供程序和供应商字段是必需的。**</span><span class="sxs-lookup"><span data-stu-id="8a5e2-161">**Provider and vendor fields are required.**</span></span>|

## <a name="response"></a><span data-ttu-id="8a5e2-162">响应</span><span class="sxs-lookup"><span data-stu-id="8a5e2-162">Response</span></span>

<span data-ttu-id="8a5e2-163">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-163">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="8a5e2-164">如果使用可选请求标头，则该方法返回`200 OK`响应代码和响应正文中的更新的[通知](../resources/alert.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-164">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="8a5e2-165">示例 1</span><span class="sxs-lookup"><span data-stu-id="8a5e2-165">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="8a5e2-166">请求</span><span class="sxs-lookup"><span data-stu-id="8a5e2-166">Request</span></span>

<span data-ttu-id="8a5e2-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-167">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8a5e2-168">响应</span><span class="sxs-lookup"><span data-stu-id="8a5e2-168">Response</span></span>

<span data-ttu-id="8a5e2-169">下面是成功响应的示例。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-169">The following is an example of a successful response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="8a5e2-170">示例 2</span><span class="sxs-lookup"><span data-stu-id="8a5e2-170">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="8a5e2-171">请求</span><span class="sxs-lookup"><span data-stu-id="8a5e2-171">Request</span></span>

<span data-ttu-id="8a5e2-172">下面的示例演示包含的请求，`Prefer`请求标头。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-172">The following example shows a request that includes the `Prefer` request header.</span></span>

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

### <a name="response"></a><span data-ttu-id="8a5e2-173">响应</span><span class="sxs-lookup"><span data-stu-id="8a5e2-173">Response</span></span>

<span data-ttu-id="8a5e2-174">下面是响应的示例时可选`Prefer: return=representation`使用请求标头。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-174">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="8a5e2-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8a5e2-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
