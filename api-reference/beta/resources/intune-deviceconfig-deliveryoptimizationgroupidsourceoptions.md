---
title: deliveryOptimizationGroupIdSourceOptions 资源类型
description: 组 id 选项类型
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d54a98bef3b9c0e0517b426332b8d3223e904c8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177852"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="56333-103">deliveryOptimizationGroupIdSourceOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="56333-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

> <span data-ttu-id="56333-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="56333-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56333-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56333-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56333-106">组 id 选项类型</span><span class="sxs-lookup"><span data-stu-id="56333-106">Group id options type</span></span>


<span data-ttu-id="56333-107">继承自[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="56333-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="56333-108">属性</span><span class="sxs-lookup"><span data-stu-id="56333-108">Properties</span></span>
|<span data-ttu-id="56333-109">属性</span><span class="sxs-lookup"><span data-stu-id="56333-109">Property</span></span>|<span data-ttu-id="56333-110">类型</span><span class="sxs-lookup"><span data-stu-id="56333-110">Type</span></span>|<span data-ttu-id="56333-111">说明</span><span class="sxs-lookup"><span data-stu-id="56333-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56333-112">groupIdSourceOption</span><span class="sxs-lookup"><span data-stu-id="56333-112">groupIdSourceOption</span></span>|[<span data-ttu-id="56333-113">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="56333-113">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="56333-114">将此策略设置为限制对特定源的对等方选择。</span><span class="sxs-lookup"><span data-stu-id="56333-114">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="56333-115">可取值为：`notConfigured`、`adSite`、`authenticatedDomainSid`、`dhcpUserOption`、`dnsSuffix`。</span><span class="sxs-lookup"><span data-stu-id="56333-115">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56333-116">关系</span><span class="sxs-lookup"><span data-stu-id="56333-116">Relationships</span></span>
<span data-ttu-id="56333-117">无</span><span class="sxs-lookup"><span data-stu-id="56333-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56333-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56333-118">JSON Representation</span></span>
<span data-ttu-id="56333-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56333-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSourceOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdSourceOptions",
  "groupIdSourceOption": "String"
}
```




