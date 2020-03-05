---
title: deviceConfigurationSettingState 资源类型
description: 给定设备的设备配置设置状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6d5f75077fbfd29853b52adc6fc2d07b5c325905
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526630"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="9744a-103">deviceConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="9744a-103">deviceConfigurationSettingState resource type</span></span>

<span data-ttu-id="9744a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9744a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9744a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9744a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9744a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9744a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9744a-107">给定设备的设备配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="9744a-107">Device Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="9744a-108">属性</span><span class="sxs-lookup"><span data-stu-id="9744a-108">Properties</span></span>
|<span data-ttu-id="9744a-109">属性</span><span class="sxs-lookup"><span data-stu-id="9744a-109">Property</span></span>|<span data-ttu-id="9744a-110">类型</span><span class="sxs-lookup"><span data-stu-id="9744a-110">Type</span></span>|<span data-ttu-id="9744a-111">说明</span><span class="sxs-lookup"><span data-stu-id="9744a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9744a-112">setting</span><span class="sxs-lookup"><span data-stu-id="9744a-112">setting</span></span>|<span data-ttu-id="9744a-113">String</span><span class="sxs-lookup"><span data-stu-id="9744a-113">String</span></span>|<span data-ttu-id="9744a-114">报告的设置</span><span class="sxs-lookup"><span data-stu-id="9744a-114">The setting that is being reported</span></span>|
|<span data-ttu-id="9744a-115">settingName</span><span class="sxs-lookup"><span data-stu-id="9744a-115">settingName</span></span>|<span data-ttu-id="9744a-116">String</span><span class="sxs-lookup"><span data-stu-id="9744a-116">String</span></span>|<span data-ttu-id="9744a-117">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="9744a-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="9744a-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9744a-118">instanceDisplayName</span></span>|<span data-ttu-id="9744a-119">String</span><span class="sxs-lookup"><span data-stu-id="9744a-119">String</span></span>|<span data-ttu-id="9744a-120">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="9744a-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="9744a-121">state</span><span class="sxs-lookup"><span data-stu-id="9744a-121">state</span></span>|[<span data-ttu-id="9744a-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="9744a-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="9744a-123">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="9744a-123">The compliance state of the setting.</span></span> <span data-ttu-id="9744a-124">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="9744a-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="9744a-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="9744a-125">errorCode</span></span>|<span data-ttu-id="9744a-126">Int64</span><span class="sxs-lookup"><span data-stu-id="9744a-126">Int64</span></span>|<span data-ttu-id="9744a-127">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="9744a-127">Error code for the setting</span></span>|
|<span data-ttu-id="9744a-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="9744a-128">errorDescription</span></span>|<span data-ttu-id="9744a-129">String</span><span class="sxs-lookup"><span data-stu-id="9744a-129">String</span></span>|<span data-ttu-id="9744a-130">错误说明</span><span class="sxs-lookup"><span data-stu-id="9744a-130">Error description</span></span>|
|<span data-ttu-id="9744a-131">userId</span><span class="sxs-lookup"><span data-stu-id="9744a-131">userId</span></span>|<span data-ttu-id="9744a-132">String</span><span class="sxs-lookup"><span data-stu-id="9744a-132">String</span></span>|<span data-ttu-id="9744a-133">UserId</span><span class="sxs-lookup"><span data-stu-id="9744a-133">UserId</span></span>|
|<span data-ttu-id="9744a-134">userName</span><span class="sxs-lookup"><span data-stu-id="9744a-134">userName</span></span>|<span data-ttu-id="9744a-135">String</span><span class="sxs-lookup"><span data-stu-id="9744a-135">String</span></span>|<span data-ttu-id="9744a-136">UserName</span><span class="sxs-lookup"><span data-stu-id="9744a-136">UserName</span></span>|
|<span data-ttu-id="9744a-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="9744a-137">userEmail</span></span>|<span data-ttu-id="9744a-138">String</span><span class="sxs-lookup"><span data-stu-id="9744a-138">String</span></span>|<span data-ttu-id="9744a-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="9744a-139">UserEmail</span></span>|
|<span data-ttu-id="9744a-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9744a-140">userPrincipalName</span></span>|<span data-ttu-id="9744a-141">字符串</span><span class="sxs-lookup"><span data-stu-id="9744a-141">String</span></span>|<span data-ttu-id="9744a-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="9744a-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="9744a-143">源</span><span class="sxs-lookup"><span data-stu-id="9744a-143">sources</span></span>|<span data-ttu-id="9744a-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9744a-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="9744a-145">参与策略</span><span class="sxs-lookup"><span data-stu-id="9744a-145">Contributing policies</span></span>|
|<span data-ttu-id="9744a-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="9744a-146">currentValue</span></span>|<span data-ttu-id="9744a-147">String</span><span class="sxs-lookup"><span data-stu-id="9744a-147">String</span></span>|<span data-ttu-id="9744a-148">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="9744a-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="9744a-149">关系</span><span class="sxs-lookup"><span data-stu-id="9744a-149">Relationships</span></span>
<span data-ttu-id="9744a-150">无</span><span class="sxs-lookup"><span data-stu-id="9744a-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9744a-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9744a-151">JSON Representation</span></span>
<span data-ttu-id="9744a-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9744a-152">Here is a JSON representation of the resource.</span></span>
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



