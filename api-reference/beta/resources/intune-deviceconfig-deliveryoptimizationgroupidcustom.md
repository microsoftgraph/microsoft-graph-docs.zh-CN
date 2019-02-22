---
title: deliveryOptimizationGroupIdCustom 资源类型
description: 自定义组 id 类型
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec3b00920d0ead3df5fe694e110825615f449ef4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177971"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="1dcc4-103">deliveryOptimizationGroupIdCustom 资源类型</span><span class="sxs-lookup"><span data-stu-id="1dcc4-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="1dcc4-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1dcc4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dcc4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1dcc4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dcc4-106">自定义组 id 类型</span><span class="sxs-lookup"><span data-stu-id="1dcc4-106">Custom group id type</span></span>


<span data-ttu-id="1dcc4-107">继承自[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="1dcc4-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1dcc4-108">属性</span><span class="sxs-lookup"><span data-stu-id="1dcc4-108">Properties</span></span>
|<span data-ttu-id="1dcc4-109">属性</span><span class="sxs-lookup"><span data-stu-id="1dcc4-109">Property</span></span>|<span data-ttu-id="1dcc4-110">类型</span><span class="sxs-lookup"><span data-stu-id="1dcc4-110">Type</span></span>|<span data-ttu-id="1dcc4-111">说明</span><span class="sxs-lookup"><span data-stu-id="1dcc4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dcc4-112">groupIdCustom</span><span class="sxs-lookup"><span data-stu-id="1dcc4-112">groupIdCustom</span></span>|<span data-ttu-id="1dcc4-113">字符串</span><span class="sxs-lookup"><span data-stu-id="1dcc4-113">String</span></span>|<span data-ttu-id="1dcc4-114">指定设备所属的任意组 ID</span><span class="sxs-lookup"><span data-stu-id="1dcc4-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="1dcc4-115">关系</span><span class="sxs-lookup"><span data-stu-id="1dcc4-115">Relationships</span></span>
<span data-ttu-id="1dcc4-116">无</span><span class="sxs-lookup"><span data-stu-id="1dcc4-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1dcc4-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1dcc4-117">JSON Representation</span></span>
<span data-ttu-id="1dcc4-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1dcc4-118">Here is a JSON representation of the resource.</span></span>
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




