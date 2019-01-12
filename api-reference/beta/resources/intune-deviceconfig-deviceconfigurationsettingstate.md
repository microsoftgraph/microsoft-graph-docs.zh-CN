---
title: deviceConfigurationSettingState 资源类型
description: 给定设备的设备配置设置状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 59eff07d2f609b69f5e5971e407733e0dbfc2577
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982167"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="63980-103">deviceConfigurationSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="63980-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="63980-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="63980-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63980-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="63980-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63980-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="63980-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63980-107">给定设备的设备配置设置状态。</span><span class="sxs-lookup"><span data-stu-id="63980-107">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="63980-108">属性</span><span class="sxs-lookup"><span data-stu-id="63980-108">Properties</span></span>
|<span data-ttu-id="63980-109">属性</span><span class="sxs-lookup"><span data-stu-id="63980-109">Property</span></span>|<span data-ttu-id="63980-110">类型</span><span class="sxs-lookup"><span data-stu-id="63980-110">Type</span></span>|<span data-ttu-id="63980-111">说明</span><span class="sxs-lookup"><span data-stu-id="63980-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63980-112">setting</span><span class="sxs-lookup"><span data-stu-id="63980-112">setting</span></span>|<span data-ttu-id="63980-113">String</span><span class="sxs-lookup"><span data-stu-id="63980-113">String</span></span>|<span data-ttu-id="63980-114">报告的设置</span><span class="sxs-lookup"><span data-stu-id="63980-114">The setting that is being reported</span></span>|
|<span data-ttu-id="63980-115">settingName</span><span class="sxs-lookup"><span data-stu-id="63980-115">settingName</span></span>|<span data-ttu-id="63980-116">String</span><span class="sxs-lookup"><span data-stu-id="63980-116">String</span></span>|<span data-ttu-id="63980-117">报告的本地化/用户友好设置名称</span><span class="sxs-lookup"><span data-stu-id="63980-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="63980-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="63980-118">instanceDisplayName</span></span>|<span data-ttu-id="63980-119">String</span><span class="sxs-lookup"><span data-stu-id="63980-119">String</span></span>|<span data-ttu-id="63980-120">报告的设置实例的名称。</span><span class="sxs-lookup"><span data-stu-id="63980-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="63980-121">state</span><span class="sxs-lookup"><span data-stu-id="63980-121">state</span></span>|[<span data-ttu-id="63980-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="63980-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="63980-123">设置合规性状态。</span><span class="sxs-lookup"><span data-stu-id="63980-123">The compliance state of the setting.</span></span> <span data-ttu-id="63980-124">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="63980-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="63980-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="63980-125">errorCode</span></span>|<span data-ttu-id="63980-126">Int64</span><span class="sxs-lookup"><span data-stu-id="63980-126">Int64</span></span>|<span data-ttu-id="63980-127">设置的错误代码</span><span class="sxs-lookup"><span data-stu-id="63980-127">Error code for the setting</span></span>|
|<span data-ttu-id="63980-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="63980-128">errorDescription</span></span>|<span data-ttu-id="63980-129">String</span><span class="sxs-lookup"><span data-stu-id="63980-129">String</span></span>|<span data-ttu-id="63980-130">错误说明</span><span class="sxs-lookup"><span data-stu-id="63980-130">Error description</span></span>|
|<span data-ttu-id="63980-131">userId</span><span class="sxs-lookup"><span data-stu-id="63980-131">userId</span></span>|<span data-ttu-id="63980-132">String</span><span class="sxs-lookup"><span data-stu-id="63980-132">String</span></span>|<span data-ttu-id="63980-133">UserId</span><span class="sxs-lookup"><span data-stu-id="63980-133">UserId</span></span>|
|<span data-ttu-id="63980-134">userName</span><span class="sxs-lookup"><span data-stu-id="63980-134">userName</span></span>|<span data-ttu-id="63980-135">String</span><span class="sxs-lookup"><span data-stu-id="63980-135">String</span></span>|<span data-ttu-id="63980-136">UserName</span><span class="sxs-lookup"><span data-stu-id="63980-136">UserName</span></span>|
|<span data-ttu-id="63980-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="63980-137">userEmail</span></span>|<span data-ttu-id="63980-138">String</span><span class="sxs-lookup"><span data-stu-id="63980-138">String</span></span>|<span data-ttu-id="63980-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="63980-139">UserEmail</span></span>|
|<span data-ttu-id="63980-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="63980-140">userPrincipalName</span></span>|<span data-ttu-id="63980-141">String</span><span class="sxs-lookup"><span data-stu-id="63980-141">String</span></span>|<span data-ttu-id="63980-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="63980-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="63980-143">sources</span><span class="sxs-lookup"><span data-stu-id="63980-143">sources</span></span>|<span data-ttu-id="63980-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="63980-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="63980-145">参与策略</span><span class="sxs-lookup"><span data-stu-id="63980-145">Contributing policies</span></span>|
|<span data-ttu-id="63980-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="63980-146">currentValue</span></span>|<span data-ttu-id="63980-147">String</span><span class="sxs-lookup"><span data-stu-id="63980-147">String</span></span>|<span data-ttu-id="63980-148">设备上设置的当前值</span><span class="sxs-lookup"><span data-stu-id="63980-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="63980-149">关系</span><span class="sxs-lookup"><span data-stu-id="63980-149">Relationships</span></span>
<span data-ttu-id="63980-150">无</span><span class="sxs-lookup"><span data-stu-id="63980-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="63980-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63980-151">JSON Representation</span></span>
<span data-ttu-id="63980-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63980-152">Here is a JSON representation of the resource.</span></span>
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





