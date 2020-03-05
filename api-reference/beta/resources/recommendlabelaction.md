---
title: recommendLabelAction 资源类型
description: 表示一个标签，应根据敏感信息类型向用户推荐针对该文件的应用程序。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2a4da2900ec12233e680238fb294c38a9e17ebbe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521234"
---
# <a name="recommendlabelaction-resource-type"></a><span data-ttu-id="81778-103">recommendLabelAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="81778-103">recommendLabelAction resource type</span></span>

<span data-ttu-id="81778-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="81778-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81778-105">表示一个标签，应根据所发现的敏感信息类型向用户推荐针对该文件的应用程序。</span><span class="sxs-lookup"><span data-stu-id="81778-105">Represents a label that should be recommended to the user for application to the file based on discovered sensitive information types.</span></span> <span data-ttu-id="81778-106">如果 Microsoft 信息保护标记策略设置为 "**推荐**" 和 "标签"，而不是 "强制" 标签，则[evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md)可能会返回**recommendLabelAction** 。</span><span class="sxs-lookup"><span data-stu-id="81778-106">The [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md) may return a **recommendLabelAction** if the Microsoft Information Protection labeling policy is set to **recommend** and label rather than enforce a label.</span></span> <span data-ttu-id="81778-107">用户或 appliation 可以选择忽略或接受建议。</span><span class="sxs-lookup"><span data-stu-id="81778-107">The user or appliation may choose to ignore or accept the recommendation.</span></span> 

## <a name="properties"></a><span data-ttu-id="81778-108">属性</span><span class="sxs-lookup"><span data-stu-id="81778-108">Properties</span></span>

| <span data-ttu-id="81778-109">属性</span><span class="sxs-lookup"><span data-stu-id="81778-109">Property</span></span>                    | <span data-ttu-id="81778-110">类型</span><span class="sxs-lookup"><span data-stu-id="81778-110">Type</span></span>                                                                     | <span data-ttu-id="81778-111">说明</span><span class="sxs-lookup"><span data-stu-id="81778-111">Description</span></span>                                                           |
| :-------------------------- | :----------------------------------------------------------------------- | :-------------------------------------------------------------------- |
| <span data-ttu-id="81778-112">actionSource</span><span class="sxs-lookup"><span data-stu-id="81778-112">actionSource</span></span>                | <span data-ttu-id="81778-113">String</span><span class="sxs-lookup"><span data-stu-id="81778-113">String</span></span>                                                                   | <span data-ttu-id="81778-114">可能的值是：`manual`、`automatic`、`recommended`、`default`。</span><span class="sxs-lookup"><span data-stu-id="81778-114">Possible values are: `manual`, `automatic`, `recommended`, `default`.</span></span> |
| <span data-ttu-id="81778-115">actions</span><span class="sxs-lookup"><span data-stu-id="81778-115">actions</span></span>                     | <span data-ttu-id="81778-116">[informationProtectionAction](informationprotectionaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="81778-116">[informationProtectionAction](informationprotectionaction.md) collection</span></span> | <span data-ttu-id="81778-117">用户接受标签时要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="81778-117">Actions to take if the label is accepted by the user.</span></span>                                                                       |
| <span data-ttu-id="81778-118">label</span><span class="sxs-lookup"><span data-stu-id="81778-118">label</span></span>                       | [<span data-ttu-id="81778-119">labelDetails</span><span class="sxs-lookup"><span data-stu-id="81778-119">labelDetails</span></span>](labeldetails.md)                                          | <span data-ttu-id="81778-120">建议使用的标签。</span><span class="sxs-lookup"><span data-stu-id="81778-120">The label that is being recommended.</span></span>                                                                      |
| <span data-ttu-id="81778-121">responsibleSensitiveTypeIds</span><span class="sxs-lookup"><span data-stu-id="81778-121">responsibleSensitiveTypeIds</span></span> | <span data-ttu-id="81778-122">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="81778-122">Guid collection</span></span>                                                          | <span data-ttu-id="81778-123">导致提供建议的敏感信息类型 Guid。</span><span class="sxs-lookup"><span data-stu-id="81778-123">The sensitive information type GUIDs that caused the recommendation to be given.</span></span>                                                                      |

## <a name="json-representation"></a><span data-ttu-id="81778-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81778-124">JSON representation</span></span>

<span data-ttu-id="81778-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81778-125">The following is a JSON representation of the resource.</span></span>

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
