---
title: windowsAutopilotDeploymentProfile 资源类型
description: Windows Autopilot 部署配置文件
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f82d48422ecff99f106d4a62b07ac8532cb546c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546995"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="c91e0-103">windowsAutopilotDeploymentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="c91e0-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="c91e0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c91e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c91e0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c91e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c91e0-106">Windows Autopilot 部署配置文件</span><span class="sxs-lookup"><span data-stu-id="c91e0-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="c91e0-107">方法</span><span class="sxs-lookup"><span data-stu-id="c91e0-107">Methods</span></span>
|<span data-ttu-id="c91e0-108">方法</span><span class="sxs-lookup"><span data-stu-id="c91e0-108">Method</span></span>|<span data-ttu-id="c91e0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c91e0-109">Return Type</span></span>|<span data-ttu-id="c91e0-110">说明</span><span class="sxs-lookup"><span data-stu-id="c91e0-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c91e0-111">获取 windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="c91e0-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="c91e0-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="c91e0-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="c91e0-113">读取[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c91e0-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="c91e0-114">分配操作</span><span class="sxs-lookup"><span data-stu-id="c91e0-114">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="c91e0-115">无</span><span class="sxs-lookup"><span data-stu-id="c91e0-115">None</span></span>|<span data-ttu-id="c91e0-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c91e0-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c91e0-117">属性</span><span class="sxs-lookup"><span data-stu-id="c91e0-117">Properties</span></span>
|<span data-ttu-id="c91e0-118">属性</span><span class="sxs-lookup"><span data-stu-id="c91e0-118">Property</span></span>|<span data-ttu-id="c91e0-119">类型</span><span class="sxs-lookup"><span data-stu-id="c91e0-119">Type</span></span>|<span data-ttu-id="c91e0-120">说明</span><span class="sxs-lookup"><span data-stu-id="c91e0-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c91e0-121">id</span><span class="sxs-lookup"><span data-stu-id="c91e0-121">id</span></span>|<span data-ttu-id="c91e0-122">字符串</span><span class="sxs-lookup"><span data-stu-id="c91e0-122">String</span></span>|<span data-ttu-id="c91e0-123">配置文件键</span><span class="sxs-lookup"><span data-stu-id="c91e0-123">Profile Key</span></span>|
|<span data-ttu-id="c91e0-124">displayName</span><span class="sxs-lookup"><span data-stu-id="c91e0-124">displayName</span></span>|<span data-ttu-id="c91e0-125">字符串</span><span class="sxs-lookup"><span data-stu-id="c91e0-125">String</span></span>|<span data-ttu-id="c91e0-126">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="c91e0-126">Name of the profile</span></span>|
|<span data-ttu-id="c91e0-127">description</span><span class="sxs-lookup"><span data-stu-id="c91e0-127">description</span></span>|<span data-ttu-id="c91e0-128">String</span><span class="sxs-lookup"><span data-stu-id="c91e0-128">String</span></span>|<span data-ttu-id="c91e0-129">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="c91e0-129">Description of the profile</span></span>|
|<span data-ttu-id="c91e0-130">language</span><span class="sxs-lookup"><span data-stu-id="c91e0-130">language</span></span>|<span data-ttu-id="c91e0-131">String</span><span class="sxs-lookup"><span data-stu-id="c91e0-131">String</span></span>|<span data-ttu-id="c91e0-132">在设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="c91e0-132">Language configured on the device</span></span>|
|<span data-ttu-id="c91e0-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c91e0-133">createdDateTime</span></span>|<span data-ttu-id="c91e0-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c91e0-134">DateTimeOffset</span></span>|<span data-ttu-id="c91e0-135">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="c91e0-135">Profile creation time</span></span>|
|<span data-ttu-id="c91e0-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c91e0-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c91e0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c91e0-137">DateTimeOffset</span></span>|<span data-ttu-id="c91e0-138">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="c91e0-138">Profile last modified time</span></span>|
|<span data-ttu-id="c91e0-139">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="c91e0-139">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="c91e0-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="c91e0-140">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="c91e0-141">"开箱即用体验" 设置</span><span class="sxs-lookup"><span data-stu-id="c91e0-141">Out of box experience setting</span></span>|
|<span data-ttu-id="c91e0-142">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="c91e0-142">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="c91e0-143">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="c91e0-143">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="c91e0-144">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="c91e0-144">Enrollment status screen setting</span></span>|
|<span data-ttu-id="c91e0-145">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="c91e0-145">extractHardwareHash</span></span>|<span data-ttu-id="c91e0-146">布尔值</span><span class="sxs-lookup"><span data-stu-id="c91e0-146">Boolean</span></span>|<span data-ttu-id="c91e0-147">配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="c91e0-147">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="c91e0-148">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="c91e0-148">deviceNameTemplate</span></span>|<span data-ttu-id="c91e0-149">String</span><span class="sxs-lookup"><span data-stu-id="c91e0-149">String</span></span>|<span data-ttu-id="c91e0-150">用于命名 AutoPilot 设备的模板。</span><span class="sxs-lookup"><span data-stu-id="c91e0-150">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="c91e0-151">它可以是自定义文本, 也可以包含设备的序列号或随机生成的数字。</span><span class="sxs-lookup"><span data-stu-id="c91e0-151">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="c91e0-152">模板生成的文本的总长度不能超过15个字符。</span><span class="sxs-lookup"><span data-stu-id="c91e0-152">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="c91e0-153">deviceType</span><span class="sxs-lookup"><span data-stu-id="c91e0-153">deviceType</span></span>|[<span data-ttu-id="c91e0-154">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="c91e0-154">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="c91e0-155">此配置文件适用的 AutoPilot 设备类型。</span><span class="sxs-lookup"><span data-stu-id="c91e0-155">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="c91e0-156">可取值为：`windowsPc`、`surfaceHub2`。</span><span class="sxs-lookup"><span data-stu-id="c91e0-156">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="c91e0-157">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="c91e0-157">enableWhiteGlove</span></span>|<span data-ttu-id="c91e0-158">布尔值</span><span class="sxs-lookup"><span data-stu-id="c91e0-158">Boolean</span></span>|<span data-ttu-id="c91e0-159">为配置文件启用 Autopilot 白色 Glove。</span><span class="sxs-lookup"><span data-stu-id="c91e0-159">Enable Autopilot White Glove for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c91e0-160">关系</span><span class="sxs-lookup"><span data-stu-id="c91e0-160">Relationships</span></span>
|<span data-ttu-id="c91e0-161">关系</span><span class="sxs-lookup"><span data-stu-id="c91e0-161">Relationship</span></span>|<span data-ttu-id="c91e0-162">类型</span><span class="sxs-lookup"><span data-stu-id="c91e0-162">Type</span></span>|<span data-ttu-id="c91e0-163">说明</span><span class="sxs-lookup"><span data-stu-id="c91e0-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c91e0-164">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="c91e0-164">assignedDevices</span></span>|<span data-ttu-id="c91e0-165">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="c91e0-165">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="c91e0-166">配置文件的已分配设备的列表。</span><span class="sxs-lookup"><span data-stu-id="c91e0-166">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="c91e0-167">assignments</span><span class="sxs-lookup"><span data-stu-id="c91e0-167">assignments</span></span>|<span data-ttu-id="c91e0-168">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c91e0-168">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="c91e0-169">配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="c91e0-169">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c91e0-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c91e0-170">JSON Representation</span></span>
<span data-ttu-id="c91e0-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c91e0-171">Here is a JSON representation of the resource.</span></span>
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





