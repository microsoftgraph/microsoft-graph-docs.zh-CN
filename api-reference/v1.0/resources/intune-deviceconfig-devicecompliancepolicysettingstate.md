---
title: deviceCompliancePolicySettingState 资源类型
description: 给定设备的设备符合性策略设置状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 05f79a5967ae97eb825d85732f207682d9add645
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028460"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="312ce-103">deviceCompliancePolicySettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="312ce-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="312ce-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="312ce-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="312ce-105">给定设备的设备符合性策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="312ce-105">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="312ce-106">属性</span><span class="sxs-lookup"><span data-stu-id="312ce-106">Properties</span></span>
|<span data-ttu-id="312ce-107">属性</span><span class="sxs-lookup"><span data-stu-id="312ce-107">Property</span></span>|<span data-ttu-id="312ce-108">类型</span><span class="sxs-lookup"><span data-stu-id="312ce-108">Type</span></span>|<span data-ttu-id="312ce-109">说明</span><span class="sxs-lookup"><span data-stu-id="312ce-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="312ce-110">setting</span><span class="sxs-lookup"><span data-stu-id="312ce-110">setting</span></span>|<span data-ttu-id="312ce-111">String</span><span class="sxs-lookup"><span data-stu-id="312ce-111">String</span></span>|<span data-ttu-id="312ce-112">报告的设置</span><span class="sxs-lookup"><span data-stu-id="312ce-112">The setting that is being reported</span></span>|
|<span data-ttu-id="312ce-113">settingName</span><span class="sxs-lookup"><span data-stu-id="312ce-113">settingName</span></span>|<span data-ttu-id="312ce-114">String</span><span class="sxs-lookup"><span data-stu-id="312ce-114">String</span></span>|<span data-ttu-id="312ce-115">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="312ce-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="312ce-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="312ce-116">instanceDisplayName</span></span>|<span data-ttu-id="312ce-117">String</span><span class="sxs-lookup"><span data-stu-id="312ce-117">String</span></span>|<span data-ttu-id="312ce-118">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="312ce-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="312ce-119">state</span><span class="sxs-lookup"><span data-stu-id="312ce-119">state</span></span>|[<span data-ttu-id="312ce-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="312ce-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="312ce-121">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="312ce-121">The compliance state of the setting.</span></span> <span data-ttu-id="312ce-122">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="312ce-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="312ce-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="312ce-123">errorCode</span></span>|<span data-ttu-id="312ce-124">Int64</span><span class="sxs-lookup"><span data-stu-id="312ce-124">Int64</span></span>|<span data-ttu-id="312ce-125">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="312ce-125">Error code for the setting</span></span>|
|<span data-ttu-id="312ce-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="312ce-126">errorDescription</span></span>|<span data-ttu-id="312ce-127">String</span><span class="sxs-lookup"><span data-stu-id="312ce-127">String</span></span>|<span data-ttu-id="312ce-128">错误说明</span><span class="sxs-lookup"><span data-stu-id="312ce-128">Error description</span></span>|
|<span data-ttu-id="312ce-129">userId</span><span class="sxs-lookup"><span data-stu-id="312ce-129">userId</span></span>|<span data-ttu-id="312ce-130">String</span><span class="sxs-lookup"><span data-stu-id="312ce-130">String</span></span>|<span data-ttu-id="312ce-131">UserId</span><span class="sxs-lookup"><span data-stu-id="312ce-131">UserId</span></span>|
|<span data-ttu-id="312ce-132">userName</span><span class="sxs-lookup"><span data-stu-id="312ce-132">userName</span></span>|<span data-ttu-id="312ce-133">String</span><span class="sxs-lookup"><span data-stu-id="312ce-133">String</span></span>|<span data-ttu-id="312ce-134">UserName</span><span class="sxs-lookup"><span data-stu-id="312ce-134">UserName</span></span>|
|<span data-ttu-id="312ce-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="312ce-135">userEmail</span></span>|<span data-ttu-id="312ce-136">String</span><span class="sxs-lookup"><span data-stu-id="312ce-136">String</span></span>|<span data-ttu-id="312ce-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="312ce-137">UserEmail</span></span>|
|<span data-ttu-id="312ce-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="312ce-138">userPrincipalName</span></span>|<span data-ttu-id="312ce-139">字符串</span><span class="sxs-lookup"><span data-stu-id="312ce-139">String</span></span>|<span data-ttu-id="312ce-140">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="312ce-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="312ce-141">源</span><span class="sxs-lookup"><span data-stu-id="312ce-141">sources</span></span>|<span data-ttu-id="312ce-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="312ce-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="312ce-143">参与策略</span><span class="sxs-lookup"><span data-stu-id="312ce-143">Contributing policies</span></span>|
|<span data-ttu-id="312ce-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="312ce-144">currentValue</span></span>|<span data-ttu-id="312ce-145">String</span><span class="sxs-lookup"><span data-stu-id="312ce-145">String</span></span>|<span data-ttu-id="312ce-146">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="312ce-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="312ce-147">关系</span><span class="sxs-lookup"><span data-stu-id="312ce-147">Relationships</span></span>
<span data-ttu-id="312ce-148">无</span><span class="sxs-lookup"><span data-stu-id="312ce-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="312ce-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="312ce-149">JSON Representation</span></span>
<span data-ttu-id="312ce-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="312ce-150">Here is a JSON representation of the resource.</span></span>
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



