---
title: referencedObject 资源类型
description: 描述对在同一目录定义中定义的另一个对象的引用。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c1c7e1554764031efbfa3a5d1c1280f4b72bc160
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007856"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="99393-103">referencedObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="99393-103">referencedObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99393-104">描述对在同一[目录定义](synchronization-directorydefinition.md)中定义的另一个对象的引用。</span><span class="sxs-lookup"><span data-stu-id="99393-104">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="99393-105">属性</span><span class="sxs-lookup"><span data-stu-id="99393-105">Properties</span></span>

| <span data-ttu-id="99393-106">属性</span><span class="sxs-lookup"><span data-stu-id="99393-106">Property</span></span>                   | <span data-ttu-id="99393-107">类型</span><span class="sxs-lookup"><span data-stu-id="99393-107">Type</span></span>                      | <span data-ttu-id="99393-108">说明</span><span class="sxs-lookup"><span data-stu-id="99393-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="99393-109">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="99393-109">referencedObjectName</span></span>        |<span data-ttu-id="99393-110">String</span><span class="sxs-lookup"><span data-stu-id="99393-110">String</span></span>                     |<span data-ttu-id="99393-111">引用的对象的名称。</span><span class="sxs-lookup"><span data-stu-id="99393-111">Name of the referenced object.</span></span> <span data-ttu-id="99393-112">必须与[目录定义](synchronization-directorydefinition.md)中的一个对象相匹配。</span><span class="sxs-lookup"><span data-stu-id="99393-112">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="99393-113">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="99393-113">referencedProperty</span></span>          |<span data-ttu-id="99393-114">String</span><span class="sxs-lookup"><span data-stu-id="99393-114">String</span></span>                     |<span data-ttu-id="99393-115">**目前不支持**。</span><span class="sxs-lookup"><span data-stu-id="99393-115">**Currently not supported**.</span></span> <span data-ttu-id="99393-116">引用的对象中属性的名称, 其值将用作引用。</span><span class="sxs-lookup"><span data-stu-id="99393-116">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99393-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99393-117">JSON representation</span></span>

<span data-ttu-id="99393-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99393-118">The following is a JSON representation of the resource.</span></span>

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
            
