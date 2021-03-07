---
title: printSettings 资源类型
description: 表示通用打印服务的租户范围设置。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 53e0db2a1923cad0af1f35baf5bed6fecd896fb3
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516987"
---
# <a name="printsettings-resource-type"></a><span data-ttu-id="4b582-103">printSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b582-103">printSettings resource type</span></span>

<span data-ttu-id="4b582-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b582-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="4b582-105">表示通用打印服务的租户范围设置。</span><span class="sxs-lookup"><span data-stu-id="4b582-105">Represents tenant-wide settings for the Universal Print service.</span></span>

## <a name="properties"></a><span data-ttu-id="4b582-106">属性</span><span class="sxs-lookup"><span data-stu-id="4b582-106">Properties</span></span>
|<span data-ttu-id="4b582-107">属性</span><span class="sxs-lookup"><span data-stu-id="4b582-107">Property</span></span>|<span data-ttu-id="4b582-108">类型</span><span class="sxs-lookup"><span data-stu-id="4b582-108">Type</span></span>|<span data-ttu-id="4b582-109">Description</span><span class="sxs-lookup"><span data-stu-id="4b582-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b582-110">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="4b582-110">documentConversionEnabled</span></span>|<span data-ttu-id="4b582-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b582-111">Boolean</span></span>|<span data-ttu-id="4b582-112">指定是否对租户启用文档转换。</span><span class="sxs-lookup"><span data-stu-id="4b582-112">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="4b582-113">如果启用文档转换，通用打印服务将自动将文档转换为与打印机兼容格式， (xps) pdf 格式。</span><span class="sxs-lookup"><span data-stu-id="4b582-113">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (xps to pdf) when needed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b582-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b582-114">JSON representation</span></span>
<span data-ttu-id="4b582-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b582-115">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printSettings",
  "documentConversionEnabled": "Boolean"
}
```

