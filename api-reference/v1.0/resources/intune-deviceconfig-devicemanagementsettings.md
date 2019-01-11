---
title: deviceManagementSettings 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3742262f2d17cdac1344379b39b4891b5b9919ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830588"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="3a46b-103">deviceManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a46b-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="3a46b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3a46b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a46b-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3a46b-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3a46b-106">属性</span><span class="sxs-lookup"><span data-stu-id="3a46b-106">Properties</span></span>
|<span data-ttu-id="3a46b-107">属性</span><span class="sxs-lookup"><span data-stu-id="3a46b-107">Property</span></span>|<span data-ttu-id="3a46b-108">类型</span><span class="sxs-lookup"><span data-stu-id="3a46b-108">Type</span></span>|<span data-ttu-id="3a46b-109">说明</span><span class="sxs-lookup"><span data-stu-id="3a46b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a46b-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="3a46b-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="3a46b-111">Int32</span><span class="sxs-lookup"><span data-stu-id="3a46b-111">Int32</span></span>|<span data-ttu-id="3a46b-112">允许设备无需签入即可保持符合性的天数。</span><span class="sxs-lookup"><span data-stu-id="3a46b-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="3a46b-113">有效值为 0 至 120</span><span class="sxs-lookup"><span data-stu-id="3a46b-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="3a46b-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="3a46b-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="3a46b-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a46b-115">Boolean</span></span>|<span data-ttu-id="3a46b-116">是否为规则的计划操作启用此功能。</span><span class="sxs-lookup"><span data-stu-id="3a46b-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="3a46b-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="3a46b-117">secureByDefault</span></span>|<span data-ttu-id="3a46b-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a46b-118">Boolean</span></span>|<span data-ttu-id="3a46b-119">它为 true 时，如果不存在目标符合性策略，则设备应为不符合。</span><span class="sxs-lookup"><span data-stu-id="3a46b-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a46b-120">关系</span><span class="sxs-lookup"><span data-stu-id="3a46b-120">Relationships</span></span>
<span data-ttu-id="3a46b-121">无</span><span class="sxs-lookup"><span data-stu-id="3a46b-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3a46b-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a46b-122">JSON Representation</span></span>
<span data-ttu-id="3a46b-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a46b-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true
}
```



