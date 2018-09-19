# <a name="update-alert"></a><span data-ttu-id="805f6-101">更新通知</span><span class="sxs-lookup"><span data-stu-id="805f6-101">Update alert</span></span>

<span data-ttu-id="805f6-102">更新任何集成的解决方案内的可编辑\*\* 通知\*\*属性，使通知状态和分配在解决方案之间保持同步。</span><span class="sxs-lookup"><span data-stu-id="805f6-102">Update an editable **alert** property within any integrated solution to keep alert status and assignments in sync across solutions.</span></span> <span data-ttu-id="805f6-103">此方法将更新具有引用的通知 ID 记录的任何解决方案。</span><span class="sxs-lookup"><span data-stu-id="805f6-103">This method updates any solution that has a record of the referenced alert ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="805f6-104">权限</span><span class="sxs-lookup"><span data-stu-id="805f6-104">Permissions</span></span>

<span data-ttu-id="805f6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="805f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="805f6-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="805f6-107">Permission type</span></span>      | <span data-ttu-id="805f6-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="805f6-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="805f6-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="805f6-109">Delegated (work or school account)</span></span> |   <span data-ttu-id="805f6-110">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="805f6-110">SecurityEvents.ReadWrite.All</span></span>  |
|<span data-ttu-id="805f6-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="805f6-111">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="805f6-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="805f6-112">Not supported.</span></span>  |
|<span data-ttu-id="805f6-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="805f6-113">Application</span></span> | <span data-ttu-id="805f6-114">SecurityEvents.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="805f6-114">SecurityEvents.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="805f6-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="805f6-115">HTTP request</span></span>

