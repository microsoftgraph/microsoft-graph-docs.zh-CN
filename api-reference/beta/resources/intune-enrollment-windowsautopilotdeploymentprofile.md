---
title: windowsAutopilotDeploymentProfile 资源类型
description: Windows Autopilot 部署配置文件
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f82d48422ecff99f106d4a62b07ac8532cb546c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794538"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="fbef9-103">windowsAutopilotDeploymentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="fbef9-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="fbef9-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fbef9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbef9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fbef9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbef9-106">Windows Autopilot 部署配置文件</span><span class="sxs-lookup"><span data-stu-id="fbef9-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="fbef9-107">方法</span><span class="sxs-lookup"><span data-stu-id="fbef9-107">Methods</span></span>
|<span data-ttu-id="fbef9-108">方法</span><span class="sxs-lookup"><span data-stu-id="fbef9-108">Method</span></span>|<span data-ttu-id="fbef9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="fbef9-109">Return Type</span></span>|<span data-ttu-id="fbef9-110">说明</span><span class="sxs-lookup"><span data-stu-id="fbef9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fbef9-111">获取 windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="fbef9-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="fbef9-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="fbef9-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="fbef9-113">读取[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fbef9-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="fbef9-114">分配操作</span><span class="sxs-lookup"><span data-stu-id="fbef9-114">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="fbef9-115">无</span><span class="sxs-lookup"><span data-stu-id="fbef9-115">None</span></span>|<span data-ttu-id="fbef9-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fbef9-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="fbef9-117">属性</span><span class="sxs-lookup"><span data-stu-id="fbef9-117">Properties</span></span>
|<span data-ttu-id="fbef9-118">属性</span><span class="sxs-lookup"><span data-stu-id="fbef9-118">Property</span></span>|<span data-ttu-id="fbef9-119">类型</span><span class="sxs-lookup"><span data-stu-id="fbef9-119">Type</span></span>|<span data-ttu-id="fbef9-120">说明</span><span class="sxs-lookup"><span data-stu-id="fbef9-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbef9-121">id</span><span class="sxs-lookup"><span data-stu-id="fbef9-121">id</span></span>|<span data-ttu-id="fbef9-122">String</span><span class="sxs-lookup"><span data-stu-id="fbef9-122">String</span></span>|<span data-ttu-id="fbef9-123">配置文件键</span><span class="sxs-lookup"><span data-stu-id="fbef9-123">Profile Key</span></span>|
|<span data-ttu-id="fbef9-124">displayName</span><span class="sxs-lookup"><span data-stu-id="fbef9-124">displayName</span></span>|<span data-ttu-id="fbef9-125">String</span><span class="sxs-lookup"><span data-stu-id="fbef9-125">String</span></span>|<span data-ttu-id="fbef9-126">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="fbef9-126">Name of the profile</span></span>|
|<span data-ttu-id="fbef9-127">description</span><span class="sxs-lookup"><span data-stu-id="fbef9-127">description</span></span>|<span data-ttu-id="fbef9-128">String</span><span class="sxs-lookup"><span data-stu-id="fbef9-128">String</span></span>|<span data-ttu-id="fbef9-129">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="fbef9-129">Description of the profile</span></span>|
|<span data-ttu-id="fbef9-130">language</span><span class="sxs-lookup"><span data-stu-id="fbef9-130">language</span></span>|<span data-ttu-id="fbef9-131">String</span><span class="sxs-lookup"><span data-stu-id="fbef9-131">String</span></span>|<span data-ttu-id="fbef9-132">在设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="fbef9-132">Language configured on the device</span></span>|
|<span data-ttu-id="fbef9-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbef9-133">createdDateTime</span></span>|<span data-ttu-id="fbef9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbef9-134">DateTimeOffset</span></span>|<span data-ttu-id="fbef9-135">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="fbef9-135">Profile creation time</span></span>|
|<span data-ttu-id="fbef9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbef9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fbef9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbef9-137">DateTimeOffset</span></span>|<span data-ttu-id="fbef9-138">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="fbef9-138">Profile last modified time</span></span>|
|<span data-ttu-id="fbef9-139">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="fbef9-139">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="fbef9-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="fbef9-140">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="fbef9-141">"开箱即用体验" 设置</span><span class="sxs-lookup"><span data-stu-id="fbef9-141">Out of box experience setting</span></span>|
|<span data-ttu-id="fbef9-142">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="fbef9-142">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="fbef9-143">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="fbef9-143">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="fbef9-144">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="fbef9-144">Enrollment status screen setting</span></span>|
|<span data-ttu-id="fbef9-145">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="fbef9-145">extractHardwareHash</span></span>|<span data-ttu-id="fbef9-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="fbef9-146">Boolean</span></span>|<span data-ttu-id="fbef9-147">配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="fbef9-147">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="fbef9-148">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="fbef9-148">deviceNameTemplate</span></span>|<span data-ttu-id="fbef9-149">String</span><span class="sxs-lookup"><span data-stu-id="fbef9-149">String</span></span>|<span data-ttu-id="fbef9-150">用于命名 AutoPilot 设备的模板。</span><span class="sxs-lookup"><span data-stu-id="fbef9-150">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="fbef9-151">它可以是自定义文本, 也可以包含设备的序列号或随机生成的数字。</span><span class="sxs-lookup"><span data-stu-id="fbef9-151">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="fbef9-152">模板生成的文本的总长度不能超过15个字符。</span><span class="sxs-lookup"><span data-stu-id="fbef9-152">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="fbef9-153">deviceType</span><span class="sxs-lookup"><span data-stu-id="fbef9-153">deviceType</span></span>|[<span data-ttu-id="fbef9-154">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="fbef9-154">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="fbef9-155">此配置文件适用的 AutoPilot 设备类型。</span><span class="sxs-lookup"><span data-stu-id="fbef9-155">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="fbef9-156">可取值为：`windowsPc`、`surfaceHub2`。</span><span class="sxs-lookup"><span data-stu-id="fbef9-156">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="fbef9-157">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="fbef9-157">enableWhiteGlove</span></span>|<span data-ttu-id="fbef9-158">布尔值</span><span class="sxs-lookup"><span data-stu-id="fbef9-158">Boolean</span></span>|<span data-ttu-id="fbef9-159">为配置文件启用 Autopilot 白色 Glove。</span><span class="sxs-lookup"><span data-stu-id="fbef9-159">Enable Autopilot White Glove for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbef9-160">关系</span><span class="sxs-lookup"><span data-stu-id="fbef9-160">Relationships</span></span>
|<span data-ttu-id="fbef9-161">关系</span><span class="sxs-lookup"><span data-stu-id="fbef9-161">Relationship</span></span>|<span data-ttu-id="fbef9-162">类型</span><span class="sxs-lookup"><span data-stu-id="fbef9-162">Type</span></span>|<span data-ttu-id="fbef9-163">说明</span><span class="sxs-lookup"><span data-stu-id="fbef9-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbef9-164">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="fbef9-164">assignedDevices</span></span>|<span data-ttu-id="fbef9-165">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="fbef9-165">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="fbef9-166">配置文件的已分配设备的列表。</span><span class="sxs-lookup"><span data-stu-id="fbef9-166">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="fbef9-167">assignments</span><span class="sxs-lookup"><span data-stu-id="fbef9-167">assignments</span></span>|<span data-ttu-id="fbef9-168">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="fbef9-168">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="fbef9-169">配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="fbef9-169">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fbef9-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fbef9-170">JSON Representation</span></span>
<span data-ttu-id="fbef9-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbef9-171">Here is a JSON representation of the resource.</span></span>
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





