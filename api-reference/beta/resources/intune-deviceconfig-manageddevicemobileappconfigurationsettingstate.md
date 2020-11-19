---
title: managedDeviceMobileAppConfigurationSettingState 资源类型
description: 给定设备的托管设备移动应用配置设置状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d9e74a4fb9b6739d5051e37af4c15c48ede6bda1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302836"
---
# <a name="manageddevicemobileappconfigurationsettingstate-resource-type"></a><span data-ttu-id="5e082-103">managedDeviceMobileAppConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e082-103">managedDeviceMobileAppConfigurationSettingState resource type</span></span>

<span data-ttu-id="5e082-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e082-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e082-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5e082-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e082-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e082-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e082-107">给定设备的托管设备移动应用配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="5e082-107">Managed Device Mobile App Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="5e082-108">属性</span><span class="sxs-lookup"><span data-stu-id="5e082-108">Properties</span></span>
|<span data-ttu-id="5e082-109">属性</span><span class="sxs-lookup"><span data-stu-id="5e082-109">Property</span></span>|<span data-ttu-id="5e082-110">类型</span><span class="sxs-lookup"><span data-stu-id="5e082-110">Type</span></span>|<span data-ttu-id="5e082-111">Description</span><span class="sxs-lookup"><span data-stu-id="5e082-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e082-112">setting</span><span class="sxs-lookup"><span data-stu-id="5e082-112">setting</span></span>|<span data-ttu-id="5e082-113">String</span><span class="sxs-lookup"><span data-stu-id="5e082-113">String</span></span>|<span data-ttu-id="5e082-114">报告的设置</span><span class="sxs-lookup"><span data-stu-id="5e082-114">The setting that is being reported</span></span>|
|<span data-ttu-id="5e082-115">settingName</span><span class="sxs-lookup"><span data-stu-id="5e082-115">settingName</span></span>|<span data-ttu-id="5e082-116">String</span><span class="sxs-lookup"><span data-stu-id="5e082-116">String</span></span>|<span data-ttu-id="5e082-117">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="5e082-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="5e082-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="5e082-118">instanceDisplayName</span></span>|<span data-ttu-id="5e082-119">String</span><span class="sxs-lookup"><span data-stu-id="5e082-119">String</span></span>|<span data-ttu-id="5e082-120">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="5e082-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="5e082-121">state</span><span class="sxs-lookup"><span data-stu-id="5e082-121">state</span></span>|[<span data-ttu-id="5e082-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="5e082-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5e082-123">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="5e082-123">The compliance state of the setting.</span></span> <span data-ttu-id="5e082-124">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="5e082-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5e082-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="5e082-125">errorCode</span></span>|<span data-ttu-id="5e082-126">Int64</span><span class="sxs-lookup"><span data-stu-id="5e082-126">Int64</span></span>|<span data-ttu-id="5e082-127">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="5e082-127">Error code for the setting</span></span>|
|<span data-ttu-id="5e082-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="5e082-128">errorDescription</span></span>|<span data-ttu-id="5e082-129">String</span><span class="sxs-lookup"><span data-stu-id="5e082-129">String</span></span>|<span data-ttu-id="5e082-130">错误说明</span><span class="sxs-lookup"><span data-stu-id="5e082-130">Error description</span></span>|
|<span data-ttu-id="5e082-131">userId</span><span class="sxs-lookup"><span data-stu-id="5e082-131">userId</span></span>|<span data-ttu-id="5e082-132">字符串</span><span class="sxs-lookup"><span data-stu-id="5e082-132">String</span></span>|<span data-ttu-id="5e082-133">UserId</span><span class="sxs-lookup"><span data-stu-id="5e082-133">UserId</span></span>|
|<span data-ttu-id="5e082-134">userName</span><span class="sxs-lookup"><span data-stu-id="5e082-134">userName</span></span>|<span data-ttu-id="5e082-135">String</span><span class="sxs-lookup"><span data-stu-id="5e082-135">String</span></span>|<span data-ttu-id="5e082-136">UserName</span><span class="sxs-lookup"><span data-stu-id="5e082-136">UserName</span></span>|
|<span data-ttu-id="5e082-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="5e082-137">userEmail</span></span>|<span data-ttu-id="5e082-138">String</span><span class="sxs-lookup"><span data-stu-id="5e082-138">String</span></span>|<span data-ttu-id="5e082-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="5e082-139">UserEmail</span></span>|
|<span data-ttu-id="5e082-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5e082-140">userPrincipalName</span></span>|<span data-ttu-id="5e082-141">字符串</span><span class="sxs-lookup"><span data-stu-id="5e082-141">String</span></span>|<span data-ttu-id="5e082-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="5e082-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="5e082-143">源</span><span class="sxs-lookup"><span data-stu-id="5e082-143">sources</span></span>|<span data-ttu-id="5e082-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5e082-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="5e082-145">参与策略</span><span class="sxs-lookup"><span data-stu-id="5e082-145">Contributing policies</span></span>|
|<span data-ttu-id="5e082-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="5e082-146">currentValue</span></span>|<span data-ttu-id="5e082-147">String</span><span class="sxs-lookup"><span data-stu-id="5e082-147">String</span></span>|<span data-ttu-id="5e082-148">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="5e082-148">Current value of setting on device</span></span>|
|<span data-ttu-id="5e082-149">settingInstanceId</span><span class="sxs-lookup"><span data-stu-id="5e082-149">settingInstanceId</span></span>|<span data-ttu-id="5e082-150">字符串</span><span class="sxs-lookup"><span data-stu-id="5e082-150">String</span></span>|<span data-ttu-id="5e082-151">SettingInstanceId</span><span class="sxs-lookup"><span data-stu-id="5e082-151">SettingInstanceId</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e082-152">关系</span><span class="sxs-lookup"><span data-stu-id="5e082-152">Relationships</span></span>
<span data-ttu-id="5e082-153">无</span><span class="sxs-lookup"><span data-stu-id="5e082-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e082-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e082-154">JSON Representation</span></span>
<span data-ttu-id="5e082-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e082-155">Here is a JSON representation of the resource.</span></span>
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




