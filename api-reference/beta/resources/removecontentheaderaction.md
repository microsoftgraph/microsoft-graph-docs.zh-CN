---
title: removeContentHeaderAction 资源类型
description: 表示一个操作，该操作指定要从信息中删除的内容标头的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 63dc9556ace567f4505b40c1882bd56b087a7835
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073423"
---
# <a name="removecontentheaderaction-resource-type"></a><span data-ttu-id="a6875-103">removeContentHeaderAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6875-103">removeContentHeaderAction resource type</span></span>

<span data-ttu-id="a6875-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6875-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6875-105">表示一个操作，该操作指定要从信息中删除的内容标头的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="a6875-105">Represents an action that specifies the details on the content header to be removed from the information, if applicable.</span></span> <span data-ttu-id="a6875-106">如果由于更新或删除标签而要删除标头，则 [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)、 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)或 [EvaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) api 可能会返回 **removeContentHeaderAction** 。</span><span class="sxs-lookup"><span data-stu-id="a6875-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeContentHeaderAction** if the header is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="a6875-107">该操作指示使用应用程序移除包含之前适用的内容头的特定 UI 元素。</span><span class="sxs-lookup"><span data-stu-id="a6875-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span>

## <a name="properties"></a><span data-ttu-id="a6875-108">属性</span><span class="sxs-lookup"><span data-stu-id="a6875-108">Properties</span></span>

| <span data-ttu-id="a6875-109">属性</span><span class="sxs-lookup"><span data-stu-id="a6875-109">Property</span></span>       | <span data-ttu-id="a6875-110">类型</span><span class="sxs-lookup"><span data-stu-id="a6875-110">Type</span></span>              | <span data-ttu-id="a6875-111">说明</span><span class="sxs-lookup"><span data-stu-id="a6875-111">Description</span></span>                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| <span data-ttu-id="a6875-112">uiElementNames</span><span class="sxs-lookup"><span data-stu-id="a6875-112">uiElementNames</span></span> | <span data-ttu-id="a6875-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="a6875-113">String collection</span></span> | <span data-ttu-id="a6875-114">要删除的标头的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="a6875-114">The name of the UI element of the header to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a6875-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6875-115">JSON representation</span></span>

<span data-ttu-id="a6875-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6875-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeContentHeaderAction",
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
  "description": "removeContentHeaderAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

