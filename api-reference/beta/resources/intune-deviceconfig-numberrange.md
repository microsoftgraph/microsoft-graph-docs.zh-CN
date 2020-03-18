---
title: numberRange 资源类型
description: 号码范围定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2e3073de15fc84f5a8cb755d6aad32caaf1ee29f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788490"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="b20e9-103">numberRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="b20e9-103">numberRange resource type</span></span>

> <span data-ttu-id="b20e9-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b20e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b20e9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b20e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b20e9-106">号码范围定义。</span><span class="sxs-lookup"><span data-stu-id="b20e9-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="b20e9-107">属性</span><span class="sxs-lookup"><span data-stu-id="b20e9-107">Properties</span></span>
|<span data-ttu-id="b20e9-108">属性</span><span class="sxs-lookup"><span data-stu-id="b20e9-108">Property</span></span>|<span data-ttu-id="b20e9-109">类型</span><span class="sxs-lookup"><span data-stu-id="b20e9-109">Type</span></span>|<span data-ttu-id="b20e9-110">说明</span><span class="sxs-lookup"><span data-stu-id="b20e9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b20e9-111">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="b20e9-111">lowerNumber</span></span>|<span data-ttu-id="b20e9-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b20e9-112">Int32</span></span>|<span data-ttu-id="b20e9-113">较小的数字。</span><span class="sxs-lookup"><span data-stu-id="b20e9-113">Lower number.</span></span>|
|<span data-ttu-id="b20e9-114">upperNumber</span><span class="sxs-lookup"><span data-stu-id="b20e9-114">upperNumber</span></span>|<span data-ttu-id="b20e9-115">Int32</span><span class="sxs-lookup"><span data-stu-id="b20e9-115">Int32</span></span>|<span data-ttu-id="b20e9-116">上限数。</span><span class="sxs-lookup"><span data-stu-id="b20e9-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b20e9-117">关系</span><span class="sxs-lookup"><span data-stu-id="b20e9-117">Relationships</span></span>
<span data-ttu-id="b20e9-118">无</span><span class="sxs-lookup"><span data-stu-id="b20e9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b20e9-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b20e9-119">JSON Representation</span></span>
<span data-ttu-id="b20e9-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b20e9-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```



