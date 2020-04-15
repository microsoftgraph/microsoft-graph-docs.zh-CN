---
title: deviceConfigurationSettingState 资源类型
description: 给定设备的设备配置设置状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4b613ae365d0842079485171b41c7d37580a66b4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445976"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="ab5eb-103">deviceConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab5eb-103">deviceConfigurationSettingState resource type</span></span>

<span data-ttu-id="ab5eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab5eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab5eb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab5eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab5eb-106">给定设备的设备配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="ab5eb-106">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="ab5eb-107">属性</span><span class="sxs-lookup"><span data-stu-id="ab5eb-107">Properties</span></span>
|<span data-ttu-id="ab5eb-108">属性</span><span class="sxs-lookup"><span data-stu-id="ab5eb-108">Property</span></span>|<span data-ttu-id="ab5eb-109">类型</span><span class="sxs-lookup"><span data-stu-id="ab5eb-109">Type</span></span>|<span data-ttu-id="ab5eb-110">说明</span><span class="sxs-lookup"><span data-stu-id="ab5eb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab5eb-111">setting</span><span class="sxs-lookup"><span data-stu-id="ab5eb-111">setting</span></span>|<span data-ttu-id="ab5eb-112">String</span><span class="sxs-lookup"><span data-stu-id="ab5eb-112">String</span></span>|<span data-ttu-id="ab5eb-113">报告的设置</span><span class="sxs-lookup"><span data-stu-id="ab5eb-113">The setting that is being reported</span></span>|
|<span data-ttu-id="ab5eb-114">settingName</span><span class="sxs-lookup"><span data-stu-id="ab5eb-114">settingName</span></span>|<span data-ttu-id="ab5eb-115">String</span><span class="sxs-lookup"><span data-stu-id="ab5eb-115">String</span></span>|<span data-ttu-id="ab5eb-116">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="ab5eb-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="ab5eb-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ab5eb-117">instanceDisplayName</span></span>|<span data-ttu-id="ab5eb-118">String</span><span class="sxs-lookup"><span data-stu-id="ab5eb-118">String</span></span>|<span data-ttu-id="ab5eb-119">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="ab5eb-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="ab5eb-120">state</span><span class="sxs-lookup"><span data-stu-id="ab5eb-120">state</span></span>|[<span data-ttu-id="ab5eb-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="ab5eb-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="ab5eb-122">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="ab5eb-122">The compliance state of the setting.</span></span> <span data-ttu-id="ab5eb-123">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="ab5eb-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="ab5eb-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="ab5eb-124">errorCode</span></span>|<span data-ttu-id="ab5eb-125">Int64</span><span class="sxs-lookup"><span data-stu-id="ab5eb-125">Int64</span></span>|<span data-ttu-id="ab5eb-126">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="ab5eb-126">Error code for the setting</span></span>|
|<span data-ttu-id="ab5eb-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="ab5eb-127">errorDescription</span></span>|<span data-ttu-id="ab5eb-128">String</span><span class="sxs-lookup"><span data-stu-id="ab5eb-128">String</span></span>|<span data-ttu-id="ab5eb-129">错误说明</span><span class="sxs-lookup"><span data-stu-id="ab5eb-129">Error description</span></span>|
|<span data-ttu-id="ab5eb-130">userId</span><span class="sxs-lookup"><span data-stu-id="ab5eb-130">userId</span></span>|<span data-ttu-id="ab5eb-131">String</span><span class="sxs-lookup"><span data-stu-id="ab5eb-131">String</span></span>|<span data-ttu-id="ab5eb-132">UserId</span><span class="sxs-lookup"><span data-stu-id="ab5eb-132">UserId</span></span>|
|<span data-ttu-id="ab5eb-133">userName</span><span class="sxs-lookup"><span data-stu-id="ab5eb-133">userName</span></span>|<span data-ttu-id="ab5eb-134">String</span><span class="sxs-lookup"><span data-stu-id="ab5eb-134">String</span></span>|<span data-ttu-id="ab5eb-135">UserName</span><span class="sxs-lookup"><span data-stu-id="ab5eb-135">UserName</span></span>|
|<span data-ttu-id="ab5eb-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="ab5eb-136">userEmail</span></span>|<span data-ttu-id="ab5eb-137">String</span><span class="sxs-lookup"><span data-stu-id="ab5eb-137">String</span></span>|<span data-ttu-id="ab5eb-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="ab5eb-138">UserEmail</span></span>|
|<span data-ttu-id="ab5eb-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ab5eb-139">userPrincipalName</span></span>|<span data-ttu-id="ab5eb-140">字符串</span><span class="sxs-lookup"><span data-stu-id="ab5eb-140">String</span></span>|<span data-ttu-id="ab5eb-141">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="ab5eb-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="ab5eb-142">源</span><span class="sxs-lookup"><span data-stu-id="ab5eb-142">sources</span></span>|<span data-ttu-id="ab5eb-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab5eb-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="ab5eb-144">参与策略</span><span class="sxs-lookup"><span data-stu-id="ab5eb-144">Contributing policies</span></span>|
|<span data-ttu-id="ab5eb-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="ab5eb-145">currentValue</span></span>|<span data-ttu-id="ab5eb-146">String</span><span class="sxs-lookup"><span data-stu-id="ab5eb-146">String</span></span>|<span data-ttu-id="ab5eb-147">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="ab5eb-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab5eb-148">关系</span><span class="sxs-lookup"><span data-stu-id="ab5eb-148">Relationships</span></span>
<span data-ttu-id="ab5eb-149">无</span><span class="sxs-lookup"><span data-stu-id="ab5eb-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab5eb-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab5eb-150">JSON Representation</span></span>
<span data-ttu-id="ab5eb-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab5eb-151">Here is a JSON representation of the resource.</span></span>
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







