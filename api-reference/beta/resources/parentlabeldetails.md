---
title: parentLabelDetails 资源类型
description: 表示信息保护父标签的标签详细信息。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8ba6dfcbb7f441c0026848eb59735db5fb4987ac
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579980"
---
# <a name="parentlabeldetails-resource-type"></a><span data-ttu-id="d0b36-103">parentLabelDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0b36-103">parentLabelDetails resource type</span></span>

<span data-ttu-id="d0b36-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0b36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0b36-105">表示信息保护父标签的标签详细信息。</span><span class="sxs-lookup"><span data-stu-id="d0b36-105">Represents the label details of an information protection parent label.</span></span> <span data-ttu-id="d0b36-106">**parentLabelDetails** 提供有关单个信息保护标签的信息。</span><span class="sxs-lookup"><span data-stu-id="d0b36-106">**parentLabelDetails** provides information about a single information protection label.</span></span> <span data-ttu-id="d0b36-107">可通过[evaluateRemoval、evaluateApplication](../api/informationprotectionlabel-evaluateremoval.md)和[extractLabel 返回](../api/informationprotectionlabel-extractLabel.md)[](../api/informationprotectionlabel-evaluateapplication.md)</span><span class="sxs-lookup"><span data-stu-id="d0b36-107">Can be returned by [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d0b36-108">属性</span><span class="sxs-lookup"><span data-stu-id="d0b36-108">Properties</span></span>

| <span data-ttu-id="d0b36-109">属性</span><span class="sxs-lookup"><span data-stu-id="d0b36-109">Property</span></span>    | <span data-ttu-id="d0b36-110">类型</span><span class="sxs-lookup"><span data-stu-id="d0b36-110">Type</span></span>    | <span data-ttu-id="d0b36-111">说明</span><span class="sxs-lookup"><span data-stu-id="d0b36-111">Description</span></span>                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="d0b36-112">color</span><span class="sxs-lookup"><span data-stu-id="d0b36-112">color</span></span>       | <span data-ttu-id="d0b36-113">String</span><span class="sxs-lookup"><span data-stu-id="d0b36-113">String</span></span>  | <span data-ttu-id="d0b36-114">用户界面应为标签显示的颜色（如果已配置）。</span><span class="sxs-lookup"><span data-stu-id="d0b36-114">The color that the user interface should display for the label, if configured.</span></span>                               |
| <span data-ttu-id="d0b36-115">说明</span><span class="sxs-lookup"><span data-stu-id="d0b36-115">description</span></span> | <span data-ttu-id="d0b36-116">String</span><span class="sxs-lookup"><span data-stu-id="d0b36-116">String</span></span>  | <span data-ttu-id="d0b36-117">管理员定义的标签说明。</span><span class="sxs-lookup"><span data-stu-id="d0b36-117">The admin-defined description for the label.</span></span>                                                                 |
| <span data-ttu-id="d0b36-118">id</span><span class="sxs-lookup"><span data-stu-id="d0b36-118">id</span></span>          | <span data-ttu-id="d0b36-119">String</span><span class="sxs-lookup"><span data-stu-id="d0b36-119">String</span></span>  | <span data-ttu-id="d0b36-120">标签 ID 是 GUID (全局唯) 。</span><span class="sxs-lookup"><span data-stu-id="d0b36-120">The label ID is a globally unique identifier (GUID).</span></span>                                                          |
| <span data-ttu-id="d0b36-121">isActive</span><span class="sxs-lookup"><span data-stu-id="d0b36-121">isActive</span></span>    | <span data-ttu-id="d0b36-122">布尔</span><span class="sxs-lookup"><span data-stu-id="d0b36-122">Boolean</span></span> | <span data-ttu-id="d0b36-123">指示标签是否处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="d0b36-123">Indicates whether the label is active or not.</span></span> <span data-ttu-id="d0b36-124">应在用户界面中隐藏或禁用活动标签。</span><span class="sxs-lookup"><span data-stu-id="d0b36-124">Active labels should be hidden or disabled in user interfaces.</span></span> |
| <span data-ttu-id="d0b36-125">name</span><span class="sxs-lookup"><span data-stu-id="d0b36-125">name</span></span>        | <span data-ttu-id="d0b36-126">String</span><span class="sxs-lookup"><span data-stu-id="d0b36-126">String</span></span>  | <span data-ttu-id="d0b36-127">标签的纯文本名称。</span><span class="sxs-lookup"><span data-stu-id="d0b36-127">The plaintext name of the label.</span></span>                                                                             |
| <span data-ttu-id="d0b36-128">sensitivity</span><span class="sxs-lookup"><span data-stu-id="d0b36-128">sensitivity</span></span> | <span data-ttu-id="d0b36-129">Int32</span><span class="sxs-lookup"><span data-stu-id="d0b36-129">Int32</span></span>   | <span data-ttu-id="d0b36-130">标签的敏感度值，其中 lower 不太敏感。</span><span class="sxs-lookup"><span data-stu-id="d0b36-130">The sensitivity value of the label, where lower is less sensitive.</span></span>                                           |
| <span data-ttu-id="d0b36-131">tooltip</span><span class="sxs-lookup"><span data-stu-id="d0b36-131">tooltip</span></span>     | <span data-ttu-id="d0b36-132">String</span><span class="sxs-lookup"><span data-stu-id="d0b36-132">String</span></span>  | <span data-ttu-id="d0b36-133">应在用户界面中为标签显示的工具提示。</span><span class="sxs-lookup"><span data-stu-id="d0b36-133">The tooltip that should be displayed for the label in a user interface.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="d0b36-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0b36-134">JSON representation</span></span>

<span data-ttu-id="d0b36-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0b36-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parentLabelDetails",
  "baseType": null
}-->

```json
{
  "color": "String",
  "description": "String",
  "id": "String",
  "isActive": true,
  "name": "String",
  "sensitivity": 1024,
  "tooltip": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "parentLabelDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->