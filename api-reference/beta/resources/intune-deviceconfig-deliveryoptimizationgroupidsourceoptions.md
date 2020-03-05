---
title: deliveryOptimizationGroupIdSourceOptions 资源类型
description: 组 id 选项类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 741b39245c26858d4cae46923d1078f568cf6945
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526767"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="4e820-103">deliveryOptimizationGroupIdSourceOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e820-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

<span data-ttu-id="4e820-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4e820-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e820-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4e820-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e820-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e820-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e820-107">组 id 选项类型</span><span class="sxs-lookup"><span data-stu-id="4e820-107">Group id options type</span></span>


<span data-ttu-id="4e820-108">继承自[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="4e820-108">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4e820-109">属性</span><span class="sxs-lookup"><span data-stu-id="4e820-109">Properties</span></span>
|<span data-ttu-id="4e820-110">属性</span><span class="sxs-lookup"><span data-stu-id="4e820-110">Property</span></span>|<span data-ttu-id="4e820-111">类型</span><span class="sxs-lookup"><span data-stu-id="4e820-111">Type</span></span>|<span data-ttu-id="4e820-112">说明</span><span class="sxs-lookup"><span data-stu-id="4e820-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e820-113">groupIdSourceOption</span><span class="sxs-lookup"><span data-stu-id="4e820-113">groupIdSourceOption</span></span>|[<span data-ttu-id="4e820-114">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="4e820-114">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="4e820-115">将此策略设置为限制对特定源的对等方选择。</span><span class="sxs-lookup"><span data-stu-id="4e820-115">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="4e820-116">可取值为：`notConfigured`、`adSite`、`authenticatedDomainSid`、`dhcpUserOption`、`dnsSuffix`。</span><span class="sxs-lookup"><span data-stu-id="4e820-116">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e820-117">关系</span><span class="sxs-lookup"><span data-stu-id="4e820-117">Relationships</span></span>
<span data-ttu-id="4e820-118">无</span><span class="sxs-lookup"><span data-stu-id="4e820-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e820-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e820-119">JSON Representation</span></span>
<span data-ttu-id="4e820-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e820-120">Here is a JSON representation of the resource.</span></span>
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



