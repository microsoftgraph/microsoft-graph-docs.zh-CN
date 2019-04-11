---
title: deviceCompliancePolicySettingState 资源类型
description: 给定设备的设备符合性策略设置状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6c204294190f2f585ad19f7cad4f68e2f7fcc03
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782203"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="2fc63-103">deviceCompliancePolicySettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="2fc63-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="2fc63-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2fc63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fc63-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2fc63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fc63-106">给定设备的设备符合性策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="2fc63-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="2fc63-107">属性</span><span class="sxs-lookup"><span data-stu-id="2fc63-107">Properties</span></span>
|<span data-ttu-id="2fc63-108">属性</span><span class="sxs-lookup"><span data-stu-id="2fc63-108">Property</span></span>|<span data-ttu-id="2fc63-109">类型</span><span class="sxs-lookup"><span data-stu-id="2fc63-109">Type</span></span>|<span data-ttu-id="2fc63-110">说明</span><span class="sxs-lookup"><span data-stu-id="2fc63-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fc63-111">setting</span><span class="sxs-lookup"><span data-stu-id="2fc63-111">setting</span></span>|<span data-ttu-id="2fc63-112">String</span><span class="sxs-lookup"><span data-stu-id="2fc63-112">String</span></span>|<span data-ttu-id="2fc63-113">报告的设置</span><span class="sxs-lookup"><span data-stu-id="2fc63-113">The setting that is being reported</span></span>|
|<span data-ttu-id="2fc63-114">settingName</span><span class="sxs-lookup"><span data-stu-id="2fc63-114">settingName</span></span>|<span data-ttu-id="2fc63-115">String</span><span class="sxs-lookup"><span data-stu-id="2fc63-115">String</span></span>|<span data-ttu-id="2fc63-116">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="2fc63-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="2fc63-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2fc63-117">instanceDisplayName</span></span>|<span data-ttu-id="2fc63-118">String</span><span class="sxs-lookup"><span data-stu-id="2fc63-118">String</span></span>|<span data-ttu-id="2fc63-119">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="2fc63-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="2fc63-120">state</span><span class="sxs-lookup"><span data-stu-id="2fc63-120">state</span></span>|[<span data-ttu-id="2fc63-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2fc63-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2fc63-122">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="2fc63-122">The compliance state of the setting.</span></span> <span data-ttu-id="2fc63-123">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="2fc63-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2fc63-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="2fc63-124">errorCode</span></span>|<span data-ttu-id="2fc63-125">Int64</span><span class="sxs-lookup"><span data-stu-id="2fc63-125">Int64</span></span>|<span data-ttu-id="2fc63-126">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="2fc63-126">Error code for the setting</span></span>|
|<span data-ttu-id="2fc63-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="2fc63-127">errorDescription</span></span>|<span data-ttu-id="2fc63-128">String</span><span class="sxs-lookup"><span data-stu-id="2fc63-128">String</span></span>|<span data-ttu-id="2fc63-129">错误说明</span><span class="sxs-lookup"><span data-stu-id="2fc63-129">Error description</span></span>|
|<span data-ttu-id="2fc63-130">userId</span><span class="sxs-lookup"><span data-stu-id="2fc63-130">userId</span></span>|<span data-ttu-id="2fc63-131">String</span><span class="sxs-lookup"><span data-stu-id="2fc63-131">String</span></span>|<span data-ttu-id="2fc63-132">UserId</span><span class="sxs-lookup"><span data-stu-id="2fc63-132">UserId</span></span>|
|<span data-ttu-id="2fc63-133">userName</span><span class="sxs-lookup"><span data-stu-id="2fc63-133">userName</span></span>|<span data-ttu-id="2fc63-134">String</span><span class="sxs-lookup"><span data-stu-id="2fc63-134">String</span></span>|<span data-ttu-id="2fc63-135">UserName</span><span class="sxs-lookup"><span data-stu-id="2fc63-135">UserName</span></span>|
|<span data-ttu-id="2fc63-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="2fc63-136">userEmail</span></span>|<span data-ttu-id="2fc63-137">String</span><span class="sxs-lookup"><span data-stu-id="2fc63-137">String</span></span>|<span data-ttu-id="2fc63-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="2fc63-138">UserEmail</span></span>|
|<span data-ttu-id="2fc63-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2fc63-139">userPrincipalName</span></span>|<span data-ttu-id="2fc63-140">String</span><span class="sxs-lookup"><span data-stu-id="2fc63-140">String</span></span>|<span data-ttu-id="2fc63-141">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="2fc63-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="2fc63-142">源</span><span class="sxs-lookup"><span data-stu-id="2fc63-142">sources</span></span>|<span data-ttu-id="2fc63-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2fc63-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="2fc63-144">参与策略</span><span class="sxs-lookup"><span data-stu-id="2fc63-144">Contributing policies</span></span>|
|<span data-ttu-id="2fc63-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="2fc63-145">currentValue</span></span>|<span data-ttu-id="2fc63-146">String</span><span class="sxs-lookup"><span data-stu-id="2fc63-146">String</span></span>|<span data-ttu-id="2fc63-147">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="2fc63-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fc63-148">关系</span><span class="sxs-lookup"><span data-stu-id="2fc63-148">Relationships</span></span>
<span data-ttu-id="2fc63-149">无</span><span class="sxs-lookup"><span data-stu-id="2fc63-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fc63-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2fc63-150">JSON Representation</span></span>
<span data-ttu-id="2fc63-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2fc63-151">Here is a JSON representation of the resource.</span></span>
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





