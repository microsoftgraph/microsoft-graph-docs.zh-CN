---
title: managedDeviceMobileAppConfigurationSettingState 资源类型
description: 给定设备的托管设备移动应用配置设置状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e760b026f775abcec54f2cd34922de56f202ab2e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48710032"
---
# <a name="manageddevicemobileappconfigurationsettingstate-resource-type"></a><span data-ttu-id="008af-103">managedDeviceMobileAppConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="008af-103">managedDeviceMobileAppConfigurationSettingState resource type</span></span>

<span data-ttu-id="008af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="008af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="008af-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="008af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="008af-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="008af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="008af-107">给定设备的托管设备移动应用配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="008af-107">Managed Device Mobile App Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="008af-108">属性</span><span class="sxs-lookup"><span data-stu-id="008af-108">Properties</span></span>
|<span data-ttu-id="008af-109">属性</span><span class="sxs-lookup"><span data-stu-id="008af-109">Property</span></span>|<span data-ttu-id="008af-110">类型</span><span class="sxs-lookup"><span data-stu-id="008af-110">Type</span></span>|<span data-ttu-id="008af-111">说明</span><span class="sxs-lookup"><span data-stu-id="008af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="008af-112">setting</span><span class="sxs-lookup"><span data-stu-id="008af-112">setting</span></span>|<span data-ttu-id="008af-113">String</span><span class="sxs-lookup"><span data-stu-id="008af-113">String</span></span>|<span data-ttu-id="008af-114">报告的设置</span><span class="sxs-lookup"><span data-stu-id="008af-114">The setting that is being reported</span></span>|
|<span data-ttu-id="008af-115">settingName</span><span class="sxs-lookup"><span data-stu-id="008af-115">settingName</span></span>|<span data-ttu-id="008af-116">String</span><span class="sxs-lookup"><span data-stu-id="008af-116">String</span></span>|<span data-ttu-id="008af-117">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="008af-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="008af-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="008af-118">instanceDisplayName</span></span>|<span data-ttu-id="008af-119">String</span><span class="sxs-lookup"><span data-stu-id="008af-119">String</span></span>|<span data-ttu-id="008af-120">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="008af-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="008af-121">state</span><span class="sxs-lookup"><span data-stu-id="008af-121">state</span></span>|[<span data-ttu-id="008af-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="008af-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="008af-123">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="008af-123">The compliance state of the setting.</span></span> <span data-ttu-id="008af-124">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="008af-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="008af-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="008af-125">errorCode</span></span>|<span data-ttu-id="008af-126">Int64</span><span class="sxs-lookup"><span data-stu-id="008af-126">Int64</span></span>|<span data-ttu-id="008af-127">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="008af-127">Error code for the setting</span></span>|
|<span data-ttu-id="008af-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="008af-128">errorDescription</span></span>|<span data-ttu-id="008af-129">String</span><span class="sxs-lookup"><span data-stu-id="008af-129">String</span></span>|<span data-ttu-id="008af-130">错误说明</span><span class="sxs-lookup"><span data-stu-id="008af-130">Error description</span></span>|
|<span data-ttu-id="008af-131">userId</span><span class="sxs-lookup"><span data-stu-id="008af-131">userId</span></span>|<span data-ttu-id="008af-132">String</span><span class="sxs-lookup"><span data-stu-id="008af-132">String</span></span>|<span data-ttu-id="008af-133">UserId</span><span class="sxs-lookup"><span data-stu-id="008af-133">UserId</span></span>|
|<span data-ttu-id="008af-134">userName</span><span class="sxs-lookup"><span data-stu-id="008af-134">userName</span></span>|<span data-ttu-id="008af-135">String</span><span class="sxs-lookup"><span data-stu-id="008af-135">String</span></span>|<span data-ttu-id="008af-136">UserName</span><span class="sxs-lookup"><span data-stu-id="008af-136">UserName</span></span>|
|<span data-ttu-id="008af-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="008af-137">userEmail</span></span>|<span data-ttu-id="008af-138">String</span><span class="sxs-lookup"><span data-stu-id="008af-138">String</span></span>|<span data-ttu-id="008af-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="008af-139">UserEmail</span></span>|
|<span data-ttu-id="008af-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="008af-140">userPrincipalName</span></span>|<span data-ttu-id="008af-141">String</span><span class="sxs-lookup"><span data-stu-id="008af-141">String</span></span>|<span data-ttu-id="008af-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="008af-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="008af-143">源</span><span class="sxs-lookup"><span data-stu-id="008af-143">sources</span></span>|<span data-ttu-id="008af-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="008af-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="008af-145">参与策略</span><span class="sxs-lookup"><span data-stu-id="008af-145">Contributing policies</span></span>|
|<span data-ttu-id="008af-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="008af-146">currentValue</span></span>|<span data-ttu-id="008af-147">String</span><span class="sxs-lookup"><span data-stu-id="008af-147">String</span></span>|<span data-ttu-id="008af-148">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="008af-148">Current value of setting on device</span></span>|
|<span data-ttu-id="008af-149">settingInstanceId</span><span class="sxs-lookup"><span data-stu-id="008af-149">settingInstanceId</span></span>|<span data-ttu-id="008af-150">String</span><span class="sxs-lookup"><span data-stu-id="008af-150">String</span></span>|<span data-ttu-id="008af-151">SettingInstanceId</span><span class="sxs-lookup"><span data-stu-id="008af-151">SettingInstanceId</span></span>|

## <a name="relationships"></a><span data-ttu-id="008af-152">关系</span><span class="sxs-lookup"><span data-stu-id="008af-152">Relationships</span></span>
<span data-ttu-id="008af-153">无</span><span class="sxs-lookup"><span data-stu-id="008af-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="008af-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="008af-154">JSON Representation</span></span>
<span data-ttu-id="008af-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="008af-155">Here is a JSON representation of the resource.</span></span>
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
      "displayName": "String",
      "sourceType": "String"
    }
  ],
  "currentValue": "String",
  "settingInstanceId": "String"
}
```





