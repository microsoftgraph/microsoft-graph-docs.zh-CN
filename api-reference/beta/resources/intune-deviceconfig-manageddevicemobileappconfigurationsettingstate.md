---
title: managedDeviceMobileAppConfigurationSettingState 资源类型
description: 给定设备的托管设备移动应用配置设置状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d828b57e6ae76e3a0babcc2b27a009e60f7a6407
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636071"
---
# <a name="manageddevicemobileappconfigurationsettingstate-resource-type"></a><span data-ttu-id="256fc-103">managedDeviceMobileAppConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="256fc-103">managedDeviceMobileAppConfigurationSettingState resource type</span></span>

> <span data-ttu-id="256fc-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="256fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="256fc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="256fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="256fc-106">给定设备的托管设备移动应用配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="256fc-106">Managed Device Mobile App Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="256fc-107">属性</span><span class="sxs-lookup"><span data-stu-id="256fc-107">Properties</span></span>
|<span data-ttu-id="256fc-108">属性</span><span class="sxs-lookup"><span data-stu-id="256fc-108">Property</span></span>|<span data-ttu-id="256fc-109">类型</span><span class="sxs-lookup"><span data-stu-id="256fc-109">Type</span></span>|<span data-ttu-id="256fc-110">Description</span><span class="sxs-lookup"><span data-stu-id="256fc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="256fc-111">setting</span><span class="sxs-lookup"><span data-stu-id="256fc-111">setting</span></span>|<span data-ttu-id="256fc-112">字符串</span><span class="sxs-lookup"><span data-stu-id="256fc-112">String</span></span>|<span data-ttu-id="256fc-113">报告的设置</span><span class="sxs-lookup"><span data-stu-id="256fc-113">The setting that is being reported</span></span>|
|<span data-ttu-id="256fc-114">settingName</span><span class="sxs-lookup"><span data-stu-id="256fc-114">settingName</span></span>|<span data-ttu-id="256fc-115">字符串</span><span class="sxs-lookup"><span data-stu-id="256fc-115">String</span></span>|<span data-ttu-id="256fc-116">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="256fc-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="256fc-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="256fc-117">instanceDisplayName</span></span>|<span data-ttu-id="256fc-118">字符串</span><span class="sxs-lookup"><span data-stu-id="256fc-118">String</span></span>|<span data-ttu-id="256fc-119">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="256fc-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="256fc-120">state</span><span class="sxs-lookup"><span data-stu-id="256fc-120">state</span></span>|[<span data-ttu-id="256fc-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="256fc-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="256fc-122">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="256fc-122">The compliance state of the setting.</span></span> <span data-ttu-id="256fc-123">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="256fc-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="256fc-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="256fc-124">errorCode</span></span>|<span data-ttu-id="256fc-125">Int64</span><span class="sxs-lookup"><span data-stu-id="256fc-125">Int64</span></span>|<span data-ttu-id="256fc-126">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="256fc-126">Error code for the setting</span></span>|
|<span data-ttu-id="256fc-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="256fc-127">errorDescription</span></span>|<span data-ttu-id="256fc-128">字符串</span><span class="sxs-lookup"><span data-stu-id="256fc-128">String</span></span>|<span data-ttu-id="256fc-129">错误说明</span><span class="sxs-lookup"><span data-stu-id="256fc-129">Error description</span></span>|
|<span data-ttu-id="256fc-130">userId</span><span class="sxs-lookup"><span data-stu-id="256fc-130">userId</span></span>|<span data-ttu-id="256fc-131">String</span><span class="sxs-lookup"><span data-stu-id="256fc-131">String</span></span>|<span data-ttu-id="256fc-132">UserId</span><span class="sxs-lookup"><span data-stu-id="256fc-132">UserId</span></span>|
|<span data-ttu-id="256fc-133">userName</span><span class="sxs-lookup"><span data-stu-id="256fc-133">userName</span></span>|<span data-ttu-id="256fc-134">字符串</span><span class="sxs-lookup"><span data-stu-id="256fc-134">String</span></span>|<span data-ttu-id="256fc-135">UserName</span><span class="sxs-lookup"><span data-stu-id="256fc-135">UserName</span></span>|
|<span data-ttu-id="256fc-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="256fc-136">userEmail</span></span>|<span data-ttu-id="256fc-137">字符串</span><span class="sxs-lookup"><span data-stu-id="256fc-137">String</span></span>|<span data-ttu-id="256fc-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="256fc-138">UserEmail</span></span>|
|<span data-ttu-id="256fc-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="256fc-139">userPrincipalName</span></span>|<span data-ttu-id="256fc-140">字符串</span><span class="sxs-lookup"><span data-stu-id="256fc-140">String</span></span>|<span data-ttu-id="256fc-141">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="256fc-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="256fc-142">源</span><span class="sxs-lookup"><span data-stu-id="256fc-142">sources</span></span>|<span data-ttu-id="256fc-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="256fc-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="256fc-144">参与策略</span><span class="sxs-lookup"><span data-stu-id="256fc-144">Contributing policies</span></span>|
|<span data-ttu-id="256fc-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="256fc-145">currentValue</span></span>|<span data-ttu-id="256fc-146">String</span><span class="sxs-lookup"><span data-stu-id="256fc-146">String</span></span>|<span data-ttu-id="256fc-147">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="256fc-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="256fc-148">关系</span><span class="sxs-lookup"><span data-stu-id="256fc-148">Relationships</span></span>
<span data-ttu-id="256fc-149">无</span><span class="sxs-lookup"><span data-stu-id="256fc-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="256fc-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="256fc-150">JSON Representation</span></span>
<span data-ttu-id="256fc-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="256fc-151">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```



