---
title: modifiedProperty 资源类型
description: 描述在目标系统中执行的更改。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 03ae8cb2c36cb811325839341c0fa8b3f395c954
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35348703"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="33405-103">modifiedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="33405-103">modifiedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33405-104">描述在目标系统中执行的更改。</span><span class="sxs-lookup"><span data-stu-id="33405-104">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="33405-105">属性</span><span class="sxs-lookup"><span data-stu-id="33405-105">Properties</span></span>

| <span data-ttu-id="33405-106">属性</span><span class="sxs-lookup"><span data-stu-id="33405-106">Property</span></span>     | <span data-ttu-id="33405-107">类型</span><span class="sxs-lookup"><span data-stu-id="33405-107">Type</span></span>        | <span data-ttu-id="33405-108">说明</span><span class="sxs-lookup"><span data-stu-id="33405-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="33405-109">displayName</span><span class="sxs-lookup"><span data-stu-id="33405-109">displayName</span></span>|<span data-ttu-id="33405-110">String</span><span class="sxs-lookup"><span data-stu-id="33405-110">String</span></span>|<span data-ttu-id="33405-111">已修改的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="33405-111">Name of property that was modified.</span></span>|
|<span data-ttu-id="33405-112">NewValue</span><span class="sxs-lookup"><span data-stu-id="33405-112">newValue</span></span>|<span data-ttu-id="33405-113">String</span><span class="sxs-lookup"><span data-stu-id="33405-113">String</span></span>|<span data-ttu-id="33405-114">新的属性值。</span><span class="sxs-lookup"><span data-stu-id="33405-114">New property value.</span></span>|
|<span data-ttu-id="33405-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="33405-115">oldValue</span></span>|<span data-ttu-id="33405-116">String</span><span class="sxs-lookup"><span data-stu-id="33405-116">String</span></span>|<span data-ttu-id="33405-117">旧属性值。</span><span class="sxs-lookup"><span data-stu-id="33405-117">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33405-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33405-118">JSON representation</span></span>

<span data-ttu-id="33405-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33405-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
