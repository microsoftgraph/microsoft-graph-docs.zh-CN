---
title: 组织资源类型
description: '表示 Azure Active Directory 租户。 '
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8674d425d6613896ac5d90263a64c2de9f109740
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313910"
---
# <a name="organization-resource-type"></a><span data-ttu-id="643b8-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="643b8-103">organization resource type</span></span>

<span data-ttu-id="643b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="643b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="643b8-105">表示用户或应用程序所登录的 Azure Active Directory 租户。</span><span class="sxs-lookup"><span data-stu-id="643b8-105">Represents the Azure Active Directory tenant that the user or application is signed in to.</span></span> <span data-ttu-id="643b8-106">只支持在此资源上执行读取和更新操作；不支持创建和删除操作。</span><span class="sxs-lookup"><span data-stu-id="643b8-106">Only the read and update operations are supported on this resource; create and delete are not supported.</span></span> <span data-ttu-id="643b8-107">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="643b8-107">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="643b8-108">使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="643b8-108">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="643b8-109">方法</span><span class="sxs-lookup"><span data-stu-id="643b8-109">Methods</span></span>

| <span data-ttu-id="643b8-110">方法</span><span class="sxs-lookup"><span data-stu-id="643b8-110">Method</span></span>       | <span data-ttu-id="643b8-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="643b8-111">Return Type</span></span>  |<span data-ttu-id="643b8-112">说明</span><span class="sxs-lookup"><span data-stu-id="643b8-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="643b8-113">获取组织</span><span class="sxs-lookup"><span data-stu-id="643b8-113">Get organization</span></span>](../api/organization-get.md) | <span data-ttu-id="643b8-114">[organization](organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="643b8-114">[organization](organization.md) collection</span></span>|<span data-ttu-id="643b8-115">读取 organization 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="643b8-115">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="643b8-116">更新 organization</span><span class="sxs-lookup"><span data-stu-id="643b8-116">Update organization</span></span>](../api/organization-update.md) | [<span data-ttu-id="643b8-117">组织</span><span class="sxs-lookup"><span data-stu-id="643b8-117">organization</span></span>](organization.md)  |<span data-ttu-id="643b8-118">更新 organization 对象。</span><span class="sxs-lookup"><span data-stu-id="643b8-118">Update organization object.</span></span> <span data-ttu-id="643b8-119">可更新的限定属性：**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones** 和 **privacyProfile**。</span><span class="sxs-lookup"><span data-stu-id="643b8-119">The only properties that can be updated are: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** and **privacyProfile**.</span></span> |
| [<span data-ttu-id="643b8-120">获取组织设置</span><span class="sxs-lookup"><span data-stu-id="643b8-120">Get organization settings</span></span>](../api/organizationsettings-get.md) | [<span data-ttu-id="643b8-121">organizationSettings</span><span class="sxs-lookup"><span data-stu-id="643b8-121">organizationSettings</span></span>](organizationsettings.md) | <span data-ttu-id="643b8-122">读取组织设置对象。</span><span class="sxs-lookup"><span data-stu-id="643b8-122">Read the organization settings object.</span></span> |
|<span data-ttu-id="643b8-123">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="643b8-123">**Open extensions**</span></span>| | |
|[<span data-ttu-id="643b8-124">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="643b8-124">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="643b8-125">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="643b8-125">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="643b8-126">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="643b8-126">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="643b8-127">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="643b8-127">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="643b8-128">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="643b8-128">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="643b8-129">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="643b8-129">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="643b8-130">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="643b8-130">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="643b8-131">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="643b8-131">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="643b8-132">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="643b8-132">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="643b8-133">属性</span><span class="sxs-lookup"><span data-stu-id="643b8-133">Properties</span></span> 
| <span data-ttu-id="643b8-134">属性</span><span class="sxs-lookup"><span data-stu-id="643b8-134">Property</span></span> | <span data-ttu-id="643b8-135">类型</span><span class="sxs-lookup"><span data-stu-id="643b8-135">Type</span></span>   | <span data-ttu-id="643b8-136">说明</span><span class="sxs-lookup"><span data-stu-id="643b8-136">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="643b8-137">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="643b8-137">assignedPlans</span></span> | <span data-ttu-id="643b8-138">[assignedPlan](assignedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="643b8-138">[assignedPlan](assignedplan.md) collection</span></span> | <span data-ttu-id="643b8-p103">与租户相关的服务计划的集合。不可为空。</span><span class="sxs-lookup"><span data-stu-id="643b8-p103">The collection of service plans associated with the tenant. Not nullable.</span></span> |
| <span data-ttu-id="643b8-141">businessPhones</span><span class="sxs-lookup"><span data-stu-id="643b8-141">businessPhones</span></span> | <span data-ttu-id="643b8-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="643b8-142">String collection</span></span> | <span data-ttu-id="643b8-143">组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="643b8-143">Telephone number for the organization.</span></span> <span data-ttu-id="643b8-144">**注意：** 虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="643b8-144">**Note:** Although this is a string collection, only one number can be set for this property.</span></span> |
| <span data-ttu-id="643b8-145">城市</span><span class="sxs-lookup"><span data-stu-id="643b8-145">city</span></span> | <span data-ttu-id="643b8-146">String</span><span class="sxs-lookup"><span data-stu-id="643b8-146">String</span></span> | <span data-ttu-id="643b8-147">组织地址所在的城市名称。</span><span class="sxs-lookup"><span data-stu-id="643b8-147">City name of the address for the organization.</span></span> |
| <span data-ttu-id="643b8-148">country</span><span class="sxs-lookup"><span data-stu-id="643b8-148">country</span></span> | <span data-ttu-id="643b8-149">String</span><span class="sxs-lookup"><span data-stu-id="643b8-149">String</span></span> | <span data-ttu-id="643b8-150">组织地址所在的国家/地区名称。</span><span class="sxs-lookup"><span data-stu-id="643b8-150">Country/region name of the address for the organization.</span></span> |
| <span data-ttu-id="643b8-151">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="643b8-151">countryLetterCode</span></span> | <span data-ttu-id="643b8-152">String</span><span class="sxs-lookup"><span data-stu-id="643b8-152">String</span></span> | <span data-ttu-id="643b8-153">组织所在的国家/地区缩写。</span><span class="sxs-lookup"><span data-stu-id="643b8-153">Country/region abbreviation for the organization.</span></span> |
| <span data-ttu-id="643b8-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="643b8-154">createdDateTime</span></span> | <span data-ttu-id="643b8-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="643b8-155">DateTimeOffset</span></span> | <span data-ttu-id="643b8-156">组织的创建时间戳。</span><span class="sxs-lookup"><span data-stu-id="643b8-156">Timestamp of when the organization was created.</span></span> <span data-ttu-id="643b8-157">值无法修改，并在组织创建时自动填充。</span><span class="sxs-lookup"><span data-stu-id="643b8-157">The value cannot be modified and is automatically populated when the organization is created.</span></span> <span data-ttu-id="643b8-158">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="643b8-158">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="643b8-159">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="643b8-159">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="643b8-160">只读。</span><span class="sxs-lookup"><span data-stu-id="643b8-160">Read-only.</span></span> |
| <span data-ttu-id="643b8-161">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="643b8-161">deletedDateTime</span></span> | <span data-ttu-id="643b8-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="643b8-162">DateTimeOffset</span></span> | <span data-ttu-id="643b8-163">表示采用 ISO 8601 格式创建 Azure AD 的日期和时间，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="643b8-163">Represents date and time of when the Azure AD tenant was deleted using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="643b8-164">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="643b8-164">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="643b8-165">只读。</span><span class="sxs-lookup"><span data-stu-id="643b8-165">Read-only.</span></span> |
| <span data-ttu-id="643b8-166">directorySizeQuota</span><span class="sxs-lookup"><span data-stu-id="643b8-166">directorySizeQuota</span></span> | [<span data-ttu-id="643b8-167">directorySizeQuota</span><span class="sxs-lookup"><span data-stu-id="643b8-167">directorySizeQuota</span></span>](directorySizeQuota.md) | <span data-ttu-id="643b8-168">组织的目录大小配额信息。</span><span class="sxs-lookup"><span data-stu-id="643b8-168">The directory size quota information of an organization.</span></span> |
| <span data-ttu-id="643b8-169">displayName</span><span class="sxs-lookup"><span data-stu-id="643b8-169">displayName</span></span> | <span data-ttu-id="643b8-170">String</span><span class="sxs-lookup"><span data-stu-id="643b8-170">String</span></span> | <span data-ttu-id="643b8-171">租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="643b8-171">The display name for the tenant.</span></span> |
| <span data-ttu-id="643b8-172">id</span><span class="sxs-lookup"><span data-stu-id="643b8-172">id</span></span> | <span data-ttu-id="643b8-173">字符串</span><span class="sxs-lookup"><span data-stu-id="643b8-173">String</span></span> | <span data-ttu-id="643b8-174">租户 ID，表示组织（或租户）的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="643b8-174">The tenant ID, a unique identifier representing the organization (or tenant).</span></span> <span data-ttu-id="643b8-175">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="643b8-175">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="643b8-176">键。</span><span class="sxs-lookup"><span data-stu-id="643b8-176">Key.</span></span> <span data-ttu-id="643b8-177">不可为空。</span><span class="sxs-lookup"><span data-stu-id="643b8-177">Not nullable.</span></span> <span data-ttu-id="643b8-178">只读。</span><span class="sxs-lookup"><span data-stu-id="643b8-178">Read-only.</span></span> |
| <span data-ttu-id="643b8-179">isMultipleDataLocationsForServicesEnabled</span><span class="sxs-lookup"><span data-stu-id="643b8-179">isMultipleDataLocationsForServicesEnabled</span></span> | <span data-ttu-id="643b8-180">布尔值</span><span class="sxs-lookup"><span data-stu-id="643b8-180">Boolean</span></span> | <span data-ttu-id="643b8-181">如果组织支持多地理位置，则为 **true**；如果组织不支持多地理位置，则为 **false**；**为空**（默认）。</span><span class="sxs-lookup"><span data-stu-id="643b8-181">**true** if organization is Multi-Geo enabled; **false** if organization is not Multi-Geo enabled; **null** (default).</span></span> <span data-ttu-id="643b8-182">只读。</span><span class="sxs-lookup"><span data-stu-id="643b8-182">Read-only.</span></span> <span data-ttu-id="643b8-183">有关详细信息，请参阅 [OneDrive Online 多地理位置](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)。</span><span class="sxs-lookup"><span data-stu-id="643b8-183">For more information, see [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span> |
| <span data-ttu-id="643b8-184">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="643b8-184">marketingNotificationEmails</span></span> | <span data-ttu-id="643b8-185">String collection</span><span class="sxs-lookup"><span data-stu-id="643b8-185">String collection</span></span> | <span data-ttu-id="643b8-186">不可为空。</span><span class="sxs-lookup"><span data-stu-id="643b8-186">Not nullable.</span></span> |
| <span data-ttu-id="643b8-187">objectType</span><span class="sxs-lookup"><span data-stu-id="643b8-187">objectType</span></span> | <span data-ttu-id="643b8-188">String</span><span class="sxs-lookup"><span data-stu-id="643b8-188">String</span></span> | <span data-ttu-id="643b8-p109">一个标识对象类型的字符串。对于租户，该值始终为“Company”。</span><span class="sxs-lookup"><span data-stu-id="643b8-p109">A string that identifies the object type. For tenants the value is always “Company”.</span></span> |
| <span data-ttu-id="643b8-191">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="643b8-191">onPremisesLastSyncDateTime</span></span> | <span data-ttu-id="643b8-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="643b8-192">DateTimeOffset</span></span> | <span data-ttu-id="643b8-193">租户上次与本地目录同步的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="643b8-193">The time and date at which the tenant was last synced with the on-premise directory.</span></span> <span data-ttu-id="643b8-194">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="643b8-194">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="643b8-195">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="643b8-195">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
| <span data-ttu-id="643b8-196">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="643b8-196">onPremisesSyncEnabled</span></span> | <span data-ttu-id="643b8-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="643b8-197">Boolean</span></span> | <span data-ttu-id="643b8-198">如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="643b8-198">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span> |
| <span data-ttu-id="643b8-199">postalCode</span><span class="sxs-lookup"><span data-stu-id="643b8-199">postalCode</span></span> | <span data-ttu-id="643b8-200">String</span><span class="sxs-lookup"><span data-stu-id="643b8-200">String</span></span> | <span data-ttu-id="643b8-201">组织地址的邮政编码。</span><span class="sxs-lookup"><span data-stu-id="643b8-201">Postal code of the address for the organization.</span></span> |
| <span data-ttu-id="643b8-202">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="643b8-202">preferredLanguage</span></span> | <span data-ttu-id="643b8-203">String</span><span class="sxs-lookup"><span data-stu-id="643b8-203">String</span></span> | <span data-ttu-id="643b8-204">组织的首选语言。</span><span class="sxs-lookup"><span data-stu-id="643b8-204">The preferred language for the organization.</span></span> <span data-ttu-id="643b8-205">应遵循 ISO 639-1 代码；例如“en”。</span><span class="sxs-lookup"><span data-stu-id="643b8-205">Should follow ISO 639-1 Code; for example "en".</span></span> |
| <span data-ttu-id="643b8-206">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="643b8-206">privacyProfile</span></span> | [<span data-ttu-id="643b8-207">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="643b8-207">privacyProfile</span></span>](privacyprofile.md) | <span data-ttu-id="643b8-208">组织的隐私配置文件。</span><span class="sxs-lookup"><span data-stu-id="643b8-208">The privacy profile of an organization.</span></span> |
| <span data-ttu-id="643b8-209">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="643b8-209">provisionedPlans</span></span> | <span data-ttu-id="643b8-210">[provisionedPlan](provisionedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="643b8-210">[provisionedPlan](provisionedplan.md) collection</span></span> | <span data-ttu-id="643b8-211">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="643b8-211">Not nullable.</span></span> |
| <span data-ttu-id="643b8-212">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="643b8-212">securityComplianceNotificationMails</span></span> | <span data-ttu-id="643b8-213">String collection</span><span class="sxs-lookup"><span data-stu-id="643b8-213">String collection</span></span> ||
| <span data-ttu-id="643b8-214">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="643b8-214">securityComplianceNotificationPhones</span></span> | <span data-ttu-id="643b8-215">String collection</span><span class="sxs-lookup"><span data-stu-id="643b8-215">String collection</span></span> ||
| <span data-ttu-id="643b8-216">state</span><span class="sxs-lookup"><span data-stu-id="643b8-216">state</span></span> | <span data-ttu-id="643b8-217">String</span><span class="sxs-lookup"><span data-stu-id="643b8-217">String</span></span> | <span data-ttu-id="643b8-218">组织地址所在的省/自治区/直辖市名称。</span><span class="sxs-lookup"><span data-stu-id="643b8-218">State name of the address for the organization.</span></span> |
| <span data-ttu-id="643b8-219">street</span><span class="sxs-lookup"><span data-stu-id="643b8-219">street</span></span> | <span data-ttu-id="643b8-220">String</span><span class="sxs-lookup"><span data-stu-id="643b8-220">String</span></span> | <span data-ttu-id="643b8-221">组织地址所在的街道名称。</span><span class="sxs-lookup"><span data-stu-id="643b8-221">Street name of the address for organization.</span></span> |
| <span data-ttu-id="643b8-222">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="643b8-222">technicalNotificationMails</span></span> |<span data-ttu-id="643b8-223">String collection</span><span class="sxs-lookup"><span data-stu-id="643b8-223">String collection</span></span> | <span data-ttu-id="643b8-224">不可为空。</span><span class="sxs-lookup"><span data-stu-id="643b8-224">Not nullable.</span></span> |
| <span data-ttu-id="643b8-225">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="643b8-225">verifiedDomains</span></span> | <span data-ttu-id="643b8-226">[verifiedDomain](verifieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="643b8-226">[verifiedDomain](verifieddomain.md) collection</span></span>|<span data-ttu-id="643b8-p112">与该租户相关联的域集合。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="643b8-p112">The collection of domains associated with this tenant. Not nullable.</span></span> |

## <a name="relationships"></a><span data-ttu-id="643b8-229">关系</span><span class="sxs-lookup"><span data-stu-id="643b8-229">Relationships</span></span>

| <span data-ttu-id="643b8-230">关系</span><span class="sxs-lookup"><span data-stu-id="643b8-230">Relationship</span></span>  | <span data-ttu-id="643b8-231">类型</span><span class="sxs-lookup"><span data-stu-id="643b8-231">Type</span></span>  |<span data-ttu-id="643b8-232">说明</span><span class="sxs-lookup"><span data-stu-id="643b8-232">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="643b8-233">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="643b8-233">certificateBasedAuthConfiguration</span></span>|<span data-ttu-id="643b8-234">[certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="643b8-234">[certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) collection</span></span>| <span data-ttu-id="643b8-235">用于管理基于证书的身份验证配置的导航属性。</span><span class="sxs-lookup"><span data-stu-id="643b8-235">Navigation property to manage  certificate-based authentication configuration.</span></span> <span data-ttu-id="643b8-236">只能在集合中创建 certificateBasedAuthConfiguration 的单个实例。</span><span class="sxs-lookup"><span data-stu-id="643b8-236">Only a single instance of certificateBasedAuthConfiguration can be created in the collection.</span></span>  |
|<span data-ttu-id="643b8-237">extensions</span><span class="sxs-lookup"><span data-stu-id="643b8-237">extensions</span></span>|<span data-ttu-id="643b8-238">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="643b8-238">[extension](extension.md) collection</span></span>|<span data-ttu-id="643b8-239">为组织资源定义的开放扩展的集合。</span><span class="sxs-lookup"><span data-stu-id="643b8-239">The collection of open extensions defined for the organization resource.</span></span> <span data-ttu-id="643b8-240">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="643b8-240">Nullable.</span></span>|
|<span data-ttu-id="643b8-241">settings</span><span class="sxs-lookup"><span data-stu-id="643b8-241">settings</span></span>|[<span data-ttu-id="643b8-242">organizationSettings</span><span class="sxs-lookup"><span data-stu-id="643b8-242">organizationSettings</span></span>](organizationsettings.md) | <span data-ttu-id="643b8-243">检索 organizationSettings 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="643b8-243">Retrieve the properties and relationships of organizationSettings object.</span></span> <span data-ttu-id="643b8-244">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="643b8-244">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="643b8-245">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="643b8-245">JSON representation</span></span>

<span data-ttu-id="643b8-246">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="643b8-246">Here is a JSON representation of the resource</span></span>

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
  "directorySizeQuota": {"@odata.type": "microsoft.graph.directorySizeQuota"},
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

## <a name="see-also"></a><span data-ttu-id="643b8-247">另请参阅</span><span class="sxs-lookup"><span data-stu-id="643b8-247">See also</span></span>

- [<span data-ttu-id="643b8-248">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="643b8-248">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="643b8-249">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="643b8-249">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="643b8-250">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="643b8-250">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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


