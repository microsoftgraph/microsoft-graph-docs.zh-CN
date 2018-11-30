---
title: orgContact 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: fb0970b2eb973e516761ba1145d66b3af7fdef5f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046986"
---
# <a name="orgcontact-resource-type"></a><span data-ttu-id="68c09-103">orgContact 资源类型</span><span class="sxs-lookup"><span data-stu-id="68c09-103">orgContact resource type</span></span>

> <span data-ttu-id="68c09-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="68c09-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68c09-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="68c09-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="68c09-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68c09-106">JSON representation</span></span>

<span data-ttu-id="68c09-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68c09-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "directReports",
    "manager",
    "memberOf"
  ],
  "@odata.type": "microsoft.graph.orgcontact"
}-->

```json
{
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "jobTitle": "string",
  "mail": "string",
  "mailNickname": "string",
  "mobilePhone": "string",
  "officeLocation": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "proxyAddresses": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string"
}

```
## <a name="properties"></a><span data-ttu-id="68c09-108">属性</span><span class="sxs-lookup"><span data-stu-id="68c09-108">Properties</span></span>
| <span data-ttu-id="68c09-109">属性</span><span class="sxs-lookup"><span data-stu-id="68c09-109">Property</span></span>     | <span data-ttu-id="68c09-110">类型</span><span class="sxs-lookup"><span data-stu-id="68c09-110">Type</span></span>   |<span data-ttu-id="68c09-111">说明</span><span class="sxs-lookup"><span data-stu-id="68c09-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68c09-112">city</span><span class="sxs-lookup"><span data-stu-id="68c09-112">city</span></span>|<span data-ttu-id="68c09-113">字符串</span><span class="sxs-lookup"><span data-stu-id="68c09-113">String</span></span>| <span data-ttu-id="68c09-114">联系人所在的市/县。</span><span class="sxs-lookup"><span data-stu-id="68c09-114">The city in which the contact is located.</span></span> |
|<span data-ttu-id="68c09-115">country</span><span class="sxs-lookup"><span data-stu-id="68c09-115">country</span></span>|<span data-ttu-id="68c09-116">字符串</span><span class="sxs-lookup"><span data-stu-id="68c09-116">String</span></span>| <span data-ttu-id="68c09-117">联系人所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="68c09-117">The country/region in which the contact is located.</span></span> |
|<span data-ttu-id="68c09-118">department</span><span class="sxs-lookup"><span data-stu-id="68c09-118">department</span></span>|<span data-ttu-id="68c09-119">字符串</span><span class="sxs-lookup"><span data-stu-id="68c09-119">String</span></span>| <span data-ttu-id="68c09-120">联系人适用于该部门的名称。</span><span class="sxs-lookup"><span data-stu-id="68c09-120">The name for the department in which the contact works.</span></span> |
|<span data-ttu-id="68c09-121">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="68c09-121">onPremisesSyncEnabled</span></span>|<span data-ttu-id="68c09-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="68c09-122">Boolean</span></span>|<span data-ttu-id="68c09-123">如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。</span><span class="sxs-lookup"><span data-stu-id="68c09-123">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default).</span></span>|
|<span data-ttu-id="68c09-124">displayName</span><span class="sxs-lookup"><span data-stu-id="68c09-124">displayName</span></span>|<span data-ttu-id="68c09-125">字符串</span><span class="sxs-lookup"><span data-stu-id="68c09-125">String</span></span>| <span data-ttu-id="68c09-126">该联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="68c09-126">The display name for the contact.</span></span> |
|<span data-ttu-id="68c09-127">givenName</span><span class="sxs-lookup"><span data-stu-id="68c09-127">givenName</span></span>|<span data-ttu-id="68c09-128">字符串</span><span class="sxs-lookup"><span data-stu-id="68c09-128">String</span></span>| <span data-ttu-id="68c09-129">联系人的给定姓名 （名字）。</span><span class="sxs-lookup"><span data-stu-id="68c09-129">The given name (first name) of the contact.</span></span> |
|<span data-ttu-id="68c09-130">jobTitle</span><span class="sxs-lookup"><span data-stu-id="68c09-130">jobTitle</span></span>|<span data-ttu-id="68c09-131">字符串</span><span class="sxs-lookup"><span data-stu-id="68c09-131">String</span></span>| <span data-ttu-id="68c09-132">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="68c09-132">The contact's job title.</span></span> |
|<span data-ttu-id="68c09-133">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="68c09-133">onPremisesLastSyncDateTime</span></span>|<span data-ttu-id="68c09-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68c09-134">DateTimeOffset</span></span>|<span data-ttu-id="68c09-135">指示的上次与内部部署目录同步对象的频率。</span><span class="sxs-lookup"><span data-stu-id="68c09-135">Indicates the last time at which the object was synced with the on-premises directory.</span></span> <span data-ttu-id="68c09-136">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="68c09-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="68c09-137">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="68c09-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="68c09-138">onPremisesProvisioningErrors</span><span class="sxs-lookup"><span data-stu-id="68c09-138">onPremisesProvisioningErrors</span></span>|<span data-ttu-id="68c09-139">[onPremisesProvisioningError](onpremisesprovisioningerror.md)集合</span><span class="sxs-lookup"><span data-stu-id="68c09-139">[onPremisesProvisioningError](onpremisesprovisioningerror.md) collection</span></span>| <span data-ttu-id="68c09-140">设置过程中使用 Microsoft 同步产品时错误。</span><span class="sxs-lookup"><span data-stu-id="68c09-140">Errors when using Microsoft synchronization product during provisioning.</span></span> |
|<span data-ttu-id="68c09-141">mail</span><span class="sxs-lookup"><span data-stu-id="68c09-141">mail</span></span>|<span data-ttu-id="68c09-142">字符串</span><span class="sxs-lookup"><span data-stu-id="68c09-142">String</span></span>| <span data-ttu-id="68c09-143">该联系人，例如，"jeff@contoso.onmicrosoft.com"的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="68c09-143">The SMTP address for the contact, for example, "jeff@contoso.onmicrosoft.com".</span></span> |
|<span data-ttu-id="68c09-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="68c09-144">mailNickname</span></span>|<span data-ttu-id="68c09-145">字符串</span><span class="sxs-lookup"><span data-stu-id="68c09-145">String</span></span>| <span data-ttu-id="68c09-146">邮件联系人的别名。</span><span class="sxs-lookup"><span data-stu-id="68c09-146">The mail alias for the contact.</span></span> |
|<span data-ttu-id="68c09-147">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="68c09-147">mobilePhone</span></span>|<span data-ttu-id="68c09-148">String</span><span class="sxs-lookup"><span data-stu-id="68c09-148">String</span></span>| <span data-ttu-id="68c09-149">联系人的主要移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="68c09-149">The primary cellular telephone number for the contact.</span></span> |
|<span data-ttu-id="68c09-150">id</span><span class="sxs-lookup"><span data-stu-id="68c09-150">id</span></span>|<span data-ttu-id="68c09-151">字符串</span><span class="sxs-lookup"><span data-stu-id="68c09-151">String</span></span>| <span data-ttu-id="68c09-152">该联系人的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="68c09-152">The unique identifier for the contact.</span></span> <span data-ttu-id="68c09-153">只读。</span><span class="sxs-lookup"><span data-stu-id="68c09-153">Read-only.</span></span>|
|<span data-ttu-id="68c09-154">officeLocation</span><span class="sxs-lookup"><span data-stu-id="68c09-154">officeLocation</span></span>|<span data-ttu-id="68c09-155">String</span><span class="sxs-lookup"><span data-stu-id="68c09-155">String</span></span>| <span data-ttu-id="68c09-156">中的业务联系人的位置的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="68c09-156">The office location in the contact's place of business.</span></span> |
|<span data-ttu-id="68c09-157">postalCode</span><span class="sxs-lookup"><span data-stu-id="68c09-157">postalCode</span></span>|<span data-ttu-id="68c09-158">字符串</span><span class="sxs-lookup"><span data-stu-id="68c09-158">String</span></span>| <span data-ttu-id="68c09-159">联系人的邮政地址的邮政编码。</span><span class="sxs-lookup"><span data-stu-id="68c09-159">The postal code for the contact's postal address.</span></span> <span data-ttu-id="68c09-160">特定于该联系人的国家/地区的邮政编码。</span><span class="sxs-lookup"><span data-stu-id="68c09-160">The postal code is specific to the contact's country/region.</span></span> <span data-ttu-id="68c09-161">在美国，此属性包含邮政编码。</span><span class="sxs-lookup"><span data-stu-id="68c09-161">In the United States of America, this attribute contains the ZIP code.</span></span> |
|<span data-ttu-id="68c09-162">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="68c09-162">proxyAddresses</span></span>|<span data-ttu-id="68c09-163">String collection</span><span class="sxs-lookup"><span data-stu-id="68c09-163">String collection</span></span>| <span data-ttu-id="68c09-164">例如： `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` **any**运算符，则需要为多值属性的筛选器表达式。</span><span class="sxs-lookup"><span data-stu-id="68c09-164">For example: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` The **any** operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="68c09-165">只读。</span><span class="sxs-lookup"><span data-stu-id="68c09-165">Read-only.</span></span> <span data-ttu-id="68c09-166">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="68c09-166">Not nullable.</span></span> <span data-ttu-id="68c09-167">支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="68c09-167">Supports $filter.</span></span> |
|<span data-ttu-id="68c09-168">状态</span><span class="sxs-lookup"><span data-stu-id="68c09-168">state</span></span>|<span data-ttu-id="68c09-169">字符串</span><span class="sxs-lookup"><span data-stu-id="68c09-169">String</span></span>| <span data-ttu-id="68c09-170">州或省中联系人的地址。</span><span class="sxs-lookup"><span data-stu-id="68c09-170">The state or province in the contact's address.</span></span> |
|<span data-ttu-id="68c09-171">streetAddress</span><span class="sxs-lookup"><span data-stu-id="68c09-171">streetAddress</span></span>|<span data-ttu-id="68c09-172">String</span><span class="sxs-lookup"><span data-stu-id="68c09-172">String</span></span>| <span data-ttu-id="68c09-173">联系人的位置的业务街道地址。</span><span class="sxs-lookup"><span data-stu-id="68c09-173">The street address of the contact's place of business.</span></span> |
|<span data-ttu-id="68c09-174">surname</span><span class="sxs-lookup"><span data-stu-id="68c09-174">surname</span></span>|<span data-ttu-id="68c09-175">字符串</span><span class="sxs-lookup"><span data-stu-id="68c09-175">String</span></span>| <span data-ttu-id="68c09-176">（家人名称或姓氏） 的联系人的姓。</span><span class="sxs-lookup"><span data-stu-id="68c09-176">The contact's surname (family name or last name).</span></span> |
|<span data-ttu-id="68c09-177">businessPhones</span><span class="sxs-lookup"><span data-stu-id="68c09-177">businessPhones</span></span>|<span data-ttu-id="68c09-178">String</span><span class="sxs-lookup"><span data-stu-id="68c09-178">String</span></span>| <span data-ttu-id="68c09-179">联系人的位置的业务主要电话号码。</span><span class="sxs-lookup"><span data-stu-id="68c09-179">The primary telephone number of the contact's place of business.</span></span> |

## <a name="relationships"></a><span data-ttu-id="68c09-180">Relationships</span><span class="sxs-lookup"><span data-stu-id="68c09-180">Relationships</span></span>
| <span data-ttu-id="68c09-181">关系</span><span class="sxs-lookup"><span data-stu-id="68c09-181">Relationship</span></span> | <span data-ttu-id="68c09-182">类型</span><span class="sxs-lookup"><span data-stu-id="68c09-182">Type</span></span>   |<span data-ttu-id="68c09-183">说明</span><span class="sxs-lookup"><span data-stu-id="68c09-183">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68c09-184">directReports</span><span class="sxs-lookup"><span data-stu-id="68c09-184">directReports</span></span>|<span data-ttu-id="68c09-185">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="68c09-185">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="68c09-186">联系人的直接下属。</span><span class="sxs-lookup"><span data-stu-id="68c09-186">The contact's direct reports.</span></span> <span data-ttu-id="68c09-187">（用户和其管理器属性设置为此联系人的联系人。） 只读的。</span><span class="sxs-lookup"><span data-stu-id="68c09-187">(The users and contacts that have their manager property set to this contact.)  Read-only.</span></span> <span data-ttu-id="68c09-188">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="68c09-188">Nullable.</span></span>|
|<span data-ttu-id="68c09-189">manager</span><span class="sxs-lookup"><span data-stu-id="68c09-189">manager</span></span>|[<span data-ttu-id="68c09-190">directoryObject</span><span class="sxs-lookup"><span data-stu-id="68c09-190">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="68c09-191">用户或此联系人的管理器的联系人。</span><span class="sxs-lookup"><span data-stu-id="68c09-191">The user or contact that is this contact's manager.</span></span> <span data-ttu-id="68c09-192">只读。</span><span class="sxs-lookup"><span data-stu-id="68c09-192">Read-only.</span></span>|
|<span data-ttu-id="68c09-193">memberOf</span><span class="sxs-lookup"><span data-stu-id="68c09-193">memberOf</span></span>|<span data-ttu-id="68c09-194">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="68c09-194">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="68c09-195">此联系人所在的组。</span><span class="sxs-lookup"><span data-stu-id="68c09-195">Groups that this contact is a member of.</span></span> <span data-ttu-id="68c09-196">只读。</span><span class="sxs-lookup"><span data-stu-id="68c09-196">Read-only.</span></span> <span data-ttu-id="68c09-197">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="68c09-197">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="68c09-198">方法</span><span class="sxs-lookup"><span data-stu-id="68c09-198">Methods</span></span>

| <span data-ttu-id="68c09-199">方法</span><span class="sxs-lookup"><span data-stu-id="68c09-199">Method</span></span>           | <span data-ttu-id="68c09-200">返回类型</span><span class="sxs-lookup"><span data-stu-id="68c09-200">Return Type</span></span>    |<span data-ttu-id="68c09-201">说明</span><span class="sxs-lookup"><span data-stu-id="68c09-201">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="68c09-202">获取 orgContact</span><span class="sxs-lookup"><span data-stu-id="68c09-202">Get orgContact</span></span>](../api/orgcontact-get.md) | [<span data-ttu-id="68c09-203">orgContact</span><span class="sxs-lookup"><span data-stu-id="68c09-203">orgContact</span></span>](orgcontact.md) |<span data-ttu-id="68c09-204">读取属性和 orgContact 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="68c09-204">Read properties and relationships of orgContact object.</span></span>|
|[<span data-ttu-id="68c09-205">获取管理器</span><span class="sxs-lookup"><span data-stu-id="68c09-205">Get manager</span></span>](../api/orgcontact-get-manager.md) |[<span data-ttu-id="68c09-206">directoryObject</span><span class="sxs-lookup"><span data-stu-id="68c09-206">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="68c09-207">获取联系人的经理。</span><span class="sxs-lookup"><span data-stu-id="68c09-207">Get the contact's manager.</span></span>|
|[<span data-ttu-id="68c09-208">List directReports</span><span class="sxs-lookup"><span data-stu-id="68c09-208">List directReports</span></span>](../api/orgcontact-list-directreports.md) |<span data-ttu-id="68c09-209">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="68c09-209">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="68c09-210">列出该联系人的直接下属。</span><span class="sxs-lookup"><span data-stu-id="68c09-210">List the contact's direct reports.</span></span>|
|[<span data-ttu-id="68c09-211">List memberOf</span><span class="sxs-lookup"><span data-stu-id="68c09-211">List memberOf</span></span>](../api/orgcontact-list-memberof.md) |<span data-ttu-id="68c09-212">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="68c09-212">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="68c09-213">获取 memberOf 对象集合。</span><span class="sxs-lookup"><span data-stu-id="68c09-213">Get a memberOf object collection.</span></span>|
|[<span data-ttu-id="68c09-214">删除</span><span class="sxs-lookup"><span data-stu-id="68c09-214">Delete</span></span>](../api/orgcontact-delete.md) | <span data-ttu-id="68c09-215">无</span><span class="sxs-lookup"><span data-stu-id="68c09-215">None</span></span> |<span data-ttu-id="68c09-216">删除 orgContact 对象。</span><span class="sxs-lookup"><span data-stu-id="68c09-216">Delete orgContact object.</span></span> |
|[<span data-ttu-id="68c09-217">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="68c09-217">checkMemberGroups</span></span>](../api/orgcontact-checkmembergroups.md)|<span data-ttu-id="68c09-218">String collection</span><span class="sxs-lookup"><span data-stu-id="68c09-218">String collection</span></span>| <span data-ttu-id="68c09-219">检查组成员身份。</span><span class="sxs-lookup"><span data-stu-id="68c09-219">Check for group membership.</span></span> |
|[<span data-ttu-id="68c09-220">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="68c09-220">getMemberGroups</span></span>](../api/orgcontact-getmembergroups.md)|<span data-ttu-id="68c09-221">String collection</span><span class="sxs-lookup"><span data-stu-id="68c09-221">String collection</span></span>| <span data-ttu-id="68c09-222">返回指定的联系人所在的所有组。</span><span class="sxs-lookup"><span data-stu-id="68c09-222">Return all the groups that the specified contact is a member of.</span></span> |
|[<span data-ttu-id="68c09-223">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="68c09-223">getMemberObjects</span></span>](../api/orgcontact-getmemberobjects.md)|<span data-ttu-id="68c09-224">String collection</span><span class="sxs-lookup"><span data-stu-id="68c09-224">String collection</span></span>| <span data-ttu-id="68c09-225">返回的 directoryObjects 联系人所在的列表。</span><span class="sxs-lookup"><span data-stu-id="68c09-225">Returns a list of directoryObjects the contact is a member of.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "orgContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->