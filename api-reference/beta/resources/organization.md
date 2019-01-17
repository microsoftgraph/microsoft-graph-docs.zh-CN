---
title: 组织资源类型
description: '代表 Azure Active Directory 租户。 '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 86263fe11ebf3bb25e17cbd2b950195fa122f778
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927448"
---
# <a name="organization-resource-type"></a><span data-ttu-id="de8fb-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="de8fb-103">organization resource type</span></span>

> <span data-ttu-id="de8fb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="de8fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de8fb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="de8fb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de8fb-106">表示用户或应用程序登录到 Azure Active Directory 租户。</span><span class="sxs-lookup"><span data-stu-id="de8fb-106">Represents the Azure Active Directory tenant that the user or application is signed in to.</span></span> <span data-ttu-id="de8fb-107">此资源; 支持仅读取和更新操作创建并删除不受支持。</span><span class="sxs-lookup"><span data-stu-id="de8fb-107">Only the read and update operations are supported on this resource; create and delete are not supported.</span></span> <span data-ttu-id="de8fb-108">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="de8fb-108">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="de8fb-109">使用此资源，可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="de8fb-109">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

## <a name="methods"></a><span data-ttu-id="de8fb-110">方法</span><span class="sxs-lookup"><span data-stu-id="de8fb-110">Methods</span></span>

