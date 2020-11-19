---
title: conditionalAccessApplications 资源类型
description: 表示策略作用域中包含和排除的应用程序和用户操作。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ba904fec35830bef6cc5a74daa1c4938bd99d250
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49269908"
---
# <a name="conditionalaccessapplications-resource-type"></a><span data-ttu-id="90cc8-103">conditionalAccessApplications 资源类型</span><span class="sxs-lookup"><span data-stu-id="90cc8-103">conditionalAccessApplications resource type</span></span>

<span data-ttu-id="90cc8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90cc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90cc8-105">表示策略中包含和排除的应用程序和用户操作。</span><span class="sxs-lookup"><span data-stu-id="90cc8-105">Represents the applications and user actions included in and excluded from the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="90cc8-106">属性</span><span class="sxs-lookup"><span data-stu-id="90cc8-106">Properties</span></span>

| <span data-ttu-id="90cc8-107">属性</span><span class="sxs-lookup"><span data-stu-id="90cc8-107">Property</span></span> | <span data-ttu-id="90cc8-108">类型</span><span class="sxs-lookup"><span data-stu-id="90cc8-108">Type</span></span> | <span data-ttu-id="90cc8-109">说明</span><span class="sxs-lookup"><span data-stu-id="90cc8-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="90cc8-110">includeApplications</span><span class="sxs-lookup"><span data-stu-id="90cc8-110">includeApplications</span></span> | <span data-ttu-id="90cc8-111">String 集合</span><span class="sxs-lookup"><span data-stu-id="90cc8-111">String collection</span></span> | <span data-ttu-id="90cc8-112">该策略应用于的应用程序 Id 列表，除非在 excludeApplications) 中显式排除 (。</span><span class="sxs-lookup"><span data-stu-id="90cc8-112">The list of application IDs the policy applies to, unless explicitly excluded (in excludeApplications).</span></span> <span data-ttu-id="90cc8-113">也可以将设置为 `All` 。</span><span class="sxs-lookup"><span data-stu-id="90cc8-113">Can also be set to `All`.</span></span> |
| <span data-ttu-id="90cc8-114">excludeApplications</span><span class="sxs-lookup"><span data-stu-id="90cc8-114">excludeApplications</span></span> | <span data-ttu-id="90cc8-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="90cc8-115">String collection</span></span> | <span data-ttu-id="90cc8-116">从策略中显式排除的应用程序 Id 的列表。</span><span class="sxs-lookup"><span data-stu-id="90cc8-116">The list of application IDs explicitly excluded from the policy.</span></span> |
| <span data-ttu-id="90cc8-117">includeUserActions</span><span class="sxs-lookup"><span data-stu-id="90cc8-117">includeUserActions</span></span> | <span data-ttu-id="90cc8-118">String 集合</span><span class="sxs-lookup"><span data-stu-id="90cc8-118">String collection</span></span> | <span data-ttu-id="90cc8-119">要包括的用户操作。</span><span class="sxs-lookup"><span data-stu-id="90cc8-119">User actions to include.</span></span> <span data-ttu-id="90cc8-120">支持的值为 `urn:user:registersecurityinfo` 和 `urn:user:registerdevice`</span><span class="sxs-lookup"><span data-stu-id="90cc8-120">Supported values are `urn:user:registersecurityinfo` and `urn:user:registerdevice`</span></span> |

## <a name="relationships"></a><span data-ttu-id="90cc8-121">关系</span><span class="sxs-lookup"><span data-stu-id="90cc8-121">Relationships</span></span>

<span data-ttu-id="90cc8-122">无。</span><span class="sxs-lookup"><span data-stu-id="90cc8-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="90cc8-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90cc8-123">JSON representation</span></span>

<span data-ttu-id="90cc8-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90cc8-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeApplications",
    "excludeApplications",
    "includeUserActions"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessApplications"
}-->

```json
{
  "includeApplications": ["String"],
  "excludeApplications": ["String"],
  "includeUserActions": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessApplications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

