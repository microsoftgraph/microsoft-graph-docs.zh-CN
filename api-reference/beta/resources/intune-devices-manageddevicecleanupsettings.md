---
title: managedDeviceCleanupSettings 资源类型
description: 定义当管理员想要清理设备时的规则。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 558c8f14f431bb10421ee77b6569f69560e8023f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968363"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="35007-103">managedDeviceCleanupSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="35007-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="35007-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35007-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35007-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35007-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35007-106">定义当管理员想要清理设备时的规则。</span><span class="sxs-lookup"><span data-stu-id="35007-106">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="35007-107">属性</span><span class="sxs-lookup"><span data-stu-id="35007-107">Properties</span></span>
|<span data-ttu-id="35007-108">属性</span><span class="sxs-lookup"><span data-stu-id="35007-108">Property</span></span>|<span data-ttu-id="35007-109">类型</span><span class="sxs-lookup"><span data-stu-id="35007-109">Type</span></span>|<span data-ttu-id="35007-110">说明</span><span class="sxs-lookup"><span data-stu-id="35007-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35007-111">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="35007-111">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="35007-112">String</span><span class="sxs-lookup"><span data-stu-id="35007-112">String</span></span>|<span data-ttu-id="35007-113">设备未联系 Intune 的天数。</span><span class="sxs-lookup"><span data-stu-id="35007-113">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35007-114">关系</span><span class="sxs-lookup"><span data-stu-id="35007-114">Relationships</span></span>
<span data-ttu-id="35007-115">无</span><span class="sxs-lookup"><span data-stu-id="35007-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35007-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35007-116">JSON Representation</span></span>
<span data-ttu-id="35007-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35007-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceCleanupSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCleanupSettings",
  "deviceInactivityBeforeRetirementInDays": "String"
}
```





