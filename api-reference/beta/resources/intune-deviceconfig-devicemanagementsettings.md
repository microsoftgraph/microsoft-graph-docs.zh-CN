---
title: deviceManagementSettings 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ea20bce4019ff04c81170b895fd5d5445db027cd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707820"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="7c6d1-103">deviceManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c6d1-103">deviceManagementSettings resource type</span></span>

<span data-ttu-id="7c6d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c6d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c6d1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7c6d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c6d1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7c6d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c6d1-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7c6d1-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7c6d1-108">属性</span><span class="sxs-lookup"><span data-stu-id="7c6d1-108">Properties</span></span>
|<span data-ttu-id="7c6d1-109">属性</span><span class="sxs-lookup"><span data-stu-id="7c6d1-109">Property</span></span>|<span data-ttu-id="7c6d1-110">类型</span><span class="sxs-lookup"><span data-stu-id="7c6d1-110">Type</span></span>|<span data-ttu-id="7c6d1-111">说明</span><span class="sxs-lookup"><span data-stu-id="7c6d1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c6d1-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="7c6d1-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="7c6d1-113">Int32</span><span class="sxs-lookup"><span data-stu-id="7c6d1-113">Int32</span></span>|<span data-ttu-id="7c6d1-114">允许设备无需签入即可保持符合性的天数。</span><span class="sxs-lookup"><span data-stu-id="7c6d1-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span>|
|<span data-ttu-id="7c6d1-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="7c6d1-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="7c6d1-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c6d1-116">Boolean</span></span>|<span data-ttu-id="7c6d1-117">是否为规则的计划操作启用此功能。</span><span class="sxs-lookup"><span data-stu-id="7c6d1-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="7c6d1-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="7c6d1-118">secureByDefault</span></span>|<span data-ttu-id="7c6d1-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c6d1-119">Boolean</span></span>|<span data-ttu-id="7c6d1-120">它为 true 时，如果不存在目标符合性策略，则设备应为不符合。</span><span class="sxs-lookup"><span data-stu-id="7c6d1-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="7c6d1-121">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="7c6d1-121">enhancedJailBreak</span></span>|<span data-ttu-id="7c6d1-122">布尔</span><span class="sxs-lookup"><span data-stu-id="7c6d1-122">Boolean</span></span>|<span data-ttu-id="7c6d1-123">功能是否已启用或不适用于增强的 jailbreak 检测。</span><span class="sxs-lookup"><span data-stu-id="7c6d1-123">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="7c6d1-124">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="7c6d1-124">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="7c6d1-125">Int32</span><span class="sxs-lookup"><span data-stu-id="7c6d1-125">Int32</span></span>|<span data-ttu-id="7c6d1-126">如果设备在指定天数内未签入，则可能会删除公司数据，并且设备将不受管理。</span><span class="sxs-lookup"><span data-stu-id="7c6d1-126">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="7c6d1-127">有效值为30至270</span><span class="sxs-lookup"><span data-stu-id="7c6d1-127">Valid values 30 to 270</span></span>|
|<span data-ttu-id="7c6d1-128">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="7c6d1-128">derivedCredentialProvider</span></span>|[<span data-ttu-id="7c6d1-129">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="7c6d1-129">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="7c6d1-130">要用于此帐户的派生的凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="7c6d1-130">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="7c6d1-131">可取值为：`notConfigured`、`entrustDataCard`、`purebred`、`xTec`、`intercede`。</span><span class="sxs-lookup"><span data-stu-id="7c6d1-131">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="7c6d1-132">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="7c6d1-132">derivedCredentialUrl</span></span>|<span data-ttu-id="7c6d1-133">String</span><span class="sxs-lookup"><span data-stu-id="7c6d1-133">String</span></span>|<span data-ttu-id="7c6d1-134">派生的凭据提供程序自助服务 URI。</span><span class="sxs-lookup"><span data-stu-id="7c6d1-134">The Derived Credential Provider self-service URI.</span></span>|
|<span data-ttu-id="7c6d1-135">androidDeviceAdministratorEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="7c6d1-135">androidDeviceAdministratorEnrollmentEnabled</span></span>|<span data-ttu-id="7c6d1-136">布尔</span><span class="sxs-lookup"><span data-stu-id="7c6d1-136">Boolean</span></span>|<span data-ttu-id="7c6d1-137">用于确定是否为此帐户启用了 Android 设备管理员注册的属性。</span><span class="sxs-lookup"><span data-stu-id="7c6d1-137">The property to determine if Android device administrator enrollment is enabled for this account.</span></span>|
|<span data-ttu-id="7c6d1-138">ignoreDevicesForUnsupportedSettingsEnabled</span><span class="sxs-lookup"><span data-stu-id="7c6d1-138">ignoreDevicesForUnsupportedSettingsEnabled</span></span>|<span data-ttu-id="7c6d1-139">布尔</span><span class="sxs-lookup"><span data-stu-id="7c6d1-139">Boolean</span></span>|<span data-ttu-id="7c6d1-140">用于确定是否忽略某些型号的设备上不受支持的合规性设置的属性。</span><span class="sxs-lookup"><span data-stu-id="7c6d1-140">The property to determine whether to ignore unsupported compliance settings on certian models of devices.</span></span>|
|<span data-ttu-id="7c6d1-141">enableLogCollection</span><span class="sxs-lookup"><span data-stu-id="7c6d1-141">enableLogCollection</span></span>|<span data-ttu-id="7c6d1-142">布尔</span><span class="sxs-lookup"><span data-stu-id="7c6d1-142">Boolean</span></span>|<span data-ttu-id="7c6d1-143">确定是否应可使用 "日志收集" 功能。</span><span class="sxs-lookup"><span data-stu-id="7c6d1-143">Determines whether the log collection feature should be available for use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c6d1-144">关系</span><span class="sxs-lookup"><span data-stu-id="7c6d1-144">Relationships</span></span>
<span data-ttu-id="7c6d1-145">无</span><span class="sxs-lookup"><span data-stu-id="7c6d1-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c6d1-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c6d1-146">JSON Representation</span></span>
<span data-ttu-id="7c6d1-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c6d1-147">Here is a JSON representation of the resource.</span></span>
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
  "derivedCredentialUrl": "String",
  "androidDeviceAdministratorEnrollmentEnabled": true,
  "ignoreDevicesForUnsupportedSettingsEnabled": true,
  "enableLogCollection": true
}
```





