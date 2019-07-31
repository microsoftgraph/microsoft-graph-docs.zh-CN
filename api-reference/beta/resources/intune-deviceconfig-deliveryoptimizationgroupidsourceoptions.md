---
title: deliveryOptimizationGroupIdSourceOptions 资源类型
description: 组 id 选项类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fc2c900828526ac4d2788c2b91e669bae04f452f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970743"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="364f9-103">deliveryOptimizationGroupIdSourceOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="364f9-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

> <span data-ttu-id="364f9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="364f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="364f9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="364f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="364f9-106">组 id 选项类型</span><span class="sxs-lookup"><span data-stu-id="364f9-106">Group id options type</span></span>


<span data-ttu-id="364f9-107">继承自[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="364f9-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="364f9-108">属性</span><span class="sxs-lookup"><span data-stu-id="364f9-108">Properties</span></span>
|<span data-ttu-id="364f9-109">属性</span><span class="sxs-lookup"><span data-stu-id="364f9-109">Property</span></span>|<span data-ttu-id="364f9-110">类型</span><span class="sxs-lookup"><span data-stu-id="364f9-110">Type</span></span>|<span data-ttu-id="364f9-111">说明</span><span class="sxs-lookup"><span data-stu-id="364f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="364f9-112">groupIdSourceOption</span><span class="sxs-lookup"><span data-stu-id="364f9-112">groupIdSourceOption</span></span>|[<span data-ttu-id="364f9-113">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="364f9-113">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="364f9-114">将此策略设置为限制对特定源的对等方选择。</span><span class="sxs-lookup"><span data-stu-id="364f9-114">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="364f9-115">可取值为：`notConfigured`、`adSite`、`authenticatedDomainSid`、`dhcpUserOption`、`dnsSuffix`。</span><span class="sxs-lookup"><span data-stu-id="364f9-115">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="364f9-116">关系</span><span class="sxs-lookup"><span data-stu-id="364f9-116">Relationships</span></span>
<span data-ttu-id="364f9-117">无</span><span class="sxs-lookup"><span data-stu-id="364f9-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="364f9-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="364f9-118">JSON Representation</span></span>
<span data-ttu-id="364f9-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="364f9-119">Here is a JSON representation of the resource.</span></span>
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





