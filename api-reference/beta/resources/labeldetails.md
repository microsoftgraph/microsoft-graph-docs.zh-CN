---
title: labelDetails 资源类型
description: 代表信息保护标签的标签详细信息。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cf031459004e0c0d56b5b09145ed897a9f960142
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523007"
---
# <a name="labeldetails-resource-type"></a><span data-ttu-id="e6078-103">labelDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6078-103">labelDetails resource type</span></span>

<span data-ttu-id="e6078-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e6078-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6078-105">代表信息保护标签的标签详细信息。</span><span class="sxs-lookup"><span data-stu-id="e6078-105">Represents the label details of an information protection label.</span></span> <span data-ttu-id="e6078-106">**labelDetails**提供有关单个信息保护标签的信息。</span><span class="sxs-lookup"><span data-stu-id="e6078-106">**labelDetails** provides information about a single information protection label.</span></span> <span data-ttu-id="e6078-107">可以由[evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)、 [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)和[extractLabel](../api/informationprotectionlabel-extractLabel.md)返回</span><span class="sxs-lookup"><span data-stu-id="e6078-107">Can be returned by [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e6078-108">属性</span><span class="sxs-lookup"><span data-stu-id="e6078-108">Properties</span></span>

| <span data-ttu-id="e6078-109">属性</span><span class="sxs-lookup"><span data-stu-id="e6078-109">Property</span></span>    | <span data-ttu-id="e6078-110">类型</span><span class="sxs-lookup"><span data-stu-id="e6078-110">Type</span></span>    | <span data-ttu-id="e6078-111">说明</span><span class="sxs-lookup"><span data-stu-id="e6078-111">Description</span></span>                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e6078-112">color</span><span class="sxs-lookup"><span data-stu-id="e6078-112">color</span></span>       | <span data-ttu-id="e6078-113">String</span><span class="sxs-lookup"><span data-stu-id="e6078-113">String</span></span>  | <span data-ttu-id="e6078-114">用户界面针对标签应显示的颜色（如果已配置）。</span><span class="sxs-lookup"><span data-stu-id="e6078-114">The color that the user interface should display for the label, if configured.</span></span>                               |
| <span data-ttu-id="e6078-115">说明</span><span class="sxs-lookup"><span data-stu-id="e6078-115">description</span></span> | <span data-ttu-id="e6078-116">String</span><span class="sxs-lookup"><span data-stu-id="e6078-116">String</span></span>  | <span data-ttu-id="e6078-117">管理员定义的标签说明。</span><span class="sxs-lookup"><span data-stu-id="e6078-117">The admin-defined description for the label.</span></span>                                                                 |
| <span data-ttu-id="e6078-118">id</span><span class="sxs-lookup"><span data-stu-id="e6078-118">id</span></span>          | <span data-ttu-id="e6078-119">String</span><span class="sxs-lookup"><span data-stu-id="e6078-119">String</span></span>  | <span data-ttu-id="e6078-120">标签 ID 是一个全局唯一标识符（GUID）。</span><span class="sxs-lookup"><span data-stu-id="e6078-120">The label ID is a globally unique identifier (GUID).</span></span>                                                          |
| <span data-ttu-id="e6078-121">isActive</span><span class="sxs-lookup"><span data-stu-id="e6078-121">isActive</span></span>    | <span data-ttu-id="e6078-122">布尔</span><span class="sxs-lookup"><span data-stu-id="e6078-122">Boolean</span></span> | <span data-ttu-id="e6078-123">指示标签是否处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="e6078-123">Indicates whether the label is active or not.</span></span> <span data-ttu-id="e6078-124">应在用户界面中隐藏或禁用活动标签。</span><span class="sxs-lookup"><span data-stu-id="e6078-124">Active labels should be hidden or disabled in user interfaces.</span></span> |
| <span data-ttu-id="e6078-125">name</span><span class="sxs-lookup"><span data-stu-id="e6078-125">name</span></span>        | <span data-ttu-id="e6078-126">字符串</span><span class="sxs-lookup"><span data-stu-id="e6078-126">String</span></span>  | <span data-ttu-id="e6078-127">标签的纯文本名称。</span><span class="sxs-lookup"><span data-stu-id="e6078-127">The plaintext name of the label.</span></span>                                                                             |
| <span data-ttu-id="e6078-128">sensitivity</span><span class="sxs-lookup"><span data-stu-id="e6078-128">sensitivity</span></span> | <span data-ttu-id="e6078-129">Int32</span><span class="sxs-lookup"><span data-stu-id="e6078-129">Int32</span></span>   | <span data-ttu-id="e6078-130">标签的敏感度值，其中较小的是不敏感的。</span><span class="sxs-lookup"><span data-stu-id="e6078-130">The sensitivity value of the label, where lower is less sensitive.</span></span>                                           |
| <span data-ttu-id="e6078-131">tooltip</span><span class="sxs-lookup"><span data-stu-id="e6078-131">tooltip</span></span>     | <span data-ttu-id="e6078-132">String</span><span class="sxs-lookup"><span data-stu-id="e6078-132">String</span></span>  | <span data-ttu-id="e6078-133">应为用户界面中的标签显示的工具提示。</span><span class="sxs-lookup"><span data-stu-id="e6078-133">The tooltip that should be displayed for the label in a user interface.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="e6078-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6078-134">JSON representation</span></span>

<span data-ttu-id="e6078-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6078-135">The following is a JSON representation of the resource.</span></span>

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