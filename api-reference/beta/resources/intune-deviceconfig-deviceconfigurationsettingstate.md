---
title: deviceConfigurationSettingState 资源类型
description: 给定设备的设备配置设置状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 596fd1d59e99a2023055ec92843474a46ae20fb6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016364"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="d3021-103">deviceConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3021-103">deviceConfigurationSettingState resource type</span></span>

<span data-ttu-id="d3021-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3021-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3021-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3021-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3021-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3021-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3021-107">给定设备的设备配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="d3021-107">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="d3021-108">属性</span><span class="sxs-lookup"><span data-stu-id="d3021-108">Properties</span></span>
|<span data-ttu-id="d3021-109">属性</span><span class="sxs-lookup"><span data-stu-id="d3021-109">Property</span></span>|<span data-ttu-id="d3021-110">类型</span><span class="sxs-lookup"><span data-stu-id="d3021-110">Type</span></span>|<span data-ttu-id="d3021-111">说明</span><span class="sxs-lookup"><span data-stu-id="d3021-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3021-112">setting</span><span class="sxs-lookup"><span data-stu-id="d3021-112">setting</span></span>|<span data-ttu-id="d3021-113">String</span><span class="sxs-lookup"><span data-stu-id="d3021-113">String</span></span>|<span data-ttu-id="d3021-114">报告的设置</span><span class="sxs-lookup"><span data-stu-id="d3021-114">The setting that is being reported</span></span>|
|<span data-ttu-id="d3021-115">settingName</span><span class="sxs-lookup"><span data-stu-id="d3021-115">settingName</span></span>|<span data-ttu-id="d3021-116">String</span><span class="sxs-lookup"><span data-stu-id="d3021-116">String</span></span>|<span data-ttu-id="d3021-117">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="d3021-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="d3021-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d3021-118">instanceDisplayName</span></span>|<span data-ttu-id="d3021-119">String</span><span class="sxs-lookup"><span data-stu-id="d3021-119">String</span></span>|<span data-ttu-id="d3021-120">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="d3021-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="d3021-121">state</span><span class="sxs-lookup"><span data-stu-id="d3021-121">state</span></span>|[<span data-ttu-id="d3021-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d3021-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d3021-123">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="d3021-123">The compliance state of the setting.</span></span> <span data-ttu-id="d3021-124">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="d3021-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d3021-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="d3021-125">errorCode</span></span>|<span data-ttu-id="d3021-126">Int64</span><span class="sxs-lookup"><span data-stu-id="d3021-126">Int64</span></span>|<span data-ttu-id="d3021-127">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="d3021-127">Error code for the setting</span></span>|
|<span data-ttu-id="d3021-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="d3021-128">errorDescription</span></span>|<span data-ttu-id="d3021-129">String</span><span class="sxs-lookup"><span data-stu-id="d3021-129">String</span></span>|<span data-ttu-id="d3021-130">错误说明</span><span class="sxs-lookup"><span data-stu-id="d3021-130">Error description</span></span>|
|<span data-ttu-id="d3021-131">userId</span><span class="sxs-lookup"><span data-stu-id="d3021-131">userId</span></span>|<span data-ttu-id="d3021-132">String</span><span class="sxs-lookup"><span data-stu-id="d3021-132">String</span></span>|<span data-ttu-id="d3021-133">UserId</span><span class="sxs-lookup"><span data-stu-id="d3021-133">UserId</span></span>|
|<span data-ttu-id="d3021-134">userName</span><span class="sxs-lookup"><span data-stu-id="d3021-134">userName</span></span>|<span data-ttu-id="d3021-135">String</span><span class="sxs-lookup"><span data-stu-id="d3021-135">String</span></span>|<span data-ttu-id="d3021-136">UserName</span><span class="sxs-lookup"><span data-stu-id="d3021-136">UserName</span></span>|
|<span data-ttu-id="d3021-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="d3021-137">userEmail</span></span>|<span data-ttu-id="d3021-138">String</span><span class="sxs-lookup"><span data-stu-id="d3021-138">String</span></span>|<span data-ttu-id="d3021-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="d3021-139">UserEmail</span></span>|
|<span data-ttu-id="d3021-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d3021-140">userPrincipalName</span></span>|<span data-ttu-id="d3021-141">String</span><span class="sxs-lookup"><span data-stu-id="d3021-141">String</span></span>|<span data-ttu-id="d3021-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="d3021-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="d3021-143">源</span><span class="sxs-lookup"><span data-stu-id="d3021-143">sources</span></span>|<span data-ttu-id="d3021-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3021-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="d3021-145">参与策略</span><span class="sxs-lookup"><span data-stu-id="d3021-145">Contributing policies</span></span>|
|<span data-ttu-id="d3021-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="d3021-146">currentValue</span></span>|<span data-ttu-id="d3021-147">String</span><span class="sxs-lookup"><span data-stu-id="d3021-147">String</span></span>|<span data-ttu-id="d3021-148">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="d3021-148">Current value of setting on device</span></span>|
|<span data-ttu-id="d3021-149">settingInstanceId</span><span class="sxs-lookup"><span data-stu-id="d3021-149">settingInstanceId</span></span>|<span data-ttu-id="d3021-150">String</span><span class="sxs-lookup"><span data-stu-id="d3021-150">String</span></span>|<span data-ttu-id="d3021-151">SettingInstanceId</span><span class="sxs-lookup"><span data-stu-id="d3021-151">SettingInstanceId</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3021-152">关系</span><span class="sxs-lookup"><span data-stu-id="d3021-152">Relationships</span></span>
<span data-ttu-id="d3021-153">无</span><span class="sxs-lookup"><span data-stu-id="d3021-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3021-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3021-154">JSON Representation</span></span>
<span data-ttu-id="d3021-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3021-155">Here is a JSON representation of the resource.</span></span>
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
      "displayName": "String",
      "sourceType": "String"
    }
  ],
  "currentValue": "String",
  "settingInstanceId": "String"
}
```






