---
title: managedDeviceCleanupSettings 资源类型
description: 定义规则，当管理员想要清除的设备。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 334b561ffa19d4161553f761ce65b7da7d9dbcfa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961895"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="6913d-103">managedDeviceCleanupSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="6913d-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="6913d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6913d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6913d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6913d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6913d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6913d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6913d-107">定义规则，当管理员想要清除的设备。</span><span class="sxs-lookup"><span data-stu-id="6913d-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>
## <a name="properties"></a><span data-ttu-id="6913d-108">属性</span><span class="sxs-lookup"><span data-stu-id="6913d-108">Properties</span></span>
|<span data-ttu-id="6913d-109">属性</span><span class="sxs-lookup"><span data-stu-id="6913d-109">Property</span></span>|<span data-ttu-id="6913d-110">类型</span><span class="sxs-lookup"><span data-stu-id="6913d-110">Type</span></span>|<span data-ttu-id="6913d-111">Description</span><span class="sxs-lookup"><span data-stu-id="6913d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6913d-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="6913d-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="6913d-113">字符串</span><span class="sxs-lookup"><span data-stu-id="6913d-113">String</span></span>|<span data-ttu-id="6913d-114">当设备尚未连接 Intune 天数。</span><span class="sxs-lookup"><span data-stu-id="6913d-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6913d-115">Relationships</span><span class="sxs-lookup"><span data-stu-id="6913d-115">Relationships</span></span>
<span data-ttu-id="6913d-116">无</span><span class="sxs-lookup"><span data-stu-id="6913d-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6913d-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6913d-117">JSON Representation</span></span>
<span data-ttu-id="6913d-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6913d-118">Here is a JSON representation of the resource.</span></span>
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





