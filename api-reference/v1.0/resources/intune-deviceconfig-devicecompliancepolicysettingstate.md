---
title: deviceCompliancePolicySettingState 资源类型
description: 给定设备的设备符合性策略设置状态。
author: tfitzmac
ms.openlocfilehash: 3dcd63327a3518314619cd7add6ac6f23e69396b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320368"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="e388a-103">deviceCompliancePolicySettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="e388a-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="e388a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e388a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e388a-105">给定设备的设备符合性策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="e388a-105">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="e388a-106">属性</span><span class="sxs-lookup"><span data-stu-id="e388a-106">Properties</span></span>
|<span data-ttu-id="e388a-107">属性</span><span class="sxs-lookup"><span data-stu-id="e388a-107">Property</span></span>|<span data-ttu-id="e388a-108">类型</span><span class="sxs-lookup"><span data-stu-id="e388a-108">Type</span></span>|<span data-ttu-id="e388a-109">说明</span><span class="sxs-lookup"><span data-stu-id="e388a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e388a-110">setting</span><span class="sxs-lookup"><span data-stu-id="e388a-110">setting</span></span>|<span data-ttu-id="e388a-111">String</span><span class="sxs-lookup"><span data-stu-id="e388a-111">String</span></span>|<span data-ttu-id="e388a-112">报告的设置</span><span class="sxs-lookup"><span data-stu-id="e388a-112">The setting that is being reported</span></span>|
|<span data-ttu-id="e388a-113">settingName</span><span class="sxs-lookup"><span data-stu-id="e388a-113">settingName</span></span>|<span data-ttu-id="e388a-114">String</span><span class="sxs-lookup"><span data-stu-id="e388a-114">String</span></span>|<span data-ttu-id="e388a-115">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="e388a-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="e388a-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e388a-116">instanceDisplayName</span></span>|<span data-ttu-id="e388a-117">String</span><span class="sxs-lookup"><span data-stu-id="e388a-117">String</span></span>|<span data-ttu-id="e388a-118">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="e388a-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="e388a-119">state</span><span class="sxs-lookup"><span data-stu-id="e388a-119">state</span></span>|[<span data-ttu-id="e388a-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="e388a-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e388a-121">设置合规性状态。</span><span class="sxs-lookup"><span data-stu-id="e388a-121">The compliance state of the setting.</span></span> <span data-ttu-id="e388a-122">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="e388a-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e388a-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="e388a-123">errorCode</span></span>|<span data-ttu-id="e388a-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e388a-124">Int64</span></span>|<span data-ttu-id="e388a-125">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="e388a-125">Error code for the setting</span></span>|
|<span data-ttu-id="e388a-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="e388a-126">errorDescription</span></span>|<span data-ttu-id="e388a-127">String</span><span class="sxs-lookup"><span data-stu-id="e388a-127">String</span></span>|<span data-ttu-id="e388a-128">错误说明</span><span class="sxs-lookup"><span data-stu-id="e388a-128">Error description</span></span>|
|<span data-ttu-id="e388a-129">userId</span><span class="sxs-lookup"><span data-stu-id="e388a-129">userId</span></span>|<span data-ttu-id="e388a-130">String</span><span class="sxs-lookup"><span data-stu-id="e388a-130">String</span></span>|<span data-ttu-id="e388a-131">UserId</span><span class="sxs-lookup"><span data-stu-id="e388a-131">UserId</span></span>|
|<span data-ttu-id="e388a-132">userName</span><span class="sxs-lookup"><span data-stu-id="e388a-132">userName</span></span>|<span data-ttu-id="e388a-133">String</span><span class="sxs-lookup"><span data-stu-id="e388a-133">String</span></span>|<span data-ttu-id="e388a-134">UserName</span><span class="sxs-lookup"><span data-stu-id="e388a-134">UserName</span></span>|
|<span data-ttu-id="e388a-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="e388a-135">userEmail</span></span>|<span data-ttu-id="e388a-136">String</span><span class="sxs-lookup"><span data-stu-id="e388a-136">String</span></span>|<span data-ttu-id="e388a-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="e388a-137">UserEmail</span></span>|
|<span data-ttu-id="e388a-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e388a-138">userPrincipalName</span></span>|<span data-ttu-id="e388a-139">String</span><span class="sxs-lookup"><span data-stu-id="e388a-139">String</span></span>|<span data-ttu-id="e388a-140">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="e388a-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="e388a-141">sources</span><span class="sxs-lookup"><span data-stu-id="e388a-141">sources</span></span>|<span data-ttu-id="e388a-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e388a-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="e388a-143">参与策略</span><span class="sxs-lookup"><span data-stu-id="e388a-143">Contributing policies</span></span>|
|<span data-ttu-id="e388a-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="e388a-144">currentValue</span></span>|<span data-ttu-id="e388a-145">String</span><span class="sxs-lookup"><span data-stu-id="e388a-145">String</span></span>|<span data-ttu-id="e388a-146">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="e388a-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="e388a-147">关系</span><span class="sxs-lookup"><span data-stu-id="e388a-147">Relationships</span></span>
<span data-ttu-id="e388a-148">无</span><span class="sxs-lookup"><span data-stu-id="e388a-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e388a-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e388a-149">JSON Representation</span></span>
<span data-ttu-id="e388a-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e388a-150">Here is a JSON representation of the resource.</span></span>
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