> <span data-ttu-id="805f6-116">**注意：** 你必须随此方法一起包括**通知** ID 作为参数，并包括其中包含 `provider` 和 `vendor` 的 vendorInformation。</span><span class="sxs-lookup"><span data-stu-id="805f6-116">**Note:** You must include the **alert** ID as a parameter and vendorInformation containing the `provider` and `vendor` with this method.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PATCH /security/alerts/{alert_id}
```

## <a name="request-headers"></a><span data-ttu-id="805f6-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="805f6-117">Request headers</span></span>

| <span data-ttu-id="805f6-118">名称</span><span class="sxs-lookup"><span data-stu-id="805f6-118">Name</span></span>       | <span data-ttu-id="805f6-119">说明</span><span class="sxs-lookup"><span data-stu-id="805f6-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="805f6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="805f6-120">Authorization</span></span>  | <span data-ttu-id="805f6-p103">Bearer {code}。必需。</span><span class="sxs-lookup"><span data-stu-id="805f6-p103">Bearer {code}. Required.</span></span>|
|<span data-ttu-id="805f6-123">Prefer</span><span class="sxs-lookup"><span data-stu-id="805f6-123">Prefer</span></span> | <span data-ttu-id="805f6-124">return=representation</span><span class="sxs-lookup"><span data-stu-id="805f6-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="805f6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="805f6-125">Request body</span></span>

<span data-ttu-id="805f6-126">在请求正文中，提供应更新的相关字段值的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="805f6-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="805f6-127">正文**必须**包含 `vendorInformation` 属性及有效的`provider` 和 `vendor` 字段。</span><span class="sxs-lookup"><span data-stu-id="805f6-127">The body **must** contain the `vendorInformation` property with valid `provider` and `vendor` fields.</span></span> <span data-ttu-id="805f6-128">下表列出了可为通知更新的字段。</span><span class="sxs-lookup"><span data-stu-id="805f6-128">The following table lists the authentication settings that can be changed for an authentication provider.</span></span> <span data-ttu-id="805f6-129">未包括在请求正文中的现有属性的值不会更改。</span><span class="sxs-lookup"><span data-stu-id="805f6-129">The values for existing properties that are not included in the request body will not change.</span></span> <span data-ttu-id="805f6-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="805f6-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="805f6-131">属性</span><span class="sxs-lookup"><span data-stu-id="805f6-131">Property</span></span>   | <span data-ttu-id="805f6-132">类型</span><span class="sxs-lookup"><span data-stu-id="805f6-132">Type</span></span> |<span data-ttu-id="805f6-133">说明</span><span class="sxs-lookup"><span data-stu-id="805f6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="805f6-134">assignedTo</span><span class="sxs-lookup"><span data-stu-id="805f6-134">assignedTo</span></span>|<span data-ttu-id="805f6-135">字符串</span><span class="sxs-lookup"><span data-stu-id="805f6-135">String</span></span>|<span data-ttu-id="805f6-136">将通知分配给其进行会审、调查或修复的分析师的姓名。</span><span class="sxs-lookup"><span data-stu-id="805f6-136">Name of the analyst the alert is assigned to for triage, investigation, or remediation.</span></span>|
|<span data-ttu-id="805f6-137">closedDateTime</span><span class="sxs-lookup"><span data-stu-id="805f6-137">closedDateTime</span></span>|<span data-ttu-id="805f6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="805f6-138">DateTimeOffset</span></span>|<span data-ttu-id="805f6-139">通知关闭的时间。</span><span class="sxs-lookup"><span data-stu-id="805f6-139">Time at which the alert was closed.</span></span> <span data-ttu-id="805f6-140">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="805f6-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="805f6-141">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="805f6-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="805f6-142">comments</span><span class="sxs-lookup"><span data-stu-id="805f6-142">comments</span></span>|<span data-ttu-id="805f6-143">字符串集合</span><span class="sxs-lookup"><span data-stu-id="805f6-143">String collection</span></span>|<span data-ttu-id="805f6-144">分析师对通知的评论（用于客户通知管理）。</span><span class="sxs-lookup"><span data-stu-id="805f6-144">Analyst comments on the alert (for customer alert management).</span></span>|
|<span data-ttu-id="805f6-145">反馈</span><span class="sxs-lookup"><span data-stu-id="805f6-145">Feedback</span></span>|<span data-ttu-id="805f6-146">alertFeedback</span><span class="sxs-lookup"><span data-stu-id="805f6-146">alertFeedback</span></span>|<span data-ttu-id="805f6-147">分析师对通知的反馈。</span><span class="sxs-lookup"><span data-stu-id="805f6-147">Analyst feedback on the alert.</span></span> <span data-ttu-id="805f6-148">可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。</span><span class="sxs-lookup"><span data-stu-id="805f6-148">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="805f6-149">status</span><span class="sxs-lookup"><span data-stu-id="805f6-149">status</span></span>|<span data-ttu-id="805f6-150">alertStatus</span><span class="sxs-lookup"><span data-stu-id="805f6-150">alertStatus</span></span>|<span data-ttu-id="805f6-151">通知生命周期状态（阶段）。</span><span class="sxs-lookup"><span data-stu-id="805f6-151">Alert lifecycle status (stage).</span></span> <span data-ttu-id="805f6-152">可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`。</span><span class="sxs-lookup"><span data-stu-id="805f6-152">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`.</span></span>|
|<span data-ttu-id="805f6-153">tags</span><span class="sxs-lookup"><span data-stu-id="805f6-153">tags</span></span>|<span data-ttu-id="805f6-154">字符串集合</span><span class="sxs-lookup"><span data-stu-id="805f6-154">String collection</span></span>|<span data-ttu-id="805f6-155">可应用于通知并可充当筛选条件的用户可定义标签（例如，“HVA”、“SAW”）</span><span class="sxs-lookup"><span data-stu-id="805f6-155">User-definable labels that can be applied to an alert and can serve as filter conditions (for example, "HVA", "SAW).</span></span>|
|<span data-ttu-id="805f6-156">vendorInformation \*</span><span class="sxs-lookup"><span data-stu-id="805f6-156">vendorInformation \*</span></span>|[<span data-ttu-id="805f6-157">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="805f6-157">securityVendorInformation</span></span>](../resources/securityvendorinformation.md)|<span data-ttu-id="805f6-158">包含安全产品/服务提供商、供应商和次级供应商相关详细信息的复杂类型（例如，vendor=Microsoft；provider=Windows Defender ATP；subProvider=AppLocker）。</span><span class="sxs-lookup"><span data-stu-id="805f6-158">Complex type containing details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span> <span data-ttu-id="805f6-159">**供应商和提供商字段为必填。**</span><span class="sxs-lookup"><span data-stu-id="805f6-159">**Provider and vendor fields are required.**</span></span>|
<span data-ttu-id="805f6-160">（\* 表示必填字段。）</span><span class="sxs-lookup"><span data-stu-id="805f6-160">(\* Indicates a mandatory field.)</span></span>

## <a name="response"></a><span data-ttu-id="805f6-161">响应</span><span class="sxs-lookup"><span data-stu-id="805f6-161">Response</span></span>

<span data-ttu-id="805f6-162">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="805f6-162">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="805f6-163">如果使用可选请求标头，则该方法返回 `200 OK` 响应代码和响应正文中的更新的[通知](../resources/alert.md)对象。</span><span class="sxs-lookup"><span data-stu-id="805f6-163">If the optional request header is used, the method returns a `200 OK` response code and the updated [alert](../resources/alert.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="805f6-164">示例 1</span><span class="sxs-lookup"><span data-stu-id="805f6-164">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="805f6-165">请求</span><span class="sxs-lookup"><span data-stu-id="805f6-165">Request</span></span>

<span data-ttu-id="805f6-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="805f6-166">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="805f6-167">响应</span><span class="sxs-lookup"><span data-stu-id="805f6-167">Response</span></span>

<span data-ttu-id="805f6-168">下面展示了一个成功的响应示例。</span><span class="sxs-lookup"><span data-stu-id="805f6-168">The following is an example of a response to a  event.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.alert"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="example-2"></a><span data-ttu-id="805f6-169">示例 2</span><span class="sxs-lookup"><span data-stu-id="805f6-169">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="805f6-170">请求</span><span class="sxs-lookup"><span data-stu-id="805f6-170">Request</span></span>

<span data-ttu-id="805f6-171">下面的示例展示一个包括 `Prefer` 请求标头的请求。</span><span class="sxs-lookup"><span data-stu-id="805f6-171">The following example shows a request that includes the `Prefer` request header.</span></span>

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

### <a name="response"></a><span data-ttu-id="805f6-172">响应</span><span class="sxs-lookup"><span data-stu-id="805f6-172">Response</span></span>

<span data-ttu-id="805f6-173">下面展示了使用可选 `Prefer: return=representation` 请求标头时的请求示例。</span><span class="sxs-lookup"><span data-stu-id="805f6-173">The following is an example of the response when the optional `Prefer: return=representation` request header is used.</span></span>

><span data-ttu-id="805f6-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="805f6-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
