---
title: deliveryOptimizationGroupIdCustom 资源类型
description: 自定义组 id 类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e439b9d4777a0b0c513d750d0b5e35783dbd9a1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947251"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="ff516-103">deliveryOptimizationGroupIdCustom 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff516-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="ff516-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff516-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff516-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff516-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff516-106">自定义组 id 类型</span><span class="sxs-lookup"><span data-stu-id="ff516-106">Custom group id type</span></span>


<span data-ttu-id="ff516-107">继承自[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="ff516-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff516-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff516-108">Properties</span></span>
|<span data-ttu-id="ff516-109">属性</span><span class="sxs-lookup"><span data-stu-id="ff516-109">Property</span></span>|<span data-ttu-id="ff516-110">类型</span><span class="sxs-lookup"><span data-stu-id="ff516-110">Type</span></span>|<span data-ttu-id="ff516-111">说明</span><span class="sxs-lookup"><span data-stu-id="ff516-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff516-112">groupIdCustom</span><span class="sxs-lookup"><span data-stu-id="ff516-112">groupIdCustom</span></span>|<span data-ttu-id="ff516-113">String</span><span class="sxs-lookup"><span data-stu-id="ff516-113">String</span></span>|<span data-ttu-id="ff516-114">指定设备所属的任意组 ID</span><span class="sxs-lookup"><span data-stu-id="ff516-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff516-115">关系</span><span class="sxs-lookup"><span data-stu-id="ff516-115">Relationships</span></span>
<span data-ttu-id="ff516-116">无</span><span class="sxs-lookup"><span data-stu-id="ff516-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff516-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff516-117">JSON Representation</span></span>
<span data-ttu-id="ff516-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff516-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdCustom",
  "groupIdCustom": "String"
}
```




