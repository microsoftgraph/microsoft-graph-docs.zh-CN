---
title: labelDetails 资源类型
description: 表示信息保护标签的标签详细信息。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 214589dfcb26497b5271008f8a358d06a4fb700f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950305"
---
# <a name="labeldetails-resource-type"></a><span data-ttu-id="3b74f-103">labelDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b74f-103">labelDetails resource type</span></span>

<span data-ttu-id="3b74f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b74f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b74f-105">表示信息保护标签的标签详细信息。</span><span class="sxs-lookup"><span data-stu-id="3b74f-105">Represents the label details of an information protection label.</span></span> <span data-ttu-id="3b74f-106">**labelDetails** 提供有关单个信息保护标签的信息。</span><span class="sxs-lookup"><span data-stu-id="3b74f-106">**labelDetails** provides information about a single information protection label.</span></span> <span data-ttu-id="3b74f-107">可通过[evaluateRemoval、evaluateApplication](../api/informationprotectionlabel-evaluateremoval.md)和[extractLabel 返回](../api/informationprotectionlabel-extractLabel.md)[](../api/informationprotectionlabel-evaluateapplication.md)</span><span class="sxs-lookup"><span data-stu-id="3b74f-107">Can be returned by [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [extractLabel](../api/informationprotectionlabel-extractLabel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3b74f-108">属性</span><span class="sxs-lookup"><span data-stu-id="3b74f-108">Properties</span></span>

| <span data-ttu-id="3b74f-109">属性</span><span class="sxs-lookup"><span data-stu-id="3b74f-109">Property</span></span>    | <span data-ttu-id="3b74f-110">类型</span><span class="sxs-lookup"><span data-stu-id="3b74f-110">Type</span></span>    | <span data-ttu-id="3b74f-111">说明</span><span class="sxs-lookup"><span data-stu-id="3b74f-111">Description</span></span>                                                                                                  |
| :---------- | :------ | :----------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="3b74f-112">color</span><span class="sxs-lookup"><span data-stu-id="3b74f-112">color</span></span>       | <span data-ttu-id="3b74f-113">String</span><span class="sxs-lookup"><span data-stu-id="3b74f-113">String</span></span>  | <span data-ttu-id="3b74f-114">用户界面应为标签显示的颜色（如果已配置）。</span><span class="sxs-lookup"><span data-stu-id="3b74f-114">The color that the user interface should display for the label, if configured.</span></span>                               |
| <span data-ttu-id="3b74f-115">说明</span><span class="sxs-lookup"><span data-stu-id="3b74f-115">description</span></span> | <span data-ttu-id="3b74f-116">String</span><span class="sxs-lookup"><span data-stu-id="3b74f-116">String</span></span>  | <span data-ttu-id="3b74f-117">管理员定义的标签说明。</span><span class="sxs-lookup"><span data-stu-id="3b74f-117">The admin-defined description for the label.</span></span>                                                                 |
| <span data-ttu-id="3b74f-118">id</span><span class="sxs-lookup"><span data-stu-id="3b74f-118">id</span></span>          | <span data-ttu-id="3b74f-119">String</span><span class="sxs-lookup"><span data-stu-id="3b74f-119">String</span></span>  | <span data-ttu-id="3b74f-120">标签 ID 是 GUID (全局唯) 。</span><span class="sxs-lookup"><span data-stu-id="3b74f-120">The label ID is a globally unique identifier (GUID).</span></span>                                                          |
| <span data-ttu-id="3b74f-121">isActive</span><span class="sxs-lookup"><span data-stu-id="3b74f-121">isActive</span></span>    | <span data-ttu-id="3b74f-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b74f-122">Boolean</span></span> | <span data-ttu-id="3b74f-123">指示标签是否处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="3b74f-123">Indicates whether the label is active or not.</span></span> <span data-ttu-id="3b74f-124">应在用户界面中隐藏或禁用活动标签。</span><span class="sxs-lookup"><span data-stu-id="3b74f-124">Active labels should be hidden or disabled in user interfaces.</span></span> |
| <span data-ttu-id="3b74f-125">name</span><span class="sxs-lookup"><span data-stu-id="3b74f-125">name</span></span>        | <span data-ttu-id="3b74f-126">String</span><span class="sxs-lookup"><span data-stu-id="3b74f-126">String</span></span>  | <span data-ttu-id="3b74f-127">标签的纯文本名称。</span><span class="sxs-lookup"><span data-stu-id="3b74f-127">The plaintext name of the label.</span></span>                                                                             |
| <span data-ttu-id="3b74f-128">敏感度</span><span class="sxs-lookup"><span data-stu-id="3b74f-128">sensitivity</span></span> | <span data-ttu-id="3b74f-129">Int32</span><span class="sxs-lookup"><span data-stu-id="3b74f-129">Int32</span></span>   | <span data-ttu-id="3b74f-130">标签的敏感度值，其中 lower 不太敏感。</span><span class="sxs-lookup"><span data-stu-id="3b74f-130">The sensitivity value of the label, where lower is less sensitive.</span></span>                                           |
| <span data-ttu-id="3b74f-131">tooltip</span><span class="sxs-lookup"><span data-stu-id="3b74f-131">tooltip</span></span>     | <span data-ttu-id="3b74f-132">String</span><span class="sxs-lookup"><span data-stu-id="3b74f-132">String</span></span>  | <span data-ttu-id="3b74f-133">应在用户界面中为标签显示的工具提示。</span><span class="sxs-lookup"><span data-stu-id="3b74f-133">The tooltip that should be displayed for the label in a user interface.</span></span>                                      |

## <a name="json-representation"></a><span data-ttu-id="3b74f-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b74f-134">JSON representation</span></span>

<span data-ttu-id="3b74f-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b74f-135">The following is a JSON representation of the resource.</span></span>

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

