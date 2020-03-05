---
title: customAction 资源类型
description: 表示标签可能提供的任何自定义操作（如果由管理员配置）。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e2a660659f8c0f3a2c6dc571e743884c54365a20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507322"
---
# <a name="customaction-resource-type"></a><span data-ttu-id="f1efa-103">customAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1efa-103">customAction resource type</span></span>

<span data-ttu-id="f1efa-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f1efa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1efa-105">表示标签可能提供的任何自定义操作（如果由管理员配置）。</span><span class="sxs-lookup"><span data-stu-id="f1efa-105">Represents any custom actions that a label may provide, if configured by the administrator.</span></span> <span data-ttu-id="f1efa-106">自定义操作可能是通过 Office 365 安全与合规中心的 PowerShell 模块定义为[informationProtectionLabel](informationProtectionLabel.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="f1efa-106">Custom actions might be defined as part of an [informationProtectionLabel](informationProtectionLabel.md) via Office 365 Security and Compliance Center's PowerShell module.</span></span> <span data-ttu-id="f1efa-107">操作必须由使用中的应用程序理解。</span><span class="sxs-lookup"><span data-stu-id="f1efa-107">The actions must be understood by the consuming application.</span></span>

## <a name="properties"></a><span data-ttu-id="f1efa-108">属性</span><span class="sxs-lookup"><span data-stu-id="f1efa-108">Properties</span></span>

| <span data-ttu-id="f1efa-109">属性</span><span class="sxs-lookup"><span data-stu-id="f1efa-109">Property</span></span>   | <span data-ttu-id="f1efa-110">类型</span><span class="sxs-lookup"><span data-stu-id="f1efa-110">Type</span></span>                                       | <span data-ttu-id="f1efa-111">说明</span><span class="sxs-lookup"><span data-stu-id="f1efa-111">Description</span></span>                                          |
| :--------- | :----------------------------------------- | :--------------------------------------------------- |
| <span data-ttu-id="f1efa-112">name</span><span class="sxs-lookup"><span data-stu-id="f1efa-112">name</span></span>       | <span data-ttu-id="f1efa-113">String</span><span class="sxs-lookup"><span data-stu-id="f1efa-113">String</span></span>                                     | <span data-ttu-id="f1efa-114">自定义操作的名称。</span><span class="sxs-lookup"><span data-stu-id="f1efa-114">Name of the custom action.</span></span>                           |
| <span data-ttu-id="f1efa-115">properties</span><span class="sxs-lookup"><span data-stu-id="f1efa-115">properties</span></span> | <span data-ttu-id="f1efa-116">[keyValuePair](keyvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1efa-116">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="f1efa-117">操作的属性（按键值对格式）。</span><span class="sxs-lookup"><span data-stu-id="f1efa-117">Properties, in key value pair format, of the action.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f1efa-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1efa-118">JSON representation</span></span>

<span data-ttu-id="f1efa-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1efa-119">The following is a JSON representation of the resource.</span></span>

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