---
title: orgContact 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9ccd36e9d04a1404bb972694fdb9c2b0d8a5ccc3
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352367"
---
# <a name="orgcontact-resource-type"></a><span data-ttu-id="f8e62-103">orgContact 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8e62-103">orgContact resource type</span></span>

<span data-ttu-id="f8e62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8e62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8e62-105">表示一个组织联系人。</span><span class="sxs-lookup"><span data-stu-id="f8e62-105">Represents an organizational contact.</span></span> <span data-ttu-id="f8e62-106">组织联系人由组织的管理员管理，不同于 [个人联系人](contact.md)。</span><span class="sxs-lookup"><span data-stu-id="f8e62-106">Organizational contacts are managed by an organization's administrators and are different from [personal contacts](contact.md).</span></span> <span data-ttu-id="f8e62-107">此外，组织联系人既可以从本地目录同步，也可以从 Exchange Online 同步，也可以是只读的。</span><span class="sxs-lookup"><span data-stu-id="f8e62-107">Additionally, organizational contacts are either synchronized from on-premises directories or from Exchange Online, and are read-only.</span></span>

<span data-ttu-id="f8e62-108">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="f8e62-108">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="f8e62-109">该资源支持通过提供 [delta](../api/orgcontact-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="f8e62-109">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/orgcontact-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="f8e62-110">方法</span><span class="sxs-lookup"><span data-stu-id="f8e62-110">Methods</span></span>

| <span data-ttu-id="f8e62-111">方法</span><span class="sxs-lookup"><span data-stu-id="f8e62-111">Method</span></span> | <span data-ttu-id="f8e62-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="f8e62-112">Return Type</span></span> | <span data-ttu-id="f8e62-113">Description</span><span class="sxs-lookup"><span data-stu-id="f8e62-113">Description</span></span> |
| ------ | ----------- | ----------- |
| [<span data-ttu-id="f8e62-114">列出组织联系人</span><span class="sxs-lookup"><span data-stu-id="f8e62-114">List organizational contacts</span></span>](../api/orgcontact-list.md) | <span data-ttu-id="f8e62-115">[orgContact](orgcontact.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f8e62-115">[orgContact](orgcontact.md) collection</span></span> | <span data-ttu-id="f8e62-116">列出组织联系人的属性。</span><span class="sxs-lookup"><span data-stu-id="f8e62-116">List properties of organizational contacts.</span></span> |
| [<span data-ttu-id="f8e62-117">获取组织联系人</span><span class="sxs-lookup"><span data-stu-id="f8e62-117">Get organizational contact</span></span>](../api/orgcontact-get.md) | [<span data-ttu-id="f8e62-118">orgContact</span><span class="sxs-lookup"><span data-stu-id="f8e62-118">orgContact</span></span>](orgcontact.md) | <span data-ttu-id="f8e62-119">读取 orgContact 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f8e62-119">Read properties and relationships of orgContact object.</span></span> |
| [<span data-ttu-id="f8e62-120">获取管理器</span><span class="sxs-lookup"><span data-stu-id="f8e62-120">Get manager</span></span>](../api/orgcontact-get-manager.md) | [<span data-ttu-id="f8e62-121">directoryObject</span><span class="sxs-lookup"><span data-stu-id="f8e62-121">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="f8e62-122">获取联系人的经理。</span><span class="sxs-lookup"><span data-stu-id="f8e62-122">Get the contact's manager.</span></span> |
| [<span data-ttu-id="f8e62-123">List directReports</span><span class="sxs-lookup"><span data-stu-id="f8e62-123">List directReports</span></span>](../api/orgcontact-list-directreports.md) | <span data-ttu-id="f8e62-124">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="f8e62-124">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="f8e62-125">列出联系人的直接下属。</span><span class="sxs-lookup"><span data-stu-id="f8e62-125">List the contact's direct reports.</span></span> |
| [<span data-ttu-id="f8e62-126">List memberOf</span><span class="sxs-lookup"><span data-stu-id="f8e62-126">List memberOf</span></span>](../api/orgcontact-list-memberof.md) | <span data-ttu-id="f8e62-127">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f8e62-127">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="f8e62-128">获取 memberOf 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f8e62-128">Get a memberOf object collection.</span></span> |
| [<span data-ttu-id="f8e62-129">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="f8e62-129">checkMemberGroups</span></span>](../api/orgcontact-checkmembergroups.md) | <span data-ttu-id="f8e62-130">String 集合</span><span class="sxs-lookup"><span data-stu-id="f8e62-130">String collection</span></span> | <span data-ttu-id="f8e62-131">检查组成员身份。</span><span class="sxs-lookup"><span data-stu-id="f8e62-131">Check for group membership.</span></span> |
| [<span data-ttu-id="f8e62-132">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="f8e62-132">getMemberGroups</span></span>](../api/orgcontact-getmembergroups.md) | <span data-ttu-id="f8e62-133">String 集合</span><span class="sxs-lookup"><span data-stu-id="f8e62-133">String collection</span></span> | <span data-ttu-id="f8e62-134">返回指定的联系人所属的所有组。</span><span class="sxs-lookup"><span data-stu-id="f8e62-134">Return all the groups that the specified contact is a member of.</span></span> |
| [<span data-ttu-id="f8e62-135">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="f8e62-135">getMemberObjects</span></span>](../api/orgcontact-getmemberobjects.md) | <span data-ttu-id="f8e62-136">String 集合</span><span class="sxs-lookup"><span data-stu-id="f8e62-136">String collection</span></span> | <span data-ttu-id="f8e62-137">返回联系人所属的 directoryObjects 的列表。</span><span class="sxs-lookup"><span data-stu-id="f8e62-137">Returns a list of directoryObjects the contact is a member of.</span></span> |

## <a name="properties"></a><span data-ttu-id="f8e62-138">属性</span><span class="sxs-lookup"><span data-stu-id="f8e62-138">Properties</span></span>

| <span data-ttu-id="f8e62-139">属性</span><span class="sxs-lookup"><span data-stu-id="f8e62-139">Property</span></span> | <span data-ttu-id="f8e62-140">类型</span><span class="sxs-lookup"><span data-stu-id="f8e62-140">Type</span></span> | <span data-ttu-id="f8e62-141">Description</span><span class="sxs-lookup"><span data-stu-id="f8e62-141">Description</span></span> |
| -------- | ---- | ----------- |
| <span data-ttu-id="f8e62-142">地址</span><span class="sxs-lookup"><span data-stu-id="f8e62-142">addresses</span></span> | <span data-ttu-id="f8e62-143">[physicalOfficeAddress](physicalofficeaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f8e62-143">[physicalOfficeAddress](physicalofficeaddress.md) collection</span></span> | <span data-ttu-id="f8e62-144">此组织联系人的邮政地址。</span><span class="sxs-lookup"><span data-stu-id="f8e62-144">Postal addresses for this organizational contact.</span></span> <span data-ttu-id="f8e62-145">目前，一个联系人只能有一个实际地址。</span><span class="sxs-lookup"><span data-stu-id="f8e62-145">For now a contact can only have one physical address.</span></span> |
| <span data-ttu-id="f8e62-146">companyName</span><span class="sxs-lookup"><span data-stu-id="f8e62-146">companyName</span></span> | <span data-ttu-id="f8e62-147">String</span><span class="sxs-lookup"><span data-stu-id="f8e62-147">String</span></span> | <span data-ttu-id="f8e62-148">此组织联系人所属的公司的名称。</span><span class="sxs-lookup"><span data-stu-id="f8e62-148">Name of the company that this organizational contact belong to.</span></span> |
| <span data-ttu-id="f8e62-149">department</span><span class="sxs-lookup"><span data-stu-id="f8e62-149">department</span></span> | <span data-ttu-id="f8e62-150">String</span><span class="sxs-lookup"><span data-stu-id="f8e62-150">String</span></span> | <span data-ttu-id="f8e62-151">联系人工作所在的部门的名称。</span><span class="sxs-lookup"><span data-stu-id="f8e62-151">The name for the department in which the contact works.</span></span> |
| <span data-ttu-id="f8e62-152">displayName</span><span class="sxs-lookup"><span data-stu-id="f8e62-152">displayName</span></span> | <span data-ttu-id="f8e62-153">字符串</span><span class="sxs-lookup"><span data-stu-id="f8e62-153">String</span></span> | <span data-ttu-id="f8e62-154">此组织联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f8e62-154">Display name for this organizational contact.</span></span> |
| <span data-ttu-id="f8e62-155">givenName</span><span class="sxs-lookup"><span data-stu-id="f8e62-155">givenName</span></span> | <span data-ttu-id="f8e62-156">字符串</span><span class="sxs-lookup"><span data-stu-id="f8e62-156">String</span></span> | <span data-ttu-id="f8e62-157">此组织联系人的名字。</span><span class="sxs-lookup"><span data-stu-id="f8e62-157">First name for this organizational contact.</span></span> |
| <span data-ttu-id="f8e62-158">id</span><span class="sxs-lookup"><span data-stu-id="f8e62-158">id</span></span> | <span data-ttu-id="f8e62-159">字符串</span><span class="sxs-lookup"><span data-stu-id="f8e62-159">String</span></span> | <span data-ttu-id="f8e62-160">此组织联系人的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f8e62-160">Unique identifier for this organizational contact.</span></span> |
| <span data-ttu-id="f8e62-161">jobTitle</span><span class="sxs-lookup"><span data-stu-id="f8e62-161">jobTitle</span></span> | <span data-ttu-id="f8e62-162">String</span><span class="sxs-lookup"><span data-stu-id="f8e62-162">String</span></span> | <span data-ttu-id="f8e62-163">此组织联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="f8e62-163">Job title for this organizational contact.</span></span> |
| <span data-ttu-id="f8e62-164">mail</span><span class="sxs-lookup"><span data-stu-id="f8e62-164">mail</span></span> | <span data-ttu-id="f8e62-165">String</span><span class="sxs-lookup"><span data-stu-id="f8e62-165">String</span></span> | <span data-ttu-id="f8e62-166">联系人的 SMTP 地址，例如，"jeff@contoso.onmicrosoft.com"。</span><span class="sxs-lookup"><span data-stu-id="f8e62-166">The SMTP address for the contact, for example, "jeff@contoso.onmicrosoft.com".</span></span> |
| <span data-ttu-id="f8e62-167">mailNickname</span><span class="sxs-lookup"><span data-stu-id="f8e62-167">mailNickname</span></span> | <span data-ttu-id="f8e62-168">String</span><span class="sxs-lookup"><span data-stu-id="f8e62-168">String</span></span> | <span data-ttu-id="f8e62-169">电子邮件别名 (电子邮件地址的一部分预挂起此组织联系人的 @ 符号) 。</span><span class="sxs-lookup"><span data-stu-id="f8e62-169">Email alias (portion of email address pre-pending the @ symbol) for this organizational contact.</span></span> |
| <span data-ttu-id="f8e62-170">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f8e62-170">onPremisesLastSyncDateTime</span></span> | <span data-ttu-id="f8e62-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8e62-171">DateTimeOffset</span></span> | <span data-ttu-id="f8e62-172">上次从本地 AD 同步此组织联系人的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f8e62-172">Date and time when this organizational contact was last synchronized from on-premises AD.</span></span> <span data-ttu-id="f8e62-173">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="f8e62-173">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f8e62-174">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="f8e62-174">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="f8e62-175">onPremisesProvisioningErrors</span><span class="sxs-lookup"><span data-stu-id="f8e62-175">onPremisesProvisioningErrors</span></span> | <span data-ttu-id="f8e62-176">[onPremisesProvisioningError](onpremisesprovisioningerror.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f8e62-176">[onPremisesProvisioningError](onpremisesprovisioningerror.md) collection</span></span> | <span data-ttu-id="f8e62-177">此组织联系人的任何同步设置错误列表。</span><span class="sxs-lookup"><span data-stu-id="f8e62-177">List of any synchronization provisioning errors for this organizational contact.</span></span> |
| <span data-ttu-id="f8e62-178">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="f8e62-178">onPremisesSyncEnabled</span></span> | <span data-ttu-id="f8e62-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8e62-179">Boolean</span></span> | <span data-ttu-id="f8e62-180">如果此对象从本地目录同步，**则为 true** ; 否则为 false。**假** 如果此对象最初是从本地目录同步，但不再同步，并且现在在 Exchange 中的 mastered;如果从未从本地目录同步此对象，则 **为 null** (默认) 。</span><span class="sxs-lookup"><span data-stu-id="f8e62-180">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced and now mastered in Exchange; **null** if this object has never been synced from an on-premises directory (default).</span></span> |
| <span data-ttu-id="f8e62-181">phones</span><span class="sxs-lookup"><span data-stu-id="f8e62-181">phones</span></span> | <span data-ttu-id="f8e62-182">[phone](phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="f8e62-182">[phone](phone.md) collection</span></span> | <span data-ttu-id="f8e62-183">此组织联系人的电话列表。</span><span class="sxs-lookup"><span data-stu-id="f8e62-183">List of phones for this organizational contact.</span></span> <span data-ttu-id="f8e62-184">电话类型可以是移动、商业和 businessFax。</span><span class="sxs-lookup"><span data-stu-id="f8e62-184">Phone types can be mobile, business, and businessFax.</span></span> <span data-ttu-id="f8e62-185">集合中仅有一种类型可以存在。</span><span class="sxs-lookup"><span data-stu-id="f8e62-185">Only one of each type can ever be present in the collection.</span></span> |
| <span data-ttu-id="f8e62-186">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="f8e62-186">proxyAddresses</span></span> | <span data-ttu-id="f8e62-187">String 集合</span><span class="sxs-lookup"><span data-stu-id="f8e62-187">String collection</span></span> | <span data-ttu-id="f8e62-188">例如： "SMTP： bob@contoso.com"、"SMTP： bob@sales.contoso.com"。</span><span class="sxs-lookup"><span data-stu-id="f8e62-188">For example: "SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com".</span></span> <span data-ttu-id="f8e62-189">需要多值属性筛选器表达式的 **any** 运算符。</span><span class="sxs-lookup"><span data-stu-id="f8e62-189">The **any** operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="f8e62-190">支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="f8e62-190">Supports $filter.</span></span> |
| <span data-ttu-id="f8e62-191">surname</span><span class="sxs-lookup"><span data-stu-id="f8e62-191">surname</span></span> | <span data-ttu-id="f8e62-192">字符串</span><span class="sxs-lookup"><span data-stu-id="f8e62-192">String</span></span> | <span data-ttu-id="f8e62-193">此组织联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="f8e62-193">Last name for this organizational contact.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f8e62-194">关系</span><span class="sxs-lookup"><span data-stu-id="f8e62-194">Relationships</span></span>

| <span data-ttu-id="f8e62-195">关系</span><span class="sxs-lookup"><span data-stu-id="f8e62-195">Relationship</span></span> | <span data-ttu-id="f8e62-196">类型</span><span class="sxs-lookup"><span data-stu-id="f8e62-196">Type</span></span> | <span data-ttu-id="f8e62-197">Description</span><span class="sxs-lookup"><span data-stu-id="f8e62-197">Description</span></span> |
| ------------ | ---- | ----------- |
| <span data-ttu-id="f8e62-198">directReports</span><span class="sxs-lookup"><span data-stu-id="f8e62-198">directReports</span></span> | <span data-ttu-id="f8e62-199">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="f8e62-199">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="f8e62-200">联系人的直接下属。</span><span class="sxs-lookup"><span data-stu-id="f8e62-200">The contact's direct reports.</span></span> <span data-ttu-id="f8e62-201"> (其 "经理" 属性设置为 "联系人" 的用户和联系人。 ) 只读。</span><span class="sxs-lookup"><span data-stu-id="f8e62-201">(The users and contacts that have their manager property set to this contact.) Read-only.</span></span> <span data-ttu-id="f8e62-202">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f8e62-202">Nullable.</span></span> |
| <span data-ttu-id="f8e62-203">manager</span><span class="sxs-lookup"><span data-stu-id="f8e62-203">manager</span></span> | [<span data-ttu-id="f8e62-204">directoryObject</span><span class="sxs-lookup"><span data-stu-id="f8e62-204">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="f8e62-205">作为此联系人的经理的用户或联系人。</span><span class="sxs-lookup"><span data-stu-id="f8e62-205">The user or contact that is this contact's manager.</span></span> <span data-ttu-id="f8e62-206">只读。</span><span class="sxs-lookup"><span data-stu-id="f8e62-206">Read-only.</span></span> |
| <span data-ttu-id="f8e62-207">memberOf</span><span class="sxs-lookup"><span data-stu-id="f8e62-207">memberOf</span></span> | <span data-ttu-id="f8e62-208">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f8e62-208">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="f8e62-209">此联系人所属的组。</span><span class="sxs-lookup"><span data-stu-id="f8e62-209">Groups that this contact is a member of.</span></span> <span data-ttu-id="f8e62-210">只读。</span><span class="sxs-lookup"><span data-stu-id="f8e62-210">Read-only.</span></span> <span data-ttu-id="f8e62-211">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f8e62-211">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f8e62-212">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8e62-212">JSON representation</span></span>

<span data-ttu-id="f8e62-213">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8e62-213">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "directReports",
    "manager",
    "memberOf"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.orgContact"
}-->

``` json
{
  "addresses": [{"@odata.type": "microsoft.graph.physicalOfficeAddress"}],
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "jobTitle": "string",
  "mail": "string",
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "string (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSyncEnabled": true,
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "proxyAddresses": ["string"],
  "surname": "string"
}
```
