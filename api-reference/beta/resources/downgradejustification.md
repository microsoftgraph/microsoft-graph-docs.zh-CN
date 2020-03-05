---
title: downgradeJustification 资源类型
description: 表示有关执行降级的原因的用户输入。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 91bcb5a8e12a159bf2c6586a0e3dc49a540a69f2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505789"
---
# <a name="downgradejustification-resource-type"></a><span data-ttu-id="60496-103">downgradeJustification 资源类型</span><span class="sxs-lookup"><span data-stu-id="60496-103">downgradeJustification resource type</span></span>

<span data-ttu-id="60496-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="60496-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60496-105">表示有关执行降级的原因的用户输入。</span><span class="sxs-lookup"><span data-stu-id="60496-105">Represents user input on why downgrade was performed.</span></span> <span data-ttu-id="60496-106">根据 Office 安全与合规中心中的标签策略配置，可能需要降级理由。</span><span class="sxs-lookup"><span data-stu-id="60496-106">Downgrade justification might be required based on label policy configuration in Office Security and Compliance Center.</span></span>

## <a name="properties"></a><span data-ttu-id="60496-107">属性</span><span class="sxs-lookup"><span data-stu-id="60496-107">Properties</span></span>

| <span data-ttu-id="60496-108">属性</span><span class="sxs-lookup"><span data-stu-id="60496-108">Property</span></span>             | <span data-ttu-id="60496-109">类型</span><span class="sxs-lookup"><span data-stu-id="60496-109">Type</span></span>    | <span data-ttu-id="60496-110">说明</span><span class="sxs-lookup"><span data-stu-id="60496-110">Description</span></span>                                                                                          |
| :------------------- | :------ | :--------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="60496-111">isDowngradeJustified</span><span class="sxs-lookup"><span data-stu-id="60496-111">isDowngradeJustified</span></span> | <span data-ttu-id="60496-112">布尔</span><span class="sxs-lookup"><span data-stu-id="60496-112">Boolean</span></span> | <span data-ttu-id="60496-113">指示降级是还是未两端对齐。</span><span class="sxs-lookup"><span data-stu-id="60496-113">Indicates whether the downgrade is or is not justified.</span></span>                                              |
| <span data-ttu-id="60496-114">justificationMessage</span><span class="sxs-lookup"><span data-stu-id="60496-114">justificationMessage</span></span> | <span data-ttu-id="60496-115">String</span><span class="sxs-lookup"><span data-stu-id="60496-115">String</span></span>  | <span data-ttu-id="60496-116">指示降级的原因的消息。</span><span class="sxs-lookup"><span data-stu-id="60496-116">Message that indicates why a downgrade is justified.</span></span> <span data-ttu-id="60496-117">该邮件将显示在 "管理日志" 中。</span><span class="sxs-lookup"><span data-stu-id="60496-117">The message will appear in administrative logs.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="60496-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60496-118">JSON representation</span></span>

<span data-ttu-id="60496-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60496-119">The following is a JSON representation of the resource.</span></span>

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