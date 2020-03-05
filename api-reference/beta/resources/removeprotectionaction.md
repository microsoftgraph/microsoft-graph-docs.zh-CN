---
title: removeProtectionAction 资源类型
description: 表示要移除其对文件的保护的操作或信息。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 63a539fe4366703aaeb7e6b16735bb0302951dd7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521143"
---
# <a name="removeprotectionaction-resource-type"></a><span data-ttu-id="8e10e-103">removeProtectionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e10e-103">removeProtectionAction resource type</span></span>

<span data-ttu-id="8e10e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8e10e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e10e-105">表示要移除其对文件的保护的操作或信息。</span><span class="sxs-lookup"><span data-stu-id="8e10e-105">Represents an action to remove protection from the file or information.</span></span> <span data-ttu-id="8e10e-106">[EvaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)、 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)或[EvaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) api 可能会返回**removeProtectionAction** ，如果由于更新或删除标签而要删除保护。</span><span class="sxs-lookup"><span data-stu-id="8e10e-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeProtectionAction** if protection is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="8e10e-107">该操作指示使用应用程序移除包含之前适用的内容头的特定 UI 元素。</span><span class="sxs-lookup"><span data-stu-id="8e10e-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span> <span data-ttu-id="8e10e-108">仅当呼叫用户具有足够的权限删除保护时，才应通过客户端库（如 Microsoft 信息保护 SDK）删除保护。</span><span class="sxs-lookup"><span data-stu-id="8e10e-108">Protection should be removed via a client library, such as the Microsoft Information Protection SDK, only if the calling user has sufficient rights to remove protection.</span></span>

## <a name="properties"></a><span data-ttu-id="8e10e-109">属性</span><span class="sxs-lookup"><span data-stu-id="8e10e-109">Properties</span></span>

<span data-ttu-id="8e10e-110">无</span><span class="sxs-lookup"><span data-stu-id="8e10e-110">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e10e-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e10e-111">JSON representation</span></span>

<span data-ttu-id="8e10e-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e10e-112">The following is a JSON representation of the resource.</span></span>

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