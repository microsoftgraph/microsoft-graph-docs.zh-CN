---
title: 约定资源类型
description: 表示合作伙伴租户与客户租户之间的现有合作关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7911d875f669e03a40cd9408e047b9f7d0aee0d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533005"
---
# <a name="contract-resource-type"></a><span data-ttu-id="0fe5e-103">约定资源类型</span><span class="sxs-lookup"><span data-stu-id="0fe5e-103">Contract resource type</span></span>

<span data-ttu-id="0fe5e-104">命名空间： microsoft. graph 表示合作伙伴租户与客户租户之间的现有合作关系。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-104">Namespace: microsoft.graph Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="0fe5e-105">**重要说明：** 仅存在于合作伙伴租户中。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-105">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="0fe5e-106">合作伙伴租户是属于 microsoft[云解决方案提供商](https://partnercenter.microsoft.com/en-us/partner/programs)、Office 365 联合或 microsoft Advisor 合作伙伴计划一部分的 microsoft 合作伙伴的 Azure AD 租户。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-106">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="0fe5e-107">Methods</span><span class="sxs-lookup"><span data-stu-id="0fe5e-107">Methods</span></span>

| <span data-ttu-id="0fe5e-108">方法</span><span class="sxs-lookup"><span data-stu-id="0fe5e-108">Method</span></span>   | <span data-ttu-id="0fe5e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0fe5e-109">Return Type</span></span> | <span data-ttu-id="0fe5e-110">说明</span><span class="sxs-lookup"><span data-stu-id="0fe5e-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="0fe5e-111">获取合同</span><span class="sxs-lookup"><span data-stu-id="0fe5e-111">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="0fe5e-112">联系</span><span class="sxs-lookup"><span data-stu-id="0fe5e-112">Contract</span></span> |<span data-ttu-id="0fe5e-113">读取特定 contract 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-113">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="0fe5e-114">列出合同</span><span class="sxs-lookup"><span data-stu-id="0fe5e-114">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="0fe5e-115">合同集合</span><span class="sxs-lookup"><span data-stu-id="0fe5e-115">Contract collection</span></span> | <span data-ttu-id="0fe5e-116">合作伙伴租户中的合同列表。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-116">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="0fe5e-117">属性</span><span class="sxs-lookup"><span data-stu-id="0fe5e-117">Properties</span></span>
| <span data-ttu-id="0fe5e-118">属性</span><span class="sxs-lookup"><span data-stu-id="0fe5e-118">Property</span></span>   | <span data-ttu-id="0fe5e-119">类型</span><span class="sxs-lookup"><span data-stu-id="0fe5e-119">Type</span></span> | <span data-ttu-id="0fe5e-120">说明</span><span class="sxs-lookup"><span data-stu-id="0fe5e-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0fe5e-121">contractType</span><span class="sxs-lookup"><span data-stu-id="0fe5e-121">contractType</span></span>|<span data-ttu-id="0fe5e-122">字符串</span><span class="sxs-lookup"><span data-stu-id="0fe5e-122">String</span></span>|<span data-ttu-id="0fe5e-123">约定的类型。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-123">Type of contract.</span></span><br><br><span data-ttu-id="0fe5e-124">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="0fe5e-124">Possible values are:</span></span><br> <span data-ttu-id="0fe5e-125">*SyndicationPartner* -专为此客户 resells 和管理 O365 和 Intune 的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-125">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="0fe5e-126">他们转售并支持其客户。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-126">They resell and support their customers.</span></span><br> <span data-ttu-id="0fe5e-127">*BreadthPartner* -合作伙伴能够为此客户提供管理支持。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-127">*BreadthPartner* - Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="0fe5e-128">但是，不允许合作伙伴转销给客户。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-128">However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="0fe5e-129">*ResellerPartner* -合作伙伴与联合合作伙伴相似，不同之处在于合作伙伴不具有对租户的独占访问权限。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-129">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="0fe5e-130">在联合案例中，客户无法购买来自 Microsoft 或其他合作伙伴的其他直接订阅。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-130">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="0fe5e-131">customerId</span><span class="sxs-lookup"><span data-stu-id="0fe5e-131">customerId</span></span>|<span data-ttu-id="0fe5e-132">Guid</span><span class="sxs-lookup"><span data-stu-id="0fe5e-132">Guid</span></span>|<span data-ttu-id="0fe5e-133">此合作关系引用的客户租户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-133">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="0fe5e-134">对应于客户租户的组织资源的 id 属性。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-134">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="0fe5e-135">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="0fe5e-135">defaultDomainName</span></span>|<span data-ttu-id="0fe5e-136">字符串</span><span class="sxs-lookup"><span data-stu-id="0fe5e-136">String</span></span>|<span data-ttu-id="0fe5e-137">客户租户的默认域名的副本。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-137">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="0fe5e-138">如果建立与客户的合作关系，则会进行复制。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-138">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="0fe5e-139">如果客户租户的默认域名发生更改，则不会自动更新该名称。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-139">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="0fe5e-140">displayName</span><span class="sxs-lookup"><span data-stu-id="0fe5e-140">displayName</span></span>|<span data-ttu-id="0fe5e-141">String</span><span class="sxs-lookup"><span data-stu-id="0fe5e-141">String</span></span>|<span data-ttu-id="0fe5e-142">客户租户的显示名称的副本。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-142">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="0fe5e-143">如果建立与客户的合作关系，则会进行复制。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-143">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="0fe5e-144">如果客户租户的显示名称发生更改，则不会自动更新。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-144">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="0fe5e-145">id</span><span class="sxs-lookup"><span data-stu-id="0fe5e-145">id</span></span>|<span data-ttu-id="0fe5e-146">字符串</span><span class="sxs-lookup"><span data-stu-id="0fe5e-146">String</span></span>| <span data-ttu-id="0fe5e-147">合作关系的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-147">The unique identifier for the partnership.</span></span> <span data-ttu-id="0fe5e-148">键，只读</span><span class="sxs-lookup"><span data-stu-id="0fe5e-148">Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="0fe5e-149">关系</span><span class="sxs-lookup"><span data-stu-id="0fe5e-149">Relationships</span></span>
<span data-ttu-id="0fe5e-150">无</span><span class="sxs-lookup"><span data-stu-id="0fe5e-150">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0fe5e-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fe5e-151">JSON representation</span></span>
<span data-ttu-id="0fe5e-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fe5e-152">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.contract"
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
<!-- {
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
