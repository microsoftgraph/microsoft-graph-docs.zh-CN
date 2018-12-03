---
title: 组织资源类型
description: '代表 Azure Active Directory 租户。 '
ms.openlocfilehash: 0dc7b55053ba70272c4e639dba4b62160f58f435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044142"
---
# <a name="organization-resource-type"></a><span data-ttu-id="fba8f-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="fba8f-103">organization resource type</span></span>

> <span data-ttu-id="fba8f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fba8f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fba8f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fba8f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fba8f-106">代表 Azure Active Directory 租户。</span><span class="sxs-lookup"><span data-stu-id="fba8f-106">Represents an Azure Active Directory tenant.</span></span> 

<span data-ttu-id="fba8f-107">通过该资源可以使用[扩展](/graph/extensibility-overview)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="fba8f-107">This resource lets you add your own data to custom properties using [extensions](/graph/extensibility-overview).</span></span>

<span data-ttu-id="fba8f-108">在租户; 支持仅读取和更新操作创建并删除不受支持。</span><span class="sxs-lookup"><span data-stu-id="fba8f-108">Only the read and update operations are supported on tenants; create and delete are not supported.</span></span> <span data-ttu-id="fba8f-109">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="fba8f-109">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="fba8f-110">方法</span><span class="sxs-lookup"><span data-stu-id="fba8f-110">Methods</span></span>

