---
title: labelDetails 资源类型
description: 代表信息保护标签的标签详细信息。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7f2ff99f6f7548e9176358219d70cd55e1232a05
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939171"
---
# <a name="labeldetails-resource-type"></a><span data-ttu-id="29f17-103">labelDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="29f17-103">labelDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29f17-104">代表信息保护标签的标签详细信息。</span><span class="sxs-lookup"><span data-stu-id="29f17-104">Represents the label details of an information protection label.</span></span> <span data-ttu-id="29f17-105">**labelDetails**提供有关单个信息保护标签的信息。</span><span class="sxs-lookup"><span data-stu-id="29f17-105">**labelDetails** provides information about a single information protection label.</span></span> <span data-ttu-id="29f17-106">可以由[evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md)、 [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)和[extractLabel](../api/informationprotectionlabel-extractLabel.md)返回</span><span class="sxs-lookup"><span data-stu-id="29f17-106">Can be returned by [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="29f17-107">属性</span><span class="sxs-lookup"><span data-stu-id="29f17-107">Properties</span></span>

| <span data-ttu-id="29f17-108">属性</span><span class="sxs-lookup"><span data-stu-id="29f17-108">Property</span></span>    | <span data-ttu-id="29f17-109">类型</span><span class="sxs-lookup"><span data-stu-id="29f17-109">Type</span></span>    | <span data-ttu-id="29f17-110">描述</span><span class="sxs-lookup"><span data-stu-id="29f17-110">Description</span></span>                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="29f17-111">color</span><span class="sxs-lookup"><span data-stu-id="29f17-111">color</span></span>       | <span data-ttu-id="29f17-112">String</span><span class="sxs-lookup"><span data-stu-id="29f17-112">String</span></span>  | <span data-ttu-id="29f17-113">用户界面针对标签应显示的颜色（如果已配置）。</span><span class="sxs-lookup"><span data-stu-id="29f17-113">The color that the user interface should display for the label, if configured.</span></span>                               |
| <span data-ttu-id="29f17-114">description</span><span class="sxs-lookup"><span data-stu-id="29f17-114">description</span></span> | <span data-ttu-id="29f17-115">String</span><span class="sxs-lookup"><span data-stu-id="29f17-115">String</span></span>  | <span data-ttu-id="29f17-116">管理员定义的标签说明。</span><span class="sxs-lookup"><span data-stu-id="29f17-116">The admin-defined description for the label.</span></span>                                                                 |
| <span data-ttu-id="29f17-117">id</span><span class="sxs-lookup"><span data-stu-id="29f17-117">id</span></span>          | <span data-ttu-id="29f17-118">String</span><span class="sxs-lookup"><span data-stu-id="29f17-118">String</span></span>  | <span data-ttu-id="29f17-119">标签 ID 是一个全局唯一标识符（GUID）。</span><span class="sxs-lookup"><span data-stu-id="29f17-119">The label ID is a globally unique identifier (GUID).</span></span>                                                          |
| <span data-ttu-id="29f17-120">isActive</span><span class="sxs-lookup"><span data-stu-id="29f17-120">isActive</span></span>    | <span data-ttu-id="29f17-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="29f17-121">Boolean</span></span> | <span data-ttu-id="29f17-122">指示标签是否处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="29f17-122">Indicates whether the label is active or not.</span></span> <span data-ttu-id="29f17-123">应在用户界面中隐藏或禁用活动标签。</span><span class="sxs-lookup"><span data-stu-id="29f17-123">Active labels should be hidden or disabled in user interfaces.</span></span> |
| <span data-ttu-id="29f17-124">name</span><span class="sxs-lookup"><span data-stu-id="29f17-124">name</span></span>        | <span data-ttu-id="29f17-125">字符串</span><span class="sxs-lookup"><span data-stu-id="29f17-125">String</span></span>  | <span data-ttu-id="29f17-126">标签的纯文本名称。</span><span class="sxs-lookup"><span data-stu-id="29f17-126">The plaintext name of the label.</span></span>                                                                             |
| <span data-ttu-id="29f17-127">sensitivity</span><span class="sxs-lookup"><span data-stu-id="29f17-127">sensitivity</span></span> | <span data-ttu-id="29f17-128">Int32</span><span class="sxs-lookup"><span data-stu-id="29f17-128">Int32</span></span>   | <span data-ttu-id="29f17-129">标签的敏感度值，其中较小的是不敏感的。</span><span class="sxs-lookup"><span data-stu-id="29f17-129">The sensitivity value of the label, where lower is less sensitive.</span></span>                                           |
| <span data-ttu-id="29f17-130">tooltip</span><span class="sxs-lookup"><span data-stu-id="29f17-130">tooltip</span></span>     | <span data-ttu-id="29f17-131">字符串</span><span class="sxs-lookup"><span data-stu-id="29f17-131">String</span></span>  | <span data-ttu-id="29f17-132">应为用户界面中的标签显示的工具提示。</span><span class="sxs-lookup"><span data-stu-id="29f17-132">The tooltip that should be displayed for the label in a user interface.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="29f17-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29f17-133">JSON representation</span></span>

<span data-ttu-id="29f17-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29f17-134">The following is a JSON representation of the resource.</span></span>

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