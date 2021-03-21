---
title: removeContentFooterAction 资源类型
description: 表示一个操作，指定要从信息中删除的内容页脚的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1e8de130b2ad346e8e1fee2077014eda9e9b94d5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962071"
---
# <a name="removecontentfooteraction-resource-type"></a><span data-ttu-id="24b0a-103">removeContentFooterAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="24b0a-103">removeContentFooterAction resource type</span></span>

<span data-ttu-id="24b0a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24b0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24b0a-105">表示一个操作，指定要从信息中删除的内容页脚的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="24b0a-105">Represents an action that specifies the details on the content footer to be removed from the information, if applicable.</span></span> <span data-ttu-id="24b0a-106">如果由于更新或删除标签而删除页脚，则 evaluateApplication、evaluateClassificationResults 或 [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) API 可能会返回 **removeContentFooterAction。** [](../api/informationprotectionlabel-evaluateApplication.md) [](../api/informationprotectionlabel-evaluateclassificationresults.md)</span><span class="sxs-lookup"><span data-stu-id="24b0a-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeContentFooterAction** if the footer is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="24b0a-107">此操作指示使用应用程序删除包含以前适用的内容页脚的特定 UI 元素。</span><span class="sxs-lookup"><span data-stu-id="24b0a-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content footer.</span></span>

## <a name="properties"></a><span data-ttu-id="24b0a-108">属性</span><span class="sxs-lookup"><span data-stu-id="24b0a-108">Properties</span></span>

| <span data-ttu-id="24b0a-109">属性</span><span class="sxs-lookup"><span data-stu-id="24b0a-109">Property</span></span>       | <span data-ttu-id="24b0a-110">类型</span><span class="sxs-lookup"><span data-stu-id="24b0a-110">Type</span></span>              | <span data-ttu-id="24b0a-111">说明</span><span class="sxs-lookup"><span data-stu-id="24b0a-111">Description</span></span>                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| <span data-ttu-id="24b0a-112">uiElementNames</span><span class="sxs-lookup"><span data-stu-id="24b0a-112">uiElementNames</span></span> | <span data-ttu-id="24b0a-113">String collection</span><span class="sxs-lookup"><span data-stu-id="24b0a-113">String collection</span></span> | <span data-ttu-id="24b0a-114">要删除的页脚的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="24b0a-114">The name of the UI element of the footer to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="24b0a-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24b0a-115">JSON representation</span></span>

<span data-ttu-id="24b0a-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24b0a-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeContentFooterAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "uiElementNames": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "removeContentFooterAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

