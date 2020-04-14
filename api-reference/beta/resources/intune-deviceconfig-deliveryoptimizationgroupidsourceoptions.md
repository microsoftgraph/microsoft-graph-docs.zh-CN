---
title: deliveryOptimizationGroupIdSourceOptions 资源类型
description: 组 id 选项类型
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1f490286de16c8ef8256e464d674d09631d7a459
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456986"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="19d05-103">deliveryOptimizationGroupIdSourceOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="19d05-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

<span data-ttu-id="19d05-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19d05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="19d05-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="19d05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19d05-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19d05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19d05-107">组 id 选项类型</span><span class="sxs-lookup"><span data-stu-id="19d05-107">Group id options type</span></span>


<span data-ttu-id="19d05-108">继承自[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="19d05-108">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="19d05-109">属性</span><span class="sxs-lookup"><span data-stu-id="19d05-109">Properties</span></span>
|<span data-ttu-id="19d05-110">属性</span><span class="sxs-lookup"><span data-stu-id="19d05-110">Property</span></span>|<span data-ttu-id="19d05-111">类型</span><span class="sxs-lookup"><span data-stu-id="19d05-111">Type</span></span>|<span data-ttu-id="19d05-112">说明</span><span class="sxs-lookup"><span data-stu-id="19d05-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19d05-113">groupIdSourceOption</span><span class="sxs-lookup"><span data-stu-id="19d05-113">groupIdSourceOption</span></span>|[<span data-ttu-id="19d05-114">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="19d05-114">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="19d05-115">将此策略设置为限制对特定源的对等方选择。</span><span class="sxs-lookup"><span data-stu-id="19d05-115">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="19d05-116">可取值为：`notConfigured`、`adSite`、`authenticatedDomainSid`、`dhcpUserOption`、`dnsSuffix`。</span><span class="sxs-lookup"><span data-stu-id="19d05-116">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19d05-117">关系</span><span class="sxs-lookup"><span data-stu-id="19d05-117">Relationships</span></span>
<span data-ttu-id="19d05-118">无</span><span class="sxs-lookup"><span data-stu-id="19d05-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19d05-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19d05-119">JSON Representation</span></span>
<span data-ttu-id="19d05-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19d05-120">Here is a JSON representation of the resource.</span></span>
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



