---
title: numberRange 资源类型
description: 号码范围定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 772ffc59bc9ac4848b6b34eee8c62f8006468784
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958716"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="fead8-103">numberRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="fead8-103">numberRange resource type</span></span>

> <span data-ttu-id="fead8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fead8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fead8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fead8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fead8-106">号码范围定义。</span><span class="sxs-lookup"><span data-stu-id="fead8-106">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="fead8-107">属性</span><span class="sxs-lookup"><span data-stu-id="fead8-107">Properties</span></span>
|<span data-ttu-id="fead8-108">属性</span><span class="sxs-lookup"><span data-stu-id="fead8-108">Property</span></span>|<span data-ttu-id="fead8-109">类型</span><span class="sxs-lookup"><span data-stu-id="fead8-109">Type</span></span>|<span data-ttu-id="fead8-110">说明</span><span class="sxs-lookup"><span data-stu-id="fead8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fead8-111">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="fead8-111">lowerNumber</span></span>|<span data-ttu-id="fead8-112">Int32</span><span class="sxs-lookup"><span data-stu-id="fead8-112">Int32</span></span>|<span data-ttu-id="fead8-113">较小的数字。</span><span class="sxs-lookup"><span data-stu-id="fead8-113">Lower number.</span></span>|
|<span data-ttu-id="fead8-114">upperNumber</span><span class="sxs-lookup"><span data-stu-id="fead8-114">upperNumber</span></span>|<span data-ttu-id="fead8-115">Int32</span><span class="sxs-lookup"><span data-stu-id="fead8-115">Int32</span></span>|<span data-ttu-id="fead8-116">上限数。</span><span class="sxs-lookup"><span data-stu-id="fead8-116">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fead8-117">关系</span><span class="sxs-lookup"><span data-stu-id="fead8-117">Relationships</span></span>
<span data-ttu-id="fead8-118">无</span><span class="sxs-lookup"><span data-stu-id="fead8-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fead8-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fead8-119">JSON Representation</span></span>
<span data-ttu-id="fead8-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fead8-120">Here is a JSON representation of the resource.</span></span>
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