| <span data-ttu-id="de8fb-111">方法</span><span class="sxs-lookup"><span data-stu-id="de8fb-111">Method</span></span>       | <span data-ttu-id="de8fb-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="de8fb-112">Return Type</span></span>  |<span data-ttu-id="de8fb-113">说明</span><span class="sxs-lookup"><span data-stu-id="de8fb-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="de8fb-114">获取组织</span><span class="sxs-lookup"><span data-stu-id="de8fb-114">Get organization</span></span>](../api/organization-get.md) | [<span data-ttu-id="de8fb-115">组织</span><span class="sxs-lookup"><span data-stu-id="de8fb-115">organization</span></span>](organization.md) |<span data-ttu-id="de8fb-116">读取 organization 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="de8fb-116">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="de8fb-117">更新</span><span class="sxs-lookup"><span data-stu-id="de8fb-117">Update</span></span>](../api/organization-update.md) | [<span data-ttu-id="de8fb-118">组织</span><span class="sxs-lookup"><span data-stu-id="de8fb-118">organization</span></span>](organization.md)  |<span data-ttu-id="de8fb-119">更新 organization 对象。</span><span class="sxs-lookup"><span data-stu-id="de8fb-119">Update organization object.</span></span> <span data-ttu-id="de8fb-120">可更新的限定属性：**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones** 和 **privacyProfile**。</span><span class="sxs-lookup"><span data-stu-id="de8fb-120">The only properties that can be updated are: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** and **privacyProfile**.</span></span> |
|<span data-ttu-id="de8fb-121">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="de8fb-121">**Open extensions**</span></span>| | |
|[<span data-ttu-id="de8fb-122">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="de8fb-122">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="de8fb-123">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="de8fb-123">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="de8fb-124">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="de8fb-124">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="de8fb-125">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="de8fb-125">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="de8fb-126">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de8fb-126">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="de8fb-127">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="de8fb-127">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="de8fb-128">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="de8fb-128">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="de8fb-129">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="de8fb-129">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="de8fb-130">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="de8fb-130">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="de8fb-131">属性</span><span class="sxs-lookup"><span data-stu-id="de8fb-131">Properties</span></span>
| <span data-ttu-id="de8fb-132">属性</span><span class="sxs-lookup"><span data-stu-id="de8fb-132">Property</span></span>     | <span data-ttu-id="de8fb-133">类型</span><span class="sxs-lookup"><span data-stu-id="de8fb-133">Type</span></span>   |<span data-ttu-id="de8fb-134">说明</span><span class="sxs-lookup"><span data-stu-id="de8fb-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de8fb-135">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="de8fb-135">assignedPlans</span></span>|<span data-ttu-id="de8fb-136">[assignedPlan](assignedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de8fb-136">[assignedPlan](assignedplan.md) collection</span></span>|<span data-ttu-id="de8fb-p104">与租户相关的服务计划的集合。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="de8fb-p104">The collection of service plans associated with the tenant. Not nullable.</span></span>            |
| <span data-ttu-id="de8fb-139">businessPhones</span><span class="sxs-lookup"><span data-stu-id="de8fb-139">businessPhones</span></span>                      | <span data-ttu-id="de8fb-140">String collection</span><span class="sxs-lookup"><span data-stu-id="de8fb-140">String collection</span></span>                                         | <span data-ttu-id="de8fb-141">组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="de8fb-141">Telephone number for the organization.</span></span> <span data-ttu-id="de8fb-142">**注意：** 虽然这是字符串集合，但是只能为该属性设置一个号码。</span><span class="sxs-lookup"><span data-stu-id="de8fb-142">**Note:** Although this is a string collection, only one number can be set for this property.</span></span>                                                                                            |
|<span data-ttu-id="de8fb-143">城市</span><span class="sxs-lookup"><span data-stu-id="de8fb-143">city</span></span>|<span data-ttu-id="de8fb-144">String</span><span class="sxs-lookup"><span data-stu-id="de8fb-144">String</span></span>| <span data-ttu-id="de8fb-145">组织地址所在的城市名称。</span><span class="sxs-lookup"><span data-stu-id="de8fb-145">City name of the address for the organization</span></span> |
|<span data-ttu-id="de8fb-146">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="de8fb-146">companyLastDirSyncTime</span></span>|<span data-ttu-id="de8fb-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de8fb-147">DateTimeOffset</span></span>|<span data-ttu-id="de8fb-p106">租户最后一次与本地目录同步的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="de8fb-p106">The time and date at which the tenant was last synced with the on-premise directory.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="de8fb-150">country</span><span class="sxs-lookup"><span data-stu-id="de8fb-150">country</span></span>|<span data-ttu-id="de8fb-151">字符串</span><span class="sxs-lookup"><span data-stu-id="de8fb-151">String</span></span>| <span data-ttu-id="de8fb-152">组织地址所在的国家/地区名称。</span><span class="sxs-lookup"><span data-stu-id="de8fb-152">Country/region name of the address for the organization</span></span> |
|<span data-ttu-id="de8fb-153">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="de8fb-153">countryLetterCode</span></span>|<span data-ttu-id="de8fb-154">字符串</span><span class="sxs-lookup"><span data-stu-id="de8fb-154">String</span></span>| <span data-ttu-id="de8fb-155">组织所在的国家/地区缩写</span><span class="sxs-lookup"><span data-stu-id="de8fb-155">Country/region abbreviation for the organization</span></span> |
|<span data-ttu-id="de8fb-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de8fb-156">createdDateTime</span></span>|<span data-ttu-id="de8fb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de8fb-157">DateTimeOffset</span></span>| <span data-ttu-id="de8fb-158">创建组织时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="de8fb-158">Timestamp of when the organization was created.</span></span> <span data-ttu-id="de8fb-159">值不能修改和创建组织时将自动填充。</span><span class="sxs-lookup"><span data-stu-id="de8fb-159">The value cannot be modified and is automatically populated when the organization is created.</span></span> <span data-ttu-id="de8fb-160">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="de8fb-160">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="de8fb-161">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="de8fb-161">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="de8fb-162">只读。</span><span class="sxs-lookup"><span data-stu-id="de8fb-162">Read-only.</span></span> |
| <span data-ttu-id="de8fb-163">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="de8fb-163">deletedDateTime</span></span>                    | <span data-ttu-id="de8fb-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de8fb-164">DateTimeOffset</span></span>                                                    | <span data-ttu-id="de8fb-165">表示日期和时间的 Azure AD 租户已删除使用 ISO 8601 格式时，始终在 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="de8fb-165">Represents date and time of when the Azure AD tenant was deleted using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="de8fb-166">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="de8fb-166">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="de8fb-167">只读。</span><span class="sxs-lookup"><span data-stu-id="de8fb-167">Read-only.</span></span>                                                                                     |
|<span data-ttu-id="de8fb-168">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="de8fb-168">dirSyncEnabled</span></span>|<span data-ttu-id="de8fb-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="de8fb-169">Boolean</span></span>|<span data-ttu-id="de8fb-170">如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="de8fb-170">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="de8fb-171">displayName</span><span class="sxs-lookup"><span data-stu-id="de8fb-171">displayName</span></span>|<span data-ttu-id="de8fb-172">String</span><span class="sxs-lookup"><span data-stu-id="de8fb-172">String</span></span>|<span data-ttu-id="de8fb-173">租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="de8fb-173">The display name for the tenant.</span></span>|
|<span data-ttu-id="de8fb-174">id</span><span class="sxs-lookup"><span data-stu-id="de8fb-174">id</span></span>|<span data-ttu-id="de8fb-175">字符串</span><span class="sxs-lookup"><span data-stu-id="de8fb-175">String</span></span>|<span data-ttu-id="de8fb-176">租户 ID，代表组织 （或租户） 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="de8fb-176">The tenant ID, a unique identifier representing the organization (or tenant).</span></span> <span data-ttu-id="de8fb-177">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="de8fb-177">Inherited from [directoryObject](directoryobject.md).</span></span> <span data-ttu-id="de8fb-178">键。</span><span class="sxs-lookup"><span data-stu-id="de8fb-178">Key.</span></span> <span data-ttu-id="de8fb-179">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="de8fb-179">Not nullable.</span></span> <span data-ttu-id="de8fb-180">只读。</span><span class="sxs-lookup"><span data-stu-id="de8fb-180">Read-only.</span></span>|
|<span data-ttu-id="de8fb-181">isMultipleDataLocationsForServicesEnabled</span><span class="sxs-lookup"><span data-stu-id="de8fb-181">isMultipleDataLocationsForServicesEnabled</span></span>|<span data-ttu-id="de8fb-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="de8fb-182">Boolean</span></span>|<span data-ttu-id="de8fb-183">**true**如果组织已启用，则多地理位置**false**如果组织不是多地理位置启用则**null**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="de8fb-183">**true** if organization is Multi-Geo enabled; **false** if organization is not Multi-Geo enabled; **null** (default).</span></span> <span data-ttu-id="de8fb-184">只读。</span><span class="sxs-lookup"><span data-stu-id="de8fb-184">Read-only.</span></span> <span data-ttu-id="de8fb-185">有关详细信息，请参阅[OneDrive 联机多地理](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)。</span><span class="sxs-lookup"><span data-stu-id="de8fb-185">For more information, see [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span>|
|<span data-ttu-id="de8fb-186">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="de8fb-186">marketingNotificationEmails</span></span>|<span data-ttu-id="de8fb-187">String collection</span><span class="sxs-lookup"><span data-stu-id="de8fb-187">String collection</span></span>| <span data-ttu-id="de8fb-188">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="de8fb-188">Not nullable.</span></span>            |
|<span data-ttu-id="de8fb-189">objectType</span><span class="sxs-lookup"><span data-stu-id="de8fb-189">objectType</span></span>|<span data-ttu-id="de8fb-190">String</span><span class="sxs-lookup"><span data-stu-id="de8fb-190">String</span></span>|<span data-ttu-id="de8fb-p111">一个标识对象类型的字符串。对于租户，该值始终为“Company”。</span><span class="sxs-lookup"><span data-stu-id="de8fb-p111">A string that identifies the object type. For tenants the value is always “Company”.</span></span> |
|<span data-ttu-id="de8fb-193">postalCode</span><span class="sxs-lookup"><span data-stu-id="de8fb-193">postalCode</span></span>|<span data-ttu-id="de8fb-194">String</span><span class="sxs-lookup"><span data-stu-id="de8fb-194">String</span></span>| <span data-ttu-id="de8fb-195">组织地址的邮政编码。</span><span class="sxs-lookup"><span data-stu-id="de8fb-195">Postal code of the address for the organization</span></span> |
|<span data-ttu-id="de8fb-196">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="de8fb-196">preferredLanguage</span></span>|<span data-ttu-id="de8fb-197">String</span><span class="sxs-lookup"><span data-stu-id="de8fb-197">String</span></span>| <span data-ttu-id="de8fb-198">组织的首选语言。</span><span class="sxs-lookup"><span data-stu-id="de8fb-198">The preferred language for the organization.</span></span> <span data-ttu-id="de8fb-199">应遵循 ISO 639-1 代码；例如“en”。</span><span class="sxs-lookup"><span data-stu-id="de8fb-199">Should follow ISO 639-1 Code; for example "en".</span></span> |
|<span data-ttu-id="de8fb-200">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="de8fb-200">privacyProfile</span></span>|[<span data-ttu-id="de8fb-201">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="de8fb-201">privacyProfile</span></span>](privacyprofile.md)| <span data-ttu-id="de8fb-202">组织的隐私配置文件。</span><span class="sxs-lookup"><span data-stu-id="de8fb-202">The privacy profile of an organization.</span></span>            |
|<span data-ttu-id="de8fb-203">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="de8fb-203">provisionedPlans</span></span>|<span data-ttu-id="de8fb-204">[ProvisionedPlan](provisionedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de8fb-204">[ProvisionedPlan](provisionedplan.md) collection</span></span>| <span data-ttu-id="de8fb-205">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="de8fb-205">Not nullable.</span></span>            |
|<span data-ttu-id="de8fb-206">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="de8fb-206">provisioningErrors</span></span>|<span data-ttu-id="de8fb-207">ProvisioningError 集合</span><span class="sxs-lookup"><span data-stu-id="de8fb-207">ProvisioningError collection</span></span>| <span data-ttu-id="de8fb-208">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="de8fb-208">Not nullable.</span></span>            |
|<span data-ttu-id="de8fb-209">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="de8fb-209">securityComplianceNotificationMails</span></span>|<span data-ttu-id="de8fb-210">String collection</span><span class="sxs-lookup"><span data-stu-id="de8fb-210">String collection</span></span>||
|<span data-ttu-id="de8fb-211">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="de8fb-211">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="de8fb-212">String collection</span><span class="sxs-lookup"><span data-stu-id="de8fb-212">String collection</span></span>||
|<span data-ttu-id="de8fb-213">state</span><span class="sxs-lookup"><span data-stu-id="de8fb-213">state</span></span>|<span data-ttu-id="de8fb-214">String</span><span class="sxs-lookup"><span data-stu-id="de8fb-214">String</span></span>| <span data-ttu-id="de8fb-215">组织地址所在的省/自治区/直辖市名称。</span><span class="sxs-lookup"><span data-stu-id="de8fb-215">State name of the address for the organization</span></span> |
|<span data-ttu-id="de8fb-216">street</span><span class="sxs-lookup"><span data-stu-id="de8fb-216">street</span></span>|<span data-ttu-id="de8fb-217">String</span><span class="sxs-lookup"><span data-stu-id="de8fb-217">String</span></span>| <span data-ttu-id="de8fb-218">组织地址所在的街道名称。</span><span class="sxs-lookup"><span data-stu-id="de8fb-218">Street name of the address for organization</span></span> |
|<span data-ttu-id="de8fb-219">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="de8fb-219">technicalNotificationMails</span></span>|<span data-ttu-id="de8fb-220">String collection</span><span class="sxs-lookup"><span data-stu-id="de8fb-220">String collection</span></span>| <span data-ttu-id="de8fb-221">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="de8fb-221">Not nullable.</span></span> |
|<span data-ttu-id="de8fb-222">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="de8fb-222">verifiedDomains</span></span>|<span data-ttu-id="de8fb-223">[VerifiedDomain](verifieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="de8fb-223">[VerifiedDomain](verifieddomain.md) collection</span></span>|<span data-ttu-id="de8fb-p113">与该租户相关联的域集合。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="de8fb-p113">The collection of domains associated with this tenant. Not nullable.</span></span>            |

## <a name="relationships"></a><span data-ttu-id="de8fb-226">Relationships</span><span class="sxs-lookup"><span data-stu-id="de8fb-226">Relationships</span></span>

| <span data-ttu-id="de8fb-227">关系</span><span class="sxs-lookup"><span data-stu-id="de8fb-227">Relationship</span></span>     | <span data-ttu-id="de8fb-228">类型</span><span class="sxs-lookup"><span data-stu-id="de8fb-228">Type</span></span>   |<span data-ttu-id="de8fb-229">说明</span><span class="sxs-lookup"><span data-stu-id="de8fb-229">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de8fb-230">extensions</span><span class="sxs-lookup"><span data-stu-id="de8fb-230">extensions</span></span>|<span data-ttu-id="de8fb-231">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="de8fb-231">[extension](extension.md) collection</span></span>|<span data-ttu-id="de8fb-232">打开扩展名为组织资源定义的集合。</span><span class="sxs-lookup"><span data-stu-id="de8fb-232">The collection of open extensions defined for the organization resource.</span></span> <span data-ttu-id="de8fb-233">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="de8fb-233">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de8fb-234">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de8fb-234">JSON representation</span></span>

<span data-ttu-id="de8fb-235">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de8fb-235">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="de8fb-236">另请参阅</span><span class="sxs-lookup"><span data-stu-id="de8fb-236">See also</span></span>

- [<span data-ttu-id="de8fb-237">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="de8fb-237">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="de8fb-238">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="de8fb-238">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="de8fb-239">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="de8fb-239">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
