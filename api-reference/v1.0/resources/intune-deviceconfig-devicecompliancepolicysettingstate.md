---
title: deviceCompliancePolicySettingState 资源类型
description: 给定设备的设备符合性策略设置状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c4d291f84a8c4404ff5b4425680260997b6b452f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572414"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="6a09c-103">deviceCompliancePolicySettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a09c-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="6a09c-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a09c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a09c-105">给定设备的设备符合性策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="6a09c-105">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="6a09c-106">属性</span><span class="sxs-lookup"><span data-stu-id="6a09c-106">Properties</span></span>
|<span data-ttu-id="6a09c-107">属性</span><span class="sxs-lookup"><span data-stu-id="6a09c-107">Property</span></span>|<span data-ttu-id="6a09c-108">类型</span><span class="sxs-lookup"><span data-stu-id="6a09c-108">Type</span></span>|<span data-ttu-id="6a09c-109">说明</span><span class="sxs-lookup"><span data-stu-id="6a09c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a09c-110">setting</span><span class="sxs-lookup"><span data-stu-id="6a09c-110">setting</span></span>|<span data-ttu-id="6a09c-111">String</span><span class="sxs-lookup"><span data-stu-id="6a09c-111">String</span></span>|<span data-ttu-id="6a09c-112">报告的设置</span><span class="sxs-lookup"><span data-stu-id="6a09c-112">The setting that is being reported</span></span>|
|<span data-ttu-id="6a09c-113">settingName</span><span class="sxs-lookup"><span data-stu-id="6a09c-113">settingName</span></span>|<span data-ttu-id="6a09c-114">String</span><span class="sxs-lookup"><span data-stu-id="6a09c-114">String</span></span>|<span data-ttu-id="6a09c-115">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="6a09c-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="6a09c-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6a09c-116">instanceDisplayName</span></span>|<span data-ttu-id="6a09c-117">String</span><span class="sxs-lookup"><span data-stu-id="6a09c-117">String</span></span>|<span data-ttu-id="6a09c-118">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="6a09c-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="6a09c-119">state</span><span class="sxs-lookup"><span data-stu-id="6a09c-119">state</span></span>|[<span data-ttu-id="6a09c-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="6a09c-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="6a09c-121">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="6a09c-121">The compliance state of the setting.</span></span> <span data-ttu-id="6a09c-122">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="6a09c-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6a09c-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="6a09c-123">errorCode</span></span>|<span data-ttu-id="6a09c-124">Int64</span><span class="sxs-lookup"><span data-stu-id="6a09c-124">Int64</span></span>|<span data-ttu-id="6a09c-125">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="6a09c-125">Error code for the setting</span></span>|
|<span data-ttu-id="6a09c-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="6a09c-126">errorDescription</span></span>|<span data-ttu-id="6a09c-127">String</span><span class="sxs-lookup"><span data-stu-id="6a09c-127">String</span></span>|<span data-ttu-id="6a09c-128">错误说明</span><span class="sxs-lookup"><span data-stu-id="6a09c-128">Error description</span></span>|
|<span data-ttu-id="6a09c-129">userId</span><span class="sxs-lookup"><span data-stu-id="6a09c-129">userId</span></span>|<span data-ttu-id="6a09c-130">String</span><span class="sxs-lookup"><span data-stu-id="6a09c-130">String</span></span>|<span data-ttu-id="6a09c-131">UserId</span><span class="sxs-lookup"><span data-stu-id="6a09c-131">UserId</span></span>|
|<span data-ttu-id="6a09c-132">userName</span><span class="sxs-lookup"><span data-stu-id="6a09c-132">userName</span></span>|<span data-ttu-id="6a09c-133">String</span><span class="sxs-lookup"><span data-stu-id="6a09c-133">String</span></span>|<span data-ttu-id="6a09c-134">UserName</span><span class="sxs-lookup"><span data-stu-id="6a09c-134">UserName</span></span>|
|<span data-ttu-id="6a09c-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="6a09c-135">userEmail</span></span>|<span data-ttu-id="6a09c-136">String</span><span class="sxs-lookup"><span data-stu-id="6a09c-136">String</span></span>|<span data-ttu-id="6a09c-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="6a09c-137">UserEmail</span></span>|
|<span data-ttu-id="6a09c-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6a09c-138">userPrincipalName</span></span>|<span data-ttu-id="6a09c-139">String</span><span class="sxs-lookup"><span data-stu-id="6a09c-139">String</span></span>|<span data-ttu-id="6a09c-140">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="6a09c-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="6a09c-141">源</span><span class="sxs-lookup"><span data-stu-id="6a09c-141">sources</span></span>|<span data-ttu-id="6a09c-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6a09c-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="6a09c-143">参与策略</span><span class="sxs-lookup"><span data-stu-id="6a09c-143">Contributing policies</span></span>|
|<span data-ttu-id="6a09c-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="6a09c-144">currentValue</span></span>|<span data-ttu-id="6a09c-145">String</span><span class="sxs-lookup"><span data-stu-id="6a09c-145">String</span></span>|<span data-ttu-id="6a09c-146">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="6a09c-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a09c-147">关系</span><span class="sxs-lookup"><span data-stu-id="6a09c-147">Relationships</span></span>
<span data-ttu-id="6a09c-148">无</span><span class="sxs-lookup"><span data-stu-id="6a09c-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a09c-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a09c-149">JSON Representation</span></span>
<span data-ttu-id="6a09c-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a09c-150">Here is a JSON representation of the resource.</span></span>
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



