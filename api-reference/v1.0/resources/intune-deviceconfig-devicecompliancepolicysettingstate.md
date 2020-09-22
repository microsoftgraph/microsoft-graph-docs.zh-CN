---
title: deviceCompliancePolicySettingState 资源类型
description: 给定设备的设备符合性策略设置状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3817f3835ce82e15204d07adc1d7bfe85233d955
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094258"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="5554e-103">deviceCompliancePolicySettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="5554e-103">deviceCompliancePolicySettingState resource type</span></span>

<span data-ttu-id="5554e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5554e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5554e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5554e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5554e-106">给定设备的设备符合性策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="5554e-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="5554e-107">属性</span><span class="sxs-lookup"><span data-stu-id="5554e-107">Properties</span></span>
|<span data-ttu-id="5554e-108">属性</span><span class="sxs-lookup"><span data-stu-id="5554e-108">Property</span></span>|<span data-ttu-id="5554e-109">类型</span><span class="sxs-lookup"><span data-stu-id="5554e-109">Type</span></span>|<span data-ttu-id="5554e-110">说明</span><span class="sxs-lookup"><span data-stu-id="5554e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5554e-111">setting</span><span class="sxs-lookup"><span data-stu-id="5554e-111">setting</span></span>|<span data-ttu-id="5554e-112">String</span><span class="sxs-lookup"><span data-stu-id="5554e-112">String</span></span>|<span data-ttu-id="5554e-113">报告的设置</span><span class="sxs-lookup"><span data-stu-id="5554e-113">The setting that is being reported</span></span>|
|<span data-ttu-id="5554e-114">settingName</span><span class="sxs-lookup"><span data-stu-id="5554e-114">settingName</span></span>|<span data-ttu-id="5554e-115">String</span><span class="sxs-lookup"><span data-stu-id="5554e-115">String</span></span>|<span data-ttu-id="5554e-116">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="5554e-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="5554e-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="5554e-117">instanceDisplayName</span></span>|<span data-ttu-id="5554e-118">String</span><span class="sxs-lookup"><span data-stu-id="5554e-118">String</span></span>|<span data-ttu-id="5554e-119">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="5554e-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="5554e-120">state</span><span class="sxs-lookup"><span data-stu-id="5554e-120">state</span></span>|[<span data-ttu-id="5554e-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="5554e-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="5554e-122">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="5554e-122">The compliance state of the setting.</span></span> <span data-ttu-id="5554e-123">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="5554e-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="5554e-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="5554e-124">errorCode</span></span>|<span data-ttu-id="5554e-125">Int64</span><span class="sxs-lookup"><span data-stu-id="5554e-125">Int64</span></span>|<span data-ttu-id="5554e-126">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="5554e-126">Error code for the setting</span></span>|
|<span data-ttu-id="5554e-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="5554e-127">errorDescription</span></span>|<span data-ttu-id="5554e-128">String</span><span class="sxs-lookup"><span data-stu-id="5554e-128">String</span></span>|<span data-ttu-id="5554e-129">错误说明</span><span class="sxs-lookup"><span data-stu-id="5554e-129">Error description</span></span>|
|<span data-ttu-id="5554e-130">userId</span><span class="sxs-lookup"><span data-stu-id="5554e-130">userId</span></span>|<span data-ttu-id="5554e-131">String</span><span class="sxs-lookup"><span data-stu-id="5554e-131">String</span></span>|<span data-ttu-id="5554e-132">UserId</span><span class="sxs-lookup"><span data-stu-id="5554e-132">UserId</span></span>|
|<span data-ttu-id="5554e-133">userName</span><span class="sxs-lookup"><span data-stu-id="5554e-133">userName</span></span>|<span data-ttu-id="5554e-134">String</span><span class="sxs-lookup"><span data-stu-id="5554e-134">String</span></span>|<span data-ttu-id="5554e-135">UserName</span><span class="sxs-lookup"><span data-stu-id="5554e-135">UserName</span></span>|
|<span data-ttu-id="5554e-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="5554e-136">userEmail</span></span>|<span data-ttu-id="5554e-137">String</span><span class="sxs-lookup"><span data-stu-id="5554e-137">String</span></span>|<span data-ttu-id="5554e-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="5554e-138">UserEmail</span></span>|
|<span data-ttu-id="5554e-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5554e-139">userPrincipalName</span></span>|<span data-ttu-id="5554e-140">String</span><span class="sxs-lookup"><span data-stu-id="5554e-140">String</span></span>|<span data-ttu-id="5554e-141">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="5554e-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="5554e-142">源</span><span class="sxs-lookup"><span data-stu-id="5554e-142">sources</span></span>|<span data-ttu-id="5554e-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5554e-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="5554e-144">参与策略</span><span class="sxs-lookup"><span data-stu-id="5554e-144">Contributing policies</span></span>|
|<span data-ttu-id="5554e-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="5554e-145">currentValue</span></span>|<span data-ttu-id="5554e-146">String</span><span class="sxs-lookup"><span data-stu-id="5554e-146">String</span></span>|<span data-ttu-id="5554e-147">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="5554e-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="5554e-148">关系</span><span class="sxs-lookup"><span data-stu-id="5554e-148">Relationships</span></span>
<span data-ttu-id="5554e-149">无</span><span class="sxs-lookup"><span data-stu-id="5554e-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5554e-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5554e-150">JSON Representation</span></span>
<span data-ttu-id="5554e-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5554e-151">Here is a JSON representation of the resource.</span></span>
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
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```









