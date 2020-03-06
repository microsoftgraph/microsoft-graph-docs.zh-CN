---
title: 组织资源类型
description: " 不支持创建和删除操作。 继承自 directoryObject。"
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bbb11149edd6263aaf65570a9068e4333c293ae6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534132"
---
# <a name="organization-resource-type"></a><span data-ttu-id="17997-104">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="17997-104">organization resource type</span></span>

<span data-ttu-id="17997-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17997-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="17997-106">表示用户或应用程序所登录的 Azure Active Directory 租户。</span><span class="sxs-lookup"><span data-stu-id="17997-106">Represents the Azure Active Directory tenant that the user or application is signed in to.</span></span> <span data-ttu-id="17997-107">只支持在此资源上执行读取和更新操作；不支持创建和删除操作。</span><span class="sxs-lookup"><span data-stu-id="17997-107">Only the read and update operations are supported on this resource; create and delete are not supported.</span></span> <span data-ttu-id="17997-108">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="17997-108">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="17997-109">使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="17997-109">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="17997-110">方法</span><span class="sxs-lookup"><span data-stu-id="17997-110">Methods</span></span>

| <span data-ttu-id="17997-111">方法</span><span class="sxs-lookup"><span data-stu-id="17997-111">Method</span></span>       | <span data-ttu-id="17997-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="17997-112">Return Type</span></span>  |<span data-ttu-id="17997-113">说明</span><span class="sxs-lookup"><span data-stu-id="17997-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="17997-114">获取组织</span><span class="sxs-lookup"><span data-stu-id="17997-114">Get organization</span></span>](../api/organization-get.md) | <span data-ttu-id="17997-115">[organization](organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17997-115">[organization](organization.md) collection</span></span>|<span data-ttu-id="17997-116">读取 organization 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="17997-116">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="17997-117">更新</span><span class="sxs-lookup"><span data-stu-id="17997-117">Update</span></span>](../api/organization-update.md) | [<span data-ttu-id="17997-118">组织</span><span class="sxs-lookup"><span data-stu-id="17997-118">organization</span></span>](organization.md)  |<span data-ttu-id="17997-119">更新 organization 对象。</span><span class="sxs-lookup"><span data-stu-id="17997-119">Update organization object.</span></span> <span data-ttu-id="17997-120">可更新的限定属性：**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones** 和 **privacyProfile**。</span><span class="sxs-lookup"><span data-stu-id="17997-120">The only properties that can be updated are: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** and **privacyProfile**.</span></span> |
|<span data-ttu-id="17997-121">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="17997-121">**Open extensions**</span></span>| 
|[<span data-ttu-id="17997-122">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="17997-122">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="17997-123">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="17997-123">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="17997-124">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="17997-124">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="17997-125">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="17997-125">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="17997-126">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17997-126">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="17997-127">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="17997-127">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="17997-128">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="17997-128">**Schema extensions**</span></span>| 
|[<span data-ttu-id="17997-129">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="17997-129">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="17997-130">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="17997-130">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="17997-131">属性</span><span class="sxs-lookup"><span data-stu-id="17997-131">Properties</span></span>

| <span data-ttu-id="17997-132">属性</span><span class="sxs-lookup"><span data-stu-id="17997-132">Property</span></span> | <span data-ttu-id="17997-133">类型</span><span class="sxs-lookup"><span data-stu-id="17997-133">Type</span></span> | <span data-ttu-id="17997-134">说明</span><span class="sxs-lookup"><span data-stu-id="17997-134">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="17997-135">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="17997-135">assignedPlans</span></span> | <span data-ttu-id="17997-136">[assignedPlan](assignedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17997-136">[assignedPlan](assignedplan.md) collection</span></span> | <span data-ttu-id="17997-p104">与租户相关的服务计划的集合。不可为空。</span><span class="sxs-lookup"><span data-stu-id="17997-p104">The collection of service plans associated with the tenant. Not nullable.</span></span> |
| <span data-ttu-id="17997-139">businessPhones</span><span class="sxs-lookup"><span data-stu-id="17997-139">businessPhones</span></span> | <span data-ttu-id="17997-140">字符串集合</span><span class="sxs-lookup"><span data-stu-id="17997-140">String collection</span></span> | <span data-ttu-id="17997-141">组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="17997-141">Telephone number for the organization.</span></span> <span data-ttu-id="17997-142">注意：虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="17997-142">NOTE: Although this is a string collection, only one number can be set for this property.</span></span> |
| <span data-ttu-id="17997-143">city</span><span class="sxs-lookup"><span data-stu-id="17997-143">city</span></span> | <span data-ttu-id="17997-144">String</span><span class="sxs-lookup"><span data-stu-id="17997-144">String</span></span> | <span data-ttu-id="17997-145">组织地址所在的城市名称。</span><span class="sxs-lookup"><span data-stu-id="17997-145">City name of the address for the organization.</span></span> |
| <span data-ttu-id="17997-146">country</span><span class="sxs-lookup"><span data-stu-id="17997-146">country</span></span> | <span data-ttu-id="17997-147">String</span><span class="sxs-lookup"><span data-stu-id="17997-147">String</span></span> | <span data-ttu-id="17997-148">组织地址所在的国家/地区名称。</span><span class="sxs-lookup"><span data-stu-id="17997-148">Country/region name of the address for the organization.</span></span> |
| <span data-ttu-id="17997-149">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="17997-149">countryLetterCode</span></span> | <span data-ttu-id="17997-150">String</span><span class="sxs-lookup"><span data-stu-id="17997-150">String</span></span> | <span data-ttu-id="17997-151">组织所在的国家/地区缩写。</span><span class="sxs-lookup"><span data-stu-id="17997-151">Country/region abbreviation for the organization.</span></span> |
| <span data-ttu-id="17997-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17997-152">createdDateTime</span></span> | <span data-ttu-id="17997-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17997-153">DateTimeOffset</span></span> | <span data-ttu-id="17997-154">组织的创建时间戳。</span><span class="sxs-lookup"><span data-stu-id="17997-154">Timestamp of when the organization was created.</span></span> <span data-ttu-id="17997-155">值无法修改，并在组织创建时自动填充。</span><span class="sxs-lookup"><span data-stu-id="17997-155">The value cannot be modified and is automatically populated when the organization is created.</span></span> <span data-ttu-id="17997-156">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="17997-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="17997-157">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="17997-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="17997-158">只读。</span><span class="sxs-lookup"><span data-stu-id="17997-158">Read-only.</span></span> |
| <span data-ttu-id="17997-159">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="17997-159">deletedDateTime</span></span> | <span data-ttu-id="17997-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17997-160">DateTimeOffset</span></span> | <span data-ttu-id="17997-161">表示采用 ISO 8601 格式创建 Azure AD 的日期和时间，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="17997-161">Represents date and time of when the Azure AD tenant was deleted using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="17997-162">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="17997-162">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="17997-163">只读。</span><span class="sxs-lookup"><span data-stu-id="17997-163">Read-only.</span></span> |
| <span data-ttu-id="17997-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17997-164">createdDateTime</span></span> | <span data-ttu-id="17997-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17997-165">DateTimeOffset</span></span> | <span data-ttu-id="17997-166">组织的创建时间戳。</span><span class="sxs-lookup"><span data-stu-id="17997-166">Timestamp of when the organization was created.</span></span> <span data-ttu-id="17997-167">值无法修改，并在组织创建时自动填充。</span><span class="sxs-lookup"><span data-stu-id="17997-167">The value cannot be modified and is automatically populated when the organization is created.</span></span> <span data-ttu-id="17997-168">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="17997-168">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="17997-169">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="17997-169">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="17997-170">只读。</span><span class="sxs-lookup"><span data-stu-id="17997-170">Read-only.</span></span> |
| <span data-ttu-id="17997-171">displayName</span><span class="sxs-lookup"><span data-stu-id="17997-171">displayName</span></span> | <span data-ttu-id="17997-172">String</span><span class="sxs-lookup"><span data-stu-id="17997-172">String</span></span> | <span data-ttu-id="17997-173">租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="17997-173">The display name for the tenant.</span></span> |
| <span data-ttu-id="17997-174">id</span><span class="sxs-lookup"><span data-stu-id="17997-174">id</span></span> | <span data-ttu-id="17997-175">字符串</span><span class="sxs-lookup"><span data-stu-id="17997-175">String</span></span> | <span data-ttu-id="17997-176">租户 ID，表示组织（或租户）的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="17997-176">The tenant ID, a unique identifier representing the organization (or tenant).</span></span> <span data-ttu-id="17997-177">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="17997-177">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="17997-178">键。</span><span class="sxs-lookup"><span data-stu-id="17997-178">Key.</span></span> <span data-ttu-id="17997-179">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="17997-179">Not nullable.</span></span> <span data-ttu-id="17997-180">只读。</span><span class="sxs-lookup"><span data-stu-id="17997-180">Read-only.</span></span> |
| <span data-ttu-id="17997-181">isMultipleDataLocationsForServicesEnabled</span><span class="sxs-lookup"><span data-stu-id="17997-181">isMultipleDataLocationsForServicesEnabled</span></span> | <span data-ttu-id="17997-182">布尔值</span><span class="sxs-lookup"><span data-stu-id="17997-182">Boolean</span></span> | <span data-ttu-id="17997-183">如果组织支持多地理位置，则为 **true**；如果组织不支持多地理位置，则为 **false**；**为空**（默认）。</span><span class="sxs-lookup"><span data-stu-id="17997-183">**true** if organization is Multi-Geo enabled; **false** if organization is not Multi-Geo enabled; **null** (default).</span></span> <span data-ttu-id="17997-184">只读。</span><span class="sxs-lookup"><span data-stu-id="17997-184">Read-only.</span></span> <span data-ttu-id="17997-185">有关详细信息，请参阅 [OneDrive Online 多地理位置](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)。</span><span class="sxs-lookup"><span data-stu-id="17997-185">For more information, see [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span> |
| <span data-ttu-id="17997-186">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="17997-186">marketingNotificationEmails</span></span> | <span data-ttu-id="17997-187">String collection</span><span class="sxs-lookup"><span data-stu-id="17997-187">String collection</span></span> | <span data-ttu-id="17997-188">不可为空。</span><span class="sxs-lookup"><span data-stu-id="17997-188">Not nullable.</span></span> |
| <span data-ttu-id="17997-189">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="17997-189">onPremisesLastSyncDateTime</span></span> | <span data-ttu-id="17997-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17997-190">DateTimeOffset</span></span> | <span data-ttu-id="17997-191">租户上次与本地目录同步的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="17997-191">The time and date at which the tenant was last synced with the on-premise directory.</span></span> <span data-ttu-id="17997-192">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="17997-192">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="17997-193">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="17997-193">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="17997-194">只读。</span><span class="sxs-lookup"><span data-stu-id="17997-194">Read-only.</span></span> |
| <span data-ttu-id="17997-195">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="17997-195">onPremisesSyncEnabled</span></span> | <span data-ttu-id="17997-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="17997-196">Boolean</span></span> | <span data-ttu-id="17997-197">如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="17997-197">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span> |
| <span data-ttu-id="17997-198">postalCode</span><span class="sxs-lookup"><span data-stu-id="17997-198">postalCode</span></span> | <span data-ttu-id="17997-199">String</span><span class="sxs-lookup"><span data-stu-id="17997-199">String</span></span> | <span data-ttu-id="17997-200">组织地址的邮政编码。</span><span class="sxs-lookup"><span data-stu-id="17997-200">Postal code of the address for the organization.</span></span> |
| <span data-ttu-id="17997-201">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="17997-201">preferredLanguage</span></span> | <span data-ttu-id="17997-202">String</span><span class="sxs-lookup"><span data-stu-id="17997-202">String</span></span> | <span data-ttu-id="17997-203">组织的首选语言。</span><span class="sxs-lookup"><span data-stu-id="17997-203">The preferred language for the organization.</span></span> <span data-ttu-id="17997-204">应遵循 ISO 639-1 代码；例如“en”。</span><span class="sxs-lookup"><span data-stu-id="17997-204">Should follow ISO 639-1 Code; for example "en".</span></span> |
| <span data-ttu-id="17997-205">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="17997-205">privacyProfile</span></span> | [<span data-ttu-id="17997-206">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="17997-206">privacyProfile</span></span>](privacyprofile.md) | <span data-ttu-id="17997-207">组织的隐私配置文件。</span><span class="sxs-lookup"><span data-stu-id="17997-207">The privacy profile of an organization.</span></span> |
| <span data-ttu-id="17997-208">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="17997-208">provisionedPlans</span></span> | <span data-ttu-id="17997-209">[ProvisionedPlan](provisionedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17997-209">[ProvisionedPlan](provisionedplan.md) collection</span></span> | <span data-ttu-id="17997-210">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="17997-210">Not nullable.</span></span> |
| <span data-ttu-id="17997-211">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="17997-211">securityComplianceNotificationMails</span></span> | <span data-ttu-id="17997-212">String collection</span><span class="sxs-lookup"><span data-stu-id="17997-212">String collection</span></span> ||
| <span data-ttu-id="17997-213">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="17997-213">securityComplianceNotificationPhones</span></span> | <span data-ttu-id="17997-214">String collection</span><span class="sxs-lookup"><span data-stu-id="17997-214">String collection</span></span>||
| <span data-ttu-id="17997-215">state</span><span class="sxs-lookup"><span data-stu-id="17997-215">state</span></span> | <span data-ttu-id="17997-216">String</span><span class="sxs-lookup"><span data-stu-id="17997-216">String</span></span> | <span data-ttu-id="17997-217">组织地址所在的省/自治区/直辖市名称。</span><span class="sxs-lookup"><span data-stu-id="17997-217">State name of the address for the organization.</span></span> |
| <span data-ttu-id="17997-218">street</span><span class="sxs-lookup"><span data-stu-id="17997-218">street</span></span> | <span data-ttu-id="17997-219">String</span><span class="sxs-lookup"><span data-stu-id="17997-219">String</span></span> | <span data-ttu-id="17997-220">组织地址所在的街道名称。</span><span class="sxs-lookup"><span data-stu-id="17997-220">Street name of the address for organization.</span></span> |
| <span data-ttu-id="17997-221">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="17997-221">technicalNotificationMails</span></span> | <span data-ttu-id="17997-222">String collection</span><span class="sxs-lookup"><span data-stu-id="17997-222">String collection</span></span> | <span data-ttu-id="17997-223">不可为空。</span><span class="sxs-lookup"><span data-stu-id="17997-223">Not nullable.</span></span> |
| <span data-ttu-id="17997-224">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="17997-224">verifiedDomains</span></span> | <span data-ttu-id="17997-225">[VerifiedDomain](verifieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17997-225">[VerifiedDomain](verifieddomain.md) collection</span></span> | <span data-ttu-id="17997-p113">与该租户相关联的域集合。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="17997-p113">The collection of domains associated with this tenant. Not nullable.</span></span> |

## <a name="relationships"></a><span data-ttu-id="17997-228">关系</span><span class="sxs-lookup"><span data-stu-id="17997-228">Relationships</span></span>
| <span data-ttu-id="17997-229">关系</span><span class="sxs-lookup"><span data-stu-id="17997-229">Relationship</span></span> | <span data-ttu-id="17997-230">类型</span><span class="sxs-lookup"><span data-stu-id="17997-230">Type</span></span>   |<span data-ttu-id="17997-231">说明</span><span class="sxs-lookup"><span data-stu-id="17997-231">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17997-232">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="17997-232">certificateBasedAuthConfiguration</span></span>|<span data-ttu-id="17997-233">[certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="17997-233">[certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) collection</span></span>| <span data-ttu-id="17997-234">用于管理基于证书的身份验证配置的导航属性。</span><span class="sxs-lookup"><span data-stu-id="17997-234">Navigation property to manage certificate-based authentication configuration.</span></span> <span data-ttu-id="17997-235">只能在集合中创建 certificateBasedAuthConfiguration 的单个实例。</span><span class="sxs-lookup"><span data-stu-id="17997-235">Only a single instance of certificateBasedAuthConfiguration can be created in the collection.</span></span>  |
|<span data-ttu-id="17997-236">extensions</span><span class="sxs-lookup"><span data-stu-id="17997-236">extensions</span></span>|<span data-ttu-id="17997-237">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="17997-237">[extension](extension.md) collection</span></span>|<span data-ttu-id="17997-p115">为组织定义的开放扩展集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="17997-p115">The collection of open extensions defined for the organization. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17997-241">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17997-241">JSON representation</span></span>

<span data-ttu-id="17997-242">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17997-242">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "extensions"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.organization"
}-->

```json
{
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["string"],
  "city": "string",
  "country": "string",
  "countryLetterCode": "string",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "string",
  "id": "string (identifier)",
  "isMultipleDataLocationsForServicesEnabled": "boolean",
  "marketingNotificationEmails": ["string"],
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "preferredLanguage": "string",
  "privacyProfile": {"@odata.type": "microsoft.graph.privacyProfile"},
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["string"],
  "securityComplianceNotificationPhones": ["string"],
  "state": "string",
  "street": "string",
  "technicalNotificationMails": ["string"],
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}]
}
```

## <a name="see-also"></a><span data-ttu-id="17997-243">另请参阅</span><span class="sxs-lookup"><span data-stu-id="17997-243">See also</span></span>

- [<span data-ttu-id="17997-244">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="17997-244">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="17997-245">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="17997-245">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="17997-246">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="17997-246">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'businessPhones' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'onPremisesLastSyncDateTime' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'onPremisesSyncEnabled' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'securityComplianceNotificationMails' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'securityComplianceNotificationPhones' found in resource definition for 'microsoft.graph.organization', but not described in markdown table."
  ],
  "tocPath": ""
}-->
