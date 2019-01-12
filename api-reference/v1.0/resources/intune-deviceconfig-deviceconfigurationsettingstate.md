---
title: deviceConfigurationSettingState 资源类型
description: 给定设备的设备配置设置状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 68c57b8842136494bf0604a31f62992f7a1c2501
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928008"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="4ea5a-103">deviceConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ea5a-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="4ea5a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4ea5a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ea5a-105">给定设备的设备配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="4ea5a-105">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="4ea5a-106">属性</span><span class="sxs-lookup"><span data-stu-id="4ea5a-106">Properties</span></span>
|<span data-ttu-id="4ea5a-107">属性</span><span class="sxs-lookup"><span data-stu-id="4ea5a-107">Property</span></span>|<span data-ttu-id="4ea5a-108">类型</span><span class="sxs-lookup"><span data-stu-id="4ea5a-108">Type</span></span>|<span data-ttu-id="4ea5a-109">说明</span><span class="sxs-lookup"><span data-stu-id="4ea5a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ea5a-110">setting</span><span class="sxs-lookup"><span data-stu-id="4ea5a-110">setting</span></span>|<span data-ttu-id="4ea5a-111">String</span><span class="sxs-lookup"><span data-stu-id="4ea5a-111">String</span></span>|<span data-ttu-id="4ea5a-112">报告的设置</span><span class="sxs-lookup"><span data-stu-id="4ea5a-112">The setting that is being reported</span></span>|
|<span data-ttu-id="4ea5a-113">settingName</span><span class="sxs-lookup"><span data-stu-id="4ea5a-113">settingName</span></span>|<span data-ttu-id="4ea5a-114">String</span><span class="sxs-lookup"><span data-stu-id="4ea5a-114">String</span></span>|<span data-ttu-id="4ea5a-115">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="4ea5a-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="4ea5a-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4ea5a-116">instanceDisplayName</span></span>|<span data-ttu-id="4ea5a-117">String</span><span class="sxs-lookup"><span data-stu-id="4ea5a-117">String</span></span>|<span data-ttu-id="4ea5a-118">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="4ea5a-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="4ea5a-119">state</span><span class="sxs-lookup"><span data-stu-id="4ea5a-119">state</span></span>|[<span data-ttu-id="4ea5a-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4ea5a-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4ea5a-121">设置合规性状态。</span><span class="sxs-lookup"><span data-stu-id="4ea5a-121">The compliance state of the setting.</span></span> <span data-ttu-id="4ea5a-122">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="4ea5a-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4ea5a-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="4ea5a-123">errorCode</span></span>|<span data-ttu-id="4ea5a-124">Int64</span><span class="sxs-lookup"><span data-stu-id="4ea5a-124">Int64</span></span>|<span data-ttu-id="4ea5a-125">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="4ea5a-125">Error code for the setting</span></span>|
|<span data-ttu-id="4ea5a-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="4ea5a-126">errorDescription</span></span>|<span data-ttu-id="4ea5a-127">String</span><span class="sxs-lookup"><span data-stu-id="4ea5a-127">String</span></span>|<span data-ttu-id="4ea5a-128">错误说明</span><span class="sxs-lookup"><span data-stu-id="4ea5a-128">Error description</span></span>|
|<span data-ttu-id="4ea5a-129">userId</span><span class="sxs-lookup"><span data-stu-id="4ea5a-129">userId</span></span>|<span data-ttu-id="4ea5a-130">String</span><span class="sxs-lookup"><span data-stu-id="4ea5a-130">String</span></span>|<span data-ttu-id="4ea5a-131">UserId</span><span class="sxs-lookup"><span data-stu-id="4ea5a-131">UserId</span></span>|
|<span data-ttu-id="4ea5a-132">userName</span><span class="sxs-lookup"><span data-stu-id="4ea5a-132">userName</span></span>|<span data-ttu-id="4ea5a-133">String</span><span class="sxs-lookup"><span data-stu-id="4ea5a-133">String</span></span>|<span data-ttu-id="4ea5a-134">UserName</span><span class="sxs-lookup"><span data-stu-id="4ea5a-134">UserName</span></span>|
|<span data-ttu-id="4ea5a-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="4ea5a-135">userEmail</span></span>|<span data-ttu-id="4ea5a-136">String</span><span class="sxs-lookup"><span data-stu-id="4ea5a-136">String</span></span>|<span data-ttu-id="4ea5a-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="4ea5a-137">UserEmail</span></span>|
|<span data-ttu-id="4ea5a-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4ea5a-138">userPrincipalName</span></span>|<span data-ttu-id="4ea5a-139">String</span><span class="sxs-lookup"><span data-stu-id="4ea5a-139">String</span></span>|<span data-ttu-id="4ea5a-140">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="4ea5a-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="4ea5a-141">sources</span><span class="sxs-lookup"><span data-stu-id="4ea5a-141">sources</span></span>|<span data-ttu-id="4ea5a-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4ea5a-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="4ea5a-143">参与策略</span><span class="sxs-lookup"><span data-stu-id="4ea5a-143">Contributing policies</span></span>|
|<span data-ttu-id="4ea5a-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="4ea5a-144">currentValue</span></span>|<span data-ttu-id="4ea5a-145">String</span><span class="sxs-lookup"><span data-stu-id="4ea5a-145">String</span></span>|<span data-ttu-id="4ea5a-146">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="4ea5a-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ea5a-147">关系</span><span class="sxs-lookup"><span data-stu-id="4ea5a-147">Relationships</span></span>
<span data-ttu-id="4ea5a-148">无</span><span class="sxs-lookup"><span data-stu-id="4ea5a-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4ea5a-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ea5a-149">JSON Representation</span></span>
<span data-ttu-id="4ea5a-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ea5a-150">Here is a JSON representation of the resource.</span></span>
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



