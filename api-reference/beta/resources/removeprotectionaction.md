---
title: removeProtectionAction 资源类型
description: 表示从文件或信息中删除保护的操作。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2b315c9d2641524d8a134f0e0b9704c51419ada4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962033"
---
# <a name="removeprotectionaction-resource-type"></a><span data-ttu-id="8cd04-103">removeProtectionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="8cd04-103">removeProtectionAction resource type</span></span>

<span data-ttu-id="8cd04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cd04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cd04-105">表示从文件或信息中删除保护的操作。</span><span class="sxs-lookup"><span data-stu-id="8cd04-105">Represents an action to remove protection from the file or information.</span></span> <span data-ttu-id="8cd04-106">如果由于更新或删除标签而要删除保护，则 evaluateApplication、evaluateClassificationResults 或 [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) API 可能会返回 **removeProtectionAction。** [](../api/informationprotectionlabel-evaluateapplication.md) [](../api/informationprotectionlabel-evaluateclassificationresults.md)</span><span class="sxs-lookup"><span data-stu-id="8cd04-106">The [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md), or [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) APIs may return the **removeProtectionAction** if protection is to be removed as a result of updating or removing the label.</span></span> <span data-ttu-id="8cd04-107">此操作指示使用应用程序删除包含以前适用的内容标头的特定 UI 元素。</span><span class="sxs-lookup"><span data-stu-id="8cd04-107">The action instructs the consuming application to remove the specific UI element that contains the previously-applicable content header.</span></span> <span data-ttu-id="8cd04-108">只有在调用用户具有删除保护的足够权限时，才应删除通过客户端库（如 Microsoft 信息保护 SDK）的保护。</span><span class="sxs-lookup"><span data-stu-id="8cd04-108">Protection should be removed via a client library, such as the Microsoft Information Protection SDK, only if the calling user has sufficient rights to remove protection.</span></span>

## <a name="properties"></a><span data-ttu-id="8cd04-109">属性</span><span class="sxs-lookup"><span data-stu-id="8cd04-109">Properties</span></span>

<span data-ttu-id="8cd04-110">无</span><span class="sxs-lookup"><span data-stu-id="8cd04-110">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cd04-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8cd04-111">JSON representation</span></span>

<span data-ttu-id="8cd04-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cd04-112">The following is a JSON representation of the resource.</span></span>

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

