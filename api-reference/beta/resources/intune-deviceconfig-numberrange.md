---
title: numberRange 资源类型
description: 号码范围定义。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27393bdac6519078c2021e3484ae58ddf43216d9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416858"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="fde19-103">numberRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="fde19-103">numberRange resource type</span></span>

> <span data-ttu-id="fde19-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="fde19-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fde19-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fde19-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fde19-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fde19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fde19-107">号码范围定义。</span><span class="sxs-lookup"><span data-stu-id="fde19-107">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="fde19-108">属性</span><span class="sxs-lookup"><span data-stu-id="fde19-108">Properties</span></span>
|<span data-ttu-id="fde19-109">属性</span><span class="sxs-lookup"><span data-stu-id="fde19-109">Property</span></span>|<span data-ttu-id="fde19-110">类型</span><span class="sxs-lookup"><span data-stu-id="fde19-110">Type</span></span>|<span data-ttu-id="fde19-111">说明</span><span class="sxs-lookup"><span data-stu-id="fde19-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fde19-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="fde19-112">lowerNumber</span></span>|<span data-ttu-id="fde19-113">Int32</span><span class="sxs-lookup"><span data-stu-id="fde19-113">Int32</span></span>|<span data-ttu-id="fde19-114">较小的数字。</span><span class="sxs-lookup"><span data-stu-id="fde19-114">Lower number.</span></span>|
|<span data-ttu-id="fde19-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="fde19-115">upperNumber</span></span>|<span data-ttu-id="fde19-116">Int32</span><span class="sxs-lookup"><span data-stu-id="fde19-116">Int32</span></span>|<span data-ttu-id="fde19-117">上限数字。</span><span class="sxs-lookup"><span data-stu-id="fde19-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fde19-118">关系</span><span class="sxs-lookup"><span data-stu-id="fde19-118">Relationships</span></span>
<span data-ttu-id="fde19-119">无</span><span class="sxs-lookup"><span data-stu-id="fde19-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fde19-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fde19-120">JSON Representation</span></span>
<span data-ttu-id="fde19-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fde19-121">Here is a JSON representation of the resource.</span></span>
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




