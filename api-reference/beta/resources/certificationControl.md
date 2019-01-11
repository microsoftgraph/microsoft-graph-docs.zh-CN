---
title: " certificationControl 资源类型"
description: 此资源包含合规性与关联的证书数据安全分数控件。
localization_priority: Normal
ms.openlocfilehash: 6f8269a85a8d3cb032f3e58457df95f4dd432c11
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810386"
---
#  <a name="certificationcontrol-resource-type"></a><span data-ttu-id="5eae5-103">certificationControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="5eae5-103">certificationControl resource type</span></span>

<span data-ttu-id="5eae5-104">包含合规性与关联的证书数据安全分数控件。</span><span class="sxs-lookup"><span data-stu-id="5eae5-104">Contains compliance certification data associated with secure score control.</span></span>

|<span data-ttu-id="5eae5-105">属性</span><span class="sxs-lookup"><span data-stu-id="5eae5-105">Property</span></span> |<span data-ttu-id="5eae5-106">类型</span><span class="sxs-lookup"><span data-stu-id="5eae5-106">Type</span></span> |<span data-ttu-id="5eae5-107">说明</span><span class="sxs-lookup"><span data-stu-id="5eae5-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="5eae5-108">name</span><span class="sxs-lookup"><span data-stu-id="5eae5-108">name</span></span> | <span data-ttu-id="5eae5-109">string</span><span class="sxs-lookup"><span data-stu-id="5eae5-109">string</span></span> | <span data-ttu-id="5eae5-110">证书控件名称</span><span class="sxs-lookup"><span data-stu-id="5eae5-110">Certification control name</span></span> |
|<span data-ttu-id="5eae5-111">url</span><span class="sxs-lookup"><span data-stu-id="5eae5-111">url</span></span> | <span data-ttu-id="5eae5-112">string</span><span class="sxs-lookup"><span data-stu-id="5eae5-112">string</span></span> | <span data-ttu-id="5eae5-113">Microsoft 服务的 URL 信任门户</span><span class="sxs-lookup"><span data-stu-id="5eae5-113">URL for the Microsoft Service Trust Portal</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5eae5-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5eae5-114">JSON representation</span></span>

<span data-ttu-id="5eae5-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5eae5-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificationControl"
}-->

```json
{
  "name": "String",
  "url": "Collection(microsoft.graph.certificationControl)"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "certificationControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
