---
title: managedDeviceCleanupSettings 资源类型
description: 定义当管理员想要清理设备时的规则。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e1facb174f0047bdef90eb745195448f0451eb3b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995096"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="eb0ef-103">managedDeviceCleanupSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb0ef-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="eb0ef-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eb0ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb0ef-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb0ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb0ef-106">定义当管理员想要清理设备时的规则。</span><span class="sxs-lookup"><span data-stu-id="eb0ef-106">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="eb0ef-107">属性</span><span class="sxs-lookup"><span data-stu-id="eb0ef-107">Properties</span></span>
|<span data-ttu-id="eb0ef-108">属性</span><span class="sxs-lookup"><span data-stu-id="eb0ef-108">Property</span></span>|<span data-ttu-id="eb0ef-109">类型</span><span class="sxs-lookup"><span data-stu-id="eb0ef-109">Type</span></span>|<span data-ttu-id="eb0ef-110">说明</span><span class="sxs-lookup"><span data-stu-id="eb0ef-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb0ef-111">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="eb0ef-111">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="eb0ef-112">String</span><span class="sxs-lookup"><span data-stu-id="eb0ef-112">String</span></span>|<span data-ttu-id="eb0ef-113">设备未联系 Intune 的天数。</span><span class="sxs-lookup"><span data-stu-id="eb0ef-113">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb0ef-114">关系</span><span class="sxs-lookup"><span data-stu-id="eb0ef-114">Relationships</span></span>
<span data-ttu-id="eb0ef-115">无</span><span class="sxs-lookup"><span data-stu-id="eb0ef-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb0ef-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb0ef-116">JSON Representation</span></span>
<span data-ttu-id="eb0ef-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb0ef-117">Here is a JSON representation of the resource.</span></span>
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





