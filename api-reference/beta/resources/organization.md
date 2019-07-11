---
title: 组织资源类型
description: '表示 Azure Active Directory 租户。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0acd2701a0dd8d08021057a545b84ae18a61adb2
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620946"
---
# <a name="organization-resource-type"></a><span data-ttu-id="e3dd5-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="e3dd5-103">organization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3dd5-104">表示用户或应用程序所登录的 Azure Active Directory 租户。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-104">Represents the Azure Active Directory tenant that the user or application is signed in to.</span></span> <span data-ttu-id="e3dd5-105">只支持在此资源上执行读取和更新操作；不支持创建和删除操作。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-105">Only the read and update operations are supported on this resource; create and delete are not supported.</span></span> <span data-ttu-id="e3dd5-106">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-106">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="e3dd5-107">使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-107">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="e3dd5-108">方法</span><span class="sxs-lookup"><span data-stu-id="e3dd5-108">Methods</span></span>

| <span data-ttu-id="e3dd5-109">方法</span><span class="sxs-lookup"><span data-stu-id="e3dd5-109">Method</span></span>       | <span data-ttu-id="e3dd5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e3dd5-110">Return Type</span></span>  |<span data-ttu-id="e3dd5-111">说明</span><span class="sxs-lookup"><span data-stu-id="e3dd5-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e3dd5-112">获取组织</span><span class="sxs-lookup"><span data-stu-id="e3dd5-112">Get organization</span></span>](../api/organization-get.md) | [<span data-ttu-id="e3dd5-113">组织</span><span class="sxs-lookup"><span data-stu-id="e3dd5-113">organization</span></span>](organization.md) |<span data-ttu-id="e3dd5-114">读取 organization 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-114">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="e3dd5-115">更新</span><span class="sxs-lookup"><span data-stu-id="e3dd5-115">Update</span></span>](../api/organization-update.md) | [<span data-ttu-id="e3dd5-116">组织</span><span class="sxs-lookup"><span data-stu-id="e3dd5-116">organization</span></span>](organization.md)  |<span data-ttu-id="e3dd5-117">更新 organization 对象。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-117">Update organization object.</span></span> <span data-ttu-id="e3dd5-118">可更新的限定属性：**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones** 和 **privacyProfile**。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-118">The only properties that can be updated are: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** and **privacyProfile**.</span></span> |
|<span data-ttu-id="e3dd5-119">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="e3dd5-119">**Open extensions**</span></span>| | |
|[<span data-ttu-id="e3dd5-120">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="e3dd5-120">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="e3dd5-121">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="e3dd5-121">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="e3dd5-122">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-122">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="e3dd5-123">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="e3dd5-123">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="e3dd5-124">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e3dd5-124">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="e3dd5-125">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-125">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="e3dd5-126">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="e3dd5-126">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="e3dd5-127">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="e3dd5-127">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="e3dd5-128">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-128">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="e3dd5-129">属性</span><span class="sxs-lookup"><span data-stu-id="e3dd5-129">Properties</span></span>
| <span data-ttu-id="e3dd5-130">属性</span><span class="sxs-lookup"><span data-stu-id="e3dd5-130">Property</span></span> | <span data-ttu-id="e3dd5-131">类型</span><span class="sxs-lookup"><span data-stu-id="e3dd5-131">Type</span></span>   | <span data-ttu-id="e3dd5-132">说明</span><span class="sxs-lookup"><span data-stu-id="e3dd5-132">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="e3dd5-133">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="e3dd5-133">assignedPlans</span></span> | <span data-ttu-id="e3dd5-134">[assignedPlan](assignedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e3dd5-134">[assignedPlan](assignedplan.md) collection</span></span> | <span data-ttu-id="e3dd5-p103">与租户相关的服务计划的集合。不可为空。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-p103">The collection of service plans associated with the tenant. Not nullable.</span></span> |
| <span data-ttu-id="e3dd5-137">businessPhones</span><span class="sxs-lookup"><span data-stu-id="e3dd5-137">businessPhones</span></span> | <span data-ttu-id="e3dd5-138">字符串集合</span><span class="sxs-lookup"><span data-stu-id="e3dd5-138">String collection</span></span> | <span data-ttu-id="e3dd5-139">组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-139">Telephone number for the organization.</span></span> <span data-ttu-id="e3dd5-140">**注意：** 虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-140">**Note:** Although this is a string collection, only one number can be set for this property.</span></span> |
| <span data-ttu-id="e3dd5-141">city</span><span class="sxs-lookup"><span data-stu-id="e3dd5-141">city</span></span> | <span data-ttu-id="e3dd5-142">String</span><span class="sxs-lookup"><span data-stu-id="e3dd5-142">String</span></span> | <span data-ttu-id="e3dd5-143">组织地址的城市名称。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-143">City name of the address for the organization.</span></span> |
| <span data-ttu-id="e3dd5-144">country</span><span class="sxs-lookup"><span data-stu-id="e3dd5-144">country</span></span> | <span data-ttu-id="e3dd5-145">String</span><span class="sxs-lookup"><span data-stu-id="e3dd5-145">String</span></span> | <span data-ttu-id="e3dd5-146">组织地址的国家/地区名称。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-146">Country/region name of the address for the organization.</span></span> |
| <span data-ttu-id="e3dd5-147">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="e3dd5-147">countryLetterCode</span></span> | <span data-ttu-id="e3dd5-148">字符串</span><span class="sxs-lookup"><span data-stu-id="e3dd5-148">String</span></span> | <span data-ttu-id="e3dd5-149">组织的国家/地区缩写。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-149">Country/region abbreviation for the organization.</span></span> |
| <span data-ttu-id="e3dd5-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3dd5-150">createdDateTime</span></span> | <span data-ttu-id="e3dd5-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3dd5-151">DateTimeOffset</span></span> | <span data-ttu-id="e3dd5-152">组织的创建时间戳。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-152">Timestamp of when the organization was created.</span></span> <span data-ttu-id="e3dd5-153">值无法修改，并在组织创建时自动填充。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-153">The value cannot be modified and is automatically populated when the organization is created.</span></span> <span data-ttu-id="e3dd5-154">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-154">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e3dd5-155">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e3dd5-156">只读。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-156">Read-only.</span></span> |
| <span data-ttu-id="e3dd5-157">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3dd5-157">deletedDateTime</span></span> | <span data-ttu-id="e3dd5-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3dd5-158">DateTimeOffset</span></span> | <span data-ttu-id="e3dd5-159">表示采用 ISO 8601 格式创建 Azure AD 的日期和时间，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-159">Represents date and time of when the Azure AD tenant was deleted using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e3dd5-160">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-160">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e3dd5-161">只读。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-161">Read-only.</span></span> |
| <span data-ttu-id="e3dd5-162">displayName</span><span class="sxs-lookup"><span data-stu-id="e3dd5-162">displayName</span></span> | <span data-ttu-id="e3dd5-163">String</span><span class="sxs-lookup"><span data-stu-id="e3dd5-163">String</span></span> | <span data-ttu-id="e3dd5-164">租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-164">The display name for the tenant.</span></span> |
| <span data-ttu-id="e3dd5-165">id</span><span class="sxs-lookup"><span data-stu-id="e3dd5-165">id</span></span> | <span data-ttu-id="e3dd5-166">字符串</span><span class="sxs-lookup"><span data-stu-id="e3dd5-166">String</span></span> | <span data-ttu-id="e3dd5-167">租户 ID，表示组织（或租户）的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-167">The tenant ID, a unique identifier representing the organization (or tenant).</span></span> <span data-ttu-id="e3dd5-168">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-168">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="e3dd5-169">键。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-169">Key.</span></span> <span data-ttu-id="e3dd5-170">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-170">Not nullable.</span></span> <span data-ttu-id="e3dd5-171">只读。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-171">Read-only.</span></span> |
| <span data-ttu-id="e3dd5-172">isMultipleDataLocationsForServicesEnabled</span><span class="sxs-lookup"><span data-stu-id="e3dd5-172">isMultipleDataLocationsForServicesEnabled</span></span> | <span data-ttu-id="e3dd5-173">布尔值</span><span class="sxs-lookup"><span data-stu-id="e3dd5-173">Boolean</span></span> | <span data-ttu-id="e3dd5-174">如果组织支持多地理位置，则为 **true**；如果组织不支持多地理位置，则为 **false**；**为空**（默认）。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-174">**true** if organization is Multi-Geo enabled; **false** if organization is not Multi-Geo enabled; **null** (default).</span></span> <span data-ttu-id="e3dd5-175">只读。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-175">Read-only.</span></span> <span data-ttu-id="e3dd5-176">有关详细信息，请参阅 [OneDrive Online 多地理位置](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-176">For more information, see [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span> |
| <span data-ttu-id="e3dd5-177">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="e3dd5-177">marketingNotificationEmails</span></span> | <span data-ttu-id="e3dd5-178">String collection</span><span class="sxs-lookup"><span data-stu-id="e3dd5-178">String collection</span></span> | <span data-ttu-id="e3dd5-179">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-179">Not nullable.</span></span> |
| <span data-ttu-id="e3dd5-180">objectType</span><span class="sxs-lookup"><span data-stu-id="e3dd5-180">objectType</span></span> | <span data-ttu-id="e3dd5-181">String</span><span class="sxs-lookup"><span data-stu-id="e3dd5-181">String</span></span> | <span data-ttu-id="e3dd5-p109">一个标识对象类型的字符串。对于租户，该值始终为“Company”。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-p109">A string that identifies the object type. For tenants the value is always “Company”.</span></span> |
| <span data-ttu-id="e3dd5-184">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e3dd5-184">onPremisesLastSyncDateTime</span></span> | <span data-ttu-id="e3dd5-185">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3dd5-185">DateTimeOffset</span></span> | <span data-ttu-id="e3dd5-186">租户上次与本地目录同步的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-186">The time and date at which the tenant was last synced with the on-premise directory.</span></span> <span data-ttu-id="e3dd5-187">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-187">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e3dd5-188">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-188">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
| <span data-ttu-id="e3dd5-189">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="e3dd5-189">onPremisesSyncEnabled</span></span> | <span data-ttu-id="e3dd5-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3dd5-190">Boolean</span></span> | <span data-ttu-id="e3dd5-191">如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-191">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span> |
| <span data-ttu-id="e3dd5-192">postalCode</span><span class="sxs-lookup"><span data-stu-id="e3dd5-192">postalCode</span></span> | <span data-ttu-id="e3dd5-193">String</span><span class="sxs-lookup"><span data-stu-id="e3dd5-193">String</span></span> | <span data-ttu-id="e3dd5-194">组织地址的邮政编码。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-194">Postal code of the address for the organization.</span></span> |
| <span data-ttu-id="e3dd5-195">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="e3dd5-195">preferredLanguage</span></span> | <span data-ttu-id="e3dd5-196">String</span><span class="sxs-lookup"><span data-stu-id="e3dd5-196">String</span></span> | <span data-ttu-id="e3dd5-197">组织的首选语言。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-197">The preferred language for the organization.</span></span> <span data-ttu-id="e3dd5-198">应遵循 ISO 639-1 代码；例如“en”。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-198">Should follow ISO 639-1 Code; for example "en".</span></span> |
| <span data-ttu-id="e3dd5-199">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="e3dd5-199">privacyProfile</span></span> | [<span data-ttu-id="e3dd5-200">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="e3dd5-200">privacyProfile</span></span>](privacyprofile.md) | <span data-ttu-id="e3dd5-201">组织的隐私配置文件。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-201">The privacy profile of an organization.</span></span> |
| <span data-ttu-id="e3dd5-202">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="e3dd5-202">provisionedPlans</span></span> | <span data-ttu-id="e3dd5-203">[provisionedPlan](provisionedplan.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3dd5-203">[provisionedPlan](provisionedplan.md) collection</span></span> | <span data-ttu-id="e3dd5-204">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-204">Not nullable.</span></span> |
| <span data-ttu-id="e3dd5-205">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="e3dd5-205">securityComplianceNotificationMails</span></span> | <span data-ttu-id="e3dd5-206">String collection</span><span class="sxs-lookup"><span data-stu-id="e3dd5-206">String collection</span></span> ||
| <span data-ttu-id="e3dd5-207">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="e3dd5-207">securityComplianceNotificationPhones</span></span> | <span data-ttu-id="e3dd5-208">String collection</span><span class="sxs-lookup"><span data-stu-id="e3dd5-208">String collection</span></span> ||
| <span data-ttu-id="e3dd5-209">state</span><span class="sxs-lookup"><span data-stu-id="e3dd5-209">state</span></span> | <span data-ttu-id="e3dd5-210">String</span><span class="sxs-lookup"><span data-stu-id="e3dd5-210">String</span></span> | <span data-ttu-id="e3dd5-211">组织地址的省/市/自治区名称。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-211">State name of the address for the organization.</span></span> |
| <span data-ttu-id="e3dd5-212">street</span><span class="sxs-lookup"><span data-stu-id="e3dd5-212">street</span></span> | <span data-ttu-id="e3dd5-213">String</span><span class="sxs-lookup"><span data-stu-id="e3dd5-213">String</span></span> | <span data-ttu-id="e3dd5-214">组织地址的街道名称。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-214">Street name of the address for organization.</span></span> |
| <span data-ttu-id="e3dd5-215">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="e3dd5-215">technicalNotificationMails</span></span> |<span data-ttu-id="e3dd5-216">String collection</span><span class="sxs-lookup"><span data-stu-id="e3dd5-216">String collection</span></span> | <span data-ttu-id="e3dd5-217">不可为空。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-217">Not nullable.</span></span> |
| <span data-ttu-id="e3dd5-218">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="e3dd5-218">verifiedDomains</span></span> | <span data-ttu-id="e3dd5-219">[verifiedDomain](verifieddomain.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3dd5-219">[verifiedDomain](verifieddomain.md) collection</span></span>|<span data-ttu-id="e3dd5-p112">与该租户相关联的域集合。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-p112">The collection of domains associated with this tenant. Not nullable.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e3dd5-222">关系</span><span class="sxs-lookup"><span data-stu-id="e3dd5-222">Relationships</span></span>

| <span data-ttu-id="e3dd5-223">关系</span><span class="sxs-lookup"><span data-stu-id="e3dd5-223">Relationship</span></span>     | <span data-ttu-id="e3dd5-224">类型</span><span class="sxs-lookup"><span data-stu-id="e3dd5-224">Type</span></span>   |<span data-ttu-id="e3dd5-225">说明</span><span class="sxs-lookup"><span data-stu-id="e3dd5-225">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3dd5-226">extensions</span><span class="sxs-lookup"><span data-stu-id="e3dd5-226">extensions</span></span>|<span data-ttu-id="e3dd5-227">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="e3dd5-227">[extension](extension.md) collection</span></span>|<span data-ttu-id="e3dd5-228">为组织资源定义的开放扩展的集合。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-228">The collection of open extensions defined for the organization resource.</span></span> <span data-ttu-id="e3dd5-229">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-229">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3dd5-230">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3dd5-230">JSON representation</span></span>

<span data-ttu-id="e3dd5-231">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3dd5-231">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions"
  ],
  "keyProperty": "id",
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
  "objectType": "string",
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
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}],
  "companyLastDirSyncTime": "2019-02-07T20:33:52.942Z",
  "dirSyncEnabled": true
}
```

## <a name="see-also"></a><span data-ttu-id="e3dd5-232">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e3dd5-232">See also</span></span>

- [<span data-ttu-id="e3dd5-233">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e3dd5-233">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="e3dd5-234">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e3dd5-234">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="e3dd5-235">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="e3dd5-235">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
