---
title: downgradeJustification 资源类型
description: 表示有关执行降级的原因的用户输入。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aacc32ac86df4eda087f49dbb3dca05a356e8080
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939423"
---
# <a name="downgradejustification-resource-type"></a><span data-ttu-id="4c6e0-103">downgradeJustification 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c6e0-103">downgradeJustification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c6e0-104">表示有关执行降级的原因的用户输入。</span><span class="sxs-lookup"><span data-stu-id="4c6e0-104">Represents user input on why downgrade was performed.</span></span> <span data-ttu-id="4c6e0-105">根据 Office 安全与合规中心中的标签策略配置，可能需要降级理由。</span><span class="sxs-lookup"><span data-stu-id="4c6e0-105">Downgrade justification might be required based on label policy configuration in Office Security and Compliance Center.</span></span>

## <a name="properties"></a><span data-ttu-id="4c6e0-106">属性</span><span class="sxs-lookup"><span data-stu-id="4c6e0-106">Properties</span></span>

| <span data-ttu-id="4c6e0-107">属性</span><span class="sxs-lookup"><span data-stu-id="4c6e0-107">Property</span></span>             | <span data-ttu-id="4c6e0-108">类型</span><span class="sxs-lookup"><span data-stu-id="4c6e0-108">Type</span></span>    | <span data-ttu-id="4c6e0-109">描述</span><span class="sxs-lookup"><span data-stu-id="4c6e0-109">Description</span></span>                                                                                          |
| :------------------- | :------ | :--------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="4c6e0-110">isDowngradeJustified</span><span class="sxs-lookup"><span data-stu-id="4c6e0-110">isDowngradeJustified</span></span> | <span data-ttu-id="4c6e0-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c6e0-111">Boolean</span></span> | <span data-ttu-id="4c6e0-112">指示降级是还是未两端对齐。</span><span class="sxs-lookup"><span data-stu-id="4c6e0-112">Indicates whether the downgrade is or is not justified.</span></span>                                              |
| <span data-ttu-id="4c6e0-113">justificationMessage</span><span class="sxs-lookup"><span data-stu-id="4c6e0-113">justificationMessage</span></span> | <span data-ttu-id="4c6e0-114">字符串</span><span class="sxs-lookup"><span data-stu-id="4c6e0-114">String</span></span>  | <span data-ttu-id="4c6e0-115">指示降级的原因的消息。</span><span class="sxs-lookup"><span data-stu-id="4c6e0-115">Message that indicates why a downgrade is justified.</span></span> <span data-ttu-id="4c6e0-116">该邮件将显示在 "管理日志" 中。</span><span class="sxs-lookup"><span data-stu-id="4c6e0-116">The message will appear in administrative logs.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4c6e0-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c6e0-117">JSON representation</span></span>

<span data-ttu-id="4c6e0-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c6e0-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.downgradeJustification",
  "baseType": null
}-->

```json
{
  "isDowngradeJustified": true,
  "justificationMessage": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "downgradeJustification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->