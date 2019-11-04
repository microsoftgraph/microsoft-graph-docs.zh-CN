---
title: protectByTemplateAction 资源类型
description: 通知应用程序应应用 Azure 信息保护保护模板。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a7a557dfd72dac9161ae29436f5fc96eb55075d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939072"
---
# <a name="protectbytemplateaction-resource-type"></a><span data-ttu-id="95ee9-103">protectByTemplateAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="95ee9-103">protectByTemplateAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95ee9-104">通知应用程序应应用 Azure 信息保护保护模板。</span><span class="sxs-lookup"><span data-stu-id="95ee9-104">Informs the application that an Azure Information Protection protection template should be applied.</span></span> <span data-ttu-id="95ee9-105">如果生成的标签已配置为应用保护，则[evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)或[evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)可能会返回**protectionByTemplateAction** 。</span><span class="sxs-lookup"><span data-stu-id="95ee9-105">**protectionByTemplateAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply protection.</span></span> <span data-ttu-id="95ee9-106">正在使用的应用程序必须从结果中读取 templateId，然后使用客户端库（如 Microsoft 信息保护 SDK）通过 Azure 信息保护来应用保护。</span><span class="sxs-lookup"><span data-stu-id="95ee9-106">The consuming application must read the templateId from the result and then use a client library, such as the Microsoft Information Protection SDK, to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="95ee9-107">属性</span><span class="sxs-lookup"><span data-stu-id="95ee9-107">Properties</span></span>

| <span data-ttu-id="95ee9-108">属性</span><span class="sxs-lookup"><span data-stu-id="95ee9-108">Property</span></span>   | <span data-ttu-id="95ee9-109">类型</span><span class="sxs-lookup"><span data-stu-id="95ee9-109">Type</span></span>   | <span data-ttu-id="95ee9-110">描述</span><span class="sxs-lookup"><span data-stu-id="95ee9-110">Description</span></span>                                                                        |
| :--------- | :----- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="95ee9-111">templateId</span><span class="sxs-lookup"><span data-stu-id="95ee9-111">templateId</span></span> | <span data-ttu-id="95ee9-112">字符串</span><span class="sxs-lookup"><span data-stu-id="95ee9-112">String</span></span> | <span data-ttu-id="95ee9-113">要应用于信息的 Azure 信息保护模板的 GUID。</span><span class="sxs-lookup"><span data-stu-id="95ee9-113">The GUID of the Azure Information Protection template to apply to the information.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="95ee9-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95ee9-114">JSON representation</span></span>

<span data-ttu-id="95ee9-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95ee9-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.protectByTemplateAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "templateId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "protectByTemplateAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->