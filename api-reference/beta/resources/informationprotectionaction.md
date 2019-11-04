---
title: informationProtectionAction 资源类型
description: 介绍 abtract informationProtectionAction 实体。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c0d3bb7ed9464bf4b41d8bd03f6c1835bdce468e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938833"
---
# <a name="informationprotectionaction-resource-type"></a><span data-ttu-id="0375f-103">informationProtectionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="0375f-103">informationProtectionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0375f-104">**InformationProtectionAction**是一个作为任何信息保护评估 api 的结果返回的抽象实体。</span><span class="sxs-lookup"><span data-stu-id="0375f-104">The **informationProtectionAction** is an abstract entity that is returned as the result of any of the information protection evaluation APIs.</span></span> <span data-ttu-id="0375f-105">对象包含以下一个或多个操作，这些操作指示应用程序如何应用、更新或删除信息保护标签。</span><span class="sxs-lookup"><span data-stu-id="0375f-105">The object contains one or more of the following actions that instruct the application on how to apply, update, or remove the information protection label.</span></span> 

* [<span data-ttu-id="0375f-106">addContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="0375f-106">addContentFooterAction</span></span>](../resources/addcontentfooteraction.md)
* [<span data-ttu-id="0375f-107">addContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="0375f-107">addContentHeaderAction</span></span>](../resources/addcontentheaderaction.md)
* [<span data-ttu-id="0375f-108">addWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="0375f-108">addWatermarkAction</span></span>](../resources/addwatermarkaction.md)
* [<span data-ttu-id="0375f-109">applyLabelAction</span><span class="sxs-lookup"><span data-stu-id="0375f-109">applyLabelAction</span></span>](../resources/applylabelaction.md)
* [<span data-ttu-id="0375f-110">customAction</span><span class="sxs-lookup"><span data-stu-id="0375f-110">customAction</span></span>](../resources/customaction.md)
* [<span data-ttu-id="0375f-111">justifyAction</span><span class="sxs-lookup"><span data-stu-id="0375f-111">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="0375f-112">metadataAction</span><span class="sxs-lookup"><span data-stu-id="0375f-112">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="0375f-113">protectAdhocAction</span><span class="sxs-lookup"><span data-stu-id="0375f-113">protectAdhocAction</span></span>](../resources/protectadhocaction.md)
* [<span data-ttu-id="0375f-114">protectByTemplateAction</span><span class="sxs-lookup"><span data-stu-id="0375f-114">protectByTemplateAction</span></span>](../resources/protectbytemplateaction.md)
* [<span data-ttu-id="0375f-115">protectionDoNotForwardAction</span><span class="sxs-lookup"><span data-stu-id="0375f-115">protectionDoNotForwardAction</span></span>](../resources/protectdonotforwardaction.md)
* [<span data-ttu-id="0375f-116">recommendLabelAction</span><span class="sxs-lookup"><span data-stu-id="0375f-116">recommendLabelAction</span></span>](../resources/recommendlabelaction.md)
* [<span data-ttu-id="0375f-117">removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="0375f-117">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="0375f-118">removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="0375f-118">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="0375f-119">removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="0375f-119">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="0375f-120">removeWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="0375f-120">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="properties"></a><span data-ttu-id="0375f-121">属性</span><span class="sxs-lookup"><span data-stu-id="0375f-121">Properties</span></span>

<span data-ttu-id="0375f-122">无</span><span class="sxs-lookup"><span data-stu-id="0375f-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0375f-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0375f-123">JSON representation</span></span>

<span data-ttu-id="0375f-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0375f-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.informationProtectionAction",
  "baseType": null
}-->

```json
{

}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->