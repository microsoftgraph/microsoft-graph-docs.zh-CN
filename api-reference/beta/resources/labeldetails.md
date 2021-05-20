---
title: labelDetails 资源类型
description: 表示信息保护标签的标签详细信息。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: eb66e395d18b7887942753abdebd91d398844290
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579289"
---
# <a name="labeldetails-resource-type"></a><span data-ttu-id="a2453-103">labelDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2453-103">labelDetails resource type</span></span>

<span data-ttu-id="a2453-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2453-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2453-105">表示信息保护标签的标签详细信息。</span><span class="sxs-lookup"><span data-stu-id="a2453-105">Represents the label details of an information protection label.</span></span> <span data-ttu-id="a2453-106">**labelDetails** 提供有关单个信息保护标签的信息。</span><span class="sxs-lookup"><span data-stu-id="a2453-106">**labelDetails** provides information about a single information protection label.</span></span> <span data-ttu-id="a2453-107">继承自 [parentLabelDetails](parentlabeldetails.md)。</span><span class="sxs-lookup"><span data-stu-id="a2453-107">Inherits from the [parentLabelDetails](parentlabeldetails.md).</span></span> <span data-ttu-id="a2453-108">可通过[evaluateRemoval、evaluateApplication](../api/informationprotectionlabel-evaluateremoval.md)和[extractLabel 返回](../api/informationprotectionlabel-extractLabel.md)[](../api/informationprotectionlabel-evaluateapplication.md)</span><span class="sxs-lookup"><span data-stu-id="a2453-108">Can be returned by [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a2453-109">属性</span><span class="sxs-lookup"><span data-stu-id="a2453-109">Properties</span></span>

| <span data-ttu-id="a2453-110">属性</span><span class="sxs-lookup"><span data-stu-id="a2453-110">Property</span></span>    | <span data-ttu-id="a2453-111">类型</span><span class="sxs-lookup"><span data-stu-id="a2453-111">Type</span></span>                                         | <span data-ttu-id="a2453-112">说明</span><span class="sxs-lookup"><span data-stu-id="a2453-112">Description</span></span>                                                                                                  |
| :---------- | :------------------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="a2453-113">color</span><span class="sxs-lookup"><span data-stu-id="a2453-113">color</span></span>       | <span data-ttu-id="a2453-114">String</span><span class="sxs-lookup"><span data-stu-id="a2453-114">String</span></span>                                       | <span data-ttu-id="a2453-115">用户界面应为标签显示的颜色（如果已配置）。</span><span class="sxs-lookup"><span data-stu-id="a2453-115">The color that the user interface should display for the label, if configured.</span></span>                               |
| <span data-ttu-id="a2453-116">说明</span><span class="sxs-lookup"><span data-stu-id="a2453-116">description</span></span> | <span data-ttu-id="a2453-117">String</span><span class="sxs-lookup"><span data-stu-id="a2453-117">String</span></span>                                       | <span data-ttu-id="a2453-118">管理员定义的标签说明。</span><span class="sxs-lookup"><span data-stu-id="a2453-118">The admin-defined description for the label.</span></span>                                                                 |
| <span data-ttu-id="a2453-119">id</span><span class="sxs-lookup"><span data-stu-id="a2453-119">id</span></span>          | <span data-ttu-id="a2453-120">String</span><span class="sxs-lookup"><span data-stu-id="a2453-120">String</span></span>                                       | <span data-ttu-id="a2453-121">标签 ID 是 GUID (全局唯) 。</span><span class="sxs-lookup"><span data-stu-id="a2453-121">The label ID is a globally unique identifier (GUID).</span></span>                                                         |
| <span data-ttu-id="a2453-122">isActive</span><span class="sxs-lookup"><span data-stu-id="a2453-122">isActive</span></span>    | <span data-ttu-id="a2453-123">布尔</span><span class="sxs-lookup"><span data-stu-id="a2453-123">Boolean</span></span>                                      | <span data-ttu-id="a2453-124">指示标签是否处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="a2453-124">Indicates whether the label is active or not.</span></span> <span data-ttu-id="a2453-125">应在用户界面中隐藏或禁用活动标签。</span><span class="sxs-lookup"><span data-stu-id="a2453-125">Active labels should be hidden or disabled in user interfaces.</span></span> |
| <span data-ttu-id="a2453-126">name</span><span class="sxs-lookup"><span data-stu-id="a2453-126">name</span></span>        | <span data-ttu-id="a2453-127">String</span><span class="sxs-lookup"><span data-stu-id="a2453-127">String</span></span>                                       | <span data-ttu-id="a2453-128">标签的纯文本名称。</span><span class="sxs-lookup"><span data-stu-id="a2453-128">The plaintext name of the label.</span></span>                                                                             |
| <span data-ttu-id="a2453-129">sensitivity</span><span class="sxs-lookup"><span data-stu-id="a2453-129">sensitivity</span></span> | <span data-ttu-id="a2453-130">Int32</span><span class="sxs-lookup"><span data-stu-id="a2453-130">Int32</span></span>                                        | <span data-ttu-id="a2453-131">标签的敏感度值，其中 lower 不太敏感。</span><span class="sxs-lookup"><span data-stu-id="a2453-131">The sensitivity value of the label, where lower is less sensitive.</span></span>                                           |
| <span data-ttu-id="a2453-132">tooltip</span><span class="sxs-lookup"><span data-stu-id="a2453-132">tooltip</span></span>     | <span data-ttu-id="a2453-133">String</span><span class="sxs-lookup"><span data-stu-id="a2453-133">String</span></span>                                       | <span data-ttu-id="a2453-134">应在用户界面中为标签显示的工具提示。</span><span class="sxs-lookup"><span data-stu-id="a2453-134">The tooltip that should be displayed for the label in a user interface.</span></span>                                      |
| <span data-ttu-id="a2453-135">父级</span><span class="sxs-lookup"><span data-stu-id="a2453-135">parent</span></span>      | <span data-ttu-id="a2453-136">parentLabelDetails</span><span class="sxs-lookup"><span data-stu-id="a2453-136">parentLabelDetails</span></span> | <span data-ttu-id="a2453-137">与子标签关联的父标签。</span><span class="sxs-lookup"><span data-stu-id="a2453-137">The parent label associated with a child label.</span></span>                                                              |

## <a name="json-representation"></a><span data-ttu-id="a2453-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2453-138">JSON representation</span></span>

<span data-ttu-id="a2453-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2453-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.labelDetails",
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
  "description": "labelDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

