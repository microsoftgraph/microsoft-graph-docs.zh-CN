# <a name="update-organization"></a><span data-ttu-id="ea3cb-101">更新组织</span><span class="sxs-lookup"><span data-stu-id="ea3cb-101">Update organization</span></span>

<span data-ttu-id="ea3cb-102">更新当前经过身份验证的组织的属性。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-102">Update the properties of the currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea3cb-103">权限</span><span class="sxs-lookup"><span data-stu-id="ea3cb-103">Permissions</span></span>

<span data-ttu-id="ea3cb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ea3cb-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea3cb-106">Permission type</span></span>      | <span data-ttu-id="ea3cb-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea3cb-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea3cb-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea3cb-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ea3cb-109">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-109">Not supported.</span></span>    |
|<span data-ttu-id="ea3cb-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea3cb-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea3cb-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-111">Not supported.</span></span>    |
|<span data-ttu-id="ea3cb-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea3cb-112">Application</span></span> | <span data-ttu-id="ea3cb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea3cb-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea3cb-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a><span data-ttu-id="ea3cb-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea3cb-115">Request headers</span></span>

| <span data-ttu-id="ea3cb-116">名称</span><span class="sxs-lookup"><span data-stu-id="ea3cb-116">Name</span></span>       | <span data-ttu-id="ea3cb-117">类型</span><span class="sxs-lookup"><span data-stu-id="ea3cb-117">Type</span></span> | <span data-ttu-id="ea3cb-118">说明</span><span class="sxs-lookup"><span data-stu-id="ea3cb-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ea3cb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea3cb-119">Authorization</span></span>  | <span data-ttu-id="ea3cb-120">string</span><span class="sxs-lookup"><span data-stu-id="ea3cb-120">string</span></span>  | <span data-ttu-id="ea3cb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea3cb-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea3cb-123">Request body</span></span>
<span data-ttu-id="ea3cb-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="ea3cb-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="ea3cb-126">为了实现最佳性能，不得添加尚未变化的现有值。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-126">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ea3cb-127">属性</span><span class="sxs-lookup"><span data-stu-id="ea3cb-127">Property</span></span>     | <span data-ttu-id="ea3cb-128">类型</span><span class="sxs-lookup"><span data-stu-id="ea3cb-128">Type</span></span>   |<span data-ttu-id="ea3cb-129">说明</span><span class="sxs-lookup"><span data-stu-id="ea3cb-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea3cb-130">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="ea3cb-130">assignedPlans</span></span>|<span data-ttu-id="ea3cb-131">AssignedPlan</span><span class="sxs-lookup"><span data-stu-id="ea3cb-131">AssignedPlan</span></span>|<span data-ttu-id="ea3cb-132">与租户相关的服务计划的集合。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-132">The collection of service plans associated with the tenant. Not nullable.</span></span> <span data-ttu-id="ea3cb-133">**注意：**不可为 null。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-133">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="ea3cb-134">city</span><span class="sxs-lookup"><span data-stu-id="ea3cb-134">city</span></span>|<span data-ttu-id="ea3cb-135">String</span><span class="sxs-lookup"><span data-stu-id="ea3cb-135">String</span></span>|            |
|<span data-ttu-id="ea3cb-136">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="ea3cb-136">companyLastDirSyncTime</span></span>|<span data-ttu-id="ea3cb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea3cb-137">DateTimeOffset</span></span>|<span data-ttu-id="ea3cb-138">租户上次与本地目录同步的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-138">The time and date at which the tenant was last synced with the on-premise directory.</span></span>|
|<span data-ttu-id="ea3cb-139">country</span><span class="sxs-lookup"><span data-stu-id="ea3cb-139">country</span></span>|<span data-ttu-id="ea3cb-140">String</span><span class="sxs-lookup"><span data-stu-id="ea3cb-140">String</span></span>|            |
|<span data-ttu-id="ea3cb-141">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="ea3cb-141">countryLetterCode</span></span>|<span data-ttu-id="ea3cb-142">String</span><span class="sxs-lookup"><span data-stu-id="ea3cb-142">String</span></span>|            |
|<span data-ttu-id="ea3cb-143">deletionTimestamp</span><span class="sxs-lookup"><span data-stu-id="ea3cb-143">deletionTimestamp</span></span>|<span data-ttu-id="ea3cb-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea3cb-144">DateTimeOffset</span></span>||
|<span data-ttu-id="ea3cb-145">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="ea3cb-145">dirSyncEnabled</span></span>|<span data-ttu-id="ea3cb-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea3cb-146">Boolean</span></span>|<span data-ttu-id="ea3cb-147">如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-147">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="ea3cb-148">displayName</span><span class="sxs-lookup"><span data-stu-id="ea3cb-148">displayName</span></span>|<span data-ttu-id="ea3cb-149">String</span><span class="sxs-lookup"><span data-stu-id="ea3cb-149">String</span></span>|<span data-ttu-id="ea3cb-150">租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-150">The display name for the tenant.</span></span>|
|<span data-ttu-id="ea3cb-151">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="ea3cb-151">marketingNotificationEmails</span></span>|<span data-ttu-id="ea3cb-152">String</span><span class="sxs-lookup"><span data-stu-id="ea3cb-152">String</span></span>|                                        <span data-ttu-id="ea3cb-153">**注意：**不可为 null。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-153">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="ea3cb-154">objectType</span><span class="sxs-lookup"><span data-stu-id="ea3cb-154">objectType</span></span>|<span data-ttu-id="ea3cb-155">String</span><span class="sxs-lookup"><span data-stu-id="ea3cb-155">String</span></span>|<span data-ttu-id="ea3cb-156">标识对象类型的字符串。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-156">A string that identifies the object type. For tenants the value is always “Company”.</span></span> <span data-ttu-id="ea3cb-157">对于租户，值始终为“Company”。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-157">A string that identifies the object type. For tenants the value is always “Company”.</span></span> <span data-ttu-id="ea3cb-158">继承自 [directoryObject](../resources/directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-158">Inherited from [directoryObject](../resources/directoryobject.md).</span></span>|
|<span data-ttu-id="ea3cb-159">postalCode</span><span class="sxs-lookup"><span data-stu-id="ea3cb-159">postalCode</span></span>|<span data-ttu-id="ea3cb-160">String</span><span class="sxs-lookup"><span data-stu-id="ea3cb-160">String</span></span>|            |
|<span data-ttu-id="ea3cb-161">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="ea3cb-161">preferredLanguage</span></span>|<span data-ttu-id="ea3cb-162">String</span><span class="sxs-lookup"><span data-stu-id="ea3cb-162">String</span></span>|            |
|<span data-ttu-id="ea3cb-163">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="ea3cb-163">provisionedPlans</span></span>|<span data-ttu-id="ea3cb-164">ProvisionedPlan</span><span class="sxs-lookup"><span data-stu-id="ea3cb-164">ProvisionedPlan</span></span>|                                        <span data-ttu-id="ea3cb-165">**注意：**不可为 null。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-165">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="ea3cb-166">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="ea3cb-166">provisioningErrors</span></span>|<span data-ttu-id="ea3cb-167">ProvisioningError</span><span class="sxs-lookup"><span data-stu-id="ea3cb-167">ProvisioningError</span></span>|                                        <span data-ttu-id="ea3cb-168">**注意：**不可为 null。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-168">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="ea3cb-169">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="ea3cb-169">securityComplianceNotificationMails</span></span>|<span data-ttu-id="ea3cb-170">String</span><span class="sxs-lookup"><span data-stu-id="ea3cb-170">String</span></span>||
|<span data-ttu-id="ea3cb-171">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="ea3cb-171">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="ea3cb-172">String</span><span class="sxs-lookup"><span data-stu-id="ea3cb-172">String</span></span>||
|<span data-ttu-id="ea3cb-173">state</span><span class="sxs-lookup"><span data-stu-id="ea3cb-173">state</span></span>|<span data-ttu-id="ea3cb-174">String</span><span class="sxs-lookup"><span data-stu-id="ea3cb-174">String</span></span>|            |
|<span data-ttu-id="ea3cb-175">street</span><span class="sxs-lookup"><span data-stu-id="ea3cb-175">street</span></span>|<span data-ttu-id="ea3cb-176">String</span><span class="sxs-lookup"><span data-stu-id="ea3cb-176">String</span></span>|            |
|<span data-ttu-id="ea3cb-177">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="ea3cb-177">technicalNotificationMails</span></span>|<span data-ttu-id="ea3cb-178">String</span><span class="sxs-lookup"><span data-stu-id="ea3cb-178">String</span></span>|                                        <span data-ttu-id="ea3cb-179">**注意：**不可为 null。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-179">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="ea3cb-180">telephoneNumber</span><span class="sxs-lookup"><span data-stu-id="ea3cb-180">telephoneNumber</span></span>|<span data-ttu-id="ea3cb-181">String</span><span class="sxs-lookup"><span data-stu-id="ea3cb-181">String</span></span>|            |
|<span data-ttu-id="ea3cb-182">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="ea3cb-182">verifiedDomains</span></span>|<span data-ttu-id="ea3cb-183">VerifiedDomain</span><span class="sxs-lookup"><span data-stu-id="ea3cb-183">VerifiedDomain</span></span>|<span data-ttu-id="ea3cb-184">与该租户相关联的域集合。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-184">The collection of domains associated with this tenant. Not nullable.</span></span> <span data-ttu-id="ea3cb-185">**注意：**不可为 null。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-185">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="ea3cb-186">响应</span><span class="sxs-lookup"><span data-stu-id="ea3cb-186">Response</span></span>

