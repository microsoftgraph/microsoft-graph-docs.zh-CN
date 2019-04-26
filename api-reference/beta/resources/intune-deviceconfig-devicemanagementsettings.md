---
title: deviceManagementSettings 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eba8ec934a29b78d7e6ca11f288a1bd787338d2b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567191"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="4cf77-103">deviceManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="4cf77-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="4cf77-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4cf77-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cf77-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4cf77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cf77-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4cf77-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="4cf77-107">属性</span><span class="sxs-lookup"><span data-stu-id="4cf77-107">Properties</span></span>
|<span data-ttu-id="4cf77-108">属性</span><span class="sxs-lookup"><span data-stu-id="4cf77-108">Property</span></span>|<span data-ttu-id="4cf77-109">类型</span><span class="sxs-lookup"><span data-stu-id="4cf77-109">Type</span></span>|<span data-ttu-id="4cf77-110">说明</span><span class="sxs-lookup"><span data-stu-id="4cf77-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cf77-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="4cf77-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="4cf77-112">Int32</span><span class="sxs-lookup"><span data-stu-id="4cf77-112">Int32</span></span>|<span data-ttu-id="4cf77-113">允许设备无需签入即可保持符合性的天数。</span><span class="sxs-lookup"><span data-stu-id="4cf77-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="4cf77-114">有效值为 0 至 120</span><span class="sxs-lookup"><span data-stu-id="4cf77-114">Valid values 0 to 120</span></span>|
|<span data-ttu-id="4cf77-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="4cf77-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="4cf77-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cf77-116">Boolean</span></span>|<span data-ttu-id="4cf77-117">是否为规则的计划操作启用此功能。</span><span class="sxs-lookup"><span data-stu-id="4cf77-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="4cf77-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="4cf77-118">secureByDefault</span></span>|<span data-ttu-id="4cf77-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cf77-119">Boolean</span></span>|<span data-ttu-id="4cf77-120">它为 true 时，如果不存在目标符合性策略，则设备应为不符合。</span><span class="sxs-lookup"><span data-stu-id="4cf77-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="4cf77-121">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="4cf77-121">enhancedJailBreak</span></span>|<span data-ttu-id="4cf77-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cf77-122">Boolean</span></span>|<span data-ttu-id="4cf77-123">功能是否已启用或不适用于增强的 jailbreak 检测。</span><span class="sxs-lookup"><span data-stu-id="4cf77-123">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="4cf77-124">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="4cf77-124">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="4cf77-125">Int32</span><span class="sxs-lookup"><span data-stu-id="4cf77-125">Int32</span></span>|<span data-ttu-id="4cf77-126">如果设备在指定天数内未签入, 则可能会删除公司数据, 并且设备将不受管理。</span><span class="sxs-lookup"><span data-stu-id="4cf77-126">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="4cf77-127">有效值为30至270</span><span class="sxs-lookup"><span data-stu-id="4cf77-127">Valid values 30 to 270</span></span>|
|<span data-ttu-id="4cf77-128">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="4cf77-128">derivedCredentialProvider</span></span>|[<span data-ttu-id="4cf77-129">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="4cf77-129">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="4cf77-130">要用于此帐户的派生的凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="4cf77-130">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="4cf77-131">可取值为：`notConfigured`、`entrustDataCard`、`purebred`、`xTec` 或 `intercede`。</span><span class="sxs-lookup"><span data-stu-id="4cf77-131">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="4cf77-132">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="4cf77-132">derivedCredentialUrl</span></span>|<span data-ttu-id="4cf77-133">String</span><span class="sxs-lookup"><span data-stu-id="4cf77-133">String</span></span>|<span data-ttu-id="4cf77-134">派生的凭据提供程序自助服务 URI。</span><span class="sxs-lookup"><span data-stu-id="4cf77-134">The Derived Credential Provider self-service URI.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cf77-135">关系</span><span class="sxs-lookup"><span data-stu-id="4cf77-135">Relationships</span></span>
<span data-ttu-id="4cf77-136">无</span><span class="sxs-lookup"><span data-stu-id="4cf77-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cf77-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4cf77-137">JSON Representation</span></span>
<span data-ttu-id="4cf77-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4cf77-138">Here is a JSON representation of the resource.</span></span>
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





