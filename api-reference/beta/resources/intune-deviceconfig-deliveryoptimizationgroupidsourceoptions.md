---
title: deliveryOptimizationGroupIdSourceOptions 资源类型
description: 组 id 选项类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dc946b3756b4008e4b61dafb02277357752c2fbd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333308"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="1e8b2-103">deliveryOptimizationGroupIdSourceOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e8b2-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

> <span data-ttu-id="1e8b2-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1e8b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e8b2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e8b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e8b2-106">组 id 选项类型</span><span class="sxs-lookup"><span data-stu-id="1e8b2-106">Group id options type</span></span>


<span data-ttu-id="1e8b2-107">继承自[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="1e8b2-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1e8b2-108">属性</span><span class="sxs-lookup"><span data-stu-id="1e8b2-108">Properties</span></span>
|<span data-ttu-id="1e8b2-109">属性</span><span class="sxs-lookup"><span data-stu-id="1e8b2-109">Property</span></span>|<span data-ttu-id="1e8b2-110">类型</span><span class="sxs-lookup"><span data-stu-id="1e8b2-110">Type</span></span>|<span data-ttu-id="1e8b2-111">说明</span><span class="sxs-lookup"><span data-stu-id="1e8b2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e8b2-112">groupIdSourceOption</span><span class="sxs-lookup"><span data-stu-id="1e8b2-112">groupIdSourceOption</span></span>|[<span data-ttu-id="1e8b2-113">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="1e8b2-113">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="1e8b2-114">将此策略设置为限制对特定源的对等方选择。</span><span class="sxs-lookup"><span data-stu-id="1e8b2-114">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="1e8b2-115">可取值为：`notConfigured`、`adSite`、`authenticatedDomainSid`、`dhcpUserOption`、`dnsSuffix`。</span><span class="sxs-lookup"><span data-stu-id="1e8b2-115">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e8b2-116">关系</span><span class="sxs-lookup"><span data-stu-id="1e8b2-116">Relationships</span></span>
<span data-ttu-id="1e8b2-117">无</span><span class="sxs-lookup"><span data-stu-id="1e8b2-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e8b2-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e8b2-118">JSON Representation</span></span>
<span data-ttu-id="1e8b2-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e8b2-119">Here is a JSON representation of the resource.</span></span>
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



