---
title: 组织资源类型
description: " 不支持创建和删除操作。 继承自 directoryObject。"
localization_priority: Priority
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9764104cc1737effe334362f5161598957f600b3
ms.sourcegitcommit: 612e1d796023433c6e15a9d66ba99d9bdc424cee
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52703641"
---
# <a name="organization-resource-type"></a><span data-ttu-id="1db07-104">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="1db07-104">organization resource type</span></span>

<span data-ttu-id="1db07-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1db07-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1db07-106">表示用户或应用程序所登录的 Azure Active Directory 租户。</span><span class="sxs-lookup"><span data-stu-id="1db07-106">Represents the Azure Active Directory tenant that the user or application is signed in to.</span></span> <span data-ttu-id="1db07-107">只支持在此资源上执行读取和更新操作；不支持创建和删除操作。</span><span class="sxs-lookup"><span data-stu-id="1db07-107">Only the read and update operations are supported on this resource; create and delete are not supported.</span></span> <span data-ttu-id="1db07-108">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="1db07-108">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="1db07-109">使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="1db07-109">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="1db07-110">方法</span><span class="sxs-lookup"><span data-stu-id="1db07-110">Methods</span></span>

| <span data-ttu-id="1db07-111">方法</span><span class="sxs-lookup"><span data-stu-id="1db07-111">Method</span></span>       | <span data-ttu-id="1db07-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="1db07-112">Return Type</span></span>  |<span data-ttu-id="1db07-113">说明</span><span class="sxs-lookup"><span data-stu-id="1db07-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1db07-114">获取组织</span><span class="sxs-lookup"><span data-stu-id="1db07-114">Get organization</span></span>](../api/organization-get.md) | <span data-ttu-id="1db07-115">[organization](organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1db07-115">[organization](organization.md) collection</span></span>|<span data-ttu-id="1db07-116">读取 organization 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1db07-116">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="1db07-117">更新</span><span class="sxs-lookup"><span data-stu-id="1db07-117">Update</span></span>](../api/organization-update.md) | [<span data-ttu-id="1db07-118">组织</span><span class="sxs-lookup"><span data-stu-id="1db07-118">organization</span></span>](organization.md)  |<span data-ttu-id="1db07-119">更新 organization 对象。</span><span class="sxs-lookup"><span data-stu-id="1db07-119">Update organization object.</span></span> <span data-ttu-id="1db07-120">可更新的限定属性：**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones** 和 **privacyProfile**。</span><span class="sxs-lookup"><span data-stu-id="1db07-120">The only properties that can be updated are: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** and **privacyProfile**.</span></span> |
|<span data-ttu-id="1db07-121">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="1db07-121">**Open extensions**</span></span>| 
|[<span data-ttu-id="1db07-122">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="1db07-122">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="1db07-123">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="1db07-123">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="1db07-124">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="1db07-124">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="1db07-125">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="1db07-125">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="1db07-126">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1db07-126">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="1db07-127">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="1db07-127">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="1db07-128">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="1db07-128">**Schema extensions**</span></span>| 
|[<span data-ttu-id="1db07-129">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="1db07-129">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="1db07-130">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="1db07-130">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
| [<span data-ttu-id="1db07-131">进行品牌打造</span><span class="sxs-lookup"><span data-stu-id="1db07-131">Get branding</span></span>](../api/organizationalbrandingproperties-get.md) | <span data-ttu-id="1db07-132">[organizationalBrandingProperties](organizationalbrandingproperties.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1db07-132">[organizationalBrandingProperties](organizationalbrandingproperties.md) collection</span></span> | <span data-ttu-id="1db07-133">获取 organizationalBrandingProperties 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1db07-133">Get an organizationalBrandingProperties object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="1db07-134">属性</span><span class="sxs-lookup"><span data-stu-id="1db07-134">Properties</span></span>

| <span data-ttu-id="1db07-135">属性</span><span class="sxs-lookup"><span data-stu-id="1db07-135">Property</span></span> | <span data-ttu-id="1db07-136">类型</span><span class="sxs-lookup"><span data-stu-id="1db07-136">Type</span></span> | <span data-ttu-id="1db07-137">说明</span><span class="sxs-lookup"><span data-stu-id="1db07-137">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="1db07-138">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="1db07-138">assignedPlans</span></span> | <span data-ttu-id="1db07-139">[assignedPlan](assignedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1db07-139">[assignedPlan](assignedplan.md) collection</span></span> | <span data-ttu-id="1db07-p104">与租户相关的服务计划的集合。不可为空。</span><span class="sxs-lookup"><span data-stu-id="1db07-p104">The collection of service plans associated with the tenant. Not nullable.</span></span> |
| <span data-ttu-id="1db07-142">businessPhones</span><span class="sxs-lookup"><span data-stu-id="1db07-142">businessPhones</span></span> | <span data-ttu-id="1db07-143">String collection</span><span class="sxs-lookup"><span data-stu-id="1db07-143">String collection</span></span> | <span data-ttu-id="1db07-p105">组织的电话号码。虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="1db07-p105">Telephone number for the organization. Although this is a string collection, only one number can be set for this property.</span></span> |
| <span data-ttu-id="1db07-146">城市</span><span class="sxs-lookup"><span data-stu-id="1db07-146">city</span></span> | <span data-ttu-id="1db07-147">String</span><span class="sxs-lookup"><span data-stu-id="1db07-147">String</span></span> | <span data-ttu-id="1db07-148">组织地址所在的城市名称。</span><span class="sxs-lookup"><span data-stu-id="1db07-148">City name of the address for the organization.</span></span> |
| <span data-ttu-id="1db07-149">country</span><span class="sxs-lookup"><span data-stu-id="1db07-149">country</span></span> | <span data-ttu-id="1db07-150">String</span><span class="sxs-lookup"><span data-stu-id="1db07-150">String</span></span> | <span data-ttu-id="1db07-151">组织地址所在的国家/地区名称。</span><span class="sxs-lookup"><span data-stu-id="1db07-151">Country/region name of the address for the organization.</span></span> |
| <span data-ttu-id="1db07-152">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="1db07-152">countryLetterCode</span></span> | <span data-ttu-id="1db07-153">String</span><span class="sxs-lookup"><span data-stu-id="1db07-153">String</span></span> | <span data-ttu-id="1db07-154">组织所在的国家/地区缩写。</span><span class="sxs-lookup"><span data-stu-id="1db07-154">Country/region abbreviation for the organization.</span></span> |
| <span data-ttu-id="1db07-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1db07-155">createdDateTime</span></span> | <span data-ttu-id="1db07-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1db07-156">DateTimeOffset</span></span> | <span data-ttu-id="1db07-157">组织的创建时间戳。</span><span class="sxs-lookup"><span data-stu-id="1db07-157">Timestamp of when the organization was created.</span></span> <span data-ttu-id="1db07-158">值无法修改，并在组织创建时自动填充。</span><span class="sxs-lookup"><span data-stu-id="1db07-158">The value cannot be modified and is automatically populated when the organization is created.</span></span> <span data-ttu-id="1db07-159">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1db07-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1db07-160">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="1db07-160">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="1db07-161">只读。</span><span class="sxs-lookup"><span data-stu-id="1db07-161">Read-only.</span></span> |
| <span data-ttu-id="1db07-162">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="1db07-162">deletedDateTime</span></span> | <span data-ttu-id="1db07-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1db07-163">DateTimeOffset</span></span> | <span data-ttu-id="1db07-164">表示采用 ISO 8601 格式创建 Azure AD 的日期和时间，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="1db07-164">Represents date and time of when the Azure AD tenant was deleted using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1db07-165">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="1db07-165">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="1db07-166">只读。</span><span class="sxs-lookup"><span data-stu-id="1db07-166">Read-only.</span></span> |
| <span data-ttu-id="1db07-167">displayName</span><span class="sxs-lookup"><span data-stu-id="1db07-167">displayName</span></span> | <span data-ttu-id="1db07-168">String</span><span class="sxs-lookup"><span data-stu-id="1db07-168">String</span></span> | <span data-ttu-id="1db07-169">租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1db07-169">The display name for the tenant.</span></span> |
| <span data-ttu-id="1db07-170">id</span><span class="sxs-lookup"><span data-stu-id="1db07-170">id</span></span> | <span data-ttu-id="1db07-171">字符串</span><span class="sxs-lookup"><span data-stu-id="1db07-171">String</span></span> | <span data-ttu-id="1db07-172">租户 ID，表示组织（或租户）的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1db07-172">The tenant ID, a unique identifier representing the organization (or tenant).</span></span> <span data-ttu-id="1db07-173">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="1db07-173">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="1db07-174">键。</span><span class="sxs-lookup"><span data-stu-id="1db07-174">Key.</span></span> <span data-ttu-id="1db07-175">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="1db07-175">Not nullable.</span></span> <span data-ttu-id="1db07-176">只读。</span><span class="sxs-lookup"><span data-stu-id="1db07-176">Read-only.</span></span> |
| <span data-ttu-id="1db07-177">isMultipleDataLocationsForServicesEnabled</span><span class="sxs-lookup"><span data-stu-id="1db07-177">isMultipleDataLocationsForServicesEnabled</span></span> | <span data-ttu-id="1db07-178">布尔值</span><span class="sxs-lookup"><span data-stu-id="1db07-178">Boolean</span></span> | <span data-ttu-id="1db07-179">`true` 如果组织已启用多异地; **未** 多地理"则显示 false 信息; **null** （默认）。</span><span class="sxs-lookup"><span data-stu-id="1db07-179">`true` if organization is Multi-Geo enabled; **false** if organization is not Multi-Geo enabled; **null** (default).</span></span> <span data-ttu-id="1db07-180">只读。</span><span class="sxs-lookup"><span data-stu-id="1db07-180">Read-only.</span></span> <span data-ttu-id="1db07-181">有关详细信息，请参阅 [OneDrive Online 多地理位置](/sharepoint/dev/solution-guidance/multigeo-introduction)。</span><span class="sxs-lookup"><span data-stu-id="1db07-181">For more information, see [OneDrive Online Multi-Geo](/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span> |
| <span data-ttu-id="1db07-182">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="1db07-182">marketingNotificationEmails</span></span> | <span data-ttu-id="1db07-183">String collection</span><span class="sxs-lookup"><span data-stu-id="1db07-183">String collection</span></span> | <span data-ttu-id="1db07-184">不可为空。</span><span class="sxs-lookup"><span data-stu-id="1db07-184">Not nullable.</span></span> |
| <span data-ttu-id="1db07-185">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1db07-185">onPremisesLastSyncDateTime</span></span> | <span data-ttu-id="1db07-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1db07-186">DateTimeOffset</span></span> | <span data-ttu-id="1db07-187">租户上次与本地目录同步的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="1db07-187">The time and date at which the tenant was last synced with the on-premises directory.</span></span> <span data-ttu-id="1db07-188">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1db07-188">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1db07-189">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="1db07-189">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="1db07-190">只读。</span><span class="sxs-lookup"><span data-stu-id="1db07-190">Read-only.</span></span>|
| <span data-ttu-id="1db07-191">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="1db07-191">onPremisesSyncEnabled</span></span> | <span data-ttu-id="1db07-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="1db07-192">Boolean</span></span> | <span data-ttu-id="1db07-193">`true` 是否此对象从本地目录同步; `false` 是否此对象最初从本地目录同步，但不再同步。</span><span class="sxs-lookup"><span data-stu-id="1db07-193">`true` if this object is synced from an on-premises directory; `false` if this object was originally synced from an on-premises directory but is no longer synced.</span></span> <span data-ttu-id="1db07-194">可为空。</span><span class="sxs-lookup"><span data-stu-id="1db07-194">Nullable.</span></span> <span data-ttu-id="1db07-195">`null` 如果此对象从未从本地目录（默认）进行同步。</span><span class="sxs-lookup"><span data-stu-id="1db07-195">`null` if this object has never been synced from an on-premises directory (default).</span></span> |
| <span data-ttu-id="1db07-196">postalCode</span><span class="sxs-lookup"><span data-stu-id="1db07-196">postalCode</span></span> | <span data-ttu-id="1db07-197">String</span><span class="sxs-lookup"><span data-stu-id="1db07-197">String</span></span> | <span data-ttu-id="1db07-198">组织地址的邮政编码。</span><span class="sxs-lookup"><span data-stu-id="1db07-198">Postal code of the address for the organization.</span></span> |
| <span data-ttu-id="1db07-199">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="1db07-199">preferredLanguage</span></span> | <span data-ttu-id="1db07-200">String</span><span class="sxs-lookup"><span data-stu-id="1db07-200">String</span></span> | <span data-ttu-id="1db07-201">组织的首选语言。</span><span class="sxs-lookup"><span data-stu-id="1db07-201">The preferred language for the organization.</span></span> <span data-ttu-id="1db07-202">应遵循 ISO 639-1 代码；例如，`en`。</span><span class="sxs-lookup"><span data-stu-id="1db07-202">Should follow ISO 639-1 Code; for example, `en`.</span></span> |
| <span data-ttu-id="1db07-203">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="1db07-203">privacyProfile</span></span> | [<span data-ttu-id="1db07-204">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="1db07-204">privacyProfile</span></span>](privacyprofile.md) | <span data-ttu-id="1db07-205">组织的隐私配置文件。</span><span class="sxs-lookup"><span data-stu-id="1db07-205">The privacy profile of an organization.</span></span> |
| <span data-ttu-id="1db07-206">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="1db07-206">provisionedPlans</span></span> | <span data-ttu-id="1db07-207">[ProvisionedPlan](provisionedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1db07-207">[ProvisionedPlan](provisionedplan.md) collection</span></span> | <span data-ttu-id="1db07-208">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="1db07-208">Not nullable.</span></span> |
| <span data-ttu-id="1db07-209">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="1db07-209">securityComplianceNotificationMails</span></span> | <span data-ttu-id="1db07-210">String collection</span><span class="sxs-lookup"><span data-stu-id="1db07-210">String collection</span></span> ||
| <span data-ttu-id="1db07-211">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="1db07-211">securityComplianceNotificationPhones</span></span> | <span data-ttu-id="1db07-212">String collection</span><span class="sxs-lookup"><span data-stu-id="1db07-212">String collection</span></span>||
| <span data-ttu-id="1db07-213">state</span><span class="sxs-lookup"><span data-stu-id="1db07-213">state</span></span> | <span data-ttu-id="1db07-214">String</span><span class="sxs-lookup"><span data-stu-id="1db07-214">String</span></span> | <span data-ttu-id="1db07-215">组织地址所在的省/自治区/直辖市名称。</span><span class="sxs-lookup"><span data-stu-id="1db07-215">State name of the address for the organization.</span></span> |
| <span data-ttu-id="1db07-216">street</span><span class="sxs-lookup"><span data-stu-id="1db07-216">street</span></span> | <span data-ttu-id="1db07-217">String</span><span class="sxs-lookup"><span data-stu-id="1db07-217">String</span></span> | <span data-ttu-id="1db07-218">组织地址所在的街道名称。</span><span class="sxs-lookup"><span data-stu-id="1db07-218">Street name of the address for organization.</span></span> |
| <span data-ttu-id="1db07-219">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="1db07-219">technicalNotificationMails</span></span> | <span data-ttu-id="1db07-220">String collection</span><span class="sxs-lookup"><span data-stu-id="1db07-220">String collection</span></span> | <span data-ttu-id="1db07-221">不可为空。</span><span class="sxs-lookup"><span data-stu-id="1db07-221">Not nullable.</span></span> |
| <span data-ttu-id="1db07-222">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="1db07-222">verifiedDomains</span></span> | <span data-ttu-id="1db07-223">[VerifiedDomain](verifieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1db07-223">[VerifiedDomain](verifieddomain.md) collection</span></span> | <span data-ttu-id="1db07-p113">与该租户相关联的域集合。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="1db07-p113">The collection of domains associated with this tenant. Not nullable.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1db07-226">关系</span><span class="sxs-lookup"><span data-stu-id="1db07-226">Relationships</span></span>
| <span data-ttu-id="1db07-227">关系</span><span class="sxs-lookup"><span data-stu-id="1db07-227">Relationship</span></span> | <span data-ttu-id="1db07-228">类型</span><span class="sxs-lookup"><span data-stu-id="1db07-228">Type</span></span>   |<span data-ttu-id="1db07-229">说明</span><span class="sxs-lookup"><span data-stu-id="1db07-229">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1db07-230">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="1db07-230">certificateBasedAuthConfiguration</span></span>|<span data-ttu-id="1db07-231">[certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1db07-231">[certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) collection</span></span>| <span data-ttu-id="1db07-232">用于管理基于证书的身份验证配置的导航属性。</span><span class="sxs-lookup"><span data-stu-id="1db07-232">Navigation property to manage certificate-based authentication configuration.</span></span> <span data-ttu-id="1db07-233">只能在集合中创建 certificateBasedAuthConfiguration 的单个实例。</span><span class="sxs-lookup"><span data-stu-id="1db07-233">Only a single instance of certificateBasedAuthConfiguration can be created in the collection.</span></span>  |
|<span data-ttu-id="1db07-234">extensions</span><span class="sxs-lookup"><span data-stu-id="1db07-234">extensions</span></span>|<span data-ttu-id="1db07-235">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="1db07-235">[extension](extension.md) collection</span></span>|<span data-ttu-id="1db07-p115">为组织定义的开放扩展集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="1db07-p115">The collection of open extensions defined for the organization. Read-only. Nullable.</span></span>|
|<span data-ttu-id="1db07-239">organizationalbranding</span><span class="sxs-lookup"><span data-stu-id="1db07-239">organizationalBranding</span></span>|<span data-ttu-id="1db07-240">[organizationalBrandingProperties](organizationalbrandingproperties.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1db07-240">[organizationalBrandingProperties](organizationalbrandingproperties.md) collection</span></span>| <span data-ttu-id="1db07-p116">为组织打造品牌。可以为 null。</span><span class="sxs-lookup"><span data-stu-id="1db07-p116">Branding for the organization. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1db07-243">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1db07-243">JSON representation</span></span>

<span data-ttu-id="1db07-244">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1db07-244">Here is a JSON representation of the resource.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="1db07-245">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1db07-245">See also</span></span>

- [<span data-ttu-id="1db07-246">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="1db07-246">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="1db07-247">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="1db07-247">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="1db07-248">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="1db07-248">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
  ],
  "tocPath": ""
}-->
