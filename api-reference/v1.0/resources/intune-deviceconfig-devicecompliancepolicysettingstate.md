---
title: deviceCompliancePolicySettingState 资源类型
description: 给定设备的设备符合性策略设置状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1d75c82cfdd53d1df51537980487e7f7ed780414
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530820"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="01fba-103">deviceCompliancePolicySettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="01fba-103">deviceCompliancePolicySettingState resource type</span></span>

<span data-ttu-id="01fba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01fba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01fba-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="01fba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01fba-106">给定设备的设备符合性策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="01fba-106">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="01fba-107">属性</span><span class="sxs-lookup"><span data-stu-id="01fba-107">Properties</span></span>
|<span data-ttu-id="01fba-108">属性</span><span class="sxs-lookup"><span data-stu-id="01fba-108">Property</span></span>|<span data-ttu-id="01fba-109">类型</span><span class="sxs-lookup"><span data-stu-id="01fba-109">Type</span></span>|<span data-ttu-id="01fba-110">说明</span><span class="sxs-lookup"><span data-stu-id="01fba-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01fba-111">setting</span><span class="sxs-lookup"><span data-stu-id="01fba-111">setting</span></span>|<span data-ttu-id="01fba-112">字符串</span><span class="sxs-lookup"><span data-stu-id="01fba-112">String</span></span>|<span data-ttu-id="01fba-113">报告的设置</span><span class="sxs-lookup"><span data-stu-id="01fba-113">The setting that is being reported</span></span>|
|<span data-ttu-id="01fba-114">settingName</span><span class="sxs-lookup"><span data-stu-id="01fba-114">settingName</span></span>|<span data-ttu-id="01fba-115">字符串</span><span class="sxs-lookup"><span data-stu-id="01fba-115">String</span></span>|<span data-ttu-id="01fba-116">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="01fba-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="01fba-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="01fba-117">instanceDisplayName</span></span>|<span data-ttu-id="01fba-118">字符串</span><span class="sxs-lookup"><span data-stu-id="01fba-118">String</span></span>|<span data-ttu-id="01fba-119">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="01fba-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="01fba-120">state</span><span class="sxs-lookup"><span data-stu-id="01fba-120">state</span></span>|[<span data-ttu-id="01fba-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="01fba-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="01fba-122">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="01fba-122">The compliance state of the setting.</span></span> <span data-ttu-id="01fba-123">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="01fba-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="01fba-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="01fba-124">errorCode</span></span>|<span data-ttu-id="01fba-125">Int64</span><span class="sxs-lookup"><span data-stu-id="01fba-125">Int64</span></span>|<span data-ttu-id="01fba-126">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="01fba-126">Error code for the setting</span></span>|
|<span data-ttu-id="01fba-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="01fba-127">errorDescription</span></span>|<span data-ttu-id="01fba-128">字符串</span><span class="sxs-lookup"><span data-stu-id="01fba-128">String</span></span>|<span data-ttu-id="01fba-129">错误说明</span><span class="sxs-lookup"><span data-stu-id="01fba-129">Error description</span></span>|
|<span data-ttu-id="01fba-130">userId</span><span class="sxs-lookup"><span data-stu-id="01fba-130">userId</span></span>|<span data-ttu-id="01fba-131">String</span><span class="sxs-lookup"><span data-stu-id="01fba-131">String</span></span>|<span data-ttu-id="01fba-132">UserId</span><span class="sxs-lookup"><span data-stu-id="01fba-132">UserId</span></span>|
|<span data-ttu-id="01fba-133">userName</span><span class="sxs-lookup"><span data-stu-id="01fba-133">userName</span></span>|<span data-ttu-id="01fba-134">字符串</span><span class="sxs-lookup"><span data-stu-id="01fba-134">String</span></span>|<span data-ttu-id="01fba-135">UserName</span><span class="sxs-lookup"><span data-stu-id="01fba-135">UserName</span></span>|
|<span data-ttu-id="01fba-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="01fba-136">userEmail</span></span>|<span data-ttu-id="01fba-137">字符串</span><span class="sxs-lookup"><span data-stu-id="01fba-137">String</span></span>|<span data-ttu-id="01fba-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="01fba-138">UserEmail</span></span>|
|<span data-ttu-id="01fba-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="01fba-139">userPrincipalName</span></span>|<span data-ttu-id="01fba-140">字符串</span><span class="sxs-lookup"><span data-stu-id="01fba-140">String</span></span>|<span data-ttu-id="01fba-141">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="01fba-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="01fba-142">源</span><span class="sxs-lookup"><span data-stu-id="01fba-142">sources</span></span>|<span data-ttu-id="01fba-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="01fba-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="01fba-144">参与策略</span><span class="sxs-lookup"><span data-stu-id="01fba-144">Contributing policies</span></span>|
|<span data-ttu-id="01fba-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="01fba-145">currentValue</span></span>|<span data-ttu-id="01fba-146">String</span><span class="sxs-lookup"><span data-stu-id="01fba-146">String</span></span>|<span data-ttu-id="01fba-147">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="01fba-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="01fba-148">关系</span><span class="sxs-lookup"><span data-stu-id="01fba-148">Relationships</span></span>
<span data-ttu-id="01fba-149">无</span><span class="sxs-lookup"><span data-stu-id="01fba-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01fba-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01fba-150">JSON Representation</span></span>
<span data-ttu-id="01fba-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01fba-151">Here is a JSON representation of the resource.</span></span>
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




