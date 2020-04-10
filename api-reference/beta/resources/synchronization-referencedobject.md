---
title: referencedObject 资源类型
description: 描述对在同一目录定义中定义的另一个对象的引用。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7779fb851812c00c15749877517b79273752ab58
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217589"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="b9c29-103">referencedObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9c29-103">referencedObject resource type</span></span>

<span data-ttu-id="b9c29-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9c29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9c29-105">描述对在同一[目录定义](synchronization-directorydefinition.md)中定义的另一个对象的引用。</span><span class="sxs-lookup"><span data-stu-id="b9c29-105">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b9c29-106">属性</span><span class="sxs-lookup"><span data-stu-id="b9c29-106">Properties</span></span>

| <span data-ttu-id="b9c29-107">属性</span><span class="sxs-lookup"><span data-stu-id="b9c29-107">Property</span></span>                   | <span data-ttu-id="b9c29-108">类型</span><span class="sxs-lookup"><span data-stu-id="b9c29-108">Type</span></span>                      | <span data-ttu-id="b9c29-109">说明</span><span class="sxs-lookup"><span data-stu-id="b9c29-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="b9c29-110">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="b9c29-110">referencedObjectName</span></span>        |<span data-ttu-id="b9c29-111">字符串</span><span class="sxs-lookup"><span data-stu-id="b9c29-111">String</span></span>                     |<span data-ttu-id="b9c29-112">引用的对象的名称。</span><span class="sxs-lookup"><span data-stu-id="b9c29-112">Name of the referenced object.</span></span> <span data-ttu-id="b9c29-113">必须与[目录定义](synchronization-directorydefinition.md)中的一个对象相匹配。</span><span class="sxs-lookup"><span data-stu-id="b9c29-113">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="b9c29-114">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="b9c29-114">referencedProperty</span></span>          |<span data-ttu-id="b9c29-115">字符串</span><span class="sxs-lookup"><span data-stu-id="b9c29-115">String</span></span>                     |<span data-ttu-id="b9c29-116">**目前不支持**。</span><span class="sxs-lookup"><span data-stu-id="b9c29-116">**Currently not supported**.</span></span> <span data-ttu-id="b9c29-117">引用的对象中属性的名称，其值将用作引用。</span><span class="sxs-lookup"><span data-stu-id="b9c29-117">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9c29-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9c29-118">JSON representation</span></span>

<span data-ttu-id="b9c29-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9c29-119">The following is a JSON representation of the resource.</span></span>

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
            
