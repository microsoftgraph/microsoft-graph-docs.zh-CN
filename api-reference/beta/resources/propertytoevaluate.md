---
title: propertyToEvaluate 资源类型
description: 定义属性的名称和值。
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7f6c08adc311c343699667ea3179b0b2d09a5a34
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272846"
---
# <a name="propertytoevaluate-resource-type"></a><span data-ttu-id="d1762-103">propertyToEvaluate 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1762-103">propertyToEvaluate resource type</span></span>

<span data-ttu-id="d1762-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1762-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1762-105">定义属性的名称和值。</span><span class="sxs-lookup"><span data-stu-id="d1762-105">Defines the name and the value of the property.</span></span>

## <a name="properties"></a><span data-ttu-id="d1762-106">属性</span><span class="sxs-lookup"><span data-stu-id="d1762-106">Properties</span></span>

| <span data-ttu-id="d1762-107">属性</span><span class="sxs-lookup"><span data-stu-id="d1762-107">Property</span></span> | <span data-ttu-id="d1762-108">类型</span><span class="sxs-lookup"><span data-stu-id="d1762-108">Type</span></span> | <span data-ttu-id="d1762-109">Description</span><span class="sxs-lookup"><span data-stu-id="d1762-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="d1762-110">propertyName</span><span class="sxs-lookup"><span data-stu-id="d1762-110">propertyName</span></span> | <span data-ttu-id="d1762-111">String</span><span class="sxs-lookup"><span data-stu-id="d1762-111">String</span></span> | <span data-ttu-id="d1762-112">提供属性名称。</span><span class="sxs-lookup"><span data-stu-id="d1762-112">Provides the property name.</span></span> |
| <span data-ttu-id="d1762-113">propertyValue</span><span class="sxs-lookup"><span data-stu-id="d1762-113">propertyValue</span></span> | <span data-ttu-id="d1762-114">String</span><span class="sxs-lookup"><span data-stu-id="d1762-114">String</span></span> | <span data-ttu-id="d1762-115">提供属性值。</span><span class="sxs-lookup"><span data-stu-id="d1762-115">Provides the property value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d1762-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1762-116">JSON representation</span></span>

<span data-ttu-id="d1762-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1762-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.propertyToEvaluate",
  "baseType": null
}-->

```json
{
  "propertyName": "String",
  "propertyValue": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "propertyToEvaluate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->