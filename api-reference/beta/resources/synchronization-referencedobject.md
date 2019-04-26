---
title: referencedObject 资源类型
description: 描述对在同一目录定义中定义的另一个对象的引用。
localization_priority: Normal
ms.openlocfilehash: 185691c970a5555d23b7b349cef546fb85be0893
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345582"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="778f5-103">referencedObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="778f5-103">referencedObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="778f5-104">描述对在同一[目录定义](synchronization-directorydefinition.md)中定义的另一个对象的引用。</span><span class="sxs-lookup"><span data-stu-id="778f5-104">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="778f5-105">属性</span><span class="sxs-lookup"><span data-stu-id="778f5-105">Properties</span></span>

| <span data-ttu-id="778f5-106">属性</span><span class="sxs-lookup"><span data-stu-id="778f5-106">Property</span></span>                   | <span data-ttu-id="778f5-107">类型</span><span class="sxs-lookup"><span data-stu-id="778f5-107">Type</span></span>                      | <span data-ttu-id="778f5-108">说明</span><span class="sxs-lookup"><span data-stu-id="778f5-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="778f5-109">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="778f5-109">referencedObjectName</span></span>        |<span data-ttu-id="778f5-110">String</span><span class="sxs-lookup"><span data-stu-id="778f5-110">String</span></span>                     |<span data-ttu-id="778f5-111">引用的对象的名称。</span><span class="sxs-lookup"><span data-stu-id="778f5-111">Name of the referenced object.</span></span> <span data-ttu-id="778f5-112">必须与[目录定义](synchronization-directorydefinition.md)中的一个对象相匹配。</span><span class="sxs-lookup"><span data-stu-id="778f5-112">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="778f5-113">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="778f5-113">referencedProperty</span></span>          |<span data-ttu-id="778f5-114">String</span><span class="sxs-lookup"><span data-stu-id="778f5-114">String</span></span>                     |<span data-ttu-id="778f5-115">**目前不支持**。</span><span class="sxs-lookup"><span data-stu-id="778f5-115">**Currently not supported**.</span></span> <span data-ttu-id="778f5-116">引用的对象中属性的名称, 其值将用作引用。</span><span class="sxs-lookup"><span data-stu-id="778f5-116">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="778f5-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="778f5-117">JSON representation</span></span>

<span data-ttu-id="778f5-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="778f5-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referencedObject"
}-->

```json
{
  "referencedObjectName": "String",
  "referencedProperty": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
            
