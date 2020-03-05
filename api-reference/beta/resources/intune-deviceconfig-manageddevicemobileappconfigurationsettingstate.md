---
title: managedDeviceMobileAppConfigurationSettingState 资源类型
description: 给定设备的托管设备移动应用配置设置状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4b044565f0ec87570bbf9584b37217c0f4881839
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529651"
---
# <a name="manageddevicemobileappconfigurationsettingstate-resource-type"></a><span data-ttu-id="f4dfa-103">managedDeviceMobileAppConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4dfa-103">managedDeviceMobileAppConfigurationSettingState resource type</span></span>

<span data-ttu-id="f4dfa-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f4dfa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4dfa-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4dfa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4dfa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4dfa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4dfa-107">给定设备的托管设备移动应用配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="f4dfa-107">Managed Device Mobile App Configuration Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="f4dfa-108">属性</span><span class="sxs-lookup"><span data-stu-id="f4dfa-108">Properties</span></span>
|<span data-ttu-id="f4dfa-109">属性</span><span class="sxs-lookup"><span data-stu-id="f4dfa-109">Property</span></span>|<span data-ttu-id="f4dfa-110">类型</span><span class="sxs-lookup"><span data-stu-id="f4dfa-110">Type</span></span>|<span data-ttu-id="f4dfa-111">说明</span><span class="sxs-lookup"><span data-stu-id="f4dfa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4dfa-112">setting</span><span class="sxs-lookup"><span data-stu-id="f4dfa-112">setting</span></span>|<span data-ttu-id="f4dfa-113">String</span><span class="sxs-lookup"><span data-stu-id="f4dfa-113">String</span></span>|<span data-ttu-id="f4dfa-114">报告的设置</span><span class="sxs-lookup"><span data-stu-id="f4dfa-114">The setting that is being reported</span></span>|
|<span data-ttu-id="f4dfa-115">settingName</span><span class="sxs-lookup"><span data-stu-id="f4dfa-115">settingName</span></span>|<span data-ttu-id="f4dfa-116">String</span><span class="sxs-lookup"><span data-stu-id="f4dfa-116">String</span></span>|<span data-ttu-id="f4dfa-117">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="f4dfa-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="f4dfa-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f4dfa-118">instanceDisplayName</span></span>|<span data-ttu-id="f4dfa-119">String</span><span class="sxs-lookup"><span data-stu-id="f4dfa-119">String</span></span>|<span data-ttu-id="f4dfa-120">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="f4dfa-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="f4dfa-121">state</span><span class="sxs-lookup"><span data-stu-id="f4dfa-121">state</span></span>|[<span data-ttu-id="f4dfa-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f4dfa-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f4dfa-123">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="f4dfa-123">The compliance state of the setting.</span></span> <span data-ttu-id="f4dfa-124">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="f4dfa-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f4dfa-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="f4dfa-125">errorCode</span></span>|<span data-ttu-id="f4dfa-126">Int64</span><span class="sxs-lookup"><span data-stu-id="f4dfa-126">Int64</span></span>|<span data-ttu-id="f4dfa-127">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="f4dfa-127">Error code for the setting</span></span>|
|<span data-ttu-id="f4dfa-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="f4dfa-128">errorDescription</span></span>|<span data-ttu-id="f4dfa-129">String</span><span class="sxs-lookup"><span data-stu-id="f4dfa-129">String</span></span>|<span data-ttu-id="f4dfa-130">错误说明</span><span class="sxs-lookup"><span data-stu-id="f4dfa-130">Error description</span></span>|
|<span data-ttu-id="f4dfa-131">userId</span><span class="sxs-lookup"><span data-stu-id="f4dfa-131">userId</span></span>|<span data-ttu-id="f4dfa-132">String</span><span class="sxs-lookup"><span data-stu-id="f4dfa-132">String</span></span>|<span data-ttu-id="f4dfa-133">UserId</span><span class="sxs-lookup"><span data-stu-id="f4dfa-133">UserId</span></span>|
|<span data-ttu-id="f4dfa-134">userName</span><span class="sxs-lookup"><span data-stu-id="f4dfa-134">userName</span></span>|<span data-ttu-id="f4dfa-135">String</span><span class="sxs-lookup"><span data-stu-id="f4dfa-135">String</span></span>|<span data-ttu-id="f4dfa-136">UserName</span><span class="sxs-lookup"><span data-stu-id="f4dfa-136">UserName</span></span>|
|<span data-ttu-id="f4dfa-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="f4dfa-137">userEmail</span></span>|<span data-ttu-id="f4dfa-138">String</span><span class="sxs-lookup"><span data-stu-id="f4dfa-138">String</span></span>|<span data-ttu-id="f4dfa-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="f4dfa-139">UserEmail</span></span>|
|<span data-ttu-id="f4dfa-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f4dfa-140">userPrincipalName</span></span>|<span data-ttu-id="f4dfa-141">字符串</span><span class="sxs-lookup"><span data-stu-id="f4dfa-141">String</span></span>|<span data-ttu-id="f4dfa-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="f4dfa-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="f4dfa-143">源</span><span class="sxs-lookup"><span data-stu-id="f4dfa-143">sources</span></span>|<span data-ttu-id="f4dfa-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4dfa-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="f4dfa-145">参与策略</span><span class="sxs-lookup"><span data-stu-id="f4dfa-145">Contributing policies</span></span>|
|<span data-ttu-id="f4dfa-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="f4dfa-146">currentValue</span></span>|<span data-ttu-id="f4dfa-147">String</span><span class="sxs-lookup"><span data-stu-id="f4dfa-147">String</span></span>|<span data-ttu-id="f4dfa-148">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="f4dfa-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4dfa-149">关系</span><span class="sxs-lookup"><span data-stu-id="f4dfa-149">Relationships</span></span>
<span data-ttu-id="f4dfa-150">无</span><span class="sxs-lookup"><span data-stu-id="f4dfa-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4dfa-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4dfa-151">JSON Representation</span></span>
<span data-ttu-id="f4dfa-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4dfa-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationSettingState",
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



