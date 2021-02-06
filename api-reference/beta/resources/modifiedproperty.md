---
title: modifiedProperty 资源类型
description: 描述在目标系统中执行的更改。
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 49c2af65022d6fddef394423b6d615dba9f20efc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136176"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="5faa5-103">modifiedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="5faa5-103">modifiedProperty resource type</span></span>

<span data-ttu-id="5faa5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5faa5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5faa5-105">描述在目标系统中执行的更改。</span><span class="sxs-lookup"><span data-stu-id="5faa5-105">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="5faa5-106">属性</span><span class="sxs-lookup"><span data-stu-id="5faa5-106">Properties</span></span>

| <span data-ttu-id="5faa5-107">属性</span><span class="sxs-lookup"><span data-stu-id="5faa5-107">Property</span></span>     | <span data-ttu-id="5faa5-108">类型</span><span class="sxs-lookup"><span data-stu-id="5faa5-108">Type</span></span>        | <span data-ttu-id="5faa5-109">说明</span><span class="sxs-lookup"><span data-stu-id="5faa5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5faa5-110">displayName</span><span class="sxs-lookup"><span data-stu-id="5faa5-110">displayName</span></span>|<span data-ttu-id="5faa5-111">字符串</span><span class="sxs-lookup"><span data-stu-id="5faa5-111">String</span></span>|<span data-ttu-id="5faa5-112">已修改的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="5faa5-112">Name of property that was modified.</span></span>|
|<span data-ttu-id="5faa5-113">NewValue</span><span class="sxs-lookup"><span data-stu-id="5faa5-113">newValue</span></span>|<span data-ttu-id="5faa5-114">String</span><span class="sxs-lookup"><span data-stu-id="5faa5-114">String</span></span>|<span data-ttu-id="5faa5-115">新属性值。</span><span class="sxs-lookup"><span data-stu-id="5faa5-115">New property value.</span></span>|
|<span data-ttu-id="5faa5-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="5faa5-116">oldValue</span></span>|<span data-ttu-id="5faa5-117">String</span><span class="sxs-lookup"><span data-stu-id="5faa5-117">String</span></span>|<span data-ttu-id="5faa5-118">旧属性值。</span><span class="sxs-lookup"><span data-stu-id="5faa5-118">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5faa5-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5faa5-119">JSON representation</span></span>

<span data-ttu-id="5faa5-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5faa5-120">The following is a JSON representation of the resource.</span></span>

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


