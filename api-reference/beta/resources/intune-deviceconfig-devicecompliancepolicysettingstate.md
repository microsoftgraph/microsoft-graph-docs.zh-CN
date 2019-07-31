---
title: deviceCompliancePolicySettingState 资源类型
description: 给定设备的设备符合性策略设置状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5f0d171854bbd0b7bd67effdb04438e44e0f14b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970533"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="05150-103">deviceCompliancePolicySettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="05150-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="05150-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="05150-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05150-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="05150-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05150-106">给定设备的设备符合性策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="05150-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="05150-107">属性</span><span class="sxs-lookup"><span data-stu-id="05150-107">Properties</span></span>
|<span data-ttu-id="05150-108">属性</span><span class="sxs-lookup"><span data-stu-id="05150-108">Property</span></span>|<span data-ttu-id="05150-109">类型</span><span class="sxs-lookup"><span data-stu-id="05150-109">Type</span></span>|<span data-ttu-id="05150-110">说明</span><span class="sxs-lookup"><span data-stu-id="05150-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05150-111">setting</span><span class="sxs-lookup"><span data-stu-id="05150-111">setting</span></span>|<span data-ttu-id="05150-112">String</span><span class="sxs-lookup"><span data-stu-id="05150-112">String</span></span>|<span data-ttu-id="05150-113">报告的设置</span><span class="sxs-lookup"><span data-stu-id="05150-113">The setting that is being reported</span></span>|
|<span data-ttu-id="05150-114">settingName</span><span class="sxs-lookup"><span data-stu-id="05150-114">settingName</span></span>|<span data-ttu-id="05150-115">String</span><span class="sxs-lookup"><span data-stu-id="05150-115">String</span></span>|<span data-ttu-id="05150-116">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="05150-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="05150-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="05150-117">instanceDisplayName</span></span>|<span data-ttu-id="05150-118">String</span><span class="sxs-lookup"><span data-stu-id="05150-118">String</span></span>|<span data-ttu-id="05150-119">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="05150-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="05150-120">state</span><span class="sxs-lookup"><span data-stu-id="05150-120">state</span></span>|[<span data-ttu-id="05150-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="05150-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="05150-122">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="05150-122">The compliance state of the setting.</span></span> <span data-ttu-id="05150-123">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="05150-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="05150-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="05150-124">errorCode</span></span>|<span data-ttu-id="05150-125">Int64</span><span class="sxs-lookup"><span data-stu-id="05150-125">Int64</span></span>|<span data-ttu-id="05150-126">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="05150-126">Error code for the setting</span></span>|
|<span data-ttu-id="05150-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="05150-127">errorDescription</span></span>|<span data-ttu-id="05150-128">String</span><span class="sxs-lookup"><span data-stu-id="05150-128">String</span></span>|<span data-ttu-id="05150-129">错误说明</span><span class="sxs-lookup"><span data-stu-id="05150-129">Error description</span></span>|
|<span data-ttu-id="05150-130">userId</span><span class="sxs-lookup"><span data-stu-id="05150-130">userId</span></span>|<span data-ttu-id="05150-131">String</span><span class="sxs-lookup"><span data-stu-id="05150-131">String</span></span>|<span data-ttu-id="05150-132">UserId</span><span class="sxs-lookup"><span data-stu-id="05150-132">UserId</span></span>|
|<span data-ttu-id="05150-133">userName</span><span class="sxs-lookup"><span data-stu-id="05150-133">userName</span></span>|<span data-ttu-id="05150-134">String</span><span class="sxs-lookup"><span data-stu-id="05150-134">String</span></span>|<span data-ttu-id="05150-135">UserName</span><span class="sxs-lookup"><span data-stu-id="05150-135">UserName</span></span>|
|<span data-ttu-id="05150-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="05150-136">userEmail</span></span>|<span data-ttu-id="05150-137">String</span><span class="sxs-lookup"><span data-stu-id="05150-137">String</span></span>|<span data-ttu-id="05150-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="05150-138">UserEmail</span></span>|
|<span data-ttu-id="05150-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="05150-139">userPrincipalName</span></span>|<span data-ttu-id="05150-140">字符串</span><span class="sxs-lookup"><span data-stu-id="05150-140">String</span></span>|<span data-ttu-id="05150-141">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="05150-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="05150-142">源</span><span class="sxs-lookup"><span data-stu-id="05150-142">sources</span></span>|<span data-ttu-id="05150-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="05150-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="05150-144">参与策略</span><span class="sxs-lookup"><span data-stu-id="05150-144">Contributing policies</span></span>|
|<span data-ttu-id="05150-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="05150-145">currentValue</span></span>|<span data-ttu-id="05150-146">String</span><span class="sxs-lookup"><span data-stu-id="05150-146">String</span></span>|<span data-ttu-id="05150-147">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="05150-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="05150-148">关系</span><span class="sxs-lookup"><span data-stu-id="05150-148">Relationships</span></span>
<span data-ttu-id="05150-149">无</span><span class="sxs-lookup"><span data-stu-id="05150-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05150-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05150-150">JSON Representation</span></span>
<span data-ttu-id="05150-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05150-151">Here is a JSON representation of the resource.</span></span>
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





