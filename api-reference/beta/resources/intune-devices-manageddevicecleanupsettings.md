---
title: managedDeviceCleanupSettings 资源类型
description: 定义当管理员想要清理设备时的规则。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67e911cb5e1b31e3be2cc20378ebe77ff305204a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725482"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="832cb-103">managedDeviceCleanupSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="832cb-103">managedDeviceCleanupSettings resource type</span></span>

<span data-ttu-id="832cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="832cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="832cb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="832cb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="832cb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="832cb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="832cb-107">定义当管理员想要清理设备时的规则。</span><span class="sxs-lookup"><span data-stu-id="832cb-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>

## <a name="properties"></a><span data-ttu-id="832cb-108">属性</span><span class="sxs-lookup"><span data-stu-id="832cb-108">Properties</span></span>
|<span data-ttu-id="832cb-109">属性</span><span class="sxs-lookup"><span data-stu-id="832cb-109">Property</span></span>|<span data-ttu-id="832cb-110">类型</span><span class="sxs-lookup"><span data-stu-id="832cb-110">Type</span></span>|<span data-ttu-id="832cb-111">说明</span><span class="sxs-lookup"><span data-stu-id="832cb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="832cb-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="832cb-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="832cb-113">String</span><span class="sxs-lookup"><span data-stu-id="832cb-113">String</span></span>|<span data-ttu-id="832cb-114">设备未联系 Intune 的天数。</span><span class="sxs-lookup"><span data-stu-id="832cb-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="832cb-115">关系</span><span class="sxs-lookup"><span data-stu-id="832cb-115">Relationships</span></span>
<span data-ttu-id="832cb-116">无</span><span class="sxs-lookup"><span data-stu-id="832cb-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="832cb-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="832cb-117">JSON Representation</span></span>
<span data-ttu-id="832cb-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="832cb-118">Here is a JSON representation of the resource.</span></span>
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





