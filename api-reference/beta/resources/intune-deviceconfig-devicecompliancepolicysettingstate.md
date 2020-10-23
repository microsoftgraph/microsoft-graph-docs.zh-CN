---
title: deviceCompliancePolicySettingState 资源类型
description: 给定设备的设备符合性策略设置状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 555e42ca8c4a2ca419b34be32afc0f8d031d9570
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724612"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="73117-103">deviceCompliancePolicySettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="73117-103">deviceCompliancePolicySettingState resource type</span></span>

<span data-ttu-id="73117-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73117-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73117-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="73117-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73117-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="73117-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73117-107">给定设备的设备符合性策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="73117-107">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="73117-108">属性</span><span class="sxs-lookup"><span data-stu-id="73117-108">Properties</span></span>
|<span data-ttu-id="73117-109">属性</span><span class="sxs-lookup"><span data-stu-id="73117-109">Property</span></span>|<span data-ttu-id="73117-110">类型</span><span class="sxs-lookup"><span data-stu-id="73117-110">Type</span></span>|<span data-ttu-id="73117-111">说明</span><span class="sxs-lookup"><span data-stu-id="73117-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73117-112">setting</span><span class="sxs-lookup"><span data-stu-id="73117-112">setting</span></span>|<span data-ttu-id="73117-113">String</span><span class="sxs-lookup"><span data-stu-id="73117-113">String</span></span>|<span data-ttu-id="73117-114">报告的设置</span><span class="sxs-lookup"><span data-stu-id="73117-114">The setting that is being reported</span></span>|
|<span data-ttu-id="73117-115">settingName</span><span class="sxs-lookup"><span data-stu-id="73117-115">settingName</span></span>|<span data-ttu-id="73117-116">String</span><span class="sxs-lookup"><span data-stu-id="73117-116">String</span></span>|<span data-ttu-id="73117-117">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="73117-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="73117-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="73117-118">instanceDisplayName</span></span>|<span data-ttu-id="73117-119">String</span><span class="sxs-lookup"><span data-stu-id="73117-119">String</span></span>|<span data-ttu-id="73117-120">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="73117-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="73117-121">state</span><span class="sxs-lookup"><span data-stu-id="73117-121">state</span></span>|[<span data-ttu-id="73117-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="73117-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="73117-123">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="73117-123">The compliance state of the setting.</span></span> <span data-ttu-id="73117-124">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="73117-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="73117-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="73117-125">errorCode</span></span>|<span data-ttu-id="73117-126">Int64</span><span class="sxs-lookup"><span data-stu-id="73117-126">Int64</span></span>|<span data-ttu-id="73117-127">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="73117-127">Error code for the setting</span></span>|
|<span data-ttu-id="73117-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="73117-128">errorDescription</span></span>|<span data-ttu-id="73117-129">String</span><span class="sxs-lookup"><span data-stu-id="73117-129">String</span></span>|<span data-ttu-id="73117-130">错误说明</span><span class="sxs-lookup"><span data-stu-id="73117-130">Error description</span></span>|
|<span data-ttu-id="73117-131">userId</span><span class="sxs-lookup"><span data-stu-id="73117-131">userId</span></span>|<span data-ttu-id="73117-132">String</span><span class="sxs-lookup"><span data-stu-id="73117-132">String</span></span>|<span data-ttu-id="73117-133">UserId</span><span class="sxs-lookup"><span data-stu-id="73117-133">UserId</span></span>|
|<span data-ttu-id="73117-134">userName</span><span class="sxs-lookup"><span data-stu-id="73117-134">userName</span></span>|<span data-ttu-id="73117-135">String</span><span class="sxs-lookup"><span data-stu-id="73117-135">String</span></span>|<span data-ttu-id="73117-136">UserName</span><span class="sxs-lookup"><span data-stu-id="73117-136">UserName</span></span>|
|<span data-ttu-id="73117-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="73117-137">userEmail</span></span>|<span data-ttu-id="73117-138">String</span><span class="sxs-lookup"><span data-stu-id="73117-138">String</span></span>|<span data-ttu-id="73117-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="73117-139">UserEmail</span></span>|
|<span data-ttu-id="73117-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="73117-140">userPrincipalName</span></span>|<span data-ttu-id="73117-141">String</span><span class="sxs-lookup"><span data-stu-id="73117-141">String</span></span>|<span data-ttu-id="73117-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="73117-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="73117-143">源</span><span class="sxs-lookup"><span data-stu-id="73117-143">sources</span></span>|<span data-ttu-id="73117-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73117-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="73117-145">参与策略</span><span class="sxs-lookup"><span data-stu-id="73117-145">Contributing policies</span></span>|
|<span data-ttu-id="73117-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="73117-146">currentValue</span></span>|<span data-ttu-id="73117-147">String</span><span class="sxs-lookup"><span data-stu-id="73117-147">String</span></span>|<span data-ttu-id="73117-148">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="73117-148">Current value of setting on device</span></span>|
|<span data-ttu-id="73117-149">settingInstanceId</span><span class="sxs-lookup"><span data-stu-id="73117-149">settingInstanceId</span></span>|<span data-ttu-id="73117-150">String</span><span class="sxs-lookup"><span data-stu-id="73117-150">String</span></span>|<span data-ttu-id="73117-151">SettingInstanceId</span><span class="sxs-lookup"><span data-stu-id="73117-151">SettingInstanceId</span></span>|

## <a name="relationships"></a><span data-ttu-id="73117-152">关系</span><span class="sxs-lookup"><span data-stu-id="73117-152">Relationships</span></span>
<span data-ttu-id="73117-153">无</span><span class="sxs-lookup"><span data-stu-id="73117-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73117-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73117-154">JSON Representation</span></span>
<span data-ttu-id="73117-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73117-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
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





