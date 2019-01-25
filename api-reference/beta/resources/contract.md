---
title: 合同资源类型
description: 表示合作伙伴租户与客户租户的现有合作伙伴关系。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6309dfc370d414ccb66065fe4048d7cece51f018
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509698"
---
# <a name="contract-resource-type"></a><span data-ttu-id="231f0-103">合同资源类型</span><span class="sxs-lookup"><span data-stu-id="231f0-103">Contract resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="231f0-104">表示合作伙伴租户与客户租户的现有合作伙伴关系。</span><span class="sxs-lookup"><span data-stu-id="231f0-104">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="231f0-p101">**重要说明：** 仅存在于合作伙伴租户中。合作伙伴租户是属于 Microsoft 合作伙伴的 Azure AD 租户，其中 Microsoft 合作伙伴是 [Microsoft 云解决方案提供商](https://partnercenter.microsoft.com/en-us/partner/programs)、Office 365 Syndication 或 Microsoft Advisor 计划的一部分。</span><span class="sxs-lookup"><span data-stu-id="231f0-p101">**Important:** Exists in partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="231f0-107">方法</span><span class="sxs-lookup"><span data-stu-id="231f0-107">Methods</span></span>

| <span data-ttu-id="231f0-108">方法</span><span class="sxs-lookup"><span data-stu-id="231f0-108">Method</span></span>   | <span data-ttu-id="231f0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="231f0-109">Return Type</span></span> | <span data-ttu-id="231f0-110">说明</span><span class="sxs-lookup"><span data-stu-id="231f0-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="231f0-111">获取合同</span><span class="sxs-lookup"><span data-stu-id="231f0-111">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="231f0-112">合同</span><span class="sxs-lookup"><span data-stu-id="231f0-112">Contract</span></span> |<span data-ttu-id="231f0-113">读取特定合同对象的属性。</span><span class="sxs-lookup"><span data-stu-id="231f0-113">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="231f0-114">列出合同</span><span class="sxs-lookup"><span data-stu-id="231f0-114">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="231f0-115">合同集合</span><span class="sxs-lookup"><span data-stu-id="231f0-115">Contract collection</span></span> | <span data-ttu-id="231f0-116">合同中伙伴租户中的合同列表。</span><span class="sxs-lookup"><span data-stu-id="231f0-116">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="231f0-117">属性</span><span class="sxs-lookup"><span data-stu-id="231f0-117">Properties</span></span>
| <span data-ttu-id="231f0-118">属性</span><span class="sxs-lookup"><span data-stu-id="231f0-118">Property</span></span>   | <span data-ttu-id="231f0-119">类型</span><span class="sxs-lookup"><span data-stu-id="231f0-119">Type</span></span> | <span data-ttu-id="231f0-120">说明</span><span class="sxs-lookup"><span data-stu-id="231f0-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="231f0-121">contractType</span><span class="sxs-lookup"><span data-stu-id="231f0-121">contractType</span></span>|<span data-ttu-id="231f0-122">String</span><span class="sxs-lookup"><span data-stu-id="231f0-122">String</span></span>|<span data-ttu-id="231f0-123">合同的类型。</span><span class="sxs-lookup"><span data-stu-id="231f0-123">Type of contract.</span></span><br><br><span data-ttu-id="231f0-124">可能的值是：</span><span class="sxs-lookup"><span data-stu-id="231f0-124">Possible values are:</span></span><br> <span data-ttu-id="231f0-p102">*SyndicationPartner* - 为此客户独家转售和管理 O365 和 Intune 的合作伙伴。他们转售并为其客户提供支持。</span><span class="sxs-lookup"><span data-stu-id="231f0-p102">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer. They resell and support their customers.</span></span><br> <span data-ttu-id="231f0-p103">*BreadthPartner* - 合作伙伴能够为此客户提供管理支持。不过，合作伙伴不得向客户进行转售。</span><span class="sxs-lookup"><span data-stu-id="231f0-p103">*BreadthPartner* - Partner has the ability to provide administrative support for this customer. However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="231f0-p104">*ResellerPartner* - 与联合合作伙伴类似，但是无权对租户进行独占访问。在联合的情况下，客户不能从 Microsoft 或其他合作伙伴购买其他直接订阅。</span><span class="sxs-lookup"><span data-stu-id="231f0-p104">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant. In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="231f0-131">customerId</span><span class="sxs-lookup"><span data-stu-id="231f0-131">customerId</span></span>|<span data-ttu-id="231f0-132">Guid</span><span class="sxs-lookup"><span data-stu-id="231f0-132">Guid</span></span>|<span data-ttu-id="231f0-p105">此合作关系引用的客户租户的唯一标识符。对应于客户租户的组织资源的 id 属性。</span><span class="sxs-lookup"><span data-stu-id="231f0-p105">The unique identifier for the customer tenant referenced by this partnership. Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="231f0-135">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="231f0-135">defaultDomainName</span></span>|<span data-ttu-id="231f0-136">String</span><span class="sxs-lookup"><span data-stu-id="231f0-136">String</span></span>|<span data-ttu-id="231f0-p106">客户租户的默认域名的副本。与客户建立合作伙伴关系时生成副本。如果客户租户的默认域名更改，此项将不会自动更新。</span><span class="sxs-lookup"><span data-stu-id="231f0-p106">A copy of the customer tenant's default domain name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="231f0-140">displayName</span><span class="sxs-lookup"><span data-stu-id="231f0-140">displayName</span></span>|<span data-ttu-id="231f0-141">String</span><span class="sxs-lookup"><span data-stu-id="231f0-141">String</span></span>|<span data-ttu-id="231f0-p107">客户租户的显示名称的副本。与客户建立合作伙伴关系时生成副本。如果客户租户的显示名称更改，此项将不会自动更新。</span><span class="sxs-lookup"><span data-stu-id="231f0-p107">A copy of the customer tenant's display name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="231f0-145">id</span><span class="sxs-lookup"><span data-stu-id="231f0-145">id</span></span>|<span data-ttu-id="231f0-146">String</span><span class="sxs-lookup"><span data-stu-id="231f0-146">String</span></span>| <span data-ttu-id="231f0-p108">合作伙伴关系的唯一标识符。键，只读。</span><span class="sxs-lookup"><span data-stu-id="231f0-p108">The unique identifier for the partnership. Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="231f0-149">关系</span><span class="sxs-lookup"><span data-stu-id="231f0-149">Relationships</span></span>
<span data-ttu-id="231f0-150">无</span><span class="sxs-lookup"><span data-stu-id="231f0-150">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="231f0-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="231f0-151">JSON representation</span></span>
<span data-ttu-id="231f0-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="231f0-152">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/contract.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
