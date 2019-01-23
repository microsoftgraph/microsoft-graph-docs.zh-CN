---
title: managedDeviceCleanupSettings 资源类型
description: 定义规则，当管理员想要清除的设备。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4bf756072dcc3cd13bda2fda59b8688b63f3cd43
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424565"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="817e8-103">managedDeviceCleanupSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="817e8-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="817e8-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="817e8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="817e8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="817e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="817e8-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="817e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="817e8-107">定义规则，当管理员想要清除的设备。</span><span class="sxs-lookup"><span data-stu-id="817e8-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="817e8-108">属性</span><span class="sxs-lookup"><span data-stu-id="817e8-108">Properties</span></span>
|<span data-ttu-id="817e8-109">属性</span><span class="sxs-lookup"><span data-stu-id="817e8-109">Property</span></span>|<span data-ttu-id="817e8-110">类型</span><span class="sxs-lookup"><span data-stu-id="817e8-110">Type</span></span>|<span data-ttu-id="817e8-111">说明</span><span class="sxs-lookup"><span data-stu-id="817e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="817e8-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="817e8-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="817e8-113">String</span><span class="sxs-lookup"><span data-stu-id="817e8-113">String</span></span>|<span data-ttu-id="817e8-114">当设备尚未连接 Intune 天数。</span><span class="sxs-lookup"><span data-stu-id="817e8-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="817e8-115">关系</span><span class="sxs-lookup"><span data-stu-id="817e8-115">Relationships</span></span>
<span data-ttu-id="817e8-116">无</span><span class="sxs-lookup"><span data-stu-id="817e8-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="817e8-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="817e8-117">JSON Representation</span></span>
<span data-ttu-id="817e8-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="817e8-118">Here is a JSON representation of the resource.</span></span>
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




