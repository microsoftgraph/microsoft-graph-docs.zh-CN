---
title: deviceCompliancePolicySettingState 资源类型
description: 给定设备的设备符合性策略设置状态。
ms.openlocfilehash: d73cbe591e30e465065e0c446c6d98d7232a049c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046782"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="b5826-103">deviceCompliancePolicySettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5826-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="b5826-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b5826-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5826-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b5826-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5826-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b5826-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5826-107">给定设备的设备符合性策略设置状态。</span><span class="sxs-lookup"><span data-stu-id="b5826-107">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="b5826-108">属性</span><span class="sxs-lookup"><span data-stu-id="b5826-108">Properties</span></span>
|<span data-ttu-id="b5826-109">属性</span><span class="sxs-lookup"><span data-stu-id="b5826-109">Property</span></span>|<span data-ttu-id="b5826-110">类型</span><span class="sxs-lookup"><span data-stu-id="b5826-110">Type</span></span>|<span data-ttu-id="b5826-111">说明</span><span class="sxs-lookup"><span data-stu-id="b5826-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5826-112">setting</span><span class="sxs-lookup"><span data-stu-id="b5826-112">setting</span></span>|<span data-ttu-id="b5826-113">String</span><span class="sxs-lookup"><span data-stu-id="b5826-113">String</span></span>|<span data-ttu-id="b5826-114">报告的设置</span><span class="sxs-lookup"><span data-stu-id="b5826-114">The setting that is being reported</span></span>|
|<span data-ttu-id="b5826-115">settingName</span><span class="sxs-lookup"><span data-stu-id="b5826-115">settingName</span></span>|<span data-ttu-id="b5826-116">String</span><span class="sxs-lookup"><span data-stu-id="b5826-116">String</span></span>|<span data-ttu-id="b5826-117">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="b5826-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="b5826-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b5826-118">instanceDisplayName</span></span>|<span data-ttu-id="b5826-119">String</span><span class="sxs-lookup"><span data-stu-id="b5826-119">String</span></span>|<span data-ttu-id="b5826-120">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="b5826-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="b5826-121">state</span><span class="sxs-lookup"><span data-stu-id="b5826-121">state</span></span>|[<span data-ttu-id="b5826-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b5826-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b5826-123">设置合规性状态。</span><span class="sxs-lookup"><span data-stu-id="b5826-123">The compliance state of the setting.</span></span> <span data-ttu-id="b5826-124">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="b5826-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b5826-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="b5826-125">errorCode</span></span>|<span data-ttu-id="b5826-126">Int64</span><span class="sxs-lookup"><span data-stu-id="b5826-126">Int64</span></span>|<span data-ttu-id="b5826-127">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="b5826-127">Error code for the setting</span></span>|
|<span data-ttu-id="b5826-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="b5826-128">errorDescription</span></span>|<span data-ttu-id="b5826-129">String</span><span class="sxs-lookup"><span data-stu-id="b5826-129">String</span></span>|<span data-ttu-id="b5826-130">错误说明</span><span class="sxs-lookup"><span data-stu-id="b5826-130">Error description</span></span>|
|<span data-ttu-id="b5826-131">userId</span><span class="sxs-lookup"><span data-stu-id="b5826-131">userId</span></span>|<span data-ttu-id="b5826-132">String</span><span class="sxs-lookup"><span data-stu-id="b5826-132">String</span></span>|<span data-ttu-id="b5826-133">UserId</span><span class="sxs-lookup"><span data-stu-id="b5826-133">UserId</span></span>|
|<span data-ttu-id="b5826-134">userName</span><span class="sxs-lookup"><span data-stu-id="b5826-134">userName</span></span>|<span data-ttu-id="b5826-135">String</span><span class="sxs-lookup"><span data-stu-id="b5826-135">String</span></span>|<span data-ttu-id="b5826-136">UserName</span><span class="sxs-lookup"><span data-stu-id="b5826-136">UserName</span></span>|
|<span data-ttu-id="b5826-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="b5826-137">userEmail</span></span>|<span data-ttu-id="b5826-138">String</span><span class="sxs-lookup"><span data-stu-id="b5826-138">String</span></span>|<span data-ttu-id="b5826-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="b5826-139">UserEmail</span></span>|
|<span data-ttu-id="b5826-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b5826-140">userPrincipalName</span></span>|<span data-ttu-id="b5826-141">String</span><span class="sxs-lookup"><span data-stu-id="b5826-141">String</span></span>|<span data-ttu-id="b5826-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="b5826-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="b5826-143">sources</span><span class="sxs-lookup"><span data-stu-id="b5826-143">sources</span></span>|<span data-ttu-id="b5826-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b5826-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="b5826-145">参与策略</span><span class="sxs-lookup"><span data-stu-id="b5826-145">Contributing policies</span></span>|
|<span data-ttu-id="b5826-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="b5826-146">currentValue</span></span>|<span data-ttu-id="b5826-147">String</span><span class="sxs-lookup"><span data-stu-id="b5826-147">String</span></span>|<span data-ttu-id="b5826-148">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="b5826-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5826-149">关系</span><span class="sxs-lookup"><span data-stu-id="b5826-149">Relationships</span></span>
<span data-ttu-id="b5826-150">无</span><span class="sxs-lookup"><span data-stu-id="b5826-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b5826-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5826-151">JSON Representation</span></span>
<span data-ttu-id="b5826-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5826-152">Here is a JSON representation of the resource.</span></span>
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





