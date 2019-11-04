---
title: customAction 资源类型
description: 表示标签可能提供的任何自定义操作（如果由管理员配置）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bbb3fc99ce474752fd2382d5777afeb1c56f632e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938868"
---
# <a name="customaction-resource-type"></a><span data-ttu-id="736f5-103">customAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="736f5-103">customAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="736f5-104">表示标签可能提供的任何自定义操作（如果由管理员配置）。</span><span class="sxs-lookup"><span data-stu-id="736f5-104">Represents any custom actions that a label may provide, if configured by the administrator.</span></span> <span data-ttu-id="736f5-105">自定义操作可能是通过 Office 365 安全与合规中心的 PowerShell 模块定义为[informationProtectionLabel](informationProtectionLabel.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="736f5-105">Custom actions might be defined as part of an [informationProtectionLabel](informationProtectionLabel.md) via Office 365 Security and Compliance Center's PowerShell module.</span></span> <span data-ttu-id="736f5-106">操作必须由使用中的应用程序理解。</span><span class="sxs-lookup"><span data-stu-id="736f5-106">The actions must be understood by the consuming application.</span></span>

## <a name="properties"></a><span data-ttu-id="736f5-107">属性</span><span class="sxs-lookup"><span data-stu-id="736f5-107">Properties</span></span>

| <span data-ttu-id="736f5-108">属性</span><span class="sxs-lookup"><span data-stu-id="736f5-108">Property</span></span>   | <span data-ttu-id="736f5-109">类型</span><span class="sxs-lookup"><span data-stu-id="736f5-109">Type</span></span>                                       | <span data-ttu-id="736f5-110">描述</span><span class="sxs-lookup"><span data-stu-id="736f5-110">Description</span></span>                                          |
| :--------- | :----------------------------------------- | :--------------------------------------------------- |
| <span data-ttu-id="736f5-111">name</span><span class="sxs-lookup"><span data-stu-id="736f5-111">name</span></span>       | <span data-ttu-id="736f5-112">字符串</span><span class="sxs-lookup"><span data-stu-id="736f5-112">String</span></span>                                     | <span data-ttu-id="736f5-113">自定义操作的名称。</span><span class="sxs-lookup"><span data-stu-id="736f5-113">Name of the custom action.</span></span>                           |
| <span data-ttu-id="736f5-114">properties</span><span class="sxs-lookup"><span data-stu-id="736f5-114">properties</span></span> | <span data-ttu-id="736f5-115">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="736f5-115">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="736f5-116">操作的属性（按键值对格式）。</span><span class="sxs-lookup"><span data-stu-id="736f5-116">Properties, in key value pair format, of the action.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="736f5-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="736f5-117">JSON representation</span></span>

<span data-ttu-id="736f5-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="736f5-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.customAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "name": "String",
  "properties": [{"@odata.type": "microsoft.graph.keyValuePair"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "customAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->