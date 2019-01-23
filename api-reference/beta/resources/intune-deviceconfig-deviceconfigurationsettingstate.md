---
title: deviceConfigurationSettingState 资源类型
description: 给定设备的设备配置设置状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9355cdf0aab60208246fdae699cda78be65d62ff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415185"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="032a6-103">deviceConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="032a6-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="032a6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="032a6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="032a6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="032a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="032a6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="032a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="032a6-107">给定设备的设备配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="032a6-107">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="032a6-108">属性</span><span class="sxs-lookup"><span data-stu-id="032a6-108">Properties</span></span>
|<span data-ttu-id="032a6-109">属性</span><span class="sxs-lookup"><span data-stu-id="032a6-109">Property</span></span>|<span data-ttu-id="032a6-110">类型</span><span class="sxs-lookup"><span data-stu-id="032a6-110">Type</span></span>|<span data-ttu-id="032a6-111">说明</span><span class="sxs-lookup"><span data-stu-id="032a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="032a6-112">setting</span><span class="sxs-lookup"><span data-stu-id="032a6-112">setting</span></span>|<span data-ttu-id="032a6-113">String</span><span class="sxs-lookup"><span data-stu-id="032a6-113">String</span></span>|<span data-ttu-id="032a6-114">报告的设置</span><span class="sxs-lookup"><span data-stu-id="032a6-114">The setting that is being reported</span></span>|
|<span data-ttu-id="032a6-115">settingName</span><span class="sxs-lookup"><span data-stu-id="032a6-115">settingName</span></span>|<span data-ttu-id="032a6-116">String</span><span class="sxs-lookup"><span data-stu-id="032a6-116">String</span></span>|<span data-ttu-id="032a6-117">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="032a6-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="032a6-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="032a6-118">instanceDisplayName</span></span>|<span data-ttu-id="032a6-119">String</span><span class="sxs-lookup"><span data-stu-id="032a6-119">String</span></span>|<span data-ttu-id="032a6-120">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="032a6-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="032a6-121">state</span><span class="sxs-lookup"><span data-stu-id="032a6-121">state</span></span>|[<span data-ttu-id="032a6-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="032a6-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="032a6-123">设置合规性状态。</span><span class="sxs-lookup"><span data-stu-id="032a6-123">The compliance state of the setting.</span></span> <span data-ttu-id="032a6-124">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="032a6-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="032a6-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="032a6-125">errorCode</span></span>|<span data-ttu-id="032a6-126">Int64</span><span class="sxs-lookup"><span data-stu-id="032a6-126">Int64</span></span>|<span data-ttu-id="032a6-127">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="032a6-127">Error code for the setting</span></span>|
|<span data-ttu-id="032a6-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="032a6-128">errorDescription</span></span>|<span data-ttu-id="032a6-129">String</span><span class="sxs-lookup"><span data-stu-id="032a6-129">String</span></span>|<span data-ttu-id="032a6-130">错误说明</span><span class="sxs-lookup"><span data-stu-id="032a6-130">Error description</span></span>|
|<span data-ttu-id="032a6-131">userId</span><span class="sxs-lookup"><span data-stu-id="032a6-131">userId</span></span>|<span data-ttu-id="032a6-132">String</span><span class="sxs-lookup"><span data-stu-id="032a6-132">String</span></span>|<span data-ttu-id="032a6-133">UserId</span><span class="sxs-lookup"><span data-stu-id="032a6-133">UserId</span></span>|
|<span data-ttu-id="032a6-134">userName</span><span class="sxs-lookup"><span data-stu-id="032a6-134">userName</span></span>|<span data-ttu-id="032a6-135">String</span><span class="sxs-lookup"><span data-stu-id="032a6-135">String</span></span>|<span data-ttu-id="032a6-136">UserName</span><span class="sxs-lookup"><span data-stu-id="032a6-136">UserName</span></span>|
|<span data-ttu-id="032a6-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="032a6-137">userEmail</span></span>|<span data-ttu-id="032a6-138">String</span><span class="sxs-lookup"><span data-stu-id="032a6-138">String</span></span>|<span data-ttu-id="032a6-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="032a6-139">UserEmail</span></span>|
|<span data-ttu-id="032a6-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="032a6-140">userPrincipalName</span></span>|<span data-ttu-id="032a6-141">String</span><span class="sxs-lookup"><span data-stu-id="032a6-141">String</span></span>|<span data-ttu-id="032a6-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="032a6-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="032a6-143">sources</span><span class="sxs-lookup"><span data-stu-id="032a6-143">sources</span></span>|<span data-ttu-id="032a6-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="032a6-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="032a6-145">参与策略</span><span class="sxs-lookup"><span data-stu-id="032a6-145">Contributing policies</span></span>|
|<span data-ttu-id="032a6-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="032a6-146">currentValue</span></span>|<span data-ttu-id="032a6-147">String</span><span class="sxs-lookup"><span data-stu-id="032a6-147">String</span></span>|<span data-ttu-id="032a6-148">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="032a6-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="032a6-149">关系</span><span class="sxs-lookup"><span data-stu-id="032a6-149">Relationships</span></span>
<span data-ttu-id="032a6-150">无</span><span class="sxs-lookup"><span data-stu-id="032a6-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="032a6-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="032a6-151">JSON Representation</span></span>
<span data-ttu-id="032a6-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="032a6-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
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