| <span data-ttu-id="fba8f-111">方法</span><span class="sxs-lookup"><span data-stu-id="fba8f-111">Method</span></span>       | <span data-ttu-id="fba8f-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="fba8f-112">Return Type</span></span>  |<span data-ttu-id="fba8f-113">说明</span><span class="sxs-lookup"><span data-stu-id="fba8f-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fba8f-114">获取组织</span><span class="sxs-lookup"><span data-stu-id="fba8f-114">Get organization</span></span>](../api/organization-get.md) | [<span data-ttu-id="fba8f-115">组织</span><span class="sxs-lookup"><span data-stu-id="fba8f-115">organization</span></span>](organization.md) |<span data-ttu-id="fba8f-116">读取 organization 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fba8f-116">Read properties and relationships of organization object.</span></span>|
|[<span data-ttu-id="fba8f-117">更新</span><span class="sxs-lookup"><span data-stu-id="fba8f-117">Update</span></span>](../api/organization-update.md) | [<span data-ttu-id="fba8f-118">组织</span><span class="sxs-lookup"><span data-stu-id="fba8f-118">organization</span></span>](organization.md)  |<span data-ttu-id="fba8f-119">更新 organization 对象。</span><span class="sxs-lookup"><span data-stu-id="fba8f-119">Update organization object.</span></span> <span data-ttu-id="fba8f-120">可更新的限定属性：**marketingNotificationMails**、**technicalNotificationMails**、**securityComplianceNotificationMails**、**securityComplianceNotificationPhones** 和 **privacyProfile**。</span><span class="sxs-lookup"><span data-stu-id="fba8f-120">The only properties that can be updated are: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** and **privacyProfile**.</span></span> |
|<span data-ttu-id="fba8f-121">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="fba8f-121">**Open extensions**</span></span>| | |
|[<span data-ttu-id="fba8f-122">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="fba8f-122">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="fba8f-123">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="fba8f-123">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="fba8f-124">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="fba8f-124">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="fba8f-125">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="fba8f-125">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="fba8f-126">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fba8f-126">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="fba8f-127">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="fba8f-127">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="fba8f-128">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="fba8f-128">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="fba8f-129">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="fba8f-129">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="fba8f-130">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="fba8f-130">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|

## <a name="properties"></a><span data-ttu-id="fba8f-131">属性</span><span class="sxs-lookup"><span data-stu-id="fba8f-131">Properties</span></span>
| <span data-ttu-id="fba8f-132">属性</span><span class="sxs-lookup"><span data-stu-id="fba8f-132">Property</span></span>     | <span data-ttu-id="fba8f-133">类型</span><span class="sxs-lookup"><span data-stu-id="fba8f-133">Type</span></span>   |<span data-ttu-id="fba8f-134">说明</span><span class="sxs-lookup"><span data-stu-id="fba8f-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fba8f-135">assignedPlans</span><span class="sxs-lookup"><span data-stu-id="fba8f-135">assignedPlans</span></span>|<span data-ttu-id="fba8f-136">[assignedPlan](assignedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fba8f-136">[assignedPlan](assignedplan.md) collection</span></span>|<span data-ttu-id="fba8f-p104">与租户相关的服务计划的集合。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="fba8f-p104">The collection of service plans associated with the tenant. Not nullable.</span></span>            |
|<span data-ttu-id="fba8f-139">城市</span><span class="sxs-lookup"><span data-stu-id="fba8f-139">city</span></span>|<span data-ttu-id="fba8f-140">String</span><span class="sxs-lookup"><span data-stu-id="fba8f-140">String</span></span>| <span data-ttu-id="fba8f-141">组织地址所在的城市名称。</span><span class="sxs-lookup"><span data-stu-id="fba8f-141">City name of the address for the organization</span></span> |
|<span data-ttu-id="fba8f-142">companyLastDirSyncTime</span><span class="sxs-lookup"><span data-stu-id="fba8f-142">companyLastDirSyncTime</span></span>|<span data-ttu-id="fba8f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fba8f-143">DateTimeOffset</span></span>|<span data-ttu-id="fba8f-p105">租户最后一次与本地目录同步的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fba8f-p105">The time and date at which the tenant was last synced with the on-premise directory.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fba8f-146">country</span><span class="sxs-lookup"><span data-stu-id="fba8f-146">country</span></span>|<span data-ttu-id="fba8f-147">字符串</span><span class="sxs-lookup"><span data-stu-id="fba8f-147">String</span></span>| <span data-ttu-id="fba8f-148">组织地址所在的国家/地区名称。</span><span class="sxs-lookup"><span data-stu-id="fba8f-148">Country/region name of the address for the organization</span></span> |
|<span data-ttu-id="fba8f-149">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="fba8f-149">countryLetterCode</span></span>|<span data-ttu-id="fba8f-150">字符串</span><span class="sxs-lookup"><span data-stu-id="fba8f-150">String</span></span>| <span data-ttu-id="fba8f-151">组织所在的国家/地区缩写</span><span class="sxs-lookup"><span data-stu-id="fba8f-151">Country/region abbreviation for the organization</span></span> |
|<span data-ttu-id="fba8f-152">deletionTimestamp</span><span class="sxs-lookup"><span data-stu-id="fba8f-152">deletionTimestamp</span></span>|<span data-ttu-id="fba8f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fba8f-153">DateTimeOffset</span></span>|<span data-ttu-id="fba8f-p106">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fba8f-p106">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="fba8f-156">dirSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="fba8f-156">dirSyncEnabled</span></span>|<span data-ttu-id="fba8f-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="fba8f-157">Boolean</span></span>|<span data-ttu-id="fba8f-158">如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="fba8f-158">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="fba8f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="fba8f-159">displayName</span></span>|<span data-ttu-id="fba8f-160">String</span><span class="sxs-lookup"><span data-stu-id="fba8f-160">String</span></span>|<span data-ttu-id="fba8f-161">租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fba8f-161">The display name for the tenant.</span></span>|
|<span data-ttu-id="fba8f-162">id</span><span class="sxs-lookup"><span data-stu-id="fba8f-162">id</span></span>|<span data-ttu-id="fba8f-163">String</span><span class="sxs-lookup"><span data-stu-id="fba8f-163">String</span></span>|<span data-ttu-id="fba8f-p107">租户的唯一标识符。继承自 [directoryObject](directoryobject.md)。键。不可为 null。只读。</span><span class="sxs-lookup"><span data-stu-id="fba8f-p107">The unique identifier for the tenant. Inherited from [directoryObject](directoryobject.md). Key. Not nullable. Read-only.</span></span>|
|<span data-ttu-id="fba8f-169">isMultipleDataLocationsForServicesEnabled</span><span class="sxs-lookup"><span data-stu-id="fba8f-169">isMultipleDataLocationsForServicesEnabled</span></span>|<span data-ttu-id="fba8f-170">布尔值</span><span class="sxs-lookup"><span data-stu-id="fba8f-170">Boolean</span></span>|<span data-ttu-id="fba8f-171">**true**如果组织已启用，则多地理位置**false**如果组织不是多地理位置启用则**null**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="fba8f-171">**true** if organization is Multi-Geo enabled; **false** if organization is not Multi-Geo enabled; **null** (default).</span></span> <span data-ttu-id="fba8f-172">只读。</span><span class="sxs-lookup"><span data-stu-id="fba8f-172">Read-only.</span></span> <span data-ttu-id="fba8f-173">有关详细信息，请参阅[OneDrive 联机多地理](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)。</span><span class="sxs-lookup"><span data-stu-id="fba8f-173">For more information, see [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).</span></span>|
|<span data-ttu-id="fba8f-174">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="fba8f-174">marketingNotificationEmails</span></span>|<span data-ttu-id="fba8f-175">String collection</span><span class="sxs-lookup"><span data-stu-id="fba8f-175">String collection</span></span>| <span data-ttu-id="fba8f-176">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="fba8f-176">Not nullable.</span></span>            |
|<span data-ttu-id="fba8f-177">objectType</span><span class="sxs-lookup"><span data-stu-id="fba8f-177">objectType</span></span>|<span data-ttu-id="fba8f-178">String</span><span class="sxs-lookup"><span data-stu-id="fba8f-178">String</span></span>|<span data-ttu-id="fba8f-p109">一个标识对象类型的字符串。对于租户，该值始终为“Company”。</span><span class="sxs-lookup"><span data-stu-id="fba8f-p109">A string that identifies the object type. For tenants the value is always “Company”.</span></span> |
|<span data-ttu-id="fba8f-181">postalCode</span><span class="sxs-lookup"><span data-stu-id="fba8f-181">postalCode</span></span>|<span data-ttu-id="fba8f-182">String</span><span class="sxs-lookup"><span data-stu-id="fba8f-182">String</span></span>| <span data-ttu-id="fba8f-183">组织地址的邮政编码。</span><span class="sxs-lookup"><span data-stu-id="fba8f-183">Postal code of the address for the organization</span></span> |
|<span data-ttu-id="fba8f-184">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="fba8f-184">preferredLanguage</span></span>|<span data-ttu-id="fba8f-185">String</span><span class="sxs-lookup"><span data-stu-id="fba8f-185">String</span></span>| <span data-ttu-id="fba8f-186">组织的首选语言。</span><span class="sxs-lookup"><span data-stu-id="fba8f-186">The preferred language for the organization.</span></span> <span data-ttu-id="fba8f-187">应遵循 ISO 639-1 代码；例如“en”。</span><span class="sxs-lookup"><span data-stu-id="fba8f-187">Should follow ISO 639-1 Code; for example "en".</span></span> |
|<span data-ttu-id="fba8f-188">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="fba8f-188">privacyProfile</span></span>|[<span data-ttu-id="fba8f-189">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="fba8f-189">privacyProfile</span></span>](privacyprofile.md)| <span data-ttu-id="fba8f-190">组织的隐私配置文件。</span><span class="sxs-lookup"><span data-stu-id="fba8f-190">The privacy profile of an organization.</span></span>            |
|<span data-ttu-id="fba8f-191">provisionedPlans</span><span class="sxs-lookup"><span data-stu-id="fba8f-191">provisionedPlans</span></span>|<span data-ttu-id="fba8f-192">[ProvisionedPlan](provisionedplan.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fba8f-192">[ProvisionedPlan](provisionedplan.md) collection</span></span>| <span data-ttu-id="fba8f-193">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="fba8f-193">Not nullable.</span></span>            |
|<span data-ttu-id="fba8f-194">provisioningErrors</span><span class="sxs-lookup"><span data-stu-id="fba8f-194">provisioningErrors</span></span>|<span data-ttu-id="fba8f-195">ProvisioningError 集合</span><span class="sxs-lookup"><span data-stu-id="fba8f-195">ProvisioningError collection</span></span>| <span data-ttu-id="fba8f-196">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="fba8f-196">Not nullable.</span></span>            |
|<span data-ttu-id="fba8f-197">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="fba8f-197">securityComplianceNotificationMails</span></span>|<span data-ttu-id="fba8f-198">String collection</span><span class="sxs-lookup"><span data-stu-id="fba8f-198">String collection</span></span>||
|<span data-ttu-id="fba8f-199">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="fba8f-199">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="fba8f-200">String collection</span><span class="sxs-lookup"><span data-stu-id="fba8f-200">String collection</span></span>||
|<span data-ttu-id="fba8f-201">state</span><span class="sxs-lookup"><span data-stu-id="fba8f-201">state</span></span>|<span data-ttu-id="fba8f-202">String</span><span class="sxs-lookup"><span data-stu-id="fba8f-202">String</span></span>| <span data-ttu-id="fba8f-203">组织地址所在的省/自治区/直辖市名称。</span><span class="sxs-lookup"><span data-stu-id="fba8f-203">State name of the address for the organization</span></span> |
|<span data-ttu-id="fba8f-204">street</span><span class="sxs-lookup"><span data-stu-id="fba8f-204">street</span></span>|<span data-ttu-id="fba8f-205">String</span><span class="sxs-lookup"><span data-stu-id="fba8f-205">String</span></span>| <span data-ttu-id="fba8f-206">组织地址所在的街道名称。</span><span class="sxs-lookup"><span data-stu-id="fba8f-206">Street name of the address for organization</span></span> |
|<span data-ttu-id="fba8f-207">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="fba8f-207">technicalNotificationMails</span></span>|<span data-ttu-id="fba8f-208">String collection</span><span class="sxs-lookup"><span data-stu-id="fba8f-208">String collection</span></span>| <span data-ttu-id="fba8f-209">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="fba8f-209">Not nullable.</span></span> |
|<span data-ttu-id="fba8f-210">telephoneNumber</span><span class="sxs-lookup"><span data-stu-id="fba8f-210">telephoneNumber</span></span>|<span data-ttu-id="fba8f-211">String</span><span class="sxs-lookup"><span data-stu-id="fba8f-211">String</span></span>| <span data-ttu-id="fba8f-212">组织的电话号码</span><span class="sxs-lookup"><span data-stu-id="fba8f-212">Telephone number for the organization</span></span> |
|<span data-ttu-id="fba8f-213">verifiedDomains</span><span class="sxs-lookup"><span data-stu-id="fba8f-213">verifiedDomains</span></span>|<span data-ttu-id="fba8f-214">[VerifiedDomain](verifieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fba8f-214">[VerifiedDomain](verifieddomain.md) collection</span></span>|<span data-ttu-id="fba8f-p111">与该租户相关联的域集合。不可为 null。</span><span class="sxs-lookup"><span data-stu-id="fba8f-p111">The collection of domains associated with this tenant. Not nullable.</span></span>            |

## <a name="relationships"></a><span data-ttu-id="fba8f-217">Relationships</span><span class="sxs-lookup"><span data-stu-id="fba8f-217">Relationships</span></span>
<span data-ttu-id="fba8f-218">| 扩展 |[扩展](extension.md)集合 |打开扩展名为组织资源定义的集合。</span><span class="sxs-lookup"><span data-stu-id="fba8f-218">|extensions|[extension](extension.md) collection|The collection of open extensions defined for the organization resource.</span></span> <span data-ttu-id="fba8f-219">可以为 null。 |</span><span class="sxs-lookup"><span data-stu-id="fba8f-219">Nullable.|</span></span>

## <a name="json-representation"></a><span data-ttu-id="fba8f-220">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fba8f-220">JSON representation</span></span>

<span data-ttu-id="fba8f-221">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fba8f-221">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="fba8f-222">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fba8f-222">See also</span></span>

- [<span data-ttu-id="fba8f-223">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="fba8f-223">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fba8f-224">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="fba8f-224">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="fba8f-225">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="fba8f-225">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
