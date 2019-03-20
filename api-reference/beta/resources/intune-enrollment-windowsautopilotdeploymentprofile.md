---
title: windowsAutopilotDeploymentProfile 资源类型
description: Windows Autopilot 部署配置文件
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69035ba93b04ac66ce9e8883c7b5f7b04dff429a
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572458"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="5a91e-103">windowsAutopilotDeploymentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a91e-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="5a91e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5a91e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a91e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5a91e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a91e-106">Windows Autopilot 部署配置文件</span><span class="sxs-lookup"><span data-stu-id="5a91e-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="5a91e-107">方法</span><span class="sxs-lookup"><span data-stu-id="5a91e-107">Methods</span></span>
|<span data-ttu-id="5a91e-108">方法</span><span class="sxs-lookup"><span data-stu-id="5a91e-108">Method</span></span>|<span data-ttu-id="5a91e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5a91e-109">Return Type</span></span>|<span data-ttu-id="5a91e-110">说明</span><span class="sxs-lookup"><span data-stu-id="5a91e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5a91e-111">获取 windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="5a91e-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="5a91e-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="5a91e-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="5a91e-113">读取[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5a91e-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="5a91e-114">分配操作</span><span class="sxs-lookup"><span data-stu-id="5a91e-114">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="5a91e-115">无</span><span class="sxs-lookup"><span data-stu-id="5a91e-115">None</span></span>|<span data-ttu-id="5a91e-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5a91e-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5a91e-117">属性</span><span class="sxs-lookup"><span data-stu-id="5a91e-117">Properties</span></span>
|<span data-ttu-id="5a91e-118">属性</span><span class="sxs-lookup"><span data-stu-id="5a91e-118">Property</span></span>|<span data-ttu-id="5a91e-119">类型</span><span class="sxs-lookup"><span data-stu-id="5a91e-119">Type</span></span>|<span data-ttu-id="5a91e-120">说明</span><span class="sxs-lookup"><span data-stu-id="5a91e-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a91e-121">id</span><span class="sxs-lookup"><span data-stu-id="5a91e-121">id</span></span>|<span data-ttu-id="5a91e-122">String</span><span class="sxs-lookup"><span data-stu-id="5a91e-122">String</span></span>|<span data-ttu-id="5a91e-123">配置文件键</span><span class="sxs-lookup"><span data-stu-id="5a91e-123">Profile Key</span></span>|
|<span data-ttu-id="5a91e-124">displayName</span><span class="sxs-lookup"><span data-stu-id="5a91e-124">displayName</span></span>|<span data-ttu-id="5a91e-125">字符串</span><span class="sxs-lookup"><span data-stu-id="5a91e-125">String</span></span>|<span data-ttu-id="5a91e-126">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="5a91e-126">Name of the profile</span></span>|
|<span data-ttu-id="5a91e-127">说明</span><span class="sxs-lookup"><span data-stu-id="5a91e-127">description</span></span>|<span data-ttu-id="5a91e-128">字符串</span><span class="sxs-lookup"><span data-stu-id="5a91e-128">String</span></span>|<span data-ttu-id="5a91e-129">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="5a91e-129">Description of the profile</span></span>|
|<span data-ttu-id="5a91e-130">language</span><span class="sxs-lookup"><span data-stu-id="5a91e-130">language</span></span>|<span data-ttu-id="5a91e-131">String</span><span class="sxs-lookup"><span data-stu-id="5a91e-131">String</span></span>|<span data-ttu-id="5a91e-132">在设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="5a91e-132">Language configured on the device</span></span>|
|<span data-ttu-id="5a91e-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a91e-133">createdDateTime</span></span>|<span data-ttu-id="5a91e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a91e-134">DateTimeOffset</span></span>|<span data-ttu-id="5a91e-135">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="5a91e-135">Profile creation time</span></span>|
|<span data-ttu-id="5a91e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a91e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5a91e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a91e-137">DateTimeOffset</span></span>|<span data-ttu-id="5a91e-138">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="5a91e-138">Profile last modified time</span></span>|
|<span data-ttu-id="5a91e-139">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="5a91e-139">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="5a91e-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="5a91e-140">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="5a91e-141">"开箱即用体验" 设置</span><span class="sxs-lookup"><span data-stu-id="5a91e-141">Out of box experience setting</span></span>|
|<span data-ttu-id="5a91e-142">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="5a91e-142">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="5a91e-143">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="5a91e-143">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="5a91e-144">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="5a91e-144">Enrollment status screen setting</span></span>|
|<span data-ttu-id="5a91e-145">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="5a91e-145">extractHardwareHash</span></span>|<span data-ttu-id="5a91e-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a91e-146">Boolean</span></span>|<span data-ttu-id="5a91e-147">配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="5a91e-147">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="5a91e-148">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="5a91e-148">deviceNameTemplate</span></span>|<span data-ttu-id="5a91e-149">字符串</span><span class="sxs-lookup"><span data-stu-id="5a91e-149">String</span></span>|<span data-ttu-id="5a91e-150">用于命名 AutoPilot 设备的模板。</span><span class="sxs-lookup"><span data-stu-id="5a91e-150">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="5a91e-151">它可以是自定义文本, 也可以包含设备的序列号或随机生成的数字。</span><span class="sxs-lookup"><span data-stu-id="5a91e-151">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="5a91e-152">模板生成的文本的总长度不能超过15个字符。</span><span class="sxs-lookup"><span data-stu-id="5a91e-152">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="5a91e-153">deviceType</span><span class="sxs-lookup"><span data-stu-id="5a91e-153">deviceType</span></span>|[<span data-ttu-id="5a91e-154">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="5a91e-154">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="5a91e-155">此配置文件适用的 AutoPilot 设备类型。</span><span class="sxs-lookup"><span data-stu-id="5a91e-155">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="5a91e-156">可取值为：`windowsPc`、`surfaceHub2`。</span><span class="sxs-lookup"><span data-stu-id="5a91e-156">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="5a91e-157">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="5a91e-157">enableWhiteGlove</span></span>|<span data-ttu-id="5a91e-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a91e-158">Boolean</span></span>|<span data-ttu-id="5a91e-159">为配置文件启用 Autopilot 白色 Glove。</span><span class="sxs-lookup"><span data-stu-id="5a91e-159">Enable Autopilot White Glove for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a91e-160">关系</span><span class="sxs-lookup"><span data-stu-id="5a91e-160">Relationships</span></span>
|<span data-ttu-id="5a91e-161">关系</span><span class="sxs-lookup"><span data-stu-id="5a91e-161">Relationship</span></span>|<span data-ttu-id="5a91e-162">类型</span><span class="sxs-lookup"><span data-stu-id="5a91e-162">Type</span></span>|<span data-ttu-id="5a91e-163">说明</span><span class="sxs-lookup"><span data-stu-id="5a91e-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a91e-164">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="5a91e-164">assignedDevices</span></span>|<span data-ttu-id="5a91e-165">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="5a91e-165">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="5a91e-166">配置文件的已分配设备的列表。</span><span class="sxs-lookup"><span data-stu-id="5a91e-166">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="5a91e-167">assignments</span><span class="sxs-lookup"><span data-stu-id="5a91e-167">assignments</span></span>|<span data-ttu-id="5a91e-168">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="5a91e-168">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="5a91e-169">配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="5a91e-169">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a91e-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a91e-170">JSON Representation</span></span>
<span data-ttu-id="5a91e-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a91e-171">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "language": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "String",
    "deviceUsageType": "String",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "String",
    "installProgressTimeoutInMinutes": 1024,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "String",
  "deviceType": "String",
  "enableWhiteGlove": true
}
```




