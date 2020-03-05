---
title: referencedObject 资源类型
description: 描述对在同一目录定义中定义的另一个对象的引用。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6c27830b1ee9762b52a7f24a0785e1b19010181d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520119"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="7928f-103">referencedObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="7928f-103">referencedObject resource type</span></span>

<span data-ttu-id="7928f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7928f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7928f-105">描述对在同一[目录定义](synchronization-directorydefinition.md)中定义的另一个对象的引用。</span><span class="sxs-lookup"><span data-stu-id="7928f-105">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7928f-106">属性</span><span class="sxs-lookup"><span data-stu-id="7928f-106">Properties</span></span>

| <span data-ttu-id="7928f-107">属性</span><span class="sxs-lookup"><span data-stu-id="7928f-107">Property</span></span>                   | <span data-ttu-id="7928f-108">类型</span><span class="sxs-lookup"><span data-stu-id="7928f-108">Type</span></span>                      | <span data-ttu-id="7928f-109">说明</span><span class="sxs-lookup"><span data-stu-id="7928f-109">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="7928f-110">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="7928f-110">referencedObjectName</span></span>        |<span data-ttu-id="7928f-111">String</span><span class="sxs-lookup"><span data-stu-id="7928f-111">String</span></span>                     |<span data-ttu-id="7928f-112">引用的对象的名称。</span><span class="sxs-lookup"><span data-stu-id="7928f-112">Name of the referenced object.</span></span> <span data-ttu-id="7928f-113">必须与[目录定义](synchronization-directorydefinition.md)中的一个对象相匹配。</span><span class="sxs-lookup"><span data-stu-id="7928f-113">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="7928f-114">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="7928f-114">referencedProperty</span></span>          |<span data-ttu-id="7928f-115">String</span><span class="sxs-lookup"><span data-stu-id="7928f-115">String</span></span>                     |<span data-ttu-id="7928f-116">**目前不支持**。</span><span class="sxs-lookup"><span data-stu-id="7928f-116">**Currently not supported**.</span></span> <span data-ttu-id="7928f-117">引用的对象中属性的名称，其值将用作引用。</span><span class="sxs-lookup"><span data-stu-id="7928f-117">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7928f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7928f-118">JSON representation</span></span>

<span data-ttu-id="7928f-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7928f-119">The following is a JSON representation of the resource.</span></span>

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
            
