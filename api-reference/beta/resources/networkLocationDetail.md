---
title: networkLocationDetail 资源类型
description: 提供用户登录时所采用的网络的名称和类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8cbf60f7e7e370c5813623643f9d14cb324950cc
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939507"
---
# <a name="networklocationdetail-resource-type"></a><span data-ttu-id="5d973-103">networkLocationDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="5d973-103">networkLocationDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d973-104">提供用户登录时所采用的网络的名称和类型。</span><span class="sxs-lookup"><span data-stu-id="5d973-104">Provides the name and type of network from which the user signed in.</span></span>

## <a name="properties"></a><span data-ttu-id="5d973-105">属性</span><span class="sxs-lookup"><span data-stu-id="5d973-105">Properties</span></span>

| <span data-ttu-id="5d973-106">属性</span><span class="sxs-lookup"><span data-stu-id="5d973-106">Property</span></span>     | <span data-ttu-id="5d973-107">类型</span><span class="sxs-lookup"><span data-stu-id="5d973-107">Type</span></span>        | <span data-ttu-id="5d973-108">描述</span><span class="sxs-lookup"><span data-stu-id="5d973-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5d973-109">networkNames</span><span class="sxs-lookup"><span data-stu-id="5d973-109">networkNames</span></span>|<span data-ttu-id="5d973-110">String collection</span><span class="sxs-lookup"><span data-stu-id="5d973-110">String collection</span></span>|<span data-ttu-id="5d973-111">提供登录时使用的网络的名称。</span><span class="sxs-lookup"><span data-stu-id="5d973-111">Provides the name of the network used when signing in.</span></span>|
|<span data-ttu-id="5d973-112">网络</span><span class="sxs-lookup"><span data-stu-id="5d973-112">networkType</span></span>|<span data-ttu-id="5d973-113">网络</span><span class="sxs-lookup"><span data-stu-id="5d973-113">networkType</span></span>| <span data-ttu-id="5d973-114">提供登录时使用的网络类型。</span><span class="sxs-lookup"><span data-stu-id="5d973-114">Provides the type of network used when signing in.</span></span> <span data-ttu-id="5d973-115">可取值为：`intranet`、`extranet`、`namedNetwork`、`trusted`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="5d973-115">Possible values are: `intranet`, `extranet`, `namedNetwork`, `trusted`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5d973-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5d973-116">JSON representation</span></span>

<span data-ttu-id="5d973-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d973-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkLocationDetail",
  "baseType": null
}-->

```json
{
  "networkNames": ["String"],
  "networkType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkLocationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->