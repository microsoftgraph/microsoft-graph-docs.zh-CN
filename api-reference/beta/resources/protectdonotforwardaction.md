---
title: protectDoNotForwardAction 资源类型
description: 通知应用程序应用 "请勿转发保护"。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: db7605fb421878f258420f79c1cd06055624e53d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521360"
---
# <a name="protectdonotforwardaction-resource-type"></a><span data-ttu-id="29cfa-103">protectDoNotForwardAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="29cfa-103">protectDoNotForwardAction resource type</span></span>

<span data-ttu-id="29cfa-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="29cfa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29cfa-105">通知应用程序应用 "请勿转发保护"。</span><span class="sxs-lookup"><span data-stu-id="29cfa-105">Informs the application to apply Do Not Forward protection.</span></span> <span data-ttu-id="29cfa-106">如果生成的标签已配置为 "应用不[转发保护](https://docs.microsoft.com/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails)"，则[evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)或[evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)可能会返回**protectionDoNotForwardAction** 。</span><span class="sxs-lookup"><span data-stu-id="29cfa-106">**protectionDoNotForwardAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply [Do Not Forward protection](https://docs.microsoft.com/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails).</span></span> <span data-ttu-id="29cfa-107">使用的应用程序必须使用客户端库通过 Azure 信息保护来应用保护。</span><span class="sxs-lookup"><span data-stu-id="29cfa-107">The consuming application must use a client library to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="29cfa-108">属性</span><span class="sxs-lookup"><span data-stu-id="29cfa-108">Properties</span></span>

<span data-ttu-id="29cfa-109">无</span><span class="sxs-lookup"><span data-stu-id="29cfa-109">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29cfa-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29cfa-110">JSON representation</span></span>

<span data-ttu-id="29cfa-111">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29cfa-111">The following is a JSON representation of the resource.</span></span>

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
