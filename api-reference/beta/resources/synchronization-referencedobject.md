---
title: referencedObject 资源类型
description: 介绍在相同的目录定义中定义的另一个对象的引用。
localization_priority: Normal
ms.openlocfilehash: 5a2aa2dcc358c856c18ea2ce9871ec634194ce54
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821033"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="c3de4-103">referencedObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3de4-103">referencedObject resource type</span></span>

> <span data-ttu-id="c3de4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c3de4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3de4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c3de4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3de4-106">介绍在相同的[目录定义](synchronization-directorydefinition.md)中定义的另一个对象的引用。</span><span class="sxs-lookup"><span data-stu-id="c3de4-106">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c3de4-107">属性</span><span class="sxs-lookup"><span data-stu-id="c3de4-107">Properties</span></span>

| <span data-ttu-id="c3de4-108">属性</span><span class="sxs-lookup"><span data-stu-id="c3de4-108">Property</span></span>                   | <span data-ttu-id="c3de4-109">类型</span><span class="sxs-lookup"><span data-stu-id="c3de4-109">Type</span></span>                      | <span data-ttu-id="c3de4-110">Description</span><span class="sxs-lookup"><span data-stu-id="c3de4-110">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="c3de4-111">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="c3de4-111">referencedObjectName</span></span>        |<span data-ttu-id="c3de4-112">字符串</span><span class="sxs-lookup"><span data-stu-id="c3de4-112">String</span></span>                     |<span data-ttu-id="c3de4-113">引用对象的名称。</span><span class="sxs-lookup"><span data-stu-id="c3de4-113">Name of the referenced object.</span></span> <span data-ttu-id="c3de4-114">必须匹配一个[目录定义](synchronization-directorydefinition.md)中的对象。</span><span class="sxs-lookup"><span data-stu-id="c3de4-114">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="c3de4-115">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="c3de4-115">referencedProperty</span></span>          |<span data-ttu-id="c3de4-116">字符串</span><span class="sxs-lookup"><span data-stu-id="c3de4-116">String</span></span>                     |<span data-ttu-id="c3de4-117">**当前不支持**。</span><span class="sxs-lookup"><span data-stu-id="c3de4-117">**Currently not supported**.</span></span> <span data-ttu-id="c3de4-118">中引用的对象，其中的值用作引用的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="c3de4-118">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3de4-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3de4-119">JSON representation</span></span>

<span data-ttu-id="c3de4-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3de4-120">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "referencedObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
            
