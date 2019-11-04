---
title: removeProtectionAction 资源类型
description: 表示要移除其对文件的保护的操作或信息。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b3ed559460947e903e3085ab48edb421045bc3c6
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939276"
---
# <a name="removeprotectionaction-resource-type"></a><span data-ttu-id="d61b1-103">removeProtectionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="d61b1-103">removeProtectionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d61b1-104">表示要移除其对文件的保护的操作或信息。</span><span class="sxs-lookup"><span data-stu-id="d61b1-104">Represents an action to remove protection from the file or information.</span></span> <span data-ttu-id="d61b1-105">[EvaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)、 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)或[EvaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) api 可能会返回**removeProtectionAction** ，如果由于更新或删除标签而要删除保护。</span><span class="sxs-lookup"><span data-stu-id="d61b1-105">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeProtectionAction** if protection is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="d61b1-106">该操作指示使用应用程序移除包含之前适用的内容头的特定 UI 元素。</span><span class="sxs-lookup"><span data-stu-id="d61b1-106">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span> <span data-ttu-id="d61b1-107">仅当呼叫用户具有足够的权限删除保护时，才应通过客户端库（如 Microsoft 信息保护 SDK）删除保护。</span><span class="sxs-lookup"><span data-stu-id="d61b1-107">Protection should be removed via a client library, such as the Microsoft Information Protection SDK, only if the calling user has sufficient rights to remove protection.</span></span>

## <a name="properties"></a><span data-ttu-id="d61b1-108">属性</span><span class="sxs-lookup"><span data-stu-id="d61b1-108">Properties</span></span>

<span data-ttu-id="d61b1-109">无</span><span class="sxs-lookup"><span data-stu-id="d61b1-109">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d61b1-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d61b1-110">JSON representation</span></span>

<span data-ttu-id="d61b1-111">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d61b1-111">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeProtectionAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "removeProtectionAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->