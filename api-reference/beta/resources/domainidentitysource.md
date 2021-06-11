---
title: domainIdentitySource 资源类型
description: domainIdentitySource 类型将非租户域标识为已连接组织的标识源。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2c558213b7198da65eaacdbf0ac42915f3638c56
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896170"
---
# <a name="domainidentitysource-resource-type"></a><span data-ttu-id="badb2-103">domainIdentitySource 资源类型</span><span class="sxs-lookup"><span data-stu-id="badb2-103">domainIdentitySource resource type</span></span>

<span data-ttu-id="badb2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="badb2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="badb2-105">在 [connectedOrganization 的标识源中使用](connectedOrganization.md)。</span><span class="sxs-lookup"><span data-stu-id="badb2-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="badb2-106">`@odata.type`该值 `#microsoft.graph.domainIdentitySource` 指示此类型将域标识为已连接组织的标识源。</span><span class="sxs-lookup"><span data-stu-id="badb2-106">The `@odata.type` value `#microsoft.graph.domainIdentitySource` indicates that this type identifies a domain as an identity source for a connected organization.</span></span>

<span data-ttu-id="badb2-107">创建新的[connectedOrganization](../api/connectedorganization-post.md)时，如果调用方在 identitySources 集合中提供 domainIdentitySource，并且域对应于 Azure Active Directory 租户的注册域，则创建的生成的 connectedOrganization 将具有包含[azureActiveDirectoryTenant](azureactivedirectorytenant.md)类型的单个成员的 identitySources 集合。</span><span class="sxs-lookup"><span data-stu-id="badb2-107">When [creating a new connectedOrganization](../api/connectedorganization-post.md), if the caller provides in the identitySources collection a domainIdentitySource and the domain corresponds to a registered domain of an Azure Active Directory tenant, then the resulting connectedOrganization that is created will have an identitySources collection containing a single member of the [azureActiveDirectoryTenant](azureactivedirectorytenant.md) type.</span></span>

## <a name="properties"></a><span data-ttu-id="badb2-108">属性</span><span class="sxs-lookup"><span data-stu-id="badb2-108">Properties</span></span>

| <span data-ttu-id="badb2-109">属性</span><span class="sxs-lookup"><span data-stu-id="badb2-109">Property</span></span>                     | <span data-ttu-id="badb2-110">类型</span><span class="sxs-lookup"><span data-stu-id="badb2-110">Type</span></span>                      | <span data-ttu-id="badb2-111">说明</span><span class="sxs-lookup"><span data-stu-id="badb2-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="badb2-112">displayName</span><span class="sxs-lookup"><span data-stu-id="badb2-112">displayName</span></span> |<span data-ttu-id="badb2-113">String</span><span class="sxs-lookup"><span data-stu-id="badb2-113">String</span></span> | <span data-ttu-id="badb2-114">标识源的名称，通常也是域名。</span><span class="sxs-lookup"><span data-stu-id="badb2-114">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="badb2-115">只读。</span><span class="sxs-lookup"><span data-stu-id="badb2-115">Read only.</span></span> |
| <span data-ttu-id="badb2-116">domainName</span><span class="sxs-lookup"><span data-stu-id="badb2-116">domainName</span></span> |<span data-ttu-id="badb2-117">String</span><span class="sxs-lookup"><span data-stu-id="badb2-117">String</span></span> | <span data-ttu-id="badb2-118">域名。</span><span class="sxs-lookup"><span data-stu-id="badb2-118">The domain name.</span></span> <span data-ttu-id="badb2-119">只读。</span><span class="sxs-lookup"><span data-stu-id="badb2-119">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="badb2-120">关系</span><span class="sxs-lookup"><span data-stu-id="badb2-120">Relationships</span></span>

<span data-ttu-id="badb2-121">无。</span><span class="sxs-lookup"><span data-stu-id="badb2-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="badb2-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="badb2-122">JSON representation</span></span>

<span data-ttu-id="badb2-123">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="badb2-123">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainIdentitySource",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainIdentitySource resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


