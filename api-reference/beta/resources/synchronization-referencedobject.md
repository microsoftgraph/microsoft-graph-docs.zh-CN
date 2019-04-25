---
title: referencedObject 资源类型
description: 描述对在同一目录定义中定义的另一个对象的引用。
localization_priority: Normal
ms.openlocfilehash: dcec232335fdf3d447097ea1ae87fbc9ea676cfe
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523235"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="c5876-103">referencedObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5876-103">referencedObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5876-104">描述对在同一[目录定义](synchronization-directorydefinition.md)中定义的另一个对象的引用。</span><span class="sxs-lookup"><span data-stu-id="c5876-104">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c5876-105">属性</span><span class="sxs-lookup"><span data-stu-id="c5876-105">Properties</span></span>

| <span data-ttu-id="c5876-106">属性</span><span class="sxs-lookup"><span data-stu-id="c5876-106">Property</span></span>                   | <span data-ttu-id="c5876-107">类型</span><span class="sxs-lookup"><span data-stu-id="c5876-107">Type</span></span>                      | <span data-ttu-id="c5876-108">说明</span><span class="sxs-lookup"><span data-stu-id="c5876-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="c5876-109">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="c5876-109">referencedObjectName</span></span>        |<span data-ttu-id="c5876-110">String</span><span class="sxs-lookup"><span data-stu-id="c5876-110">String</span></span>                     |<span data-ttu-id="c5876-111">引用的对象的名称。</span><span class="sxs-lookup"><span data-stu-id="c5876-111">Name of the referenced object.</span></span> <span data-ttu-id="c5876-112">必须与[目录定义](synchronization-directorydefinition.md)中的一个对象相匹配。</span><span class="sxs-lookup"><span data-stu-id="c5876-112">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="c5876-113">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="c5876-113">referencedProperty</span></span>          |<span data-ttu-id="c5876-114">String</span><span class="sxs-lookup"><span data-stu-id="c5876-114">String</span></span>                     |<span data-ttu-id="c5876-115">**目前不支持**。</span><span class="sxs-lookup"><span data-stu-id="c5876-115">**Currently not supported**.</span></span> <span data-ttu-id="c5876-116">引用的对象中属性的名称, 其值将用作引用。</span><span class="sxs-lookup"><span data-stu-id="c5876-116">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5876-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5876-117">JSON representation</span></span>

<span data-ttu-id="c5876-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5876-118">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-referencedobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
            
