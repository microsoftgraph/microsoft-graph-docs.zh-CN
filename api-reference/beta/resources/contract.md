---
title: 合同资源类型
description: 表示合作伙伴租户与客户租户的现有合作关系。
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d1c573b43587ef5213f876b6532358fe5465f84b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962639"
---
# <a name="contract-resource-type"></a><span data-ttu-id="15ac0-103">合同资源类型</span><span class="sxs-lookup"><span data-stu-id="15ac0-103">Contract resource type</span></span>

<span data-ttu-id="15ac0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15ac0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15ac0-105">表示合作伙伴租户与客户租户的现有合作关系。</span><span class="sxs-lookup"><span data-stu-id="15ac0-105">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="15ac0-106">**重要提示：** 仅存在于合作伙伴租户中。</span><span class="sxs-lookup"><span data-stu-id="15ac0-106">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="15ac0-107">合作伙伴租户是属于 Microsoft 云解决方案提供商、Office 365 联合或 Microsoft Advisor 合作伙伴计划一部分的 [Microsoft](https://partnercenter.microsoft.com/en-us/partner/programs)合作伙伴的 Azure AD 租户。</span><span class="sxs-lookup"><span data-stu-id="15ac0-107">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="15ac0-108">Methods</span><span class="sxs-lookup"><span data-stu-id="15ac0-108">Methods</span></span>

| <span data-ttu-id="15ac0-109">方法</span><span class="sxs-lookup"><span data-stu-id="15ac0-109">Method</span></span>   | <span data-ttu-id="15ac0-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="15ac0-110">Return Type</span></span> | <span data-ttu-id="15ac0-111">说明</span><span class="sxs-lookup"><span data-stu-id="15ac0-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="15ac0-112">获取合同</span><span class="sxs-lookup"><span data-stu-id="15ac0-112">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="15ac0-113">合同</span><span class="sxs-lookup"><span data-stu-id="15ac0-113">Contract</span></span> |<span data-ttu-id="15ac0-114">读取特定合约对象的属性。</span><span class="sxs-lookup"><span data-stu-id="15ac0-114">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="15ac0-115">列出合同</span><span class="sxs-lookup"><span data-stu-id="15ac0-115">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="15ac0-116">合同集合</span><span class="sxs-lookup"><span data-stu-id="15ac0-116">Contract collection</span></span> | <span data-ttu-id="15ac0-117">合作伙伴租户中的合同列表。</span><span class="sxs-lookup"><span data-stu-id="15ac0-117">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="15ac0-118">属性</span><span class="sxs-lookup"><span data-stu-id="15ac0-118">Properties</span></span>
| <span data-ttu-id="15ac0-119">属性</span><span class="sxs-lookup"><span data-stu-id="15ac0-119">Property</span></span>   | <span data-ttu-id="15ac0-120">类型</span><span class="sxs-lookup"><span data-stu-id="15ac0-120">Type</span></span> | <span data-ttu-id="15ac0-121">说明</span><span class="sxs-lookup"><span data-stu-id="15ac0-121">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="15ac0-122">contractType</span><span class="sxs-lookup"><span data-stu-id="15ac0-122">contractType</span></span>|<span data-ttu-id="15ac0-123">String</span><span class="sxs-lookup"><span data-stu-id="15ac0-123">String</span></span>|<span data-ttu-id="15ac0-124">合同类型。</span><span class="sxs-lookup"><span data-stu-id="15ac0-124">Type of contract.</span></span> <span data-ttu-id="15ac0-125">可能的值是  `SyndicationPartner` `BreadthPartner` `ResellerPartner` ：、、。</span><span class="sxs-lookup"><span data-stu-id="15ac0-125">Possible values are:  `SyndicationPartner`, `BreadthPartner`, `ResellerPartner`.</span></span> <span data-ttu-id="15ac0-126">请参阅下表 [中的更多内容](#contracttype-values)。</span><span class="sxs-lookup"><span data-stu-id="15ac0-126">See more in the [table below](#contracttype-values).</span></span> |
|<span data-ttu-id="15ac0-127">customerId</span><span class="sxs-lookup"><span data-stu-id="15ac0-127">customerId</span></span>|<span data-ttu-id="15ac0-128">Guid</span><span class="sxs-lookup"><span data-stu-id="15ac0-128">Guid</span></span>|<span data-ttu-id="15ac0-129">此合作关系引用的客户租户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="15ac0-129">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="15ac0-130">对应于客户租户的组织资源的 id 属性。</span><span class="sxs-lookup"><span data-stu-id="15ac0-130">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="15ac0-131">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="15ac0-131">defaultDomainName</span></span>|<span data-ttu-id="15ac0-132">String</span><span class="sxs-lookup"><span data-stu-id="15ac0-132">String</span></span>|<span data-ttu-id="15ac0-133">客户租户的默认域名的副本。</span><span class="sxs-lookup"><span data-stu-id="15ac0-133">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="15ac0-134">建立与客户的合作关系后，即会进行复制。</span><span class="sxs-lookup"><span data-stu-id="15ac0-134">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="15ac0-135">如果客户租户的默认域名发生更改，将不会自动更新它。</span><span class="sxs-lookup"><span data-stu-id="15ac0-135">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="15ac0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="15ac0-136">displayName</span></span>|<span data-ttu-id="15ac0-137">String</span><span class="sxs-lookup"><span data-stu-id="15ac0-137">String</span></span>|<span data-ttu-id="15ac0-138">客户租户显示名称。</span><span class="sxs-lookup"><span data-stu-id="15ac0-138">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="15ac0-139">建立与客户的合作关系后，即会进行复制。</span><span class="sxs-lookup"><span data-stu-id="15ac0-139">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="15ac0-140">如果客户租户的订阅发生更改，将不会显示名称更新。</span><span class="sxs-lookup"><span data-stu-id="15ac0-140">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="15ac0-141">id</span><span class="sxs-lookup"><span data-stu-id="15ac0-141">id</span></span>|<span data-ttu-id="15ac0-142">String</span><span class="sxs-lookup"><span data-stu-id="15ac0-142">String</span></span>| <span data-ttu-id="15ac0-143">合作关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="15ac0-143">The unique identifier for the partnership.</span></span> <span data-ttu-id="15ac0-144">键，只读</span><span class="sxs-lookup"><span data-stu-id="15ac0-144">Key, read-only</span></span> |

### <a name="contracttype-values"></a><span data-ttu-id="15ac0-145">contractType 值</span><span class="sxs-lookup"><span data-stu-id="15ac0-145">contractType values</span></span>

|<span data-ttu-id="15ac0-146">成员</span><span class="sxs-lookup"><span data-stu-id="15ac0-146">Member</span></span>|<span data-ttu-id="15ac0-147">说明</span><span class="sxs-lookup"><span data-stu-id="15ac0-147">Description</span></span>|
|:---|:---|
|<span data-ttu-id="15ac0-148">SyndicationPartner</span><span class="sxs-lookup"><span data-stu-id="15ac0-148">SyndicationPartner</span></span>|<span data-ttu-id="15ac0-149">专门 *转售和管理* 此客户的 O365 和 Intune 的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="15ac0-149">Partner that *exclusively* resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="15ac0-150">他们转售和支持其客户。</span><span class="sxs-lookup"><span data-stu-id="15ac0-150">They resell and support their customers.</span></span>|
|<span data-ttu-id="15ac0-151">BreadthPartner</span><span class="sxs-lookup"><span data-stu-id="15ac0-151">BreadthPartner</span></span>|<span data-ttu-id="15ac0-152">合作伙伴能够为此客户提供管理支持。</span><span class="sxs-lookup"><span data-stu-id="15ac0-152">Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="15ac0-153">但是，不允许合作伙伴转售给客户。</span><span class="sxs-lookup"><span data-stu-id="15ac0-153">However, the partner is not allowed to resell to the customer.</span></span>|
|<span data-ttu-id="15ac0-154">ResellerPartner</span><span class="sxs-lookup"><span data-stu-id="15ac0-154">ResellerPartner</span></span>|<span data-ttu-id="15ac0-155">与联合合作伙伴类似的合作伙伴，只不过合作伙伴没有对租户的独占访问权限。</span><span class="sxs-lookup"><span data-stu-id="15ac0-155">Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="15ac0-156">在联合情况下，客户无法从 Microsoft 或其他合作伙伴购买其他直接订阅。</span><span class="sxs-lookup"><span data-stu-id="15ac0-156">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15ac0-157">关系</span><span class="sxs-lookup"><span data-stu-id="15ac0-157">Relationships</span></span>
<span data-ttu-id="15ac0-158">无</span><span class="sxs-lookup"><span data-stu-id="15ac0-158">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="15ac0-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15ac0-159">JSON representation</span></span>
<span data-ttu-id="15ac0-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15ac0-160">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Contract"
}-->

```json
{
  "contractType": "String",
  "customerId": "Guid",
  "defaultDomainName": "String",
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


