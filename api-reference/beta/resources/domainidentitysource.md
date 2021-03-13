---
title: domainIdentitySource 资源类型
description: domainIdentitySource 类型将非租户域标识为已连接组织的标识源。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ae616c98b2ca20ec4e5d9c7aceeba5bdeb538e81
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759662"
---
# <a name="domainidentitysource-resource-type"></a><span data-ttu-id="751c3-103">domainIdentitySource 资源类型</span><span class="sxs-lookup"><span data-stu-id="751c3-103">domainIdentitySource resource type</span></span>

<span data-ttu-id="751c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="751c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="751c3-105">在 [connectedOrganization 的标识源中使用](connectedOrganization.md)。</span><span class="sxs-lookup"><span data-stu-id="751c3-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="751c3-106">`@odata.type`该值 `#microsoft.graph.domainIdentitySource` 指示此类型将域标识为已连接组织的标识源。</span><span class="sxs-lookup"><span data-stu-id="751c3-106">The `@odata.type` value `#microsoft.graph.domainIdentitySource` indicates that this type identifies a domain as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="751c3-107">属性</span><span class="sxs-lookup"><span data-stu-id="751c3-107">Properties</span></span>

| <span data-ttu-id="751c3-108">属性</span><span class="sxs-lookup"><span data-stu-id="751c3-108">Property</span></span>                     | <span data-ttu-id="751c3-109">类型</span><span class="sxs-lookup"><span data-stu-id="751c3-109">Type</span></span>                      | <span data-ttu-id="751c3-110">说明</span><span class="sxs-lookup"><span data-stu-id="751c3-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="751c3-111">displayName</span><span class="sxs-lookup"><span data-stu-id="751c3-111">displayName</span></span> |<span data-ttu-id="751c3-112">String</span><span class="sxs-lookup"><span data-stu-id="751c3-112">String</span></span> | <span data-ttu-id="751c3-113">标识源的名称，通常也是域名。</span><span class="sxs-lookup"><span data-stu-id="751c3-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="751c3-114">只读。</span><span class="sxs-lookup"><span data-stu-id="751c3-114">Read only.</span></span> |
| <span data-ttu-id="751c3-115">domainName</span><span class="sxs-lookup"><span data-stu-id="751c3-115">domainName</span></span> |<span data-ttu-id="751c3-116">String</span><span class="sxs-lookup"><span data-stu-id="751c3-116">String</span></span> | <span data-ttu-id="751c3-117">域名。</span><span class="sxs-lookup"><span data-stu-id="751c3-117">The domain name.</span></span> <span data-ttu-id="751c3-118">只读。</span><span class="sxs-lookup"><span data-stu-id="751c3-118">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="751c3-119">关系</span><span class="sxs-lookup"><span data-stu-id="751c3-119">Relationships</span></span>

<span data-ttu-id="751c3-120">无。</span><span class="sxs-lookup"><span data-stu-id="751c3-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="751c3-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="751c3-121">JSON representation</span></span>

<span data-ttu-id="751c3-122">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="751c3-122">The following is a JSON representation of the type.</span></span>

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


