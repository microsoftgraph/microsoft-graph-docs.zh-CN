---
title: deviceManagementSettings 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 079d957d14e5f891af691ba7b41916adb8ac9669
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946964"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="e76f9-103">deviceManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="e76f9-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="e76f9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e76f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e76f9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e76f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e76f9-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e76f9-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e76f9-107">属性</span><span class="sxs-lookup"><span data-stu-id="e76f9-107">Properties</span></span>
|<span data-ttu-id="e76f9-108">属性</span><span class="sxs-lookup"><span data-stu-id="e76f9-108">Property</span></span>|<span data-ttu-id="e76f9-109">类型</span><span class="sxs-lookup"><span data-stu-id="e76f9-109">Type</span></span>|<span data-ttu-id="e76f9-110">说明</span><span class="sxs-lookup"><span data-stu-id="e76f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e76f9-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="e76f9-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="e76f9-112">Int32</span><span class="sxs-lookup"><span data-stu-id="e76f9-112">Int32</span></span>|<span data-ttu-id="e76f9-113">允许设备无需签入即可保持符合性的天数。</span><span class="sxs-lookup"><span data-stu-id="e76f9-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="e76f9-114">有效值为 0 至 120</span><span class="sxs-lookup"><span data-stu-id="e76f9-114">Valid values 0 to 120</span></span>|
|<span data-ttu-id="e76f9-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="e76f9-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="e76f9-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="e76f9-116">Boolean</span></span>|<span data-ttu-id="e76f9-117">是否为规则的计划操作启用此功能。</span><span class="sxs-lookup"><span data-stu-id="e76f9-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="e76f9-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="e76f9-118">secureByDefault</span></span>|<span data-ttu-id="e76f9-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="e76f9-119">Boolean</span></span>|<span data-ttu-id="e76f9-120">它为 true 时，如果不存在目标符合性策略，则设备应为不符合。</span><span class="sxs-lookup"><span data-stu-id="e76f9-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="e76f9-121">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="e76f9-121">enhancedJailBreak</span></span>|<span data-ttu-id="e76f9-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="e76f9-122">Boolean</span></span>|<span data-ttu-id="e76f9-123">功能是否已启用或不适用于增强的 jailbreak 检测。</span><span class="sxs-lookup"><span data-stu-id="e76f9-123">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="e76f9-124">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="e76f9-124">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="e76f9-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e76f9-125">Int32</span></span>|<span data-ttu-id="e76f9-126">如果设备在指定天数内未签入, 则可能会删除公司数据, 并且设备将不受管理。</span><span class="sxs-lookup"><span data-stu-id="e76f9-126">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="e76f9-127">有效值为30至270</span><span class="sxs-lookup"><span data-stu-id="e76f9-127">Valid values 30 to 270</span></span>|
|<span data-ttu-id="e76f9-128">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="e76f9-128">derivedCredentialProvider</span></span>|[<span data-ttu-id="e76f9-129">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="e76f9-129">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="e76f9-130">要用于此帐户的派生的凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="e76f9-130">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="e76f9-131">可取值为：`notConfigured`、`entrustDataCard`、`purebred`、`xTec`、`intercede`。</span><span class="sxs-lookup"><span data-stu-id="e76f9-131">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="e76f9-132">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="e76f9-132">derivedCredentialUrl</span></span>|<span data-ttu-id="e76f9-133">String</span><span class="sxs-lookup"><span data-stu-id="e76f9-133">String</span></span>|<span data-ttu-id="e76f9-134">派生的凭据提供程序自助服务 URI。</span><span class="sxs-lookup"><span data-stu-id="e76f9-134">The Derived Credential Provider self-service URI.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e76f9-135">关系</span><span class="sxs-lookup"><span data-stu-id="e76f9-135">Relationships</span></span>
<span data-ttu-id="e76f9-136">无</span><span class="sxs-lookup"><span data-stu-id="e76f9-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e76f9-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e76f9-137">JSON Representation</span></span>
<span data-ttu-id="e76f9-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e76f9-138">Here is a JSON representation of the resource.</span></span>
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
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024,
  "derivedCredentialProvider": "String",
  "derivedCredentialUrl": "String"
}
```




