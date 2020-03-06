---
title: deviceConfigurationSettingState 资源类型
description: 给定设备的设备配置设置状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aafa0147bac2acfcaa1f77291be1451c907b2f72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530771"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="d391c-103">deviceConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="d391c-103">deviceConfigurationSettingState resource type</span></span>

<span data-ttu-id="d391c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d391c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d391c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d391c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d391c-106">给定设备的设备配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="d391c-106">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="d391c-107">属性</span><span class="sxs-lookup"><span data-stu-id="d391c-107">Properties</span></span>
|<span data-ttu-id="d391c-108">属性</span><span class="sxs-lookup"><span data-stu-id="d391c-108">Property</span></span>|<span data-ttu-id="d391c-109">类型</span><span class="sxs-lookup"><span data-stu-id="d391c-109">Type</span></span>|<span data-ttu-id="d391c-110">说明</span><span class="sxs-lookup"><span data-stu-id="d391c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d391c-111">setting</span><span class="sxs-lookup"><span data-stu-id="d391c-111">setting</span></span>|<span data-ttu-id="d391c-112">字符串</span><span class="sxs-lookup"><span data-stu-id="d391c-112">String</span></span>|<span data-ttu-id="d391c-113">报告的设置</span><span class="sxs-lookup"><span data-stu-id="d391c-113">The setting that is being reported</span></span>|
|<span data-ttu-id="d391c-114">settingName</span><span class="sxs-lookup"><span data-stu-id="d391c-114">settingName</span></span>|<span data-ttu-id="d391c-115">字符串</span><span class="sxs-lookup"><span data-stu-id="d391c-115">String</span></span>|<span data-ttu-id="d391c-116">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="d391c-116">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="d391c-117">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d391c-117">instanceDisplayName</span></span>|<span data-ttu-id="d391c-118">字符串</span><span class="sxs-lookup"><span data-stu-id="d391c-118">String</span></span>|<span data-ttu-id="d391c-119">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="d391c-119">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="d391c-120">state</span><span class="sxs-lookup"><span data-stu-id="d391c-120">state</span></span>|[<span data-ttu-id="d391c-121">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d391c-121">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d391c-122">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="d391c-122">The compliance state of the setting.</span></span> <span data-ttu-id="d391c-123">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="d391c-123">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d391c-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="d391c-124">errorCode</span></span>|<span data-ttu-id="d391c-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d391c-125">Int64</span></span>|<span data-ttu-id="d391c-126">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="d391c-126">Error code for the setting</span></span>|
|<span data-ttu-id="d391c-127">errorDescription</span><span class="sxs-lookup"><span data-stu-id="d391c-127">errorDescription</span></span>|<span data-ttu-id="d391c-128">字符串</span><span class="sxs-lookup"><span data-stu-id="d391c-128">String</span></span>|<span data-ttu-id="d391c-129">错误说明</span><span class="sxs-lookup"><span data-stu-id="d391c-129">Error description</span></span>|
|<span data-ttu-id="d391c-130">userId</span><span class="sxs-lookup"><span data-stu-id="d391c-130">userId</span></span>|<span data-ttu-id="d391c-131">String</span><span class="sxs-lookup"><span data-stu-id="d391c-131">String</span></span>|<span data-ttu-id="d391c-132">UserId</span><span class="sxs-lookup"><span data-stu-id="d391c-132">UserId</span></span>|
|<span data-ttu-id="d391c-133">userName</span><span class="sxs-lookup"><span data-stu-id="d391c-133">userName</span></span>|<span data-ttu-id="d391c-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d391c-134">String</span></span>|<span data-ttu-id="d391c-135">UserName</span><span class="sxs-lookup"><span data-stu-id="d391c-135">UserName</span></span>|
|<span data-ttu-id="d391c-136">userEmail</span><span class="sxs-lookup"><span data-stu-id="d391c-136">userEmail</span></span>|<span data-ttu-id="d391c-137">字符串</span><span class="sxs-lookup"><span data-stu-id="d391c-137">String</span></span>|<span data-ttu-id="d391c-138">UserEmail</span><span class="sxs-lookup"><span data-stu-id="d391c-138">UserEmail</span></span>|
|<span data-ttu-id="d391c-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d391c-139">userPrincipalName</span></span>|<span data-ttu-id="d391c-140">字符串</span><span class="sxs-lookup"><span data-stu-id="d391c-140">String</span></span>|<span data-ttu-id="d391c-141">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="d391c-141">UserPrincipalName.</span></span>|
|<span data-ttu-id="d391c-142">源</span><span class="sxs-lookup"><span data-stu-id="d391c-142">sources</span></span>|<span data-ttu-id="d391c-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d391c-143">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="d391c-144">参与策略</span><span class="sxs-lookup"><span data-stu-id="d391c-144">Contributing policies</span></span>|
|<span data-ttu-id="d391c-145">currentValue</span><span class="sxs-lookup"><span data-stu-id="d391c-145">currentValue</span></span>|<span data-ttu-id="d391c-146">String</span><span class="sxs-lookup"><span data-stu-id="d391c-146">String</span></span>|<span data-ttu-id="d391c-147">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="d391c-147">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="d391c-148">关系</span><span class="sxs-lookup"><span data-stu-id="d391c-148">Relationships</span></span>
<span data-ttu-id="d391c-149">无</span><span class="sxs-lookup"><span data-stu-id="d391c-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d391c-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d391c-150">JSON Representation</span></span>
<span data-ttu-id="d391c-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d391c-151">Here is a JSON representation of the resource.</span></span>
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




