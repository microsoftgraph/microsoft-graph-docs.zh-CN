# <a name="update-organization"></a><span data-ttu-id="1c562-101">更新组织</span><span class="sxs-lookup"><span data-stu-id="1c562-101">Update organization</span></span>

<span data-ttu-id="1c562-102">更新当前经过身份验证的组织的属性。</span><span class="sxs-lookup"><span data-stu-id="1c562-102">Update the properties of the currently authenticated organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c562-103">权限</span><span class="sxs-lookup"><span data-stu-id="1c562-103">Permissions</span></span>
<span data-ttu-id="1c562-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1c562-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1c562-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c562-106">Permission type</span></span>      | <span data-ttu-id="1c562-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c562-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c562-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c562-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1c562-109">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c562-109">Not supported.</span></span>    |
|<span data-ttu-id="1c562-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c562-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c562-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c562-111">Not supported.</span></span>    |
|<span data-ttu-id="1c562-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c562-112">Application</span></span> | <span data-ttu-id="1c562-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c562-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c562-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c562-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /organization

```
## <a name="request-headers"></a><span data-ttu-id="1c562-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c562-115">Request headers</span></span>
| <span data-ttu-id="1c562-116">名称</span><span class="sxs-lookup"><span data-stu-id="1c562-116">Name</span></span>       | <span data-ttu-id="1c562-117">类型</span><span class="sxs-lookup"><span data-stu-id="1c562-117">Type</span></span> | <span data-ttu-id="1c562-118">说明</span><span class="sxs-lookup"><span data-stu-id="1c562-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1c562-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c562-119">Authorization</span></span>  | <span data-ttu-id="1c562-120">string</span><span class="sxs-lookup"><span data-stu-id="1c562-120">string</span></span>  | <span data-ttu-id="1c562-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c562-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c562-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c562-123">Request body</span></span>
<span data-ttu-id="1c562-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="1c562-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1c562-127">属性</span><span class="sxs-lookup"><span data-stu-id="1c562-127">Property</span></span>     | <span data-ttu-id="1c562-128">类型</span><span class="sxs-lookup"><span data-stu-id="1c562-128">Type</span></span>   |<span data-ttu-id="1c562-129">说明</span><span class="sxs-lookup"><span data-stu-id="1c562-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c562-130">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="1c562-130">assignedPlans</span></span>|<span data-ttu-id="1c562-131">AssignedPlan</span><span class="sxs-lookup"><span data-stu-id="1c562-131">AssignedPlan</span></span>|<span data-ttu-id="1c562-p104">与租户相关的服务计划的集合。                          **注意：**不可为 null。</span><span class="sxs-lookup"><span data-stu-id="1c562-p104">The collection of service plans associated with the tenant.                            **Notes**: not nullable.</span></span>            |
|<span data-ttu-id="1c562-134">城市</span><span class="sxs-lookup"><span data-stu-id="1c562-134">city</span></span>|<span data-ttu-id="1c562-135">String</span><span class="sxs-lookup"><span data-stu-id="1c562-135">String</span></span>|            |
|<span data-ttu-id="1c562-136">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="1c562-136">companyLastDirSyncTime</span></span>|<span data-ttu-id="1c562-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c562-137">DateTimeOffset</span></span>|<span data-ttu-id="1c562-138">租户上次与本地目录同步的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="1c562-138">The time and date at which the tenant was last synced with the on-premise directory.</span></span>|
|<span data-ttu-id="1c562-139">country</span><span class="sxs-lookup"><span data-stu-id="1c562-139">country</span></span>|<span data-ttu-id="1c562-140">String</span><span class="sxs-lookup"><span data-stu-id="1c562-140">String</span></span>|            |
|<span data-ttu-id="1c562-141">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="1c562-141">countryLetterCode</span></span>|<span data-ttu-id="1c562-142">String</span><span class="sxs-lookup"><span data-stu-id="1c562-142">String</span></span>|            |
|<span data-ttu-id="1c562-143">deletionTimestamp</span><span class="sxs-lookup"><span data-stu-id="1c562-143">deletionTimestamp</span></span>|<span data-ttu-id="1c562-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c562-144">DateTimeOffset</span></span>||
|<span data-ttu-id="1c562-145">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="1c562-145">dirSyncEnabled</span></span>|<span data-ttu-id="1c562-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1c562-146">Boolean</span></span>|<span data-ttu-id="1c562-147">如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="1c562-147">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="1c562-148">displayName</span><span class="sxs-lookup"><span data-stu-id="1c562-148">displayName</span></span>|<span data-ttu-id="1c562-149">String</span><span class="sxs-lookup"><span data-stu-id="1c562-149">String</span></span>|<span data-ttu-id="1c562-150">租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1c562-150">The display name for the tenant.</span></span>|
|<span data-ttu-id="1c562-151">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="1c562-151">marketingNotificationEmails</span></span>|<span data-ttu-id="1c562-152">String</span><span class="sxs-lookup"><span data-stu-id="1c562-152">String</span></span>|                                        <span data-ttu-id="1c562-153">**注意：**不可为 null。</span><span class="sxs-lookup"><span data-stu-id="1c562-153">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="1c562-154">objectType</span><span class="sxs-lookup"><span data-stu-id="1c562-154">objectType</span></span>|<span data-ttu-id="1c562-155">String</span><span class="sxs-lookup"><span data-stu-id="1c562-155">String</span></span>|<span data-ttu-id="1c562-p105">一个标识对象类型的字符串。对于租户，该值始终为“公司”。继承自 [directoryObject](../resources/directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="1c562-p105">A string that identifies the object type. For tenants the value is always “Company”. Inherited from [directoryObject](../resources/directoryobject.md).</span></span>|
|<span data-ttu-id="1c562-159">postalCode</span><span class="sxs-lookup"><span data-stu-id="1c562-159">postalCode</span></span>|<span data-ttu-id="1c562-160">String</span><span class="sxs-lookup"><span data-stu-id="1c562-160">String</span></span>|            |
|<span data-ttu-id="1c562-161">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="1c562-161">preferredLanguage</span></span>|<span data-ttu-id="1c562-162">String</span><span class="sxs-lookup"><span data-stu-id="1c562-162">String</span></span>|            |
|<span data-ttu-id="1c562-163">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="1c562-163">provisionedPlans</span></span>|<span data-ttu-id="1c562-164">ProvisionedPlan</span><span class="sxs-lookup"><span data-stu-id="1c562-164">ProvisionedPlan</span></span>|                                        <span data-ttu-id="1c562-165">**注意：**不可为 null。</span><span class="sxs-lookup"><span data-stu-id="1c562-165">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="1c562-166">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="1c562-166">provisioningErrors</span></span>|<span data-ttu-id="1c562-167">ProvisioningError</span><span class="sxs-lookup"><span data-stu-id="1c562-167">ProvisioningError</span></span>|                                        <span data-ttu-id="1c562-168">**注意：**不可为 null。</span><span class="sxs-lookup"><span data-stu-id="1c562-168">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="1c562-169">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="1c562-169">securityComplianceNotificationMails</span></span>|<span data-ttu-id="1c562-170">String</span><span class="sxs-lookup"><span data-stu-id="1c562-170">String</span></span>||
|<span data-ttu-id="1c562-171">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="1c562-171">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="1c562-172">String</span><span class="sxs-lookup"><span data-stu-id="1c562-172">String</span></span>||
|<span data-ttu-id="1c562-173">state</span><span class="sxs-lookup"><span data-stu-id="1c562-173">state</span></span>|<span data-ttu-id="1c562-174">String</span><span class="sxs-lookup"><span data-stu-id="1c562-174">String</span></span>|            |
|<span data-ttu-id="1c562-175">street</span><span class="sxs-lookup"><span data-stu-id="1c562-175">street</span></span>|<span data-ttu-id="1c562-176">String</span><span class="sxs-lookup"><span data-stu-id="1c562-176">String</span></span>|            |
|<span data-ttu-id="1c562-177">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="1c562-177">technicalNotificationMails</span></span>|<span data-ttu-id="1c562-178">String</span><span class="sxs-lookup"><span data-stu-id="1c562-178">String</span></span>|                                        <span data-ttu-id="1c562-179">**注意：**不可为 null。</span><span class="sxs-lookup"><span data-stu-id="1c562-179">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="1c562-180">telephoneNumber</span><span class="sxs-lookup"><span data-stu-id="1c562-180">telephoneNumber</span></span>|<span data-ttu-id="1c562-181">String</span><span class="sxs-lookup"><span data-stu-id="1c562-181">String</span></span>|            |
|<span data-ttu-id="1c562-182">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="1c562-182">verifiedDomains</span></span>|<span data-ttu-id="1c562-183">VerifiedDomain</span><span class="sxs-lookup"><span data-stu-id="1c562-183">VerifiedDomain</span></span>|<span data-ttu-id="1c562-p106">与该租户相关联的域集合。                          **注意：**不可为 null。</span><span class="sxs-lookup"><span data-stu-id="1c562-p106">The collection of domains associated with this tenant.                            **Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="1c562-186">响应</span><span class="sxs-lookup"><span data-stu-id="1c562-186">Response</span></span>

<span data-ttu-id="1c562-187">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [organization](../resources/organization.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1c562-187">If successful, this method returns a `200 OK` response code and updated [organization](../resources/organization.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1c562-188">示例</span><span class="sxs-lookup"><span data-stu-id="1c562-188">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c562-189">请求</span><span class="sxs-lookup"><span data-stu-id="1c562-189">Request</span></span>
<span data-ttu-id="1c562-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1c562-190">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="1c562-191">响应</span><span class="sxs-lookup"><span data-stu-id="1c562-191">Response</span></span>
<span data-ttu-id="1c562-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1c562-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
