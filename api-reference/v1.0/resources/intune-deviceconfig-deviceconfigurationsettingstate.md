---
title: deviceConfigurationSettingState 资源类型
description: 给定设备的设备配置设置状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c50ed17421b88f2cb6137458ff853bfa92796c2b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031666"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="82d78-103">deviceConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="82d78-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="82d78-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82d78-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82d78-105">给定设备的设备配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="82d78-105">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="82d78-106">属性</span><span class="sxs-lookup"><span data-stu-id="82d78-106">Properties</span></span>
|<span data-ttu-id="82d78-107">属性</span><span class="sxs-lookup"><span data-stu-id="82d78-107">Property</span></span>|<span data-ttu-id="82d78-108">类型</span><span class="sxs-lookup"><span data-stu-id="82d78-108">Type</span></span>|<span data-ttu-id="82d78-109">说明</span><span class="sxs-lookup"><span data-stu-id="82d78-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82d78-110">setting</span><span class="sxs-lookup"><span data-stu-id="82d78-110">setting</span></span>|<span data-ttu-id="82d78-111">String</span><span class="sxs-lookup"><span data-stu-id="82d78-111">String</span></span>|<span data-ttu-id="82d78-112">报告的设置</span><span class="sxs-lookup"><span data-stu-id="82d78-112">The setting that is being reported</span></span>|
|<span data-ttu-id="82d78-113">settingName</span><span class="sxs-lookup"><span data-stu-id="82d78-113">settingName</span></span>|<span data-ttu-id="82d78-114">String</span><span class="sxs-lookup"><span data-stu-id="82d78-114">String</span></span>|<span data-ttu-id="82d78-115">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="82d78-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="82d78-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="82d78-116">instanceDisplayName</span></span>|<span data-ttu-id="82d78-117">String</span><span class="sxs-lookup"><span data-stu-id="82d78-117">String</span></span>|<span data-ttu-id="82d78-118">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="82d78-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="82d78-119">state</span><span class="sxs-lookup"><span data-stu-id="82d78-119">state</span></span>|[<span data-ttu-id="82d78-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="82d78-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="82d78-121">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="82d78-121">The compliance state of the setting.</span></span> <span data-ttu-id="82d78-122">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="82d78-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="82d78-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="82d78-123">errorCode</span></span>|<span data-ttu-id="82d78-124">Int64</span><span class="sxs-lookup"><span data-stu-id="82d78-124">Int64</span></span>|<span data-ttu-id="82d78-125">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="82d78-125">Error code for the setting</span></span>|
|<span data-ttu-id="82d78-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="82d78-126">errorDescription</span></span>|<span data-ttu-id="82d78-127">String</span><span class="sxs-lookup"><span data-stu-id="82d78-127">String</span></span>|<span data-ttu-id="82d78-128">错误说明</span><span class="sxs-lookup"><span data-stu-id="82d78-128">Error description</span></span>|
|<span data-ttu-id="82d78-129">userId</span><span class="sxs-lookup"><span data-stu-id="82d78-129">userId</span></span>|<span data-ttu-id="82d78-130">String</span><span class="sxs-lookup"><span data-stu-id="82d78-130">String</span></span>|<span data-ttu-id="82d78-131">UserId</span><span class="sxs-lookup"><span data-stu-id="82d78-131">UserId</span></span>|
|<span data-ttu-id="82d78-132">userName</span><span class="sxs-lookup"><span data-stu-id="82d78-132">userName</span></span>|<span data-ttu-id="82d78-133">String</span><span class="sxs-lookup"><span data-stu-id="82d78-133">String</span></span>|<span data-ttu-id="82d78-134">UserName</span><span class="sxs-lookup"><span data-stu-id="82d78-134">UserName</span></span>|
|<span data-ttu-id="82d78-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="82d78-135">userEmail</span></span>|<span data-ttu-id="82d78-136">String</span><span class="sxs-lookup"><span data-stu-id="82d78-136">String</span></span>|<span data-ttu-id="82d78-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="82d78-137">UserEmail</span></span>|
|<span data-ttu-id="82d78-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="82d78-138">userPrincipalName</span></span>|<span data-ttu-id="82d78-139">字符串</span><span class="sxs-lookup"><span data-stu-id="82d78-139">String</span></span>|<span data-ttu-id="82d78-140">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="82d78-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="82d78-141">源</span><span class="sxs-lookup"><span data-stu-id="82d78-141">sources</span></span>|<span data-ttu-id="82d78-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82d78-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="82d78-143">参与策略</span><span class="sxs-lookup"><span data-stu-id="82d78-143">Contributing policies</span></span>|
|<span data-ttu-id="82d78-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="82d78-144">currentValue</span></span>|<span data-ttu-id="82d78-145">String</span><span class="sxs-lookup"><span data-stu-id="82d78-145">String</span></span>|<span data-ttu-id="82d78-146">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="82d78-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="82d78-147">关系</span><span class="sxs-lookup"><span data-stu-id="82d78-147">Relationships</span></span>
<span data-ttu-id="82d78-148">无</span><span class="sxs-lookup"><span data-stu-id="82d78-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82d78-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82d78-149">JSON Representation</span></span>
<span data-ttu-id="82d78-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82d78-150">Here is a JSON representation of the resource.</span></span>
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



