---
title: removeContentFooterAction 资源类型
description: 表示一个操作，该操作指定要从信息中删除的内容页脚的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 62bd0fbefeb9bf246619bc470c5552cd20d174d2
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939444"
---
# <a name="removecontentfooteraction-resource-type"></a><span data-ttu-id="32ec2-103">removeContentFooterAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="32ec2-103">removeContentFooterAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32ec2-104">表示一个操作，该操作指定要从信息中删除的内容页脚的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="32ec2-104">Represents an action that specifies the details on the content footer to be removed from the information, if applicable.</span></span> <span data-ttu-id="32ec2-105">如果由于更新或删除标签而要删除页脚， [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md)、 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)或[EvaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) api 可能会返回**removeContentFooterAction** 。</span><span class="sxs-lookup"><span data-stu-id="32ec2-105">The [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeContentFooterAction** if the footer is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="32ec2-106">该操作指示使用应用程序移除包含之前适用的内容页脚的特定 UI 元素。</span><span class="sxs-lookup"><span data-stu-id="32ec2-106">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content footer.</span></span>

## <a name="properties"></a><span data-ttu-id="32ec2-107">属性</span><span class="sxs-lookup"><span data-stu-id="32ec2-107">Properties</span></span>

| <span data-ttu-id="32ec2-108">属性</span><span class="sxs-lookup"><span data-stu-id="32ec2-108">Property</span></span>       | <span data-ttu-id="32ec2-109">类型</span><span class="sxs-lookup"><span data-stu-id="32ec2-109">Type</span></span>              | <span data-ttu-id="32ec2-110">描述</span><span class="sxs-lookup"><span data-stu-id="32ec2-110">Description</span></span>                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| <span data-ttu-id="32ec2-111">uiElementNames</span><span class="sxs-lookup"><span data-stu-id="32ec2-111">uiElementNames</span></span> | <span data-ttu-id="32ec2-112">String collection</span><span class="sxs-lookup"><span data-stu-id="32ec2-112">String collection</span></span> | <span data-ttu-id="32ec2-113">要删除的页脚的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="32ec2-113">The name of the UI element of the footer to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="32ec2-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="32ec2-114">JSON representation</span></span>

<span data-ttu-id="32ec2-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="32ec2-115">The following is a JSON representation of the resource.</span></span>

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