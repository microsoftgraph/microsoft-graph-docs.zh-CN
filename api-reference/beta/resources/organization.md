---
title: 组织资源类型
description: '代表 Azure Active Directory 租户。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d06ba07c3cee402b88ad5e85e1b0bacc59b9810c
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642140"
---
# <a name="organization-resource-type"></a><span data-ttu-id="0d013-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="0d013-103">organization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d013-104">表示用户或应用程序登录到 Azure Active Directory 租户。</span><span class="sxs-lookup"><span data-stu-id="0d013-104">Represents the Azure Active Directory tenant that the user or application is signed in to.</span></span> <span data-ttu-id="0d013-105">此资源; 支持仅读取和更新操作创建并删除不受支持。</span><span class="sxs-lookup"><span data-stu-id="0d013-105">Only the read and update operations are supported on this resource; create and delete are not supported.</span></span> <span data-ttu-id="0d013-106">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="0d013-106">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="0d013-107">使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="0d013-107">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="0d013-108">方法</span><span class="sxs-lookup"><span data-stu-id="0d013-108">Methods</span></span>

| <span data-ttu-id="0d013-109">方法</span><span class="sxs-lookup"><span data-stu-id="0d013-109">Method</span></span>       | <span data-ttu-id="0d013-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0d013-110">Return Type</span></span>  |<span data-ttu-id="0d013-111">说明</span><span class="sxs-lookup"><span data-stu-id="0d013-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0d013-112">获取组织</span><span class="sxs-lookup"><span data-stu-id="0d013-112">Get organization</span></span>](../api/organization-get.md) | [<span data-ttu-id="0d013-113">组织</span><span class="sxs-lookup"><span data-stu-id="0d013-113">organization</span></span>](organization.md) |<span data-ttu-id="0d013-114">读取 organization 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0d013-114">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="0d013-115">更新</span><span class="sxs-lookup"><span data-stu-id="0d013-115">Update</span></span>](../api/organization-update.md) | [<span data-ttu-id="0d013-116">组织</span><span class="sxs-lookup"><span data-stu-id="0d013-116">organization</span></span>](organization.md)  |<span data-ttu-id="0d013-117">更新 organization 对象。</span><span class="sxs-lookup"><span data-stu-id="0d013-117">Update organization object.</span></span> <span data-ttu-id="0d013-118">可更新的限定属性：**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones** 和 **privacyProfile**。</span><span class="sxs-lookup"><span data-stu-id="0d013-118">The only properties that can be updated are: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** and **privacyProfile**.</span></span> |
|<span data-ttu-id="0d013-119">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="0d013-119">**Open extensions**</span></span>| | |
|[<span data-ttu-id="0d013-120">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="0d013-120">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="0d013-121">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="0d013-121">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="0d013-122">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="0d013-122">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="0d013-123">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="0d013-123">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="0d013-124">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d013-124">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="0d013-125">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="0d013-125">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="0d013-126">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="0d013-126">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="0d013-127">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="0d013-127">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="0d013-128">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="0d013-128">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="0d013-129">属性</span><span class="sxs-lookup"><span data-stu-id="0d013-129">Properties</span></span>
| <span data-ttu-id="0d013-130">属性</span><span class="sxs-lookup"><span data-stu-id="0d013-130">Property</span></span>     | <span data-ttu-id="0d013-131">类型</span><span class="sxs-lookup"><span data-stu-id="0d013-131">Type</span></span>   |<span data-ttu-id="0d013-132">说明</span><span class="sxs-lookup"><span data-stu-id="0d013-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d013-133">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="0d013-133">assignedPlans</span></span>|<span data-ttu-id="0d013-134">[assignedPlan](assignedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d013-134">[assignedPlan](assignedplan.md) collection</span></span>|<span data-ttu-id="0d013-p103">与租户相关的服务计划的集合。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="0d013-p103">The collection of service plans associated with the tenant. Not nullable.</span></span>            |
| <span data-ttu-id="0d013-137">businessPhones</span><span class="sxs-lookup"><span data-stu-id="0d013-137">businessPhones</span></span>                      | <span data-ttu-id="0d013-138">String collection</span><span class="sxs-lookup"><span data-stu-id="0d013-138">String collection</span></span>                                         | <span data-ttu-id="0d013-139">组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="0d013-139">Telephone number for the organization.</span></span> <span data-ttu-id="0d013-140">**注意：** 虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="0d013-140">**Note:** Although this is a string collection, only one number can be set for this property.</span></span>                                                                                            |
|<span data-ttu-id="0d013-141">city</span><span class="sxs-lookup"><span data-stu-id="0d013-141">city</span></span>|<span data-ttu-id="0d013-142">String</span><span class="sxs-lookup"><span data-stu-id="0d013-142">String</span></span>| <span data-ttu-id="0d013-143">组织地址所在的城市名称。</span><span class="sxs-lookup"><span data-stu-id="0d013-143">City name of the address for the organization</span></span> |
|<span data-ttu-id="0d013-144">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="0d013-144">companyLastDirSyncTime</span></span>|<span data-ttu-id="0d013-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d013-145">DateTimeOffset</span></span>|<span data-ttu-id="0d013-p105">租户最后一次与本地目录同步的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0d013-p105">The time and date at which the tenant was last synced with the on-premise directory.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0d013-148">country</span><span class="sxs-lookup"><span data-stu-id="0d013-148">country</span></span>|<span data-ttu-id="0d013-149">字符串</span><span class="sxs-lookup"><span data-stu-id="0d013-149">String</span></span>| <span data-ttu-id="0d013-150">组织地址所在的国家/地区名称。</span><span class="sxs-lookup"><span data-stu-id="0d013-150">Country/region name of the address for the organization</span></span> |
|<span data-ttu-id="0d013-151">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="0d013-151">countryLetterCode</span></span>|<span data-ttu-id="0d013-152">字符串</span><span class="sxs-lookup"><span data-stu-id="0d013-152">String</span></span>| <span data-ttu-id="0d013-153">组织所在的国家/地区缩写</span><span class="sxs-lookup"><span data-stu-id="0d013-153">Country/region abbreviation for the organization</span></span> |
|<span data-ttu-id="0d013-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d013-154">createdDateTime</span></span>|<span data-ttu-id="0d013-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d013-155">DateTimeOffset</span></span>| <span data-ttu-id="0d013-156">创建组织时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="0d013-156">Timestamp of when the organization was created.</span></span> <span data-ttu-id="0d013-157">值不能修改和创建组织时将自动填充。</span><span class="sxs-lookup"><span data-stu-id="0d013-157">The value cannot be modified and is automatically populated when the organization is created.</span></span> <span data-ttu-id="0d013-158">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="0d013-158">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0d013-159">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="0d013-159">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0d013-160">只读。</span><span class="sxs-lookup"><span data-stu-id="0d013-160">Read-only.</span></span> |
| <span data-ttu-id="0d013-161">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d013-161">deletedDateTime</span></span>                    | <span data-ttu-id="0d013-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d013-162">DateTimeOffset</span></span>                                                    | <span data-ttu-id="0d013-163">表示日期和时间的 Azure AD 租户已删除使用 ISO 8601 格式时，始终在 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0d013-163">Represents date and time of when the Azure AD tenant was deleted using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0d013-164">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="0d013-164">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0d013-165">只读。</span><span class="sxs-lookup"><span data-stu-id="0d013-165">Read-only.</span></span>                                                                                     |
|<span data-ttu-id="0d013-166">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="0d013-166">dirSyncEnabled</span></span>|<span data-ttu-id="0d013-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d013-167">Boolean</span></span>|<span data-ttu-id="0d013-168">如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="0d013-168">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="0d013-169">displayName</span><span class="sxs-lookup"><span data-stu-id="0d013-169">displayName</span></span>|<span data-ttu-id="0d013-170">String</span><span class="sxs-lookup"><span data-stu-id="0d013-170">String</span></span>|<span data-ttu-id="0d013-171">租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0d013-171">The display name for the tenant.</span></span>|
|<span data-ttu-id="0d013-172">id</span><span class="sxs-lookup"><span data-stu-id="0d013-172">id</span></span>|<span data-ttu-id="0d013-173">String</span><span class="sxs-lookup"><span data-stu-id="0d013-173">String</span></span>|<span data-ttu-id="0d013-174">租户 ID，代表组织 （或租户） 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0d013-174">The tenant ID, a unique identifier representing the organization (or tenant).</span></span> <span data-ttu-id="0d013-175">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="0d013-175">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="0d013-176">键。</span><span class="sxs-lookup"><span data-stu-id="0d013-176">Key.</span></span> <span data-ttu-id="0d013-177">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="0d013-177">Not nullable.</span></span> <span data-ttu-id="0d013-178">只读。</span><span class="sxs-lookup"><span data-stu-id="0d013-178">Read-only.</span></span>|
|<span data-ttu-id="0d013-179">isMultipleDataLocationsForServicesEnabled</span><span class="sxs-lookup"><span data-stu-id="0d013-179">isMultipleDataLocationsForServicesEnabled</span></span>|<span data-ttu-id="0d013-180">布尔值</span><span class="sxs-lookup"><span data-stu-id="0d013-180">Boolean</span></span>|<span data-ttu-id="0d013-181">**true**如果组织已启用，则多地理位置**false**如果组织不是多地理位置启用则**null**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="0d013-181">**true** if organization is Multi-Geo enabled; **false** if organization is not Multi-Geo enabled; **null** (default).</span></span> <span data-ttu-id="0d013-182">只读。</span><span class="sxs-lookup"><span data-stu-id="0d013-182">Read-only.</span></span> <span data-ttu-id="0d013-183">有关详细信息，请参阅 [OneDrive Online 多地理位置](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)。</span><span class="sxs-lookup"><span data-stu-id="0d013-183">For more information, see [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span>|
|<span data-ttu-id="0d013-184">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="0d013-184">marketingNotificationEmails</span></span>|<span data-ttu-id="0d013-185">String collection</span><span class="sxs-lookup"><span data-stu-id="0d013-185">String collection</span></span>| <span data-ttu-id="0d013-186">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="0d013-186">Not nullable.</span></span>            |
|<span data-ttu-id="0d013-187">objectType</span><span class="sxs-lookup"><span data-stu-id="0d013-187">objectType</span></span>|<span data-ttu-id="0d013-188">String</span><span class="sxs-lookup"><span data-stu-id="0d013-188">String</span></span>|<span data-ttu-id="0d013-p110">一个标识对象类型的字符串。对于租户，该值始终为“Company”。</span><span class="sxs-lookup"><span data-stu-id="0d013-p110">A string that identifies the object type. For tenants the value is always “Company”.</span></span> |
|<span data-ttu-id="0d013-191">postalCode</span><span class="sxs-lookup"><span data-stu-id="0d013-191">postalCode</span></span>|<span data-ttu-id="0d013-192">String</span><span class="sxs-lookup"><span data-stu-id="0d013-192">String</span></span>| <span data-ttu-id="0d013-193">组织地址的邮政编码。</span><span class="sxs-lookup"><span data-stu-id="0d013-193">Postal code of the address for the organization</span></span> |
|<span data-ttu-id="0d013-194">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="0d013-194">preferredLanguage</span></span>|<span data-ttu-id="0d013-195">String</span><span class="sxs-lookup"><span data-stu-id="0d013-195">String</span></span>| <span data-ttu-id="0d013-196">组织的首选语言。</span><span class="sxs-lookup"><span data-stu-id="0d013-196">The preferred language for the organization.</span></span> <span data-ttu-id="0d013-197">应遵循 ISO 639-1 代码；例如“en”。</span><span class="sxs-lookup"><span data-stu-id="0d013-197">Should follow ISO 639-1 Code; for example "en".</span></span> |
|<span data-ttu-id="0d013-198">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="0d013-198">privacyProfile</span></span>|[<span data-ttu-id="0d013-199">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="0d013-199">privacyProfile</span></span>](privacyprofile.md)| <span data-ttu-id="0d013-200">组织的隐私配置文件。</span><span class="sxs-lookup"><span data-stu-id="0d013-200">The privacy profile of an organization.</span></span>            |
|<span data-ttu-id="0d013-201">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="0d013-201">provisionedPlans</span></span>|<span data-ttu-id="0d013-202">[ProvisionedPlan](provisionedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d013-202">[ProvisionedPlan](provisionedplan.md) collection</span></span>| <span data-ttu-id="0d013-203">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="0d013-203">Not nullable.</span></span>            |
|<span data-ttu-id="0d013-204">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="0d013-204">provisioningErrors</span></span>|<span data-ttu-id="0d013-205">ProvisioningError 集合</span><span class="sxs-lookup"><span data-stu-id="0d013-205">ProvisioningError collection</span></span>| <span data-ttu-id="0d013-206">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="0d013-206">Not nullable.</span></span>            |
|<span data-ttu-id="0d013-207">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="0d013-207">securityComplianceNotificationMails</span></span>|<span data-ttu-id="0d013-208">String collection</span><span class="sxs-lookup"><span data-stu-id="0d013-208">String collection</span></span>||
|<span data-ttu-id="0d013-209">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="0d013-209">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="0d013-210">String collection</span><span class="sxs-lookup"><span data-stu-id="0d013-210">String collection</span></span>||
|<span data-ttu-id="0d013-211">state</span><span class="sxs-lookup"><span data-stu-id="0d013-211">state</span></span>|<span data-ttu-id="0d013-212">String</span><span class="sxs-lookup"><span data-stu-id="0d013-212">String</span></span>| <span data-ttu-id="0d013-213">组织地址所在的省/自治区/直辖市名称。</span><span class="sxs-lookup"><span data-stu-id="0d013-213">State name of the address for the organization</span></span> |
|<span data-ttu-id="0d013-214">street</span><span class="sxs-lookup"><span data-stu-id="0d013-214">street</span></span>|<span data-ttu-id="0d013-215">String</span><span class="sxs-lookup"><span data-stu-id="0d013-215">String</span></span>| <span data-ttu-id="0d013-216">组织地址所在的街道名称。</span><span class="sxs-lookup"><span data-stu-id="0d013-216">Street name of the address for organization</span></span> |
|<span data-ttu-id="0d013-217">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="0d013-217">technicalNotificationMails</span></span>|<span data-ttu-id="0d013-218">String collection</span><span class="sxs-lookup"><span data-stu-id="0d013-218">String collection</span></span>| <span data-ttu-id="0d013-219">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="0d013-219">Not nullable.</span></span> |
|<span data-ttu-id="0d013-220">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="0d013-220">verifiedDomains</span></span>|<span data-ttu-id="0d013-221">[VerifiedDomain](verifieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0d013-221">[VerifiedDomain](verifieddomain.md) collection</span></span>|<span data-ttu-id="0d013-p112">与该租户相关联的域集合。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="0d013-p112">The collection of domains associated with this tenant. Not nullable.</span></span>            |

## <a name="relationships"></a><span data-ttu-id="0d013-224">关系</span><span class="sxs-lookup"><span data-stu-id="0d013-224">Relationships</span></span>

| <span data-ttu-id="0d013-225">关系</span><span class="sxs-lookup"><span data-stu-id="0d013-225">Relationship</span></span>     | <span data-ttu-id="0d013-226">类型</span><span class="sxs-lookup"><span data-stu-id="0d013-226">Type</span></span>   |<span data-ttu-id="0d013-227">说明</span><span class="sxs-lookup"><span data-stu-id="0d013-227">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d013-228">extensions</span><span class="sxs-lookup"><span data-stu-id="0d013-228">extensions</span></span>|<span data-ttu-id="0d013-229">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="0d013-229">[extension](extension.md) collection</span></span>|<span data-ttu-id="0d013-230">打开扩展名为组织资源定义的集合。</span><span class="sxs-lookup"><span data-stu-id="0d013-230">The collection of open extensions defined for the organization resource.</span></span> <span data-ttu-id="0d013-231">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="0d013-231">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d013-232">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d013-232">JSON representation</span></span>

<span data-ttu-id="0d013-233">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d013-233">Here is a JSON representation of the resource</span></span>

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
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}]
}
```

## <a name="see-also"></a><span data-ttu-id="0d013-234">另请参阅</span><span class="sxs-lookup"><span data-stu-id="0d013-234">See also</span></span>

- [<span data-ttu-id="0d013-235">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="0d013-235">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="0d013-236">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="0d013-236">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="0d013-237">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="0d013-237">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/organization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
