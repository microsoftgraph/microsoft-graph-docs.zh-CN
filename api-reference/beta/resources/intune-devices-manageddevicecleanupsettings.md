---
title: managedDeviceCleanupSettings 资源类型
description: 定义规则，当管理员想要清除的设备。
author: tfitzmac
ms.openlocfilehash: 84650c4d2d182fe0da30ced56786a2c0216a6358
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304086"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="d5a90-103">managedDeviceCleanupSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5a90-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="d5a90-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d5a90-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5a90-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d5a90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5a90-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d5a90-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5a90-107">定义规则，当管理员想要清除的设备。</span><span class="sxs-lookup"><span data-stu-id="d5a90-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>
## <a name="properties"></a><span data-ttu-id="d5a90-108">属性</span><span class="sxs-lookup"><span data-stu-id="d5a90-108">Properties</span></span>
|<span data-ttu-id="d5a90-109">属性</span><span class="sxs-lookup"><span data-stu-id="d5a90-109">Property</span></span>|<span data-ttu-id="d5a90-110">类型</span><span class="sxs-lookup"><span data-stu-id="d5a90-110">Type</span></span>|<span data-ttu-id="d5a90-111">说明</span><span class="sxs-lookup"><span data-stu-id="d5a90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5a90-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="d5a90-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="d5a90-113">字符串</span><span class="sxs-lookup"><span data-stu-id="d5a90-113">String</span></span>|<span data-ttu-id="d5a90-114">当设备尚未连接 Intune 天数。</span><span class="sxs-lookup"><span data-stu-id="d5a90-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5a90-115">Relationships</span><span class="sxs-lookup"><span data-stu-id="d5a90-115">Relationships</span></span>
<span data-ttu-id="d5a90-116">无</span><span class="sxs-lookup"><span data-stu-id="d5a90-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d5a90-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5a90-117">JSON Representation</span></span>
<span data-ttu-id="d5a90-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5a90-118">Here is a JSON representation of the resource.</span></span>
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





