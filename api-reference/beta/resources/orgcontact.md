---
title: orgContact 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 08611fc9a98931dabbf66802df37a346d4117b58
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721822"
---
# <a name="orgcontact-resource-type"></a><span data-ttu-id="b3962-103">orgContact 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3962-103">orgContact resource type</span></span>

<span data-ttu-id="b3962-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3962-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3962-105">代表组织联系人。</span><span class="sxs-lookup"><span data-stu-id="b3962-105">Represents an organizational contact.</span></span> <span data-ttu-id="b3962-106">组织联系人由组织的管理员管理，不同于 [个人联系人](contact.md)。</span><span class="sxs-lookup"><span data-stu-id="b3962-106">Organizational contacts are managed by an organization's administrators and are different from [personal contacts](contact.md).</span></span> <span data-ttu-id="b3962-107">此外，组织联系人从本地目录或 Exchange Online 同步，并且只读。</span><span class="sxs-lookup"><span data-stu-id="b3962-107">Additionally, organizational contacts are either synchronized from on-premises directories or from Exchange Online, and are read-only.</span></span>

<span data-ttu-id="b3962-108">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="b3962-108">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="b3962-109">该资源支持通过提供 [delta](../api/orgcontact-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="b3962-109">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/orgcontact-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="b3962-110">方法</span><span class="sxs-lookup"><span data-stu-id="b3962-110">Methods</span></span>

| <span data-ttu-id="b3962-111">方法</span><span class="sxs-lookup"><span data-stu-id="b3962-111">Method</span></span> | <span data-ttu-id="b3962-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="b3962-112">Return Type</span></span> | <span data-ttu-id="b3962-113">说明</span><span class="sxs-lookup"><span data-stu-id="b3962-113">Description</span></span> |
| ------ | ----------- | ----------- |
| [<span data-ttu-id="b3962-114">列出组织联系人</span><span class="sxs-lookup"><span data-stu-id="b3962-114">List organizational contacts</span></span>](../api/orgcontact-list.md) | <span data-ttu-id="b3962-115">[orgContact](orgcontact.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b3962-115">[orgContact](orgcontact.md) collection</span></span> | <span data-ttu-id="b3962-116">列出组织联系人的属性。</span><span class="sxs-lookup"><span data-stu-id="b3962-116">List properties of organizational contacts.</span></span> |
| [<span data-ttu-id="b3962-117">获取组织联系人</span><span class="sxs-lookup"><span data-stu-id="b3962-117">Get organizational contact</span></span>](../api/orgcontact-get.md) | [<span data-ttu-id="b3962-118">orgContact</span><span class="sxs-lookup"><span data-stu-id="b3962-118">orgContact</span></span>](orgcontact.md) | <span data-ttu-id="b3962-119">读取 orgContact 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b3962-119">Read properties and relationships of orgContact object.</span></span> |
| [<span data-ttu-id="b3962-120">获取经理</span><span class="sxs-lookup"><span data-stu-id="b3962-120">Get manager</span></span>](../api/orgcontact-get-manager.md) | [<span data-ttu-id="b3962-121">directoryObject</span><span class="sxs-lookup"><span data-stu-id="b3962-121">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="b3962-122">获取联系人的经理。</span><span class="sxs-lookup"><span data-stu-id="b3962-122">Get the contact's manager.</span></span> |
| [<span data-ttu-id="b3962-123">List directReports</span><span class="sxs-lookup"><span data-stu-id="b3962-123">List directReports</span></span>](../api/orgcontact-list-directreports.md) | <span data-ttu-id="b3962-124">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="b3962-124">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="b3962-125">列出联系人的直接下属。</span><span class="sxs-lookup"><span data-stu-id="b3962-125">List the contact's direct reports.</span></span> |
| [<span data-ttu-id="b3962-126">List memberOf</span><span class="sxs-lookup"><span data-stu-id="b3962-126">List memberOf</span></span>](../api/orgcontact-list-memberof.md) | <span data-ttu-id="b3962-127">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b3962-127">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="b3962-128">获取 memberOf 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b3962-128">Get a memberOf object collection.</span></span> |
| [<span data-ttu-id="b3962-129">checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="b3962-129">checkMemberGroups</span></span>](../api/orgcontact-checkmembergroups.md) | <span data-ttu-id="b3962-130">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b3962-130">String collection</span></span> | <span data-ttu-id="b3962-131">检查组成员身份。</span><span class="sxs-lookup"><span data-stu-id="b3962-131">Check for group membership.</span></span> |
| [<span data-ttu-id="b3962-132">getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="b3962-132">getMemberGroups</span></span>](../api/orgcontact-getmembergroups.md) | <span data-ttu-id="b3962-133">String 集合</span><span class="sxs-lookup"><span data-stu-id="b3962-133">String collection</span></span> | <span data-ttu-id="b3962-134">返回指定联系人是其中成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="b3962-134">Return all the groups that the specified contact is a member of.</span></span> |
| [<span data-ttu-id="b3962-135">getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="b3962-135">getMemberObjects</span></span>](../api/orgcontact-getmemberobjects.md) | <span data-ttu-id="b3962-136">String 集合</span><span class="sxs-lookup"><span data-stu-id="b3962-136">String collection</span></span> | <span data-ttu-id="b3962-137">返回联系人是其中一个成员的 directoryObjects 列表。</span><span class="sxs-lookup"><span data-stu-id="b3962-137">Returns a list of directoryObjects the contact is a member of.</span></span> |

## <a name="properties"></a><span data-ttu-id="b3962-138">属性</span><span class="sxs-lookup"><span data-stu-id="b3962-138">Properties</span></span>

| <span data-ttu-id="b3962-139">属性</span><span class="sxs-lookup"><span data-stu-id="b3962-139">Property</span></span> | <span data-ttu-id="b3962-140">类型</span><span class="sxs-lookup"><span data-stu-id="b3962-140">Type</span></span> | <span data-ttu-id="b3962-141">说明</span><span class="sxs-lookup"><span data-stu-id="b3962-141">Description</span></span> |
| -------- | ---- | ----------- |
| <span data-ttu-id="b3962-142">地址</span><span class="sxs-lookup"><span data-stu-id="b3962-142">addresses</span></span> | <span data-ttu-id="b3962-143">[physicalOfficeAddress](physicalofficeaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b3962-143">[physicalOfficeAddress](physicalofficeaddress.md) collection</span></span> | <span data-ttu-id="b3962-144">此组织联系人的邮政地址。</span><span class="sxs-lookup"><span data-stu-id="b3962-144">Postal addresses for this organizational contact.</span></span> <span data-ttu-id="b3962-145">目前，联系人只能有一个物理地址。</span><span class="sxs-lookup"><span data-stu-id="b3962-145">For now a contact can only have one physical address.</span></span> |
| <span data-ttu-id="b3962-146">companyName</span><span class="sxs-lookup"><span data-stu-id="b3962-146">companyName</span></span> | <span data-ttu-id="b3962-147">String</span><span class="sxs-lookup"><span data-stu-id="b3962-147">String</span></span> | <span data-ttu-id="b3962-148">此组织联系人所属的公司的名称。</span><span class="sxs-lookup"><span data-stu-id="b3962-148">Name of the company that this organizational contact belong to.</span></span> |
| <span data-ttu-id="b3962-149">department</span><span class="sxs-lookup"><span data-stu-id="b3962-149">department</span></span> | <span data-ttu-id="b3962-150">String</span><span class="sxs-lookup"><span data-stu-id="b3962-150">String</span></span> | <span data-ttu-id="b3962-151">联系人工作部门的名称。</span><span class="sxs-lookup"><span data-stu-id="b3962-151">The name for the department in which the contact works.</span></span> |
| <span data-ttu-id="b3962-152">displayName</span><span class="sxs-lookup"><span data-stu-id="b3962-152">displayName</span></span> | <span data-ttu-id="b3962-153">String</span><span class="sxs-lookup"><span data-stu-id="b3962-153">String</span></span> | <span data-ttu-id="b3962-154">此组织联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b3962-154">Display name for this organizational contact.</span></span> |
| <span data-ttu-id="b3962-155">givenName</span><span class="sxs-lookup"><span data-stu-id="b3962-155">givenName</span></span> | <span data-ttu-id="b3962-156">String</span><span class="sxs-lookup"><span data-stu-id="b3962-156">String</span></span> | <span data-ttu-id="b3962-157">此组织联系人的名字。</span><span class="sxs-lookup"><span data-stu-id="b3962-157">First name for this organizational contact.</span></span> |
| <span data-ttu-id="b3962-158">id</span><span class="sxs-lookup"><span data-stu-id="b3962-158">id</span></span> | <span data-ttu-id="b3962-159">String</span><span class="sxs-lookup"><span data-stu-id="b3962-159">String</span></span> | <span data-ttu-id="b3962-160">此组织联系人的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b3962-160">Unique identifier for this organizational contact.</span></span> |
| <span data-ttu-id="b3962-161">jobTitle</span><span class="sxs-lookup"><span data-stu-id="b3962-161">jobTitle</span></span> | <span data-ttu-id="b3962-162">String</span><span class="sxs-lookup"><span data-stu-id="b3962-162">String</span></span> | <span data-ttu-id="b3962-163">此组织联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="b3962-163">Job title for this organizational contact.</span></span> |
| <span data-ttu-id="b3962-164">mail</span><span class="sxs-lookup"><span data-stu-id="b3962-164">mail</span></span> | <span data-ttu-id="b3962-165">String</span><span class="sxs-lookup"><span data-stu-id="b3962-165">String</span></span> | <span data-ttu-id="b3962-166">联系人的 SMTP 地址，例如"jeff@contoso.onmicrosoft.com"。</span><span class="sxs-lookup"><span data-stu-id="b3962-166">The SMTP address for the contact, for example, "jeff@contoso.onmicrosoft.com".</span></span> |
| <span data-ttu-id="b3962-167">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b3962-167">mailNickname</span></span> | <span data-ttu-id="b3962-168">String</span><span class="sxs-lookup"><span data-stu-id="b3962-168">String</span></span> | <span data-ttu-id="b3962-169">电子邮件别名 (电子邮件地址的一部分，预挂起此) @ 符号。</span><span class="sxs-lookup"><span data-stu-id="b3962-169">Email alias (portion of email address pre-pending the @ symbol) for this organizational contact.</span></span> |
| <span data-ttu-id="b3962-170">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b3962-170">onPremisesLastSyncDateTime</span></span> | <span data-ttu-id="b3962-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3962-171">DateTimeOffset</span></span> | <span data-ttu-id="b3962-172">上次从本地 AD 同步此组织联系人的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b3962-172">Date and time when this organizational contact was last synchronized from on-premises AD.</span></span> <span data-ttu-id="b3962-173">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="b3962-173">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b3962-174">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="b3962-174">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="b3962-175">onPremisesProvisioningErrors</span><span class="sxs-lookup"><span data-stu-id="b3962-175">onPremisesProvisioningErrors</span></span> | <span data-ttu-id="b3962-176">[onPremisesProvisioningError](onpremisesprovisioningerror.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b3962-176">[onPremisesProvisioningError](onpremisesprovisioningerror.md) collection</span></span> | <span data-ttu-id="b3962-177">此组织联系人的任何同步设置错误的列表。</span><span class="sxs-lookup"><span data-stu-id="b3962-177">List of any synchronization provisioning errors for this organizational contact.</span></span> |
| <span data-ttu-id="b3962-178">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="b3962-178">onPremisesSyncEnabled</span></span> | <span data-ttu-id="b3962-179">布尔</span><span class="sxs-lookup"><span data-stu-id="b3962-179">Boolean</span></span> | <span data-ttu-id="b3962-180">如果此对象从本地目录同步，则其为 **true;\*\*\*\*假** 如果此对象最初从本地目录同步，但不再同步，现在在 Exchange 中主控;**如果** 此对象从未从本地目录同步，则 (默认值) 。</span><span class="sxs-lookup"><span data-stu-id="b3962-180">**true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced and now mastered in Exchange; **null** if this object has never been synced from an on-premises directory (default).</span></span> |
| <span data-ttu-id="b3962-181">phones</span><span class="sxs-lookup"><span data-stu-id="b3962-181">phones</span></span> | <span data-ttu-id="b3962-182">[phone](phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="b3962-182">[phone](phone.md) collection</span></span> | <span data-ttu-id="b3962-183">此组织联系人的电话列表。</span><span class="sxs-lookup"><span data-stu-id="b3962-183">List of phones for this organizational contact.</span></span> <span data-ttu-id="b3962-184">电话类型可以是移动、商业和 businessFax。</span><span class="sxs-lookup"><span data-stu-id="b3962-184">Phone types can be mobile, business, and businessFax.</span></span> <span data-ttu-id="b3962-185">集合中只能存在每种类型之一。</span><span class="sxs-lookup"><span data-stu-id="b3962-185">Only one of each type can ever be present in the collection.</span></span> |
| <span data-ttu-id="b3962-186">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="b3962-186">proxyAddresses</span></span> | <span data-ttu-id="b3962-187">String 集合</span><span class="sxs-lookup"><span data-stu-id="b3962-187">String collection</span></span> | <span data-ttu-id="b3962-188">例如："SMTP： bob@contoso.com"、"smtp： bob@sales.contoso.com"。</span><span class="sxs-lookup"><span data-stu-id="b3962-188">For example: "SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com".</span></span> <span data-ttu-id="b3962-189">需要多值属性筛选器表达式的 **any** 运算符。</span><span class="sxs-lookup"><span data-stu-id="b3962-189">The **any** operator is required for filter expressions on multi-valued properties.</span></span> <span data-ttu-id="b3962-190">支持 $filter。</span><span class="sxs-lookup"><span data-stu-id="b3962-190">Supports $filter.</span></span> |
| <span data-ttu-id="b3962-191">surname</span><span class="sxs-lookup"><span data-stu-id="b3962-191">surname</span></span> | <span data-ttu-id="b3962-192">String</span><span class="sxs-lookup"><span data-stu-id="b3962-192">String</span></span> | <span data-ttu-id="b3962-193">此组织联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="b3962-193">Last name for this organizational contact.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b3962-194">关系</span><span class="sxs-lookup"><span data-stu-id="b3962-194">Relationships</span></span>

| <span data-ttu-id="b3962-195">关系</span><span class="sxs-lookup"><span data-stu-id="b3962-195">Relationship</span></span> | <span data-ttu-id="b3962-196">类型</span><span class="sxs-lookup"><span data-stu-id="b3962-196">Type</span></span> | <span data-ttu-id="b3962-197">说明</span><span class="sxs-lookup"><span data-stu-id="b3962-197">Description</span></span> |
| ------------ | ---- | ----------- |
| <span data-ttu-id="b3962-198">directReports</span><span class="sxs-lookup"><span data-stu-id="b3962-198">directReports</span></span> | <span data-ttu-id="b3962-199">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="b3962-199">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="b3962-200">联系人的直接下属。</span><span class="sxs-lookup"><span data-stu-id="b3962-200">The contact's direct reports.</span></span> <span data-ttu-id="b3962-201"> (其经理属性设置为此联系人的用户和联系人。) 只读。</span><span class="sxs-lookup"><span data-stu-id="b3962-201">(The users and contacts that have their manager property set to this contact.) Read-only.</span></span> <span data-ttu-id="b3962-202">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b3962-202">Nullable.</span></span> |
| <span data-ttu-id="b3962-203">manager</span><span class="sxs-lookup"><span data-stu-id="b3962-203">manager</span></span> | [<span data-ttu-id="b3962-204">directoryObject</span><span class="sxs-lookup"><span data-stu-id="b3962-204">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="b3962-205">作为此联系人的经理的用户或联系人。</span><span class="sxs-lookup"><span data-stu-id="b3962-205">The user or contact that is this contact's manager.</span></span> <span data-ttu-id="b3962-206">只读。</span><span class="sxs-lookup"><span data-stu-id="b3962-206">Read-only.</span></span> |
| <span data-ttu-id="b3962-207">memberOf</span><span class="sxs-lookup"><span data-stu-id="b3962-207">memberOf</span></span> | <span data-ttu-id="b3962-208">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b3962-208">[directoryObject](directoryobject.md) collection</span></span> | <span data-ttu-id="b3962-209">此联系人是其中一个成员的组。</span><span class="sxs-lookup"><span data-stu-id="b3962-209">Groups that this contact is a member of.</span></span> <span data-ttu-id="b3962-210">只读。</span><span class="sxs-lookup"><span data-stu-id="b3962-210">Read-only.</span></span> <span data-ttu-id="b3962-211">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="b3962-211">Nullable.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b3962-212">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3962-212">JSON representation</span></span>

<span data-ttu-id="b3962-213">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3962-213">Here is a JSON representation of the resource</span></span>

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
