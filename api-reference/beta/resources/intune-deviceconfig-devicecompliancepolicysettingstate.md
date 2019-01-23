---
title: deviceCompliancePolicySettingState 资源类型
description: 给定设备的设备符合性策略设置状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b17930161f66ca83d59e3f2f62777a79f82b79f0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425734"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="4eb60-103">deviceCompliancePolicySettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="4eb60-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="4eb60-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4eb60-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4eb60-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4eb60-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4eb60-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4eb60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4eb60-107">给定设备的设备符合性策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="4eb60-107">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="4eb60-108">属性</span><span class="sxs-lookup"><span data-stu-id="4eb60-108">Properties</span></span>
|<span data-ttu-id="4eb60-109">属性</span><span class="sxs-lookup"><span data-stu-id="4eb60-109">Property</span></span>|<span data-ttu-id="4eb60-110">类型</span><span class="sxs-lookup"><span data-stu-id="4eb60-110">Type</span></span>|<span data-ttu-id="4eb60-111">说明</span><span class="sxs-lookup"><span data-stu-id="4eb60-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eb60-112">setting</span><span class="sxs-lookup"><span data-stu-id="4eb60-112">setting</span></span>|<span data-ttu-id="4eb60-113">String</span><span class="sxs-lookup"><span data-stu-id="4eb60-113">String</span></span>|<span data-ttu-id="4eb60-114">报告的设置</span><span class="sxs-lookup"><span data-stu-id="4eb60-114">The setting that is being reported</span></span>|
|<span data-ttu-id="4eb60-115">settingName</span><span class="sxs-lookup"><span data-stu-id="4eb60-115">settingName</span></span>|<span data-ttu-id="4eb60-116">String</span><span class="sxs-lookup"><span data-stu-id="4eb60-116">String</span></span>|<span data-ttu-id="4eb60-117">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="4eb60-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="4eb60-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4eb60-118">instanceDisplayName</span></span>|<span data-ttu-id="4eb60-119">String</span><span class="sxs-lookup"><span data-stu-id="4eb60-119">String</span></span>|<span data-ttu-id="4eb60-120">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="4eb60-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="4eb60-121">state</span><span class="sxs-lookup"><span data-stu-id="4eb60-121">state</span></span>|[<span data-ttu-id="4eb60-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4eb60-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4eb60-123">设置合规性状态。</span><span class="sxs-lookup"><span data-stu-id="4eb60-123">The compliance state of the setting.</span></span> <span data-ttu-id="4eb60-124">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="4eb60-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4eb60-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="4eb60-125">errorCode</span></span>|<span data-ttu-id="4eb60-126">Int64</span><span class="sxs-lookup"><span data-stu-id="4eb60-126">Int64</span></span>|<span data-ttu-id="4eb60-127">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="4eb60-127">Error code for the setting</span></span>|
|<span data-ttu-id="4eb60-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="4eb60-128">errorDescription</span></span>|<span data-ttu-id="4eb60-129">String</span><span class="sxs-lookup"><span data-stu-id="4eb60-129">String</span></span>|<span data-ttu-id="4eb60-130">错误说明</span><span class="sxs-lookup"><span data-stu-id="4eb60-130">Error description</span></span>|
|<span data-ttu-id="4eb60-131">userId</span><span class="sxs-lookup"><span data-stu-id="4eb60-131">userId</span></span>|<span data-ttu-id="4eb60-132">String</span><span class="sxs-lookup"><span data-stu-id="4eb60-132">String</span></span>|<span data-ttu-id="4eb60-133">UserId</span><span class="sxs-lookup"><span data-stu-id="4eb60-133">UserId</span></span>|
|<span data-ttu-id="4eb60-134">userName</span><span class="sxs-lookup"><span data-stu-id="4eb60-134">userName</span></span>|<span data-ttu-id="4eb60-135">String</span><span class="sxs-lookup"><span data-stu-id="4eb60-135">String</span></span>|<span data-ttu-id="4eb60-136">UserName</span><span class="sxs-lookup"><span data-stu-id="4eb60-136">UserName</span></span>|
|<span data-ttu-id="4eb60-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="4eb60-137">userEmail</span></span>|<span data-ttu-id="4eb60-138">String</span><span class="sxs-lookup"><span data-stu-id="4eb60-138">String</span></span>|<span data-ttu-id="4eb60-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="4eb60-139">UserEmail</span></span>|
|<span data-ttu-id="4eb60-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4eb60-140">userPrincipalName</span></span>|<span data-ttu-id="4eb60-141">String</span><span class="sxs-lookup"><span data-stu-id="4eb60-141">String</span></span>|<span data-ttu-id="4eb60-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="4eb60-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="4eb60-143">sources</span><span class="sxs-lookup"><span data-stu-id="4eb60-143">sources</span></span>|<span data-ttu-id="4eb60-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4eb60-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="4eb60-145">参与策略</span><span class="sxs-lookup"><span data-stu-id="4eb60-145">Contributing policies</span></span>|
|<span data-ttu-id="4eb60-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="4eb60-146">currentValue</span></span>|<span data-ttu-id="4eb60-147">String</span><span class="sxs-lookup"><span data-stu-id="4eb60-147">String</span></span>|<span data-ttu-id="4eb60-148">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="4eb60-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="4eb60-149">关系</span><span class="sxs-lookup"><span data-stu-id="4eb60-149">Relationships</span></span>
<span data-ttu-id="4eb60-150">无</span><span class="sxs-lookup"><span data-stu-id="4eb60-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4eb60-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4eb60-151">JSON Representation</span></span>
<span data-ttu-id="4eb60-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4eb60-152">Here is a JSON representation of the resource.</span></span>
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




