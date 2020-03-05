---
title: 组织资源类型
description: '表示 Azure Active Directory 租户。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cb347dcd95b60a0afcbb4704f65f9339db2973e6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522128"
---
# <a name="organization-resource-type"></a><span data-ttu-id="8fb0a-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="8fb0a-103">organization resource type</span></span>

<span data-ttu-id="8fb0a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8fb0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fb0a-105">表示用户或应用程序所登录的 Azure Active Directory 租户。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-105">Represents the Azure Active Directory tenant that the user or application is signed in to.</span></span> <span data-ttu-id="8fb0a-106">只支持在此资源上执行读取和更新操作；不支持创建和删除操作。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-106">Only the read and update operations are supported on this resource; create and delete are not supported.</span></span> <span data-ttu-id="8fb0a-107">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-107">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="8fb0a-108">使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-108">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="8fb0a-109">方法</span><span class="sxs-lookup"><span data-stu-id="8fb0a-109">Methods</span></span>

| <span data-ttu-id="8fb0a-110">方法</span><span class="sxs-lookup"><span data-stu-id="8fb0a-110">Method</span></span>       | <span data-ttu-id="8fb0a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="8fb0a-111">Return Type</span></span>  |<span data-ttu-id="8fb0a-112">说明</span><span class="sxs-lookup"><span data-stu-id="8fb0a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8fb0a-113">获取组织</span><span class="sxs-lookup"><span data-stu-id="8fb0a-113">Get organization</span></span>](../api/organization-get.md) | <span data-ttu-id="8fb0a-114">[organization](organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8fb0a-114">[organization](organization.md) collection</span></span>|<span data-ttu-id="8fb0a-115">读取 organization 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-115">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="8fb0a-116">更新 organization</span><span class="sxs-lookup"><span data-stu-id="8fb0a-116">Update organization</span></span>](../api/organization-update.md) | [<span data-ttu-id="8fb0a-117">组织</span><span class="sxs-lookup"><span data-stu-id="8fb0a-117">organization</span></span>](organization.md)  |<span data-ttu-id="8fb0a-118">更新 organization 对象。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-118">Update organization object.</span></span> <span data-ttu-id="8fb0a-119">可更新的限定属性：**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones** 和 **privacyProfile**。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-119">The only properties that can be updated are: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** and **privacyProfile**.</span></span> |
|<span data-ttu-id="8fb0a-120">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="8fb0a-120">**Open extensions**</span></span>| | |
|[<span data-ttu-id="8fb0a-121">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="8fb0a-121">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="8fb0a-122">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="8fb0a-122">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="8fb0a-123">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-123">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="8fb0a-124">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="8fb0a-124">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="8fb0a-125">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8fb0a-125">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="8fb0a-126">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-126">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="8fb0a-127">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="8fb0a-127">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="8fb0a-128">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="8fb0a-128">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="8fb0a-129">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-129">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="8fb0a-130">属性</span><span class="sxs-lookup"><span data-stu-id="8fb0a-130">Properties</span></span>
| <span data-ttu-id="8fb0a-131">属性</span><span class="sxs-lookup"><span data-stu-id="8fb0a-131">Property</span></span> | <span data-ttu-id="8fb0a-132">类型</span><span class="sxs-lookup"><span data-stu-id="8fb0a-132">Type</span></span>   | <span data-ttu-id="8fb0a-133">说明</span><span class="sxs-lookup"><span data-stu-id="8fb0a-133">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="8fb0a-134">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="8fb0a-134">assignedPlans</span></span> | <span data-ttu-id="8fb0a-135">[assignedPlan](assignedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8fb0a-135">[assignedPlan](assignedplan.md) collection</span></span> | <span data-ttu-id="8fb0a-p103">与租户相关的服务计划的集合。不可为空。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-p103">The collection of service plans associated with the tenant. Not nullable.</span></span> |
| <span data-ttu-id="8fb0a-138">businessPhones</span><span class="sxs-lookup"><span data-stu-id="8fb0a-138">businessPhones</span></span> | <span data-ttu-id="8fb0a-139">字符串集合</span><span class="sxs-lookup"><span data-stu-id="8fb0a-139">String collection</span></span> | <span data-ttu-id="8fb0a-140">组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-140">Telephone number for the organization.</span></span> <span data-ttu-id="8fb0a-141">**注意：** 虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-141">**Note:** Although this is a string collection, only one number can be set for this property.</span></span> |
| <span data-ttu-id="8fb0a-142">城市</span><span class="sxs-lookup"><span data-stu-id="8fb0a-142">city</span></span> | <span data-ttu-id="8fb0a-143">String</span><span class="sxs-lookup"><span data-stu-id="8fb0a-143">String</span></span> | <span data-ttu-id="8fb0a-144">组织地址所在的城市名称。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-144">City name of the address for the organization.</span></span> |
| <span data-ttu-id="8fb0a-145">country</span><span class="sxs-lookup"><span data-stu-id="8fb0a-145">country</span></span> | <span data-ttu-id="8fb0a-146">String</span><span class="sxs-lookup"><span data-stu-id="8fb0a-146">String</span></span> | <span data-ttu-id="8fb0a-147">组织地址所在的国家/地区名称。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-147">Country/region name of the address for the organization.</span></span> |
| <span data-ttu-id="8fb0a-148">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="8fb0a-148">countryLetterCode</span></span> | <span data-ttu-id="8fb0a-149">String</span><span class="sxs-lookup"><span data-stu-id="8fb0a-149">String</span></span> | <span data-ttu-id="8fb0a-150">组织所在的国家/地区缩写。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-150">Country/region abbreviation for the organization.</span></span> |
| <span data-ttu-id="8fb0a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8fb0a-151">createdDateTime</span></span> | <span data-ttu-id="8fb0a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fb0a-152">DateTimeOffset</span></span> | <span data-ttu-id="8fb0a-153">组织的创建时间戳。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-153">Timestamp of when the organization was created.</span></span> <span data-ttu-id="8fb0a-154">值无法修改，并在组织创建时自动填充。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-154">The value cannot be modified and is automatically populated when the organization is created.</span></span> <span data-ttu-id="8fb0a-155">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-155">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8fb0a-156">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="8fb0a-157">只读。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-157">Read-only.</span></span> |
| <span data-ttu-id="8fb0a-158">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fb0a-158">deletedDateTime</span></span> | <span data-ttu-id="8fb0a-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fb0a-159">DateTimeOffset</span></span> | <span data-ttu-id="8fb0a-160">表示采用 ISO 8601 格式创建 Azure AD 的日期和时间，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-160">Represents date and time of when the Azure AD tenant was deleted using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8fb0a-161">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="8fb0a-162">只读。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-162">Read-only.</span></span> |
| <span data-ttu-id="8fb0a-163">displayName</span><span class="sxs-lookup"><span data-stu-id="8fb0a-163">displayName</span></span> | <span data-ttu-id="8fb0a-164">String</span><span class="sxs-lookup"><span data-stu-id="8fb0a-164">String</span></span> | <span data-ttu-id="8fb0a-165">租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-165">The display name for the tenant.</span></span> |
| <span data-ttu-id="8fb0a-166">id</span><span class="sxs-lookup"><span data-stu-id="8fb0a-166">id</span></span> | <span data-ttu-id="8fb0a-167">字符串</span><span class="sxs-lookup"><span data-stu-id="8fb0a-167">String</span></span> | <span data-ttu-id="8fb0a-168">租户 ID，表示组织（或租户）的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-168">The tenant ID, a unique identifier representing the organization (or tenant).</span></span> <span data-ttu-id="8fb0a-169">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-169">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="8fb0a-170">键。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-170">Key.</span></span> <span data-ttu-id="8fb0a-171">不可为空。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-171">Not nullable.</span></span> <span data-ttu-id="8fb0a-172">只读。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-172">Read-only.</span></span> |
| <span data-ttu-id="8fb0a-173">isMultipleDataLocationsForServicesEnabled</span><span class="sxs-lookup"><span data-stu-id="8fb0a-173">isMultipleDataLocationsForServicesEnabled</span></span> | <span data-ttu-id="8fb0a-174">布尔值</span><span class="sxs-lookup"><span data-stu-id="8fb0a-174">Boolean</span></span> | <span data-ttu-id="8fb0a-175">如果组织支持多地理位置，则为 **true**；如果组织不支持多地理位置，则为 **false**；**为空**（默认）。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-175">**true** if organization is Multi-Geo enabled; **false** if organization is not Multi-Geo enabled; **null** (default).</span></span> <span data-ttu-id="8fb0a-176">只读。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-176">Read-only.</span></span> <span data-ttu-id="8fb0a-177">有关详细信息，请参阅 [OneDrive Online 多地理位置](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-177">For more information, see [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span> |
| <span data-ttu-id="8fb0a-178">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="8fb0a-178">marketingNotificationEmails</span></span> | <span data-ttu-id="8fb0a-179">String collection</span><span class="sxs-lookup"><span data-stu-id="8fb0a-179">String collection</span></span> | <span data-ttu-id="8fb0a-180">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-180">Not nullable.</span></span> |
| <span data-ttu-id="8fb0a-181">objectType</span><span class="sxs-lookup"><span data-stu-id="8fb0a-181">objectType</span></span> | <span data-ttu-id="8fb0a-182">String</span><span class="sxs-lookup"><span data-stu-id="8fb0a-182">String</span></span> | <span data-ttu-id="8fb0a-p109">一个标识对象类型的字符串。对于租户，该值始终为“Company”。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-p109">A string that identifies the object type. For tenants the value is always “Company”.</span></span> |
| <span data-ttu-id="8fb0a-185">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8fb0a-185">onPremisesLastSyncDateTime</span></span> | <span data-ttu-id="8fb0a-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fb0a-186">DateTimeOffset</span></span> | <span data-ttu-id="8fb0a-187">租户上次与本地目录同步的时间和日期。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-187">The time and date at which the tenant was last synced with the on-premise directory.</span></span> <span data-ttu-id="8fb0a-188">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-188">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8fb0a-189">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-189">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
| <span data-ttu-id="8fb0a-190">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="8fb0a-190">onPremisesSyncEnabled</span></span> | <span data-ttu-id="8fb0a-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fb0a-191">Boolean</span></span> | <span data-ttu-id="8fb0a-192">如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-192">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span> |
| <span data-ttu-id="8fb0a-193">postalCode</span><span class="sxs-lookup"><span data-stu-id="8fb0a-193">postalCode</span></span> | <span data-ttu-id="8fb0a-194">String</span><span class="sxs-lookup"><span data-stu-id="8fb0a-194">String</span></span> | <span data-ttu-id="8fb0a-195">组织地址的邮政编码。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-195">Postal code of the address for the organization.</span></span> |
| <span data-ttu-id="8fb0a-196">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="8fb0a-196">preferredLanguage</span></span> | <span data-ttu-id="8fb0a-197">String</span><span class="sxs-lookup"><span data-stu-id="8fb0a-197">String</span></span> | <span data-ttu-id="8fb0a-198">组织的首选语言。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-198">The preferred language for the organization.</span></span> <span data-ttu-id="8fb0a-199">应遵循 ISO 639-1 代码；例如“en”。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-199">Should follow ISO 639-1 Code; for example "en".</span></span> |
| <span data-ttu-id="8fb0a-200">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="8fb0a-200">privacyProfile</span></span> | [<span data-ttu-id="8fb0a-201">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="8fb0a-201">privacyProfile</span></span>](privacyprofile.md) | <span data-ttu-id="8fb0a-202">组织的隐私配置文件。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-202">The privacy profile of an organization.</span></span> |
| <span data-ttu-id="8fb0a-203">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="8fb0a-203">provisionedPlans</span></span> | <span data-ttu-id="8fb0a-204">[provisionedPlan](provisionedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8fb0a-204">[provisionedPlan](provisionedplan.md) collection</span></span> | <span data-ttu-id="8fb0a-205">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-205">Not nullable.</span></span> |
| <span data-ttu-id="8fb0a-206">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="8fb0a-206">securityComplianceNotificationMails</span></span> | <span data-ttu-id="8fb0a-207">String collection</span><span class="sxs-lookup"><span data-stu-id="8fb0a-207">String collection</span></span> ||
| <span data-ttu-id="8fb0a-208">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="8fb0a-208">securityComplianceNotificationPhones</span></span> | <span data-ttu-id="8fb0a-209">String collection</span><span class="sxs-lookup"><span data-stu-id="8fb0a-209">String collection</span></span> ||
| <span data-ttu-id="8fb0a-210">state</span><span class="sxs-lookup"><span data-stu-id="8fb0a-210">state</span></span> | <span data-ttu-id="8fb0a-211">String</span><span class="sxs-lookup"><span data-stu-id="8fb0a-211">String</span></span> | <span data-ttu-id="8fb0a-212">组织地址所在的省/自治区/直辖市名称。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-212">State name of the address for the organization.</span></span> |
| <span data-ttu-id="8fb0a-213">street</span><span class="sxs-lookup"><span data-stu-id="8fb0a-213">street</span></span> | <span data-ttu-id="8fb0a-214">String</span><span class="sxs-lookup"><span data-stu-id="8fb0a-214">String</span></span> | <span data-ttu-id="8fb0a-215">组织地址所在的街道名称。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-215">Street name of the address for organization.</span></span> |
| <span data-ttu-id="8fb0a-216">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="8fb0a-216">technicalNotificationMails</span></span> |<span data-ttu-id="8fb0a-217">String 集合</span><span class="sxs-lookup"><span data-stu-id="8fb0a-217">String collection</span></span> | <span data-ttu-id="8fb0a-218">不可为空。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-218">Not nullable.</span></span> |
| <span data-ttu-id="8fb0a-219">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="8fb0a-219">verifiedDomains</span></span> | <span data-ttu-id="8fb0a-220">[verifiedDomain](verifieddomain.md)集合</span><span class="sxs-lookup"><span data-stu-id="8fb0a-220">[verifiedDomain](verifieddomain.md) collection</span></span>|<span data-ttu-id="8fb0a-p112">与该租户相关联的域集合。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-p112">The collection of domains associated with this tenant. Not nullable.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8fb0a-223">关系</span><span class="sxs-lookup"><span data-stu-id="8fb0a-223">Relationships</span></span>

| <span data-ttu-id="8fb0a-224">关系</span><span class="sxs-lookup"><span data-stu-id="8fb0a-224">Relationship</span></span>  | <span data-ttu-id="8fb0a-225">类型</span><span class="sxs-lookup"><span data-stu-id="8fb0a-225">Type</span></span>  |<span data-ttu-id="8fb0a-226">说明</span><span class="sxs-lookup"><span data-stu-id="8fb0a-226">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fb0a-227">certificateBasedAuthConfiguration</span><span class="sxs-lookup"><span data-stu-id="8fb0a-227">certificateBasedAuthConfiguration</span></span>|<span data-ttu-id="8fb0a-228">[certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8fb0a-228">[certificateBasedAuthConfiguration](certificatebasedauthconfiguration.md) collection</span></span>| <span data-ttu-id="8fb0a-229">用于管理基于证书的身份验证配置的导航属性。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-229">Navigation property to manage  certificate-based authentication configuration.</span></span> <span data-ttu-id="8fb0a-230">只能在集合中创建 certificateBasedAuthConfiguration 的单个实例。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-230">Only a single instance of certificateBasedAuthConfiguration can be created in the collection.</span></span>  |
|<span data-ttu-id="8fb0a-231">extensions</span><span class="sxs-lookup"><span data-stu-id="8fb0a-231">extensions</span></span>|<span data-ttu-id="8fb0a-232">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="8fb0a-232">[extension](extension.md) collection</span></span>|<span data-ttu-id="8fb0a-233">为组织资源定义的开放扩展的集合。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-233">The collection of open extensions defined for the organization resource.</span></span> <span data-ttu-id="8fb0a-234">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-234">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8fb0a-235">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8fb0a-235">JSON representation</span></span>

<span data-ttu-id="8fb0a-236">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fb0a-236">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="8fb0a-237">另请参阅</span><span class="sxs-lookup"><span data-stu-id="8fb0a-237">See also</span></span>

- [<span data-ttu-id="8fb0a-238">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="8fb0a-238">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="8fb0a-239">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="8fb0a-239">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="8fb0a-240">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="8fb0a-240">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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
