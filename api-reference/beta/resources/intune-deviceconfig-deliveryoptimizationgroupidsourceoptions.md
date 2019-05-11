---
title: deliveryOptimizationGroupIdSourceOptions 资源类型
description: 组 id 选项类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8931c2e2a8a6dc3848b4ec73236443f9707aacea
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947223"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="ca663-103">deliveryOptimizationGroupIdSourceOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca663-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

> <span data-ttu-id="ca663-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ca663-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca663-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ca663-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca663-106">组 id 选项类型</span><span class="sxs-lookup"><span data-stu-id="ca663-106">Group id options type</span></span>


<span data-ttu-id="ca663-107">继承自[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="ca663-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ca663-108">属性</span><span class="sxs-lookup"><span data-stu-id="ca663-108">Properties</span></span>
|<span data-ttu-id="ca663-109">属性</span><span class="sxs-lookup"><span data-stu-id="ca663-109">Property</span></span>|<span data-ttu-id="ca663-110">类型</span><span class="sxs-lookup"><span data-stu-id="ca663-110">Type</span></span>|<span data-ttu-id="ca663-111">说明</span><span class="sxs-lookup"><span data-stu-id="ca663-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca663-112">groupIdSourceOption</span><span class="sxs-lookup"><span data-stu-id="ca663-112">groupIdSourceOption</span></span>|[<span data-ttu-id="ca663-113">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="ca663-113">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="ca663-114">将此策略设置为限制对特定源的对等方选择。</span><span class="sxs-lookup"><span data-stu-id="ca663-114">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="ca663-115">可取值为：`notConfigured`、`adSite`、`authenticatedDomainSid`、`dhcpUserOption`、`dnsSuffix`。</span><span class="sxs-lookup"><span data-stu-id="ca663-115">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca663-116">关系</span><span class="sxs-lookup"><span data-stu-id="ca663-116">Relationships</span></span>
<span data-ttu-id="ca663-117">无</span><span class="sxs-lookup"><span data-stu-id="ca663-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca663-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca663-118">JSON Representation</span></span>
<span data-ttu-id="ca663-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca663-119">Here is a JSON representation of the resource.</span></span>
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




