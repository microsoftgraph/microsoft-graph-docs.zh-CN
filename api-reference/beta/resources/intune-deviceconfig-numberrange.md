---
title: numberRange 资源类型
description: 号码范围定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8f637cb10e36ba1f2d7c45e391adc64c6e9eb00b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722997"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="09ebc-103">numberRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="09ebc-103">numberRange resource type</span></span>

<span data-ttu-id="09ebc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09ebc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09ebc-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="09ebc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09ebc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="09ebc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09ebc-107">号码范围定义。</span><span class="sxs-lookup"><span data-stu-id="09ebc-107">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="09ebc-108">属性</span><span class="sxs-lookup"><span data-stu-id="09ebc-108">Properties</span></span>
|<span data-ttu-id="09ebc-109">属性</span><span class="sxs-lookup"><span data-stu-id="09ebc-109">Property</span></span>|<span data-ttu-id="09ebc-110">类型</span><span class="sxs-lookup"><span data-stu-id="09ebc-110">Type</span></span>|<span data-ttu-id="09ebc-111">说明</span><span class="sxs-lookup"><span data-stu-id="09ebc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09ebc-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="09ebc-112">lowerNumber</span></span>|<span data-ttu-id="09ebc-113">Int32</span><span class="sxs-lookup"><span data-stu-id="09ebc-113">Int32</span></span>|<span data-ttu-id="09ebc-114">较小的数字。</span><span class="sxs-lookup"><span data-stu-id="09ebc-114">Lower number.</span></span>|
|<span data-ttu-id="09ebc-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="09ebc-115">upperNumber</span></span>|<span data-ttu-id="09ebc-116">Int32</span><span class="sxs-lookup"><span data-stu-id="09ebc-116">Int32</span></span>|<span data-ttu-id="09ebc-117">上限数。</span><span class="sxs-lookup"><span data-stu-id="09ebc-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09ebc-118">关系</span><span class="sxs-lookup"><span data-stu-id="09ebc-118">Relationships</span></span>
<span data-ttu-id="09ebc-119">无</span><span class="sxs-lookup"><span data-stu-id="09ebc-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09ebc-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09ebc-120">JSON Representation</span></span>
<span data-ttu-id="09ebc-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09ebc-121">Here is a JSON representation of the resource.</span></span>
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





