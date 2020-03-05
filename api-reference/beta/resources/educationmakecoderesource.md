---
title: educationMakeCodeResource 资源类型
description: 一个 MakeCode 资源
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 708efc4e72abeba9ff0acfe6e4768c61518e1a6b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501708"
---
# <a name="educationmakecoderesource-resource-type"></a><span data-ttu-id="243e8-103">educationMakeCodeResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="243e8-103">educationMakeCodeResource resource type</span></span>

<span data-ttu-id="243e8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="243e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="243e8-105">一个代表[MakeCode](https://www.microsoft.com/en-us/makecode)项目的资源。</span><span class="sxs-lookup"><span data-stu-id="243e8-105">A resource representing a [MakeCode](https://www.microsoft.com/en-us/makecode) project.</span></span>

## <a name="properties"></a><span data-ttu-id="243e8-106">属性</span><span class="sxs-lookup"><span data-stu-id="243e8-106">Properties</span></span>

| <span data-ttu-id="243e8-107">属性</span><span class="sxs-lookup"><span data-stu-id="243e8-107">Property</span></span>     | <span data-ttu-id="243e8-108">类型</span><span class="sxs-lookup"><span data-stu-id="243e8-108">Type</span></span>        | <span data-ttu-id="243e8-109">说明</span><span class="sxs-lookup"><span data-stu-id="243e8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="243e8-110">projectId</span><span class="sxs-lookup"><span data-stu-id="243e8-110">projectId</span></span>|<span data-ttu-id="243e8-111">String</span><span class="sxs-lookup"><span data-stu-id="243e8-111">String</span></span>|<span data-ttu-id="243e8-112">MakeCode 项目的 ID</span><span class="sxs-lookup"><span data-stu-id="243e8-112">ID of the MakeCode project</span></span>|
|<span data-ttu-id="243e8-113">hostWebUrl</span><span class="sxs-lookup"><span data-stu-id="243e8-113">hostWebUrl</span></span>|<span data-ttu-id="243e8-114">String</span><span class="sxs-lookup"><span data-stu-id="243e8-114">String</span></span>|<span data-ttu-id="243e8-115">MakeCode 资源类型的主机（例如，arcade、microbit）</span><span class="sxs-lookup"><span data-stu-id="243e8-115">Host for the type of MakeCode resource (for example, arcade, microbit)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="243e8-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="243e8-116">JSON representation</span></span>

<span data-ttu-id="243e8-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="243e8-117">The following is a JSON representation of the resource.</span></span>

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