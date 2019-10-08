---
title: educationMakeCodeResource 资源类型
description: 一个 MakeCode 资源
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5ffab7e11675996e79aed746cfe4624b28e37aab
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418284"
---
# <a name="educationmakecoderesource-resource-type"></a><span data-ttu-id="3e715-103">educationMakeCodeResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e715-103">educationMakeCodeResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e715-104">一个代表[MakeCode](https://www.microsoft.com/en-us/makecode)项目的资源。</span><span class="sxs-lookup"><span data-stu-id="3e715-104">A resource representing a [MakeCode](https://www.microsoft.com/en-us/makecode) project.</span></span>

## <a name="properties"></a><span data-ttu-id="3e715-105">属性</span><span class="sxs-lookup"><span data-stu-id="3e715-105">Properties</span></span>

| <span data-ttu-id="3e715-106">属性</span><span class="sxs-lookup"><span data-stu-id="3e715-106">Property</span></span>     | <span data-ttu-id="3e715-107">类型</span><span class="sxs-lookup"><span data-stu-id="3e715-107">Type</span></span>        | <span data-ttu-id="3e715-108">说明</span><span class="sxs-lookup"><span data-stu-id="3e715-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3e715-109">projectId</span><span class="sxs-lookup"><span data-stu-id="3e715-109">projectId</span></span>|<span data-ttu-id="3e715-110">String</span><span class="sxs-lookup"><span data-stu-id="3e715-110">String</span></span>|<span data-ttu-id="3e715-111">MakeCode 项目的 ID</span><span class="sxs-lookup"><span data-stu-id="3e715-111">ID of the MakeCode project</span></span>|
|<span data-ttu-id="3e715-112">hostWebUrl</span><span class="sxs-lookup"><span data-stu-id="3e715-112">hostWebUrl</span></span>|<span data-ttu-id="3e715-113">String</span><span class="sxs-lookup"><span data-stu-id="3e715-113">String</span></span>|<span data-ttu-id="3e715-114">MakeCode 资源类型的主机（例如，arcade、microbit）</span><span class="sxs-lookup"><span data-stu-id="3e715-114">Host for the type of MakeCode resource (for example, arcade, microbit)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e715-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e715-115">JSON representation</span></span>

<span data-ttu-id="3e715-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e715-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationMakeCodeResource",
  "baseType": "microsoft.graph.educationResource"
}-->

```json
{
  "projectId": "String",
  "hostWebUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationMakeCodeResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->