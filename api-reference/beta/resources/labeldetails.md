---
title: labelDetails 资源类型
description: 代表信息保护标签的标签详细信息。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6b475c96b3ecbc2caa0aa147e3fc8fd0253ac243
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084035"
---
# <a name="labeldetails-resource-type"></a><span data-ttu-id="b687c-103">labelDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="b687c-103">labelDetails resource type</span></span>

<span data-ttu-id="b687c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b687c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b687c-105">代表信息保护标签的标签详细信息。</span><span class="sxs-lookup"><span data-stu-id="b687c-105">Represents the label details of an information protection label.</span></span> <span data-ttu-id="b687c-106">**labelDetails** 提供有关单个信息保护标签的信息。</span><span class="sxs-lookup"><span data-stu-id="b687c-106">**labelDetails** provides information about a single information protection label.</span></span> <span data-ttu-id="b687c-107">可以由[evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)、 [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)和[extractLabel](../api/informationprotectionlabel-extractLabel.md)返回</span><span class="sxs-lookup"><span data-stu-id="b687c-107">Can be returned by [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b687c-108">属性</span><span class="sxs-lookup"><span data-stu-id="b687c-108">Properties</span></span>

| <span data-ttu-id="b687c-109">属性</span><span class="sxs-lookup"><span data-stu-id="b687c-109">Property</span></span>    | <span data-ttu-id="b687c-110">类型</span><span class="sxs-lookup"><span data-stu-id="b687c-110">Type</span></span>    | <span data-ttu-id="b687c-111">说明</span><span class="sxs-lookup"><span data-stu-id="b687c-111">Description</span></span>                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b687c-112">color</span><span class="sxs-lookup"><span data-stu-id="b687c-112">color</span></span>       | <span data-ttu-id="b687c-113">String</span><span class="sxs-lookup"><span data-stu-id="b687c-113">String</span></span>  | <span data-ttu-id="b687c-114">用户界面针对标签应显示的颜色（如果已配置）。</span><span class="sxs-lookup"><span data-stu-id="b687c-114">The color that the user interface should display for the label, if configured.</span></span>                               |
| <span data-ttu-id="b687c-115">说明</span><span class="sxs-lookup"><span data-stu-id="b687c-115">description</span></span> | <span data-ttu-id="b687c-116">字符串</span><span class="sxs-lookup"><span data-stu-id="b687c-116">String</span></span>  | <span data-ttu-id="b687c-117">管理员定义的标签说明。</span><span class="sxs-lookup"><span data-stu-id="b687c-117">The admin-defined description for the label.</span></span>                                                                 |
| <span data-ttu-id="b687c-118">id</span><span class="sxs-lookup"><span data-stu-id="b687c-118">id</span></span>          | <span data-ttu-id="b687c-119">字符串</span><span class="sxs-lookup"><span data-stu-id="b687c-119">String</span></span>  | <span data-ttu-id="b687c-120">标签 ID 是 (GUID) 的全局唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b687c-120">The label ID is a globally unique identifier (GUID).</span></span>                                                          |
| <span data-ttu-id="b687c-121">isActive</span><span class="sxs-lookup"><span data-stu-id="b687c-121">isActive</span></span>    | <span data-ttu-id="b687c-122">布尔</span><span class="sxs-lookup"><span data-stu-id="b687c-122">Boolean</span></span> | <span data-ttu-id="b687c-123">指示标签是否处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="b687c-123">Indicates whether the label is active or not.</span></span> <span data-ttu-id="b687c-124">应在用户界面中隐藏或禁用活动标签。</span><span class="sxs-lookup"><span data-stu-id="b687c-124">Active labels should be hidden or disabled in user interfaces.</span></span> |
| <span data-ttu-id="b687c-125">名称</span><span class="sxs-lookup"><span data-stu-id="b687c-125">name</span></span>        | <span data-ttu-id="b687c-126">字符串</span><span class="sxs-lookup"><span data-stu-id="b687c-126">String</span></span>  | <span data-ttu-id="b687c-127">标签的纯文本名称。</span><span class="sxs-lookup"><span data-stu-id="b687c-127">The plaintext name of the label.</span></span>                                                                             |
| <span data-ttu-id="b687c-128">sensitivity</span><span class="sxs-lookup"><span data-stu-id="b687c-128">sensitivity</span></span> | <span data-ttu-id="b687c-129">Int32</span><span class="sxs-lookup"><span data-stu-id="b687c-129">Int32</span></span>   | <span data-ttu-id="b687c-130">标签的敏感度值，其中较小的是不敏感的。</span><span class="sxs-lookup"><span data-stu-id="b687c-130">The sensitivity value of the label, where lower is less sensitive.</span></span>                                           |
| <span data-ttu-id="b687c-131">tooltip</span><span class="sxs-lookup"><span data-stu-id="b687c-131">tooltip</span></span>     | <span data-ttu-id="b687c-132">字符串</span><span class="sxs-lookup"><span data-stu-id="b687c-132">String</span></span>  | <span data-ttu-id="b687c-133">应为用户界面中的标签显示的工具提示。</span><span class="sxs-lookup"><span data-stu-id="b687c-133">The tooltip that should be displayed for the label in a user interface.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="b687c-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b687c-134">JSON representation</span></span>

<span data-ttu-id="b687c-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b687c-135">The following is a JSON representation of the resource.</span></span>

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

