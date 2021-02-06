---
title: referencedObject 资源类型
description: 描述对同一目录定义中定义的另一个对象的引用。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c6e273474c70919bab3c30335a26477509eca8cc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132520"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="9b021-103">referencedObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b021-103">referencedObject resource type</span></span>

<span data-ttu-id="9b021-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b021-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b021-105">描述对同一目录定义中定义的另 [一个对象的引用](synchronization-directorydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="9b021-105">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9b021-106">属性</span><span class="sxs-lookup"><span data-stu-id="9b021-106">Properties</span></span>

| <span data-ttu-id="9b021-107">属性</span><span class="sxs-lookup"><span data-stu-id="9b021-107">Property</span></span>                   | <span data-ttu-id="9b021-108">类型</span><span class="sxs-lookup"><span data-stu-id="9b021-108">Type</span></span>                      | <span data-ttu-id="9b021-109">说明</span><span class="sxs-lookup"><span data-stu-id="9b021-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="9b021-110">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="9b021-110">referencedObjectName</span></span>        |<span data-ttu-id="9b021-111">字符串</span><span class="sxs-lookup"><span data-stu-id="9b021-111">String</span></span>                     |<span data-ttu-id="9b021-112">引用的对象的名称。</span><span class="sxs-lookup"><span data-stu-id="9b021-112">Name of the referenced object.</span></span> <span data-ttu-id="9b021-113">必须与目录定义中的对象 [之一匹配](synchronization-directorydefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="9b021-113">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="9b021-114">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="9b021-114">referencedProperty</span></span>          |<span data-ttu-id="9b021-115">字符串</span><span class="sxs-lookup"><span data-stu-id="9b021-115">String</span></span>                     |<span data-ttu-id="9b021-116">**当前不受支持**。</span><span class="sxs-lookup"><span data-stu-id="9b021-116">**Currently not supported**.</span></span> <span data-ttu-id="9b021-117">引用对象中的属性的名称，用作引用的值。</span><span class="sxs-lookup"><span data-stu-id="9b021-117">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9b021-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b021-118">JSON representation</span></span>

<span data-ttu-id="9b021-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b021-119">The following is a JSON representation of the resource.</span></span>

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
            


