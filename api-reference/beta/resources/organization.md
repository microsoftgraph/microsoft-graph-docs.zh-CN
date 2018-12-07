---
title: 组织资源类型
description: '代表 Azure Active Directory 租户。 '
ms.openlocfilehash: 053656eb042ca04f2d487d47ee62624875fa4e17
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191142"
---
# <a name="organization-resource-type"></a><span data-ttu-id="461d1-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="461d1-103">organization resource type</span></span>

> <span data-ttu-id="461d1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="461d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="461d1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="461d1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="461d1-106">代表 Azure Active Directory 租户。</span><span class="sxs-lookup"><span data-stu-id="461d1-106">Represents an Azure Active Directory tenant.</span></span> 

<span data-ttu-id="461d1-107">通过该资源可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="461d1-107">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

<span data-ttu-id="461d1-108">在租户; 支持仅读取和更新操作创建并删除不受支持。</span><span class="sxs-lookup"><span data-stu-id="461d1-108">Only the read and update operations are supported on tenants; create and delete are not supported.</span></span> <span data-ttu-id="461d1-109">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="461d1-109">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="461d1-110">方法</span><span class="sxs-lookup"><span data-stu-id="461d1-110">Methods</span></span>

| <span data-ttu-id="461d1-111">方法</span><span class="sxs-lookup"><span data-stu-id="461d1-111">Method</span></span>       | <span data-ttu-id="461d1-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="461d1-112">Return Type</span></span>  |<span data-ttu-id="461d1-113">说明</span><span class="sxs-lookup"><span data-stu-id="461d1-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="461d1-114">获取组织</span><span class="sxs-lookup"><span data-stu-id="461d1-114">Get organization</span></span>](../api/organization-get.md) | [<span data-ttu-id="461d1-115">组织</span><span class="sxs-lookup"><span data-stu-id="461d1-115">organization</span></span>](organization.md) |<span data-ttu-id="461d1-116">读取 organization 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="461d1-116">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="461d1-117">更新</span><span class="sxs-lookup"><span data-stu-id="461d1-117">Update</span></span>](../api/organization-update.md) | [<span data-ttu-id="461d1-118">组织</span><span class="sxs-lookup"><span data-stu-id="461d1-118">organization</span></span>](organization.md)  |<span data-ttu-id="461d1-119">更新 organization 对象。</span><span class="sxs-lookup"><span data-stu-id="461d1-119">Update organization object.</span></span> <span data-ttu-id="461d1-120">可更新的限定属性：**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones** 和 **privacyProfile**。</span><span class="sxs-lookup"><span data-stu-id="461d1-120">The only properties that can be updated are: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** and **privacyProfile**.</span></span> |
|<span data-ttu-id="461d1-121">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="461d1-121">**Open extensions**</span></span>| | |
|[<span data-ttu-id="461d1-122">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="461d1-122">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="461d1-123">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="461d1-123">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="461d1-124">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="461d1-124">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="461d1-125">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="461d1-125">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="461d1-126">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="461d1-126">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="461d1-127">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="461d1-127">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="461d1-128">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="461d1-128">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="461d1-129">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="461d1-129">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="461d1-130">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="461d1-130">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="461d1-131">属性</span><span class="sxs-lookup"><span data-stu-id="461d1-131">Properties</span></span>
| <span data-ttu-id="461d1-132">属性</span><span class="sxs-lookup"><span data-stu-id="461d1-132">Property</span></span>     | <span data-ttu-id="461d1-133">类型</span><span class="sxs-lookup"><span data-stu-id="461d1-133">Type</span></span>   |<span data-ttu-id="461d1-134">说明</span><span class="sxs-lookup"><span data-stu-id="461d1-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="461d1-135">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="461d1-135">assignedPlans</span></span>|<span data-ttu-id="461d1-136">[assignedPlan](assignedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="461d1-136">[assignedPlan](assignedplan.md) collection</span></span>|<span data-ttu-id="461d1-p104">与租户相关的服务计划的集合。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="461d1-p104">The collection of service plans associated with the tenant. Not nullable.</span></span>            |
|<span data-ttu-id="461d1-139">城市</span><span class="sxs-lookup"><span data-stu-id="461d1-139">city</span></span>|<span data-ttu-id="461d1-140">String</span><span class="sxs-lookup"><span data-stu-id="461d1-140">String</span></span>| <span data-ttu-id="461d1-141">组织地址所在的城市名称。</span><span class="sxs-lookup"><span data-stu-id="461d1-141">City name of the address for the organization</span></span> |
|<span data-ttu-id="461d1-142">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="461d1-142">companyLastDirSyncTime</span></span>|<span data-ttu-id="461d1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="461d1-143">DateTimeOffset</span></span>|<span data-ttu-id="461d1-p105">租户最后一次与本地目录同步的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="461d1-p105">The time and date at which the tenant was last synced with the on-premise directory.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="461d1-146">country</span><span class="sxs-lookup"><span data-stu-id="461d1-146">country</span></span>|<span data-ttu-id="461d1-147">字符串</span><span class="sxs-lookup"><span data-stu-id="461d1-147">String</span></span>| <span data-ttu-id="461d1-148">组织地址所在的国家/地区名称。</span><span class="sxs-lookup"><span data-stu-id="461d1-148">Country/region name of the address for the organization</span></span> |
|<span data-ttu-id="461d1-149">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="461d1-149">countryLetterCode</span></span>|<span data-ttu-id="461d1-150">字符串</span><span class="sxs-lookup"><span data-stu-id="461d1-150">String</span></span>| <span data-ttu-id="461d1-151">组织所在的国家/地区缩写</span><span class="sxs-lookup"><span data-stu-id="461d1-151">Country/region abbreviation for the organization</span></span> |
|<span data-ttu-id="461d1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="461d1-152">createdDateTime</span></span>|<span data-ttu-id="461d1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="461d1-153">DateTimeOffset</span></span>| <span data-ttu-id="461d1-154">创建组织时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="461d1-154">Timestamp of when the organization was created.</span></span> <span data-ttu-id="461d1-155">值不能修改和创建组织时将自动填充。</span><span class="sxs-lookup"><span data-stu-id="461d1-155">The value cannot be modified and is automatically populated when the organization is created.</span></span> <span data-ttu-id="461d1-156">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="461d1-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="461d1-157">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="461d1-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="461d1-158">只读。</span><span class="sxs-lookup"><span data-stu-id="461d1-158">Read-only.</span></span> |
|<span data-ttu-id="461d1-159">deletionTimestamp</span><span class="sxs-lookup"><span data-stu-id="461d1-159">deletionTimestamp</span></span>|<span data-ttu-id="461d1-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="461d1-160">DateTimeOffset</span></span>|<span data-ttu-id="461d1-p107">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="461d1-p107">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="461d1-163">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="461d1-163">dirSyncEnabled</span></span>|<span data-ttu-id="461d1-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="461d1-164">Boolean</span></span>|<span data-ttu-id="461d1-165">如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="461d1-165">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="461d1-166">displayName</span><span class="sxs-lookup"><span data-stu-id="461d1-166">displayName</span></span>|<span data-ttu-id="461d1-167">String</span><span class="sxs-lookup"><span data-stu-id="461d1-167">String</span></span>|<span data-ttu-id="461d1-168">租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="461d1-168">The display name for the tenant.</span></span>|
|<span data-ttu-id="461d1-169">id</span><span class="sxs-lookup"><span data-stu-id="461d1-169">id</span></span>|<span data-ttu-id="461d1-170">String</span><span class="sxs-lookup"><span data-stu-id="461d1-170">String</span></span>|<span data-ttu-id="461d1-p108">租户的唯一标识符。继承自 [directoryObject](directoryobject.md)。键。不可为 null。只读。</span><span class="sxs-lookup"><span data-stu-id="461d1-p108">The unique identifier for the tenant. Inherited from [directoryObject](directoryobject.md). Key. Not nullable. Read-only.</span></span>|
|<span data-ttu-id="461d1-176">isMultipleDataLocationsForServicesEnabled</span><span class="sxs-lookup"><span data-stu-id="461d1-176">isMultipleDataLocationsForServicesEnabled</span></span>|<span data-ttu-id="461d1-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="461d1-177">Boolean</span></span>|<span data-ttu-id="461d1-178">**true**如果组织已启用，则多地理位置**false**如果组织不是多地理位置启用则**null**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="461d1-178">**true** if organization is Multi-Geo enabled; **false** if organization is not Multi-Geo enabled; **null** (default).</span></span> <span data-ttu-id="461d1-179">只读。</span><span class="sxs-lookup"><span data-stu-id="461d1-179">Read-only.</span></span> <span data-ttu-id="461d1-180">有关详细信息，请参阅[OneDrive 联机多地理](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)。</span><span class="sxs-lookup"><span data-stu-id="461d1-180">For more information, see [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span>|
|<span data-ttu-id="461d1-181">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="461d1-181">marketingNotificationEmails</span></span>|<span data-ttu-id="461d1-182">String collection</span><span class="sxs-lookup"><span data-stu-id="461d1-182">String collection</span></span>| <span data-ttu-id="461d1-183">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="461d1-183">Not nullable.</span></span>            |
|<span data-ttu-id="461d1-184">objectType</span><span class="sxs-lookup"><span data-stu-id="461d1-184">objectType</span></span>|<span data-ttu-id="461d1-185">String</span><span class="sxs-lookup"><span data-stu-id="461d1-185">String</span></span>|<span data-ttu-id="461d1-p110">一个标识对象类型的字符串。对于租户，该值始终为“Company”。</span><span class="sxs-lookup"><span data-stu-id="461d1-p110">A string that identifies the object type. For tenants the value is always “Company”.</span></span> |
|<span data-ttu-id="461d1-188">postalCode</span><span class="sxs-lookup"><span data-stu-id="461d1-188">postalCode</span></span>|<span data-ttu-id="461d1-189">String</span><span class="sxs-lookup"><span data-stu-id="461d1-189">String</span></span>| <span data-ttu-id="461d1-190">组织地址的邮政编码。</span><span class="sxs-lookup"><span data-stu-id="461d1-190">Postal code of the address for the organization</span></span> |
|<span data-ttu-id="461d1-191">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="461d1-191">preferredLanguage</span></span>|<span data-ttu-id="461d1-192">String</span><span class="sxs-lookup"><span data-stu-id="461d1-192">String</span></span>| <span data-ttu-id="461d1-193">组织的首选语言。</span><span class="sxs-lookup"><span data-stu-id="461d1-193">The preferred language for the organization.</span></span> <span data-ttu-id="461d1-194">应遵循 ISO 639-1 代码；例如“en”。</span><span class="sxs-lookup"><span data-stu-id="461d1-194">Should follow ISO 639-1 Code; for example "en".</span></span> |
|<span data-ttu-id="461d1-195">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="461d1-195">privacyProfile</span></span>|[<span data-ttu-id="461d1-196">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="461d1-196">privacyProfile</span></span>](privacyprofile.md)| <span data-ttu-id="461d1-197">组织的隐私配置文件。</span><span class="sxs-lookup"><span data-stu-id="461d1-197">The privacy profile of an organization.</span></span>            |
|<span data-ttu-id="461d1-198">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="461d1-198">provisionedPlans</span></span>|<span data-ttu-id="461d1-199">[ProvisionedPlan](provisionedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="461d1-199">[ProvisionedPlan](provisionedplan.md) collection</span></span>| <span data-ttu-id="461d1-200">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="461d1-200">Not nullable.</span></span>            |
|<span data-ttu-id="461d1-201">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="461d1-201">provisioningErrors</span></span>|<span data-ttu-id="461d1-202">ProvisioningError 集合</span><span class="sxs-lookup"><span data-stu-id="461d1-202">ProvisioningError collection</span></span>| <span data-ttu-id="461d1-203">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="461d1-203">Not nullable.</span></span>            |
|<span data-ttu-id="461d1-204">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="461d1-204">securityComplianceNotificationMails</span></span>|<span data-ttu-id="461d1-205">String collection</span><span class="sxs-lookup"><span data-stu-id="461d1-205">String collection</span></span>||
|<span data-ttu-id="461d1-206">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="461d1-206">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="461d1-207">String collection</span><span class="sxs-lookup"><span data-stu-id="461d1-207">String collection</span></span>||
|<span data-ttu-id="461d1-208">state</span><span class="sxs-lookup"><span data-stu-id="461d1-208">state</span></span>|<span data-ttu-id="461d1-209">String</span><span class="sxs-lookup"><span data-stu-id="461d1-209">String</span></span>| <span data-ttu-id="461d1-210">组织地址所在的省/自治区/直辖市名称。</span><span class="sxs-lookup"><span data-stu-id="461d1-210">State name of the address for the organization</span></span> |
|<span data-ttu-id="461d1-211">street</span><span class="sxs-lookup"><span data-stu-id="461d1-211">street</span></span>|<span data-ttu-id="461d1-212">String</span><span class="sxs-lookup"><span data-stu-id="461d1-212">String</span></span>| <span data-ttu-id="461d1-213">组织地址所在的街道名称。</span><span class="sxs-lookup"><span data-stu-id="461d1-213">Street name of the address for organization</span></span> |
|<span data-ttu-id="461d1-214">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="461d1-214">technicalNotificationMails</span></span>|<span data-ttu-id="461d1-215">String collection</span><span class="sxs-lookup"><span data-stu-id="461d1-215">String collection</span></span>| <span data-ttu-id="461d1-216">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="461d1-216">Not nullable.</span></span> |
|<span data-ttu-id="461d1-217">telephoneNumber</span><span class="sxs-lookup"><span data-stu-id="461d1-217">telephoneNumber</span></span>|<span data-ttu-id="461d1-218">String</span><span class="sxs-lookup"><span data-stu-id="461d1-218">String</span></span>| <span data-ttu-id="461d1-219">组织的电话号码</span><span class="sxs-lookup"><span data-stu-id="461d1-219">Telephone number for the organization</span></span> |
|<span data-ttu-id="461d1-220">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="461d1-220">verifiedDomains</span></span>|<span data-ttu-id="461d1-221">[VerifiedDomain](verifieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="461d1-221">[VerifiedDomain](verifieddomain.md) collection</span></span>|<span data-ttu-id="461d1-p112">与该租户相关联的域集合。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="461d1-p112">The collection of domains associated with this tenant. Not nullable.</span></span>            |

## <a name="relationships"></a><span data-ttu-id="461d1-224">Relationships</span><span class="sxs-lookup"><span data-stu-id="461d1-224">Relationships</span></span>
<span data-ttu-id="461d1-225">| 扩展 |[扩展](extension.md)集合 |打开扩展名为组织资源定义的集合。</span><span class="sxs-lookup"><span data-stu-id="461d1-225">|extensions|[extension](extension.md) collection|The collection of open extensions defined for the organization resource.</span></span> <span data-ttu-id="461d1-226">可以为 null。 |</span><span class="sxs-lookup"><span data-stu-id="461d1-226">Nullable.|</span></span>

## <a name="json-representation"></a><span data-ttu-id="461d1-227">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="461d1-227">JSON representation</span></span>

<span data-ttu-id="461d1-228">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="461d1-228">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="461d1-229">另请参阅</span><span class="sxs-lookup"><span data-stu-id="461d1-229">See also</span></span>

- [<span data-ttu-id="461d1-230">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="461d1-230">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="461d1-231">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="461d1-231">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="461d1-232">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="461d1-232">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
