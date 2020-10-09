---
title: protectDoNotForwardAction 资源类型
description: 通知应用程序应用 "请勿转发保护"。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8fdb60651e98148eefb7bd964e8c4cd13ff81663
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404383"
---
# <a name="protectdonotforwardaction-resource-type"></a><span data-ttu-id="db547-103">protectDoNotForwardAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="db547-103">protectDoNotForwardAction resource type</span></span>

<span data-ttu-id="db547-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db547-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db547-105">通知应用程序应用 "请勿转发保护"。</span><span class="sxs-lookup"><span data-stu-id="db547-105">Informs the application to apply Do Not Forward protection.</span></span> <span data-ttu-id="db547-106">如果生成的标签已配置为 "应用不[转发保护](/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails)"，则[evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)或[evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)可能会返回**protectionDoNotForwardAction** 。</span><span class="sxs-lookup"><span data-stu-id="db547-106">**protectionDoNotForwardAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply [Do Not Forward protection](/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails).</span></span> <span data-ttu-id="db547-107">使用的应用程序必须使用客户端库通过 Azure 信息保护来应用保护。</span><span class="sxs-lookup"><span data-stu-id="db547-107">The consuming application must use a client library to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="db547-108">属性</span><span class="sxs-lookup"><span data-stu-id="db547-108">Properties</span></span>

<span data-ttu-id="db547-109">无</span><span class="sxs-lookup"><span data-stu-id="db547-109">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db547-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db547-110">JSON representation</span></span>

<span data-ttu-id="db547-111">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db547-111">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.protectDoNotForwardAction",
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
  "description": "protectDoNotForwardAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->