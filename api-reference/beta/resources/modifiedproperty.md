---
title: modifiedProperty 资源类型
description: 描述在目标系统中执行的更改。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5ae34932d2c08d472f27167c02993b2ef916faae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522622"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="9ca79-103">modifiedProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ca79-103">modifiedProperty resource type</span></span>

<span data-ttu-id="9ca79-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9ca79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ca79-105">描述在目标系统中执行的更改。</span><span class="sxs-lookup"><span data-stu-id="9ca79-105">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="9ca79-106">属性</span><span class="sxs-lookup"><span data-stu-id="9ca79-106">Properties</span></span>

| <span data-ttu-id="9ca79-107">属性</span><span class="sxs-lookup"><span data-stu-id="9ca79-107">Property</span></span>     | <span data-ttu-id="9ca79-108">类型</span><span class="sxs-lookup"><span data-stu-id="9ca79-108">Type</span></span>        | <span data-ttu-id="9ca79-109">说明</span><span class="sxs-lookup"><span data-stu-id="9ca79-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9ca79-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9ca79-110">displayName</span></span>|<span data-ttu-id="9ca79-111">String</span><span class="sxs-lookup"><span data-stu-id="9ca79-111">String</span></span>|<span data-ttu-id="9ca79-112">已修改的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="9ca79-112">Name of property that was modified.</span></span>|
|<span data-ttu-id="9ca79-113">NewValue</span><span class="sxs-lookup"><span data-stu-id="9ca79-113">newValue</span></span>|<span data-ttu-id="9ca79-114">String</span><span class="sxs-lookup"><span data-stu-id="9ca79-114">String</span></span>|<span data-ttu-id="9ca79-115">新的属性值。</span><span class="sxs-lookup"><span data-stu-id="9ca79-115">New property value.</span></span>|
|<span data-ttu-id="9ca79-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="9ca79-116">oldValue</span></span>|<span data-ttu-id="9ca79-117">String</span><span class="sxs-lookup"><span data-stu-id="9ca79-117">String</span></span>|<span data-ttu-id="9ca79-118">旧属性值。</span><span class="sxs-lookup"><span data-stu-id="9ca79-118">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ca79-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ca79-119">JSON representation</span></span>

<span data-ttu-id="9ca79-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ca79-120">The following is a JSON representation of the resource.</span></span>

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
