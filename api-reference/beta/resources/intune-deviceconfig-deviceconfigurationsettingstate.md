---
title: deviceConfigurationSettingState 资源类型
description: 给定设备的设备配置设置状态。
author: tfitzmac
ms.openlocfilehash: 7ca50fe6a6186578739b166b1239a309824d1e51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316112"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="6f3ad-103">deviceConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f3ad-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="6f3ad-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6f3ad-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f3ad-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6f3ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f3ad-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6f3ad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f3ad-107">给定设备的设备配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="6f3ad-107">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="6f3ad-108">属性</span><span class="sxs-lookup"><span data-stu-id="6f3ad-108">Properties</span></span>
|<span data-ttu-id="6f3ad-109">属性</span><span class="sxs-lookup"><span data-stu-id="6f3ad-109">Property</span></span>|<span data-ttu-id="6f3ad-110">类型</span><span class="sxs-lookup"><span data-stu-id="6f3ad-110">Type</span></span>|<span data-ttu-id="6f3ad-111">说明</span><span class="sxs-lookup"><span data-stu-id="6f3ad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f3ad-112">setting</span><span class="sxs-lookup"><span data-stu-id="6f3ad-112">setting</span></span>|<span data-ttu-id="6f3ad-113">String</span><span class="sxs-lookup"><span data-stu-id="6f3ad-113">String</span></span>|<span data-ttu-id="6f3ad-114">报告的设置</span><span class="sxs-lookup"><span data-stu-id="6f3ad-114">The setting that is being reported</span></span>|
|<span data-ttu-id="6f3ad-115">settingName</span><span class="sxs-lookup"><span data-stu-id="6f3ad-115">settingName</span></span>|<span data-ttu-id="6f3ad-116">String</span><span class="sxs-lookup"><span data-stu-id="6f3ad-116">String</span></span>|<span data-ttu-id="6f3ad-117">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="6f3ad-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="6f3ad-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6f3ad-118">instanceDisplayName</span></span>|<span data-ttu-id="6f3ad-119">String</span><span class="sxs-lookup"><span data-stu-id="6f3ad-119">String</span></span>|<span data-ttu-id="6f3ad-120">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="6f3ad-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="6f3ad-121">state</span><span class="sxs-lookup"><span data-stu-id="6f3ad-121">state</span></span>|[<span data-ttu-id="6f3ad-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="6f3ad-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="6f3ad-123">设置合规性状态。</span><span class="sxs-lookup"><span data-stu-id="6f3ad-123">The compliance state of the setting.</span></span> <span data-ttu-id="6f3ad-124">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="6f3ad-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6f3ad-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="6f3ad-125">errorCode</span></span>|<span data-ttu-id="6f3ad-126">Int64</span><span class="sxs-lookup"><span data-stu-id="6f3ad-126">Int64</span></span>|<span data-ttu-id="6f3ad-127">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="6f3ad-127">Error code for the setting</span></span>|
|<span data-ttu-id="6f3ad-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="6f3ad-128">errorDescription</span></span>|<span data-ttu-id="6f3ad-129">String</span><span class="sxs-lookup"><span data-stu-id="6f3ad-129">String</span></span>|<span data-ttu-id="6f3ad-130">错误说明</span><span class="sxs-lookup"><span data-stu-id="6f3ad-130">Error description</span></span>|
|<span data-ttu-id="6f3ad-131">userId</span><span class="sxs-lookup"><span data-stu-id="6f3ad-131">userId</span></span>|<span data-ttu-id="6f3ad-132">String</span><span class="sxs-lookup"><span data-stu-id="6f3ad-132">String</span></span>|<span data-ttu-id="6f3ad-133">UserId</span><span class="sxs-lookup"><span data-stu-id="6f3ad-133">UserId</span></span>|
|<span data-ttu-id="6f3ad-134">userName</span><span class="sxs-lookup"><span data-stu-id="6f3ad-134">userName</span></span>|<span data-ttu-id="6f3ad-135">String</span><span class="sxs-lookup"><span data-stu-id="6f3ad-135">String</span></span>|<span data-ttu-id="6f3ad-136">UserName</span><span class="sxs-lookup"><span data-stu-id="6f3ad-136">UserName</span></span>|
|<span data-ttu-id="6f3ad-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="6f3ad-137">userEmail</span></span>|<span data-ttu-id="6f3ad-138">String</span><span class="sxs-lookup"><span data-stu-id="6f3ad-138">String</span></span>|<span data-ttu-id="6f3ad-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="6f3ad-139">UserEmail</span></span>|
|<span data-ttu-id="6f3ad-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6f3ad-140">userPrincipalName</span></span>|<span data-ttu-id="6f3ad-141">String</span><span class="sxs-lookup"><span data-stu-id="6f3ad-141">String</span></span>|<span data-ttu-id="6f3ad-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="6f3ad-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="6f3ad-143">sources</span><span class="sxs-lookup"><span data-stu-id="6f3ad-143">sources</span></span>|<span data-ttu-id="6f3ad-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6f3ad-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="6f3ad-145">参与策略</span><span class="sxs-lookup"><span data-stu-id="6f3ad-145">Contributing policies</span></span>|
|<span data-ttu-id="6f3ad-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="6f3ad-146">currentValue</span></span>|<span data-ttu-id="6f3ad-147">String</span><span class="sxs-lookup"><span data-stu-id="6f3ad-147">String</span></span>|<span data-ttu-id="6f3ad-148">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="6f3ad-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f3ad-149">关系</span><span class="sxs-lookup"><span data-stu-id="6f3ad-149">Relationships</span></span>
<span data-ttu-id="6f3ad-150">无</span><span class="sxs-lookup"><span data-stu-id="6f3ad-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6f3ad-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f3ad-151">JSON Representation</span></span>
<span data-ttu-id="6f3ad-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f3ad-152">Here is a JSON representation of the resource.</span></span>
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





