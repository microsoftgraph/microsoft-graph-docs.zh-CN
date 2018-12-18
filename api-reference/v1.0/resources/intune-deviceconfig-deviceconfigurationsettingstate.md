---
title: deviceConfigurationSettingState 资源类型
description: 给定设备的设备配置设置状态。
author: tfitzmac
ms.openlocfilehash: 545cb9bf0be410a5e9a0e25dbc242399c6dbc61f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320641"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="f1458-103">deviceConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1458-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="f1458-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f1458-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1458-105">给定设备的设备配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="f1458-105">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="f1458-106">属性</span><span class="sxs-lookup"><span data-stu-id="f1458-106">Properties</span></span>
|<span data-ttu-id="f1458-107">属性</span><span class="sxs-lookup"><span data-stu-id="f1458-107">Property</span></span>|<span data-ttu-id="f1458-108">类型</span><span class="sxs-lookup"><span data-stu-id="f1458-108">Type</span></span>|<span data-ttu-id="f1458-109">说明</span><span class="sxs-lookup"><span data-stu-id="f1458-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1458-110">setting</span><span class="sxs-lookup"><span data-stu-id="f1458-110">setting</span></span>|<span data-ttu-id="f1458-111">String</span><span class="sxs-lookup"><span data-stu-id="f1458-111">String</span></span>|<span data-ttu-id="f1458-112">报告的设置</span><span class="sxs-lookup"><span data-stu-id="f1458-112">The setting that is being reported</span></span>|
|<span data-ttu-id="f1458-113">settingName</span><span class="sxs-lookup"><span data-stu-id="f1458-113">settingName</span></span>|<span data-ttu-id="f1458-114">String</span><span class="sxs-lookup"><span data-stu-id="f1458-114">String</span></span>|<span data-ttu-id="f1458-115">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="f1458-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="f1458-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1458-116">instanceDisplayName</span></span>|<span data-ttu-id="f1458-117">String</span><span class="sxs-lookup"><span data-stu-id="f1458-117">String</span></span>|<span data-ttu-id="f1458-118">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="f1458-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="f1458-119">state</span><span class="sxs-lookup"><span data-stu-id="f1458-119">state</span></span>|[<span data-ttu-id="f1458-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f1458-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f1458-121">设置合规性状态。</span><span class="sxs-lookup"><span data-stu-id="f1458-121">The compliance state of the setting.</span></span> <span data-ttu-id="f1458-122">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="f1458-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f1458-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="f1458-123">errorCode</span></span>|<span data-ttu-id="f1458-124">Int64</span><span class="sxs-lookup"><span data-stu-id="f1458-124">Int64</span></span>|<span data-ttu-id="f1458-125">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="f1458-125">Error code for the setting</span></span>|
|<span data-ttu-id="f1458-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="f1458-126">errorDescription</span></span>|<span data-ttu-id="f1458-127">String</span><span class="sxs-lookup"><span data-stu-id="f1458-127">String</span></span>|<span data-ttu-id="f1458-128">错误说明</span><span class="sxs-lookup"><span data-stu-id="f1458-128">Error description</span></span>|
|<span data-ttu-id="f1458-129">userId</span><span class="sxs-lookup"><span data-stu-id="f1458-129">userId</span></span>|<span data-ttu-id="f1458-130">String</span><span class="sxs-lookup"><span data-stu-id="f1458-130">String</span></span>|<span data-ttu-id="f1458-131">UserId</span><span class="sxs-lookup"><span data-stu-id="f1458-131">UserId</span></span>|
|<span data-ttu-id="f1458-132">userName</span><span class="sxs-lookup"><span data-stu-id="f1458-132">userName</span></span>|<span data-ttu-id="f1458-133">String</span><span class="sxs-lookup"><span data-stu-id="f1458-133">String</span></span>|<span data-ttu-id="f1458-134">UserName</span><span class="sxs-lookup"><span data-stu-id="f1458-134">UserName</span></span>|
|<span data-ttu-id="f1458-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="f1458-135">userEmail</span></span>|<span data-ttu-id="f1458-136">String</span><span class="sxs-lookup"><span data-stu-id="f1458-136">String</span></span>|<span data-ttu-id="f1458-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="f1458-137">UserEmail</span></span>|
|<span data-ttu-id="f1458-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f1458-138">userPrincipalName</span></span>|<span data-ttu-id="f1458-139">String</span><span class="sxs-lookup"><span data-stu-id="f1458-139">String</span></span>|<span data-ttu-id="f1458-140">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="f1458-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="f1458-141">sources</span><span class="sxs-lookup"><span data-stu-id="f1458-141">sources</span></span>|<span data-ttu-id="f1458-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f1458-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="f1458-143">参与策略</span><span class="sxs-lookup"><span data-stu-id="f1458-143">Contributing policies</span></span>|
|<span data-ttu-id="f1458-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="f1458-144">currentValue</span></span>|<span data-ttu-id="f1458-145">String</span><span class="sxs-lookup"><span data-stu-id="f1458-145">String</span></span>|<span data-ttu-id="f1458-146">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="f1458-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1458-147">关系</span><span class="sxs-lookup"><span data-stu-id="f1458-147">Relationships</span></span>
<span data-ttu-id="f1458-148">无</span><span class="sxs-lookup"><span data-stu-id="f1458-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f1458-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1458-149">JSON Representation</span></span>
<span data-ttu-id="f1458-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1458-150">Here is a JSON representation of the resource.</span></span>
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



