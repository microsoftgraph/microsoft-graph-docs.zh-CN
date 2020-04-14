---
title: 约定资源类型
description: 表示合作伙伴租户与客户租户之间的现有合作关系。
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cbf58924c8d8abec95346364a0c3723f8a44f8fb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458062"
---
# <a name="contract-resource-type"></a><span data-ttu-id="72397-103">约定资源类型</span><span class="sxs-lookup"><span data-stu-id="72397-103">Contract resource type</span></span>

<span data-ttu-id="72397-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72397-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72397-105">表示合作伙伴租户与客户租户之间的现有合作关系。</span><span class="sxs-lookup"><span data-stu-id="72397-105">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="72397-106">**重要说明：** 仅存在于合作伙伴租户中。</span><span class="sxs-lookup"><span data-stu-id="72397-106">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="72397-107">合作伙伴租户是属于 microsoft[云解决方案提供商](https://partnercenter.microsoft.com/en-us/partner/programs)、Office 365 联合或 microsoft Advisor 合作伙伴计划一部分的 microsoft 合作伙伴的 Azure AD 租户。</span><span class="sxs-lookup"><span data-stu-id="72397-107">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="72397-108">方法</span><span class="sxs-lookup"><span data-stu-id="72397-108">Methods</span></span>

| <span data-ttu-id="72397-109">方法</span><span class="sxs-lookup"><span data-stu-id="72397-109">Method</span></span>   | <span data-ttu-id="72397-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="72397-110">Return Type</span></span> | <span data-ttu-id="72397-111">说明</span><span class="sxs-lookup"><span data-stu-id="72397-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="72397-112">获取合同</span><span class="sxs-lookup"><span data-stu-id="72397-112">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="72397-113">联系</span><span class="sxs-lookup"><span data-stu-id="72397-113">Contract</span></span> |<span data-ttu-id="72397-114">读取特定 contract 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="72397-114">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="72397-115">列出合同</span><span class="sxs-lookup"><span data-stu-id="72397-115">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="72397-116">合同集合</span><span class="sxs-lookup"><span data-stu-id="72397-116">Contract collection</span></span> | <span data-ttu-id="72397-117">合作伙伴租户中的合同列表。</span><span class="sxs-lookup"><span data-stu-id="72397-117">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="72397-118">属性</span><span class="sxs-lookup"><span data-stu-id="72397-118">Properties</span></span>
| <span data-ttu-id="72397-119">属性</span><span class="sxs-lookup"><span data-stu-id="72397-119">Property</span></span>   | <span data-ttu-id="72397-120">类型</span><span class="sxs-lookup"><span data-stu-id="72397-120">Type</span></span> | <span data-ttu-id="72397-121">说明</span><span class="sxs-lookup"><span data-stu-id="72397-121">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="72397-122">contractType</span><span class="sxs-lookup"><span data-stu-id="72397-122">contractType</span></span>|<span data-ttu-id="72397-123">String</span><span class="sxs-lookup"><span data-stu-id="72397-123">String</span></span>|<span data-ttu-id="72397-124">约定的类型。</span><span class="sxs-lookup"><span data-stu-id="72397-124">Type of contract.</span></span><br><br><span data-ttu-id="72397-125">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="72397-125">Possible values are:</span></span><br> <span data-ttu-id="72397-126">*SyndicationPartner* -专为此客户 resells 和管理 O365 和 Intune 的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="72397-126">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="72397-127">他们转售并支持其客户。</span><span class="sxs-lookup"><span data-stu-id="72397-127">They resell and support their customers.</span></span><br> <span data-ttu-id="72397-128">*BreadthPartner* -合作伙伴能够为此客户提供管理支持。</span><span class="sxs-lookup"><span data-stu-id="72397-128">*BreadthPartner* - Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="72397-129">但是，不允许合作伙伴转销给客户。</span><span class="sxs-lookup"><span data-stu-id="72397-129">However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="72397-130">*ResellerPartner* -合作伙伴与联合合作伙伴相似，不同之处在于合作伙伴不具有对租户的独占访问权限。</span><span class="sxs-lookup"><span data-stu-id="72397-130">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="72397-131">在联合案例中，客户无法购买来自 Microsoft 或其他合作伙伴的其他直接订阅。</span><span class="sxs-lookup"><span data-stu-id="72397-131">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="72397-132">customerId</span><span class="sxs-lookup"><span data-stu-id="72397-132">customerId</span></span>|<span data-ttu-id="72397-133">Guid</span><span class="sxs-lookup"><span data-stu-id="72397-133">Guid</span></span>|<span data-ttu-id="72397-134">此合作关系引用的客户租户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="72397-134">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="72397-135">对应于客户租户的组织资源的 id 属性。</span><span class="sxs-lookup"><span data-stu-id="72397-135">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="72397-136">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="72397-136">defaultDomainName</span></span>|<span data-ttu-id="72397-137">String</span><span class="sxs-lookup"><span data-stu-id="72397-137">String</span></span>|<span data-ttu-id="72397-138">客户租户的默认域名的副本。</span><span class="sxs-lookup"><span data-stu-id="72397-138">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="72397-139">如果建立与客户的合作关系，则会进行复制。</span><span class="sxs-lookup"><span data-stu-id="72397-139">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="72397-140">如果客户租户的默认域名发生更改，则不会自动更新该名称。</span><span class="sxs-lookup"><span data-stu-id="72397-140">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="72397-141">displayName</span><span class="sxs-lookup"><span data-stu-id="72397-141">displayName</span></span>|<span data-ttu-id="72397-142">String</span><span class="sxs-lookup"><span data-stu-id="72397-142">String</span></span>|<span data-ttu-id="72397-143">客户租户的显示名称的副本。</span><span class="sxs-lookup"><span data-stu-id="72397-143">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="72397-144">如果建立与客户的合作关系，则会进行复制。</span><span class="sxs-lookup"><span data-stu-id="72397-144">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="72397-145">如果客户租户的显示名称发生更改，则不会自动更新。</span><span class="sxs-lookup"><span data-stu-id="72397-145">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="72397-146">id</span><span class="sxs-lookup"><span data-stu-id="72397-146">id</span></span>|<span data-ttu-id="72397-147">String</span><span class="sxs-lookup"><span data-stu-id="72397-147">String</span></span>| <span data-ttu-id="72397-148">合作关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="72397-148">The unique identifier for the partnership.</span></span> <span data-ttu-id="72397-149">键，只读</span><span class="sxs-lookup"><span data-stu-id="72397-149">Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="72397-150">关系</span><span class="sxs-lookup"><span data-stu-id="72397-150">Relationships</span></span>
<span data-ttu-id="72397-151">无</span><span class="sxs-lookup"><span data-stu-id="72397-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="72397-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72397-152">JSON representation</span></span>
<span data-ttu-id="72397-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72397-153">Here is a JSON representation of the resource.</span></span>

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
