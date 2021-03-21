---
title: removeContentHeaderAction 资源类型
description: 表示一个操作，指定要从信息中删除的内容标头的详细信息（如果适用）。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 9170556f5fc04e7b270d9886cd81f48c45e07122
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962062"
---
# <a name="removecontentheaderaction-resource-type"></a><span data-ttu-id="62783-103">removeContentHeaderAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="62783-103">removeContentHeaderAction resource type</span></span>

<span data-ttu-id="62783-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62783-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62783-105">表示一个操作，指定要从信息中删除的内容标头的详细信息（如果适用）。</span><span class="sxs-lookup"><span data-stu-id="62783-105">Represents an action that specifies the details on the content header to be removed from the information, if applicable.</span></span> <span data-ttu-id="62783-106">如果由于更新或删除标签而删除标头，则 evaluateApplication、evaluateClassificationResults 或 [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) API 可能会返回 **removeContentHeaderAction。** [](../api/informationprotectionlabel-evaluateapplication.md) [](../api/informationprotectionlabel-evaluateclassificationresults.md)</span><span class="sxs-lookup"><span data-stu-id="62783-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeContentHeaderAction** if the header is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="62783-107">此操作指示使用应用程序删除包含以前适用的内容标头的特定 UI 元素。</span><span class="sxs-lookup"><span data-stu-id="62783-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span>

## <a name="properties"></a><span data-ttu-id="62783-108">属性</span><span class="sxs-lookup"><span data-stu-id="62783-108">Properties</span></span>

| <span data-ttu-id="62783-109">属性</span><span class="sxs-lookup"><span data-stu-id="62783-109">Property</span></span>       | <span data-ttu-id="62783-110">类型</span><span class="sxs-lookup"><span data-stu-id="62783-110">Type</span></span>              | <span data-ttu-id="62783-111">说明</span><span class="sxs-lookup"><span data-stu-id="62783-111">Description</span></span>                                                |
| :------------- | :---------------- | :--------------------------------------------------------- |
| <span data-ttu-id="62783-112">uiElementNames</span><span class="sxs-lookup"><span data-stu-id="62783-112">uiElementNames</span></span> | <span data-ttu-id="62783-113">String collection</span><span class="sxs-lookup"><span data-stu-id="62783-113">String collection</span></span> | <span data-ttu-id="62783-114">要删除的标题的 UI 元素的名称。</span><span class="sxs-lookup"><span data-stu-id="62783-114">The name of the UI element of the header to be removed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="62783-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62783-115">JSON representation</span></span>

<span data-ttu-id="62783-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62783-116">The following is a JSON representation of the resource.</span></span>

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