<span data-ttu-id="ea3cb-187">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/organization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-187">If successful, this method returns a `200 OK` response code and updated [organization](../resources/organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea3cb-188">示例</span><span class="sxs-lookup"><span data-stu-id="ea3cb-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="ea3cb-189">请求</span><span class="sxs-lookup"><span data-stu-id="ea3cb-189">Request</span></span>

<span data-ttu-id="ea3cb-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-190">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```

<br/>

### <a name="response"></a><span data-ttu-id="ea3cb-191">响应</span><span class="sxs-lookup"><span data-stu-id="ea3cb-191">Response</span></span>

<span data-ttu-id="ea3cb-192">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-192">Here is an example of the response.</span></span> <span data-ttu-id="ea3cb-193">**注意**：为简洁起见，可能会截断此处展示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-193">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ea3cb-194">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea3cb-194">All default properties will be returned from the actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 411

{
  "assignedPlans": [
    {
      "assignedDateTime": "datetime-value",
      "capabilityStatus": "capabilityStatus-value",
      "service": "service-value",
      "servicePlanId": "servicePlanId-value"
    }
  ],
  "businessPhones": [
    "businessPhones-value"
  ],
  "city": "city-value",
  "country": "country-value",
  "countryLetterCode": "countryLetterCode-value",
  "displayName": "displayName-value"
}
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
