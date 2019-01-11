---
title: 合同资源类型
description: 表示合作伙伴租户与客户租户的现有合作伙伴关系。
localization_priority: Normal
ms.openlocfilehash: e502c72003c6d65305430bc1bf5a539d7235b5ef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815321"
---
# <a name="contract-resource-type"></a><span data-ttu-id="01b6e-103">合同资源类型</span><span class="sxs-lookup"><span data-stu-id="01b6e-103">Contract resource type</span></span>

> <span data-ttu-id="01b6e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="01b6e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01b6e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="01b6e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01b6e-106">表示合作伙伴租户与客户租户的现有合作伙伴关系。</span><span class="sxs-lookup"><span data-stu-id="01b6e-106">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="01b6e-p102">**重要说明：** 仅存在于合作伙伴租户中。合作伙伴租户是属于 Microsoft 合作伙伴的 Azure AD 租户，其中 Microsoft 合作伙伴是 [Microsoft 云解决方案提供商](https://partnercenter.microsoft.com/en-us/partner/programs)、Office 365 Syndication 或 Microsoft Advisor 计划的一部分。</span><span class="sxs-lookup"><span data-stu-id="01b6e-p102">**Important:** Exists in partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="01b6e-109">方法</span><span class="sxs-lookup"><span data-stu-id="01b6e-109">Methods</span></span>

| <span data-ttu-id="01b6e-110">方法</span><span class="sxs-lookup"><span data-stu-id="01b6e-110">Method</span></span>   | <span data-ttu-id="01b6e-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="01b6e-111">Return Type</span></span> | <span data-ttu-id="01b6e-112">说明</span><span class="sxs-lookup"><span data-stu-id="01b6e-112">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="01b6e-113">获取合同</span><span class="sxs-lookup"><span data-stu-id="01b6e-113">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="01b6e-114">合同</span><span class="sxs-lookup"><span data-stu-id="01b6e-114">Contract</span></span> |<span data-ttu-id="01b6e-115">读取特定合同对象的属性。</span><span class="sxs-lookup"><span data-stu-id="01b6e-115">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="01b6e-116">列出合同</span><span class="sxs-lookup"><span data-stu-id="01b6e-116">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="01b6e-117">合同集合</span><span class="sxs-lookup"><span data-stu-id="01b6e-117">Contract collection</span></span> | <span data-ttu-id="01b6e-118">合同中伙伴租户中的合同列表。</span><span class="sxs-lookup"><span data-stu-id="01b6e-118">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="01b6e-119">属性</span><span class="sxs-lookup"><span data-stu-id="01b6e-119">Properties</span></span>
| <span data-ttu-id="01b6e-120">属性</span><span class="sxs-lookup"><span data-stu-id="01b6e-120">Property</span></span>   | <span data-ttu-id="01b6e-121">类型</span><span class="sxs-lookup"><span data-stu-id="01b6e-121">Type</span></span> | <span data-ttu-id="01b6e-122">说明</span><span class="sxs-lookup"><span data-stu-id="01b6e-122">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="01b6e-123">contractType</span><span class="sxs-lookup"><span data-stu-id="01b6e-123">contractType</span></span>|<span data-ttu-id="01b6e-124">String</span><span class="sxs-lookup"><span data-stu-id="01b6e-124">String</span></span>|<span data-ttu-id="01b6e-125">合同的类型。</span><span class="sxs-lookup"><span data-stu-id="01b6e-125">Type of contract.</span></span><br><br><span data-ttu-id="01b6e-126">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="01b6e-126">Possible values are:</span></span><br> <span data-ttu-id="01b6e-p103">*SyndicationPartner* - 为此客户独家转售和管理 O365 和 Intune 的合作伙伴。他们转售并为其客户提供支持。</span><span class="sxs-lookup"><span data-stu-id="01b6e-p103">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer. They resell and support their customers.</span></span><br> <span data-ttu-id="01b6e-p104">*BreadthPartner* - 合作伙伴能够为此客户提供管理支持。不过，合作伙伴不得向客户进行转售。</span><span class="sxs-lookup"><span data-stu-id="01b6e-p104">*BreadthPartner* - Partner has the ability to provide administrative support for this customer. However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="01b6e-p105">*ResellerPartner* - 与联合合作伙伴类似，但是无权对租户进行独占访问。在联合的情况下，客户不能从 Microsoft 或其他合作伙伴购买其他直接订阅。</span><span class="sxs-lookup"><span data-stu-id="01b6e-p105">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant. In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="01b6e-133">customerId</span><span class="sxs-lookup"><span data-stu-id="01b6e-133">customerId</span></span>|<span data-ttu-id="01b6e-134">Guid</span><span class="sxs-lookup"><span data-stu-id="01b6e-134">Guid</span></span>|<span data-ttu-id="01b6e-p106">此合作关系引用的客户租户的唯一标识符。对应于客户租户的组织资源的 id 属性。</span><span class="sxs-lookup"><span data-stu-id="01b6e-p106">The unique identifier for the customer tenant referenced by this partnership. Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="01b6e-137">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="01b6e-137">defaultDomainName</span></span>|<span data-ttu-id="01b6e-138">字符串</span><span class="sxs-lookup"><span data-stu-id="01b6e-138">String</span></span>|<span data-ttu-id="01b6e-p107">客户租户的默认域名的副本。与客户建立合作伙伴关系时生成副本。如果客户租户的默认域名更改，此项将不会自动更新。</span><span class="sxs-lookup"><span data-stu-id="01b6e-p107">A copy of the customer tenant's default domain name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="01b6e-142">displayName</span><span class="sxs-lookup"><span data-stu-id="01b6e-142">displayName</span></span>|<span data-ttu-id="01b6e-143">字符串</span><span class="sxs-lookup"><span data-stu-id="01b6e-143">String</span></span>|<span data-ttu-id="01b6e-p108">客户租户的显示名称的副本。与客户建立合作伙伴关系时生成副本。如果客户租户的显示名称更改，此项将不会自动更新。</span><span class="sxs-lookup"><span data-stu-id="01b6e-p108">A copy of the customer tenant's display name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="01b6e-147">id</span><span class="sxs-lookup"><span data-stu-id="01b6e-147">id</span></span>|<span data-ttu-id="01b6e-148">字符串</span><span class="sxs-lookup"><span data-stu-id="01b6e-148">String</span></span>| <span data-ttu-id="01b6e-p109">合作伙伴关系的唯一标识符。键，只读。</span><span class="sxs-lookup"><span data-stu-id="01b6e-p109">The unique identifier for the partnership. Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="01b6e-151">关系</span><span class="sxs-lookup"><span data-stu-id="01b6e-151">Relationships</span></span>
<span data-ttu-id="01b6e-152">无</span><span class="sxs-lookup"><span data-stu-id="01b6e-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="01b6e-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01b6e-153">JSON representation</span></span>
<span data-ttu-id="01b6e-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01b6e-154">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
