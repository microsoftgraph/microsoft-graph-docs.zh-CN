---
title: windowsAutopilotDeploymentProfile 资源类型
description: Windows Autopilot 部署配置文件
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 55703bc3b531a3671b70882a18f41522dd9a5c73
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327764"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="cc0b3-103">windowsAutopilotDeploymentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc0b3-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="cc0b3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cc0b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc0b3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc0b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc0b3-106">Windows Autopilot 部署配置文件</span><span class="sxs-lookup"><span data-stu-id="cc0b3-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="cc0b3-107">方法</span><span class="sxs-lookup"><span data-stu-id="cc0b3-107">Methods</span></span>
|<span data-ttu-id="cc0b3-108">方法</span><span class="sxs-lookup"><span data-stu-id="cc0b3-108">Method</span></span>|<span data-ttu-id="cc0b3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cc0b3-109">Return Type</span></span>|<span data-ttu-id="cc0b3-110">说明</span><span class="sxs-lookup"><span data-stu-id="cc0b3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cc0b3-111">获取 windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="cc0b3-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="cc0b3-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="cc0b3-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="cc0b3-113">读取[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc0b3-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="cc0b3-114">分配操作</span><span class="sxs-lookup"><span data-stu-id="cc0b3-114">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="cc0b3-115">无</span><span class="sxs-lookup"><span data-stu-id="cc0b3-115">None</span></span>|<span data-ttu-id="cc0b3-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cc0b3-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cc0b3-117">属性</span><span class="sxs-lookup"><span data-stu-id="cc0b3-117">Properties</span></span>
|<span data-ttu-id="cc0b3-118">属性</span><span class="sxs-lookup"><span data-stu-id="cc0b3-118">Property</span></span>|<span data-ttu-id="cc0b3-119">类型</span><span class="sxs-lookup"><span data-stu-id="cc0b3-119">Type</span></span>|<span data-ttu-id="cc0b3-120">说明</span><span class="sxs-lookup"><span data-stu-id="cc0b3-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc0b3-121">id</span><span class="sxs-lookup"><span data-stu-id="cc0b3-121">id</span></span>|<span data-ttu-id="cc0b3-122">字符串</span><span class="sxs-lookup"><span data-stu-id="cc0b3-122">String</span></span>|<span data-ttu-id="cc0b3-123">配置文件键</span><span class="sxs-lookup"><span data-stu-id="cc0b3-123">Profile Key</span></span>|
|<span data-ttu-id="cc0b3-124">displayName</span><span class="sxs-lookup"><span data-stu-id="cc0b3-124">displayName</span></span>|<span data-ttu-id="cc0b3-125">字符串</span><span class="sxs-lookup"><span data-stu-id="cc0b3-125">String</span></span>|<span data-ttu-id="cc0b3-126">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="cc0b3-126">Name of the profile</span></span>|
|<span data-ttu-id="cc0b3-127">说明</span><span class="sxs-lookup"><span data-stu-id="cc0b3-127">description</span></span>|<span data-ttu-id="cc0b3-128">String</span><span class="sxs-lookup"><span data-stu-id="cc0b3-128">String</span></span>|<span data-ttu-id="cc0b3-129">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="cc0b3-129">Description of the profile</span></span>|
|<span data-ttu-id="cc0b3-130">language</span><span class="sxs-lookup"><span data-stu-id="cc0b3-130">language</span></span>|<span data-ttu-id="cc0b3-131">String</span><span class="sxs-lookup"><span data-stu-id="cc0b3-131">String</span></span>|<span data-ttu-id="cc0b3-132">在设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="cc0b3-132">Language configured on the device</span></span>|
|<span data-ttu-id="cc0b3-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc0b3-133">createdDateTime</span></span>|<span data-ttu-id="cc0b3-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc0b3-134">DateTimeOffset</span></span>|<span data-ttu-id="cc0b3-135">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="cc0b3-135">Profile creation time</span></span>|
|<span data-ttu-id="cc0b3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc0b3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="cc0b3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc0b3-137">DateTimeOffset</span></span>|<span data-ttu-id="cc0b3-138">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="cc0b3-138">Profile last modified time</span></span>|
|<span data-ttu-id="cc0b3-139">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="cc0b3-139">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="cc0b3-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="cc0b3-140">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="cc0b3-141">"开箱即用体验" 设置</span><span class="sxs-lookup"><span data-stu-id="cc0b3-141">Out of box experience setting</span></span>|
|<span data-ttu-id="cc0b3-142">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="cc0b3-142">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="cc0b3-143">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="cc0b3-143">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="cc0b3-144">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="cc0b3-144">Enrollment status screen setting</span></span>|
|<span data-ttu-id="cc0b3-145">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="cc0b3-145">extractHardwareHash</span></span>|<span data-ttu-id="cc0b3-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc0b3-146">Boolean</span></span>|<span data-ttu-id="cc0b3-147">配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="cc0b3-147">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="cc0b3-148">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="cc0b3-148">deviceNameTemplate</span></span>|<span data-ttu-id="cc0b3-149">String</span><span class="sxs-lookup"><span data-stu-id="cc0b3-149">String</span></span>|<span data-ttu-id="cc0b3-150">用于命名 AutoPilot 设备的模板。</span><span class="sxs-lookup"><span data-stu-id="cc0b3-150">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="cc0b3-151">它可以是自定义文本, 也可以包含设备的序列号或随机生成的数字。</span><span class="sxs-lookup"><span data-stu-id="cc0b3-151">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="cc0b3-152">模板生成的文本的总长度不能超过15个字符。</span><span class="sxs-lookup"><span data-stu-id="cc0b3-152">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="cc0b3-153">deviceType</span><span class="sxs-lookup"><span data-stu-id="cc0b3-153">deviceType</span></span>|[<span data-ttu-id="cc0b3-154">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="cc0b3-154">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="cc0b3-155">此配置文件适用的 AutoPilot 设备类型。</span><span class="sxs-lookup"><span data-stu-id="cc0b3-155">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="cc0b3-156">可取值为：`windowsPc`、`surfaceHub2`。</span><span class="sxs-lookup"><span data-stu-id="cc0b3-156">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="cc0b3-157">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="cc0b3-157">enableWhiteGlove</span></span>|<span data-ttu-id="cc0b3-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc0b3-158">Boolean</span></span>|<span data-ttu-id="cc0b3-159">为配置文件启用 Autopilot 白色 Glove。</span><span class="sxs-lookup"><span data-stu-id="cc0b3-159">Enable Autopilot White Glove for the profile.</span></span>|
|<span data-ttu-id="cc0b3-160">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cc0b3-160">roleScopeTagIds</span></span>|<span data-ttu-id="cc0b3-161">String collection</span><span class="sxs-lookup"><span data-stu-id="cc0b3-161">String collection</span></span>|<span data-ttu-id="cc0b3-162">配置文件的范围标记。</span><span class="sxs-lookup"><span data-stu-id="cc0b3-162">Scope tags for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc0b3-163">关系</span><span class="sxs-lookup"><span data-stu-id="cc0b3-163">Relationships</span></span>
|<span data-ttu-id="cc0b3-164">关系</span><span class="sxs-lookup"><span data-stu-id="cc0b3-164">Relationship</span></span>|<span data-ttu-id="cc0b3-165">类型</span><span class="sxs-lookup"><span data-stu-id="cc0b3-165">Type</span></span>|<span data-ttu-id="cc0b3-166">说明</span><span class="sxs-lookup"><span data-stu-id="cc0b3-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc0b3-167">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="cc0b3-167">assignedDevices</span></span>|<span data-ttu-id="cc0b3-168">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="cc0b3-168">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="cc0b3-169">配置文件的已分配设备的列表。</span><span class="sxs-lookup"><span data-stu-id="cc0b3-169">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="cc0b3-170">assignments</span><span class="sxs-lookup"><span data-stu-id="cc0b3-170">assignments</span></span>|<span data-ttu-id="cc0b3-171">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="cc0b3-171">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="cc0b3-172">配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="cc0b3-172">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cc0b3-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc0b3-173">JSON Representation</span></span>
<span data-ttu-id="cc0b3-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc0b3-174">Here is a JSON representation of the resource.</span></span>
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
  "enableWhiteGlove": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```



