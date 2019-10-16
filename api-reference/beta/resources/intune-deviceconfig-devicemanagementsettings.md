---
title: deviceManagementSettings 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fdc01e2c9cd4aabf47c900bd38bb2b0f7035308b
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538964"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="68daa-103">deviceManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="68daa-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="68daa-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="68daa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68daa-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="68daa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68daa-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="68daa-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="68daa-107">属性</span><span class="sxs-lookup"><span data-stu-id="68daa-107">Properties</span></span>
|<span data-ttu-id="68daa-108">属性</span><span class="sxs-lookup"><span data-stu-id="68daa-108">Property</span></span>|<span data-ttu-id="68daa-109">类型</span><span class="sxs-lookup"><span data-stu-id="68daa-109">Type</span></span>|<span data-ttu-id="68daa-110">说明</span><span class="sxs-lookup"><span data-stu-id="68daa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68daa-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="68daa-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="68daa-112">Int32</span><span class="sxs-lookup"><span data-stu-id="68daa-112">Int32</span></span>|<span data-ttu-id="68daa-113">允许设备无需签入即可保持符合性的天数。</span><span class="sxs-lookup"><span data-stu-id="68daa-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span>|
|<span data-ttu-id="68daa-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="68daa-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="68daa-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="68daa-115">Boolean</span></span>|<span data-ttu-id="68daa-116">是否为规则的计划操作启用此功能。</span><span class="sxs-lookup"><span data-stu-id="68daa-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="68daa-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="68daa-117">secureByDefault</span></span>|<span data-ttu-id="68daa-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="68daa-118">Boolean</span></span>|<span data-ttu-id="68daa-119">它为 true 时，如果不存在目标符合性策略，则设备应为不符合。</span><span class="sxs-lookup"><span data-stu-id="68daa-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="68daa-120">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="68daa-120">enhancedJailBreak</span></span>|<span data-ttu-id="68daa-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="68daa-121">Boolean</span></span>|<span data-ttu-id="68daa-122">功能是否已启用或不适用于增强的 jailbreak 检测。</span><span class="sxs-lookup"><span data-stu-id="68daa-122">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="68daa-123">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="68daa-123">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="68daa-124">Int32</span><span class="sxs-lookup"><span data-stu-id="68daa-124">Int32</span></span>|<span data-ttu-id="68daa-125">如果设备在指定天数内未签入，则可能会删除公司数据，并且设备将不受管理。</span><span class="sxs-lookup"><span data-stu-id="68daa-125">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="68daa-126">有效值为30至270</span><span class="sxs-lookup"><span data-stu-id="68daa-126">Valid values 30 to 270</span></span>|
|<span data-ttu-id="68daa-127">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="68daa-127">derivedCredentialProvider</span></span>|[<span data-ttu-id="68daa-128">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="68daa-128">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="68daa-129">要用于此帐户的派生的凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="68daa-129">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="68daa-130">可取值为：`notConfigured`、`entrustDataCard`、`purebred`、`xTec`、`intercede`。</span><span class="sxs-lookup"><span data-stu-id="68daa-130">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="68daa-131">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="68daa-131">derivedCredentialUrl</span></span>|<span data-ttu-id="68daa-132">字符串</span><span class="sxs-lookup"><span data-stu-id="68daa-132">String</span></span>|<span data-ttu-id="68daa-133">派生的凭据提供程序自助服务 URI。</span><span class="sxs-lookup"><span data-stu-id="68daa-133">The Derived Credential Provider self-service URI.</span></span>|
|<span data-ttu-id="68daa-134">androidDeviceAdministratorEnrollmentEnabled</span><span class="sxs-lookup"><span data-stu-id="68daa-134">androidDeviceAdministratorEnrollmentEnabled</span></span>|<span data-ttu-id="68daa-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="68daa-135">Boolean</span></span>|<span data-ttu-id="68daa-136">用于确定是否为此帐户启用了 Android 设备管理员注册的属性。</span><span class="sxs-lookup"><span data-stu-id="68daa-136">The property to determine if Android device administrator enrollment is enabled for this account.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68daa-137">关系</span><span class="sxs-lookup"><span data-stu-id="68daa-137">Relationships</span></span>
<span data-ttu-id="68daa-138">无</span><span class="sxs-lookup"><span data-stu-id="68daa-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68daa-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68daa-139">JSON Representation</span></span>
<span data-ttu-id="68daa-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68daa-140">Here is a JSON representation of the resource.</span></span>
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
  "androidDeviceAdministratorEnrollmentEnabled": true
}
```



