---
title: protectByTemplateAction 资源类型
description: 通知应用程序应应用 Azure 信息保护保护模板。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3fc936179a0c0764492a3dc8d677060931a1223a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521367"
---
# <a name="protectbytemplateaction-resource-type"></a><span data-ttu-id="f35d9-103">protectByTemplateAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="f35d9-103">protectByTemplateAction resource type</span></span>

<span data-ttu-id="f35d9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f35d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f35d9-105">通知应用程序应应用 Azure 信息保护保护模板。</span><span class="sxs-lookup"><span data-stu-id="f35d9-105">Informs the application that an Azure Information Protection protection template should be applied.</span></span> <span data-ttu-id="f35d9-106">如果生成的标签已配置为应用保护，则[evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)或[evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)可能会返回**protectionByTemplateAction** 。</span><span class="sxs-lookup"><span data-stu-id="f35d9-106">**protectionByTemplateAction** may be returned by [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md) or [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) if the resulting label has been configured to apply protection.</span></span> <span data-ttu-id="f35d9-107">正在使用的应用程序必须从结果中读取 templateId，然后使用客户端库（如 Microsoft 信息保护 SDK）通过 Azure 信息保护来应用保护。</span><span class="sxs-lookup"><span data-stu-id="f35d9-107">The consuming application must read the templateId from the result and then use a client library, such as the Microsoft Information Protection SDK, to apply protection via Azure Information Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="f35d9-108">属性</span><span class="sxs-lookup"><span data-stu-id="f35d9-108">Properties</span></span>

| <span data-ttu-id="f35d9-109">属性</span><span class="sxs-lookup"><span data-stu-id="f35d9-109">Property</span></span>   | <span data-ttu-id="f35d9-110">类型</span><span class="sxs-lookup"><span data-stu-id="f35d9-110">Type</span></span>   | <span data-ttu-id="f35d9-111">说明</span><span class="sxs-lookup"><span data-stu-id="f35d9-111">Description</span></span>                                                                        |
| :--------- | :----- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="f35d9-112">templateId</span><span class="sxs-lookup"><span data-stu-id="f35d9-112">templateId</span></span> | <span data-ttu-id="f35d9-113">String</span><span class="sxs-lookup"><span data-stu-id="f35d9-113">String</span></span> | <span data-ttu-id="f35d9-114">要应用于信息的 Azure 信息保护模板的 GUID。</span><span class="sxs-lookup"><span data-stu-id="f35d9-114">The GUID of the Azure Information Protection template to apply to the information.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f35d9-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f35d9-115">JSON representation</span></span>

<span data-ttu-id="f35d9-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f35d9-116">The following is a JSON representation of the resource.</span></span>

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