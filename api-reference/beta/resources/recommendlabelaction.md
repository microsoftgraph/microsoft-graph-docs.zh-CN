---
title: recommendLabelAction 资源类型
description: 表示一个标签，应根据敏感信息类型向用户推荐针对该文件的应用程序。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54f2a872c0aa64eb79e0b8755ddc6b3788f14055
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939374"
---
# <a name="recommendlabelaction-resource-type"></a><span data-ttu-id="0ad01-103">recommendLabelAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ad01-103">recommendLabelAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ad01-104">表示一个标签，应根据所发现的敏感信息类型向用户推荐针对该文件的应用程序。</span><span class="sxs-lookup"><span data-stu-id="0ad01-104">Represents a label that should be recommended to the user for application to the file based on discovered sensitive information types.</span></span> <span data-ttu-id="0ad01-105">如果 Microsoft 信息保护标记策略设置为 "**推荐**" 和 "标签"，而不是 "强制" 标签，则[evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md)可能会返回**recommendLabelAction** 。</span><span class="sxs-lookup"><span data-stu-id="0ad01-105">The [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) may return a **recommendLabelAction** if the Microsoft Information Protection labeling policy is set to **recommend** and label rather than enforce a label.</span></span> <span data-ttu-id="0ad01-106">用户或 appliation 可以选择忽略或接受建议。</span><span class="sxs-lookup"><span data-stu-id="0ad01-106">The user or appliation may choose to ignore or accept the recommendation.</span></span> 

## <a name="properties"></a><span data-ttu-id="0ad01-107">属性</span><span class="sxs-lookup"><span data-stu-id="0ad01-107">Properties</span></span>

| <span data-ttu-id="0ad01-108">属性</span><span class="sxs-lookup"><span data-stu-id="0ad01-108">Property</span></span>                    | <span data-ttu-id="0ad01-109">类型</span><span class="sxs-lookup"><span data-stu-id="0ad01-109">Type</span></span>                                                                     | <span data-ttu-id="0ad01-110">描述</span><span class="sxs-lookup"><span data-stu-id="0ad01-110">Description</span></span>                                                           |
| :-------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| <span data-ttu-id="0ad01-111">actionSource</span><span class="sxs-lookup"><span data-stu-id="0ad01-111">actionSource</span></span>                | <span data-ttu-id="0ad01-112">String</span><span class="sxs-lookup"><span data-stu-id="0ad01-112">String</span></span>                                                                   | <span data-ttu-id="0ad01-113">可能的值是：`manual`、`automatic`、`recommended`、`default`。</span><span class="sxs-lookup"><span data-stu-id="0ad01-113">Possible values are: `manual`, `automatic`, `recommended`, `default`.</span></span> |
| <span data-ttu-id="0ad01-114">actions</span><span class="sxs-lookup"><span data-stu-id="0ad01-114">actions</span></span>                     | <span data-ttu-id="0ad01-115">[informationProtectionAction](informationprotectionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="0ad01-115">[informationProtectionAction](informationprotectionaction.md) collection</span></span> | <span data-ttu-id="0ad01-116">用户接受标签时要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="0ad01-116">Actions to take if the label is accepted by the user.</span></span>                                                                       |
| <span data-ttu-id="0ad01-117">label</span><span class="sxs-lookup"><span data-stu-id="0ad01-117">label</span></span>                       | [<span data-ttu-id="0ad01-118">labelDetails</span><span class="sxs-lookup"><span data-stu-id="0ad01-118">labelDetails</span></span>](labeldetails.md)                                          | <span data-ttu-id="0ad01-119">建议使用的标签。</span><span class="sxs-lookup"><span data-stu-id="0ad01-119">The label that is being recommended.</span></span>                                                                      |
| <span data-ttu-id="0ad01-120">responsibleSensitiveTypeIds</span><span class="sxs-lookup"><span data-stu-id="0ad01-120">responsibleSensitiveTypeIds</span></span> | <span data-ttu-id="0ad01-121">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="0ad01-121">Guid collection</span></span>                                                          | <span data-ttu-id="0ad01-122">导致提供建议的敏感信息类型 Guid。</span><span class="sxs-lookup"><span data-stu-id="0ad01-122">The sensitive information type GUIDs that caused the recommendation to be given.</span></span>                                                                      |

## <a name="json-representation"></a><span data-ttu-id="0ad01-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ad01-123">JSON representation</span></span>

<span data-ttu-id="0ad01-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ad01-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recommendLabelAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "actionSource": "String",
  "actions": [{"@odata.type": "microsoft.graph.informationProtectionAction"}],
  "label": {"@odata.type": "microsoft.graph.labelDetails"},
  "responsibleSensitiveTypeIds": ["Guid"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recommendLabelAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
