---
title: deliveryOptimizationGroupIdSourceOptions 资源类型
description: 组 id 选项类型
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0cd541fd9ff3a91f40be1b6ccea67787cdad2567
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565805"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="8e65b-103">deliveryOptimizationGroupIdSourceOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e65b-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

> <span data-ttu-id="8e65b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8e65b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e65b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e65b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e65b-106">组 id 选项类型</span><span class="sxs-lookup"><span data-stu-id="8e65b-106">Group id options type</span></span>


<span data-ttu-id="8e65b-107">继承自[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="8e65b-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8e65b-108">属性</span><span class="sxs-lookup"><span data-stu-id="8e65b-108">Properties</span></span>
|<span data-ttu-id="8e65b-109">属性</span><span class="sxs-lookup"><span data-stu-id="8e65b-109">Property</span></span>|<span data-ttu-id="8e65b-110">类型</span><span class="sxs-lookup"><span data-stu-id="8e65b-110">Type</span></span>|<span data-ttu-id="8e65b-111">说明</span><span class="sxs-lookup"><span data-stu-id="8e65b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e65b-112">groupIdSourceOption</span><span class="sxs-lookup"><span data-stu-id="8e65b-112">groupIdSourceOption</span></span>|[<span data-ttu-id="8e65b-113">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="8e65b-113">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="8e65b-114">将此策略设置为限制对特定源的对等方选择。</span><span class="sxs-lookup"><span data-stu-id="8e65b-114">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="8e65b-115">可取值为：`notConfigured`、`adSite`、`authenticatedDomainSid`、`dhcpUserOption` 或 `dnsSuffix`。</span><span class="sxs-lookup"><span data-stu-id="8e65b-115">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e65b-116">关系</span><span class="sxs-lookup"><span data-stu-id="8e65b-116">Relationships</span></span>
<span data-ttu-id="8e65b-117">无</span><span class="sxs-lookup"><span data-stu-id="8e65b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e65b-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e65b-118">JSON Representation</span></span>
<span data-ttu-id="8e65b-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e65b-119">Here is a JSON representation of the resource.</span></span>
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





