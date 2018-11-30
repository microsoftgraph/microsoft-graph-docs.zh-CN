---
title: referencedObject 资源类型
description: 介绍在相同的目录定义中定义的另一个对象的引用。
ms.openlocfilehash: 63645048fd8ba6ad949da43baa261b2842ea4016
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048703"
---
# <a name="referencedobject-resource-type"></a><span data-ttu-id="8708b-103">referencedObject 资源类型</span><span class="sxs-lookup"><span data-stu-id="8708b-103">referencedObject resource type</span></span>

> <span data-ttu-id="8708b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8708b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8708b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8708b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8708b-106">介绍在相同的[目录定义](synchronization-directorydefinition.md)中定义的另一个对象的引用。</span><span class="sxs-lookup"><span data-stu-id="8708b-106">Describes a reference to another object defined in the same [directory definition](synchronization-directorydefinition.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8708b-107">属性</span><span class="sxs-lookup"><span data-stu-id="8708b-107">Properties</span></span>

| <span data-ttu-id="8708b-108">属性</span><span class="sxs-lookup"><span data-stu-id="8708b-108">Property</span></span>                   | <span data-ttu-id="8708b-109">类型</span><span class="sxs-lookup"><span data-stu-id="8708b-109">Type</span></span>                      | <span data-ttu-id="8708b-110">说明</span><span class="sxs-lookup"><span data-stu-id="8708b-110">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="8708b-111">referencedObjectName</span><span class="sxs-lookup"><span data-stu-id="8708b-111">referencedObjectName</span></span>        |<span data-ttu-id="8708b-112">字符串</span><span class="sxs-lookup"><span data-stu-id="8708b-112">String</span></span>                     |<span data-ttu-id="8708b-113">引用对象的名称。</span><span class="sxs-lookup"><span data-stu-id="8708b-113">Name of the referenced object.</span></span> <span data-ttu-id="8708b-114">必须匹配一个[目录定义](synchronization-directorydefinition.md)中的对象。</span><span class="sxs-lookup"><span data-stu-id="8708b-114">Must match one of the objects in the [directory definition](synchronization-directorydefinition.md).</span></span>|
|<span data-ttu-id="8708b-115">referencedProperty</span><span class="sxs-lookup"><span data-stu-id="8708b-115">referencedProperty</span></span>          |<span data-ttu-id="8708b-116">字符串</span><span class="sxs-lookup"><span data-stu-id="8708b-116">String</span></span>                     |<span data-ttu-id="8708b-117">**当前不支持**。</span><span class="sxs-lookup"><span data-stu-id="8708b-117">**Currently not supported**.</span></span> <span data-ttu-id="8708b-118">中引用的对象，其中的值用作引用的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="8708b-118">Name of the property in the referenced object, the value for which is used as the reference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8708b-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8708b-119">JSON representation</span></span>

<span data-ttu-id="8708b-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8708b-120">The following is a JSON representation of the resource.</span></span>

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
            