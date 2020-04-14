---
title: modifiedProperty 资源类型
description: 描述在目标系统中执行的更改。
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 78b2447c1bdeab986382ec2d7c5d20787c1f15e2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459795"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="4a02f-103">modifiedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a02f-103">modifiedProperty resource type</span></span>

<span data-ttu-id="4a02f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a02f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a02f-105">描述在目标系统中执行的更改。</span><span class="sxs-lookup"><span data-stu-id="4a02f-105">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="4a02f-106">属性</span><span class="sxs-lookup"><span data-stu-id="4a02f-106">Properties</span></span>

| <span data-ttu-id="4a02f-107">属性</span><span class="sxs-lookup"><span data-stu-id="4a02f-107">Property</span></span>     | <span data-ttu-id="4a02f-108">类型</span><span class="sxs-lookup"><span data-stu-id="4a02f-108">Type</span></span>        | <span data-ttu-id="4a02f-109">说明</span><span class="sxs-lookup"><span data-stu-id="4a02f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4a02f-110">displayName</span><span class="sxs-lookup"><span data-stu-id="4a02f-110">displayName</span></span>|<span data-ttu-id="4a02f-111">String</span><span class="sxs-lookup"><span data-stu-id="4a02f-111">String</span></span>|<span data-ttu-id="4a02f-112">已修改的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="4a02f-112">Name of property that was modified.</span></span>|
|<span data-ttu-id="4a02f-113">NewValue</span><span class="sxs-lookup"><span data-stu-id="4a02f-113">newValue</span></span>|<span data-ttu-id="4a02f-114">String</span><span class="sxs-lookup"><span data-stu-id="4a02f-114">String</span></span>|<span data-ttu-id="4a02f-115">新的属性值。</span><span class="sxs-lookup"><span data-stu-id="4a02f-115">New property value.</span></span>|
|<span data-ttu-id="4a02f-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="4a02f-116">oldValue</span></span>|<span data-ttu-id="4a02f-117">String</span><span class="sxs-lookup"><span data-stu-id="4a02f-117">String</span></span>|<span data-ttu-id="4a02f-118">旧属性值。</span><span class="sxs-lookup"><span data-stu-id="4a02f-118">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a02f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a02f-119">JSON representation</span></span>

<span data-ttu-id="4a02f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a02f-120">The following is a JSON representation of the resource.</span></span>

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
