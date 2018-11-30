---
title: deviceManagementSettings 资源类型
description: 尚未记录
ms.openlocfilehash: 4a07c879e20139c9138fc7315172655aa48a40eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008970"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="97ae8-103">deviceManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="97ae8-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="97ae8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="97ae8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97ae8-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="97ae8-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="97ae8-106">属性</span><span class="sxs-lookup"><span data-stu-id="97ae8-106">Properties</span></span>
|<span data-ttu-id="97ae8-107">属性</span><span class="sxs-lookup"><span data-stu-id="97ae8-107">Property</span></span>|<span data-ttu-id="97ae8-108">类型</span><span class="sxs-lookup"><span data-stu-id="97ae8-108">Type</span></span>|<span data-ttu-id="97ae8-109">说明</span><span class="sxs-lookup"><span data-stu-id="97ae8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97ae8-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="97ae8-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="97ae8-111">Int32</span><span class="sxs-lookup"><span data-stu-id="97ae8-111">Int32</span></span>|<span data-ttu-id="97ae8-112">允许设备无需签入即可保持符合性的天数。</span><span class="sxs-lookup"><span data-stu-id="97ae8-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="97ae8-113">有效值为 0 至 120</span><span class="sxs-lookup"><span data-stu-id="97ae8-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="97ae8-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="97ae8-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="97ae8-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="97ae8-115">Boolean</span></span>|<span data-ttu-id="97ae8-116">是否为规则的计划操作启用此功能。</span><span class="sxs-lookup"><span data-stu-id="97ae8-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="97ae8-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="97ae8-117">secureByDefault</span></span>|<span data-ttu-id="97ae8-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="97ae8-118">Boolean</span></span>|<span data-ttu-id="97ae8-119">它为 true 时，如果不存在目标符合性策略，则设备应为不符合。</span><span class="sxs-lookup"><span data-stu-id="97ae8-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="97ae8-120">关系</span><span class="sxs-lookup"><span data-stu-id="97ae8-120">Relationships</span></span>
<span data-ttu-id="97ae8-121">无</span><span class="sxs-lookup"><span data-stu-id="97ae8-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="97ae8-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97ae8-122">JSON Representation</span></span>
<span data-ttu-id="97ae8-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97ae8-123">Here is a JSON representation of the resource.</span></span>
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



