---
title: deviceManagementSettings 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4f676eed1acbf6711f526e612bd6c073b749607d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417663"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="eb050-103">deviceManagementSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb050-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="eb050-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="eb050-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eb050-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eb050-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb050-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb050-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb050-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="eb050-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="eb050-108">属性</span><span class="sxs-lookup"><span data-stu-id="eb050-108">Properties</span></span>
|<span data-ttu-id="eb050-109">属性</span><span class="sxs-lookup"><span data-stu-id="eb050-109">Property</span></span>|<span data-ttu-id="eb050-110">类型</span><span class="sxs-lookup"><span data-stu-id="eb050-110">Type</span></span>|<span data-ttu-id="eb050-111">说明</span><span class="sxs-lookup"><span data-stu-id="eb050-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb050-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="eb050-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="eb050-113">Int32</span><span class="sxs-lookup"><span data-stu-id="eb050-113">Int32</span></span>|<span data-ttu-id="eb050-114">允许设备无需签入即可保持符合性的天数。</span><span class="sxs-lookup"><span data-stu-id="eb050-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="eb050-115">有效值为 0 至 120</span><span class="sxs-lookup"><span data-stu-id="eb050-115">Valid values 0 to 120</span></span>|
|<span data-ttu-id="eb050-116">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="eb050-116">isScheduledActionEnabled</span></span>|<span data-ttu-id="eb050-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb050-117">Boolean</span></span>|<span data-ttu-id="eb050-118">是否为规则的计划操作启用此功能。</span><span class="sxs-lookup"><span data-stu-id="eb050-118">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="eb050-119">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="eb050-119">secureByDefault</span></span>|<span data-ttu-id="eb050-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb050-120">Boolean</span></span>|<span data-ttu-id="eb050-121">它为 true 时，如果不存在目标符合性策略，则设备应为不符合。</span><span class="sxs-lookup"><span data-stu-id="eb050-121">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="eb050-122">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="eb050-122">enhancedJailBreak</span></span>|<span data-ttu-id="eb050-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb050-123">Boolean</span></span>|<span data-ttu-id="eb050-124">功能启用或非增强 jailbreak 检测。</span><span class="sxs-lookup"><span data-stu-id="eb050-124">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="eb050-125">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="eb050-125">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="eb050-126">Int32</span><span class="sxs-lookup"><span data-stu-id="eb050-126">Int32</span></span>|<span data-ttu-id="eb050-127">当设备不检查指定天数，公司数据可能会删除，设备将不会在管理下。</span><span class="sxs-lookup"><span data-stu-id="eb050-127">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="eb050-128">有效值 30 到 270</span><span class="sxs-lookup"><span data-stu-id="eb050-128">Valid values 30 to 270</span></span>|
|<span data-ttu-id="eb050-129">derivedCredentialProvider</span><span class="sxs-lookup"><span data-stu-id="eb050-129">derivedCredentialProvider</span></span>|[<span data-ttu-id="eb050-130">derivedCredentialProviderType</span><span class="sxs-lookup"><span data-stu-id="eb050-130">derivedCredentialProviderType</span></span>](../resources/intune-deviceconfig-derivedcredentialprovidertype.md)|<span data-ttu-id="eb050-131">派生凭据提供程序以使用此帐户。</span><span class="sxs-lookup"><span data-stu-id="eb050-131">The Derived Credential Provider to use for this account.</span></span> <span data-ttu-id="eb050-132">可取值为：`notConfigured`、`entrustDataCard`、`purebred`、`xTec`、`intercede`。</span><span class="sxs-lookup"><span data-stu-id="eb050-132">Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.</span></span>|
|<span data-ttu-id="eb050-133">derivedCredentialUrl</span><span class="sxs-lookup"><span data-stu-id="eb050-133">derivedCredentialUrl</span></span>|<span data-ttu-id="eb050-134">String</span><span class="sxs-lookup"><span data-stu-id="eb050-134">String</span></span>|<span data-ttu-id="eb050-135">派生凭据提供程序自助服务 URI。</span><span class="sxs-lookup"><span data-stu-id="eb050-135">The Derived Credential Provider self-service URI.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb050-136">关系</span><span class="sxs-lookup"><span data-stu-id="eb050-136">Relationships</span></span>
<span data-ttu-id="eb050-137">无</span><span class="sxs-lookup"><span data-stu-id="eb050-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb050-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb050-138">JSON Representation</span></span>
<span data-ttu-id="eb050-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb050-139">Here is a JSON representation of the resource.</span></span>
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




