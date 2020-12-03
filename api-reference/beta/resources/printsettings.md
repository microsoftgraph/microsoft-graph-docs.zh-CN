---
title: printSettings 资源类型
description: 表示通用打印服务的租户范围的设置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 01c98eb68031018e6f7a32837e49a2095c7880d2
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521234"
---
# <a name="printsettings-resource-type"></a><span data-ttu-id="92060-103">printSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="92060-103">printSettings resource type</span></span>

<span data-ttu-id="92060-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92060-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92060-105">表示通用打印服务的租户范围的设置。</span><span class="sxs-lookup"><span data-stu-id="92060-105">Represents tenant-wide settings for the Universal Print service.</span></span>

## <a name="properties"></a><span data-ttu-id="92060-106">属性</span><span class="sxs-lookup"><span data-stu-id="92060-106">Properties</span></span>
| <span data-ttu-id="92060-107">属性</span><span class="sxs-lookup"><span data-stu-id="92060-107">Property</span></span>     | <span data-ttu-id="92060-108">类型</span><span class="sxs-lookup"><span data-stu-id="92060-108">Type</span></span>        | <span data-ttu-id="92060-109">说明</span><span class="sxs-lookup"><span data-stu-id="92060-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="92060-110">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="92060-110">documentConversionEnabled</span></span>|<span data-ttu-id="92060-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="92060-111">Boolean</span></span>|<span data-ttu-id="92060-112">指定是否为租户启用文档转换。</span><span class="sxs-lookup"><span data-stu-id="92060-112">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="92060-113">如果启用了文档转换，则通用打印服务会在需要时自动将文档转换为与打印机 (xps) 兼容的格式。</span><span class="sxs-lookup"><span data-stu-id="92060-113">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (xps to pdf) when needed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92060-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92060-114">JSON representation</span></span>

<span data-ttu-id="92060-115">以下是 printSettings 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92060-115">The following is a JSON representation of printSettings.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printSettings"
}-->

```json
{
  "documentConversionEnabled": true
}
```


