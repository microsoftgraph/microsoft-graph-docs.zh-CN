---
title: deviceCompliancePolicySettingState 资源类型
description: 给定设备的设备符合性策略设置状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f2700f348c8d2f1915e7cfd14221951894eb68f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526683"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="83b0c-103">deviceCompliancePolicySettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="83b0c-103">deviceCompliancePolicySettingState resource type</span></span>

<span data-ttu-id="83b0c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="83b0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83b0c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="83b0c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83b0c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83b0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83b0c-107">给定设备的设备符合性策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="83b0c-107">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="83b0c-108">属性</span><span class="sxs-lookup"><span data-stu-id="83b0c-108">Properties</span></span>
|<span data-ttu-id="83b0c-109">属性</span><span class="sxs-lookup"><span data-stu-id="83b0c-109">Property</span></span>|<span data-ttu-id="83b0c-110">类型</span><span class="sxs-lookup"><span data-stu-id="83b0c-110">Type</span></span>|<span data-ttu-id="83b0c-111">说明</span><span class="sxs-lookup"><span data-stu-id="83b0c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83b0c-112">setting</span><span class="sxs-lookup"><span data-stu-id="83b0c-112">setting</span></span>|<span data-ttu-id="83b0c-113">String</span><span class="sxs-lookup"><span data-stu-id="83b0c-113">String</span></span>|<span data-ttu-id="83b0c-114">报告的设置</span><span class="sxs-lookup"><span data-stu-id="83b0c-114">The setting that is being reported</span></span>|
|<span data-ttu-id="83b0c-115">settingName</span><span class="sxs-lookup"><span data-stu-id="83b0c-115">settingName</span></span>|<span data-ttu-id="83b0c-116">String</span><span class="sxs-lookup"><span data-stu-id="83b0c-116">String</span></span>|<span data-ttu-id="83b0c-117">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="83b0c-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="83b0c-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="83b0c-118">instanceDisplayName</span></span>|<span data-ttu-id="83b0c-119">String</span><span class="sxs-lookup"><span data-stu-id="83b0c-119">String</span></span>|<span data-ttu-id="83b0c-120">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="83b0c-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="83b0c-121">state</span><span class="sxs-lookup"><span data-stu-id="83b0c-121">state</span></span>|[<span data-ttu-id="83b0c-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="83b0c-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="83b0c-123">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="83b0c-123">The compliance state of the setting.</span></span> <span data-ttu-id="83b0c-124">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="83b0c-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="83b0c-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="83b0c-125">errorCode</span></span>|<span data-ttu-id="83b0c-126">Int64</span><span class="sxs-lookup"><span data-stu-id="83b0c-126">Int64</span></span>|<span data-ttu-id="83b0c-127">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="83b0c-127">Error code for the setting</span></span>|
|<span data-ttu-id="83b0c-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="83b0c-128">errorDescription</span></span>|<span data-ttu-id="83b0c-129">String</span><span class="sxs-lookup"><span data-stu-id="83b0c-129">String</span></span>|<span data-ttu-id="83b0c-130">错误说明</span><span class="sxs-lookup"><span data-stu-id="83b0c-130">Error description</span></span>|
|<span data-ttu-id="83b0c-131">userId</span><span class="sxs-lookup"><span data-stu-id="83b0c-131">userId</span></span>|<span data-ttu-id="83b0c-132">String</span><span class="sxs-lookup"><span data-stu-id="83b0c-132">String</span></span>|<span data-ttu-id="83b0c-133">UserId</span><span class="sxs-lookup"><span data-stu-id="83b0c-133">UserId</span></span>|
|<span data-ttu-id="83b0c-134">userName</span><span class="sxs-lookup"><span data-stu-id="83b0c-134">userName</span></span>|<span data-ttu-id="83b0c-135">String</span><span class="sxs-lookup"><span data-stu-id="83b0c-135">String</span></span>|<span data-ttu-id="83b0c-136">UserName</span><span class="sxs-lookup"><span data-stu-id="83b0c-136">UserName</span></span>|
|<span data-ttu-id="83b0c-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="83b0c-137">userEmail</span></span>|<span data-ttu-id="83b0c-138">String</span><span class="sxs-lookup"><span data-stu-id="83b0c-138">String</span></span>|<span data-ttu-id="83b0c-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="83b0c-139">UserEmail</span></span>|
|<span data-ttu-id="83b0c-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="83b0c-140">userPrincipalName</span></span>|<span data-ttu-id="83b0c-141">字符串</span><span class="sxs-lookup"><span data-stu-id="83b0c-141">String</span></span>|<span data-ttu-id="83b0c-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="83b0c-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="83b0c-143">源</span><span class="sxs-lookup"><span data-stu-id="83b0c-143">sources</span></span>|<span data-ttu-id="83b0c-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="83b0c-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="83b0c-145">参与策略</span><span class="sxs-lookup"><span data-stu-id="83b0c-145">Contributing policies</span></span>|
|<span data-ttu-id="83b0c-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="83b0c-146">currentValue</span></span>|<span data-ttu-id="83b0c-147">String</span><span class="sxs-lookup"><span data-stu-id="83b0c-147">String</span></span>|<span data-ttu-id="83b0c-148">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="83b0c-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="83b0c-149">关系</span><span class="sxs-lookup"><span data-stu-id="83b0c-149">Relationships</span></span>
<span data-ttu-id="83b0c-150">无</span><span class="sxs-lookup"><span data-stu-id="83b0c-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83b0c-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83b0c-151">JSON Representation</span></span>
<span data-ttu-id="83b0c-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83b0c-152">Here is a JSON representation of the resource.</span></span>
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



