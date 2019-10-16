---
title: windowsAutopilotDeploymentProfile 资源类型
description: Windows Autopilot 部署配置文件
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1eec544e946b35433e2dca8f6521ff0e7df38c22
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538677"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="a3608-103">windowsAutopilotDeploymentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3608-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="a3608-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a3608-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3608-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3608-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3608-106">Windows Autopilot 部署配置文件</span><span class="sxs-lookup"><span data-stu-id="a3608-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="a3608-107">方法</span><span class="sxs-lookup"><span data-stu-id="a3608-107">Methods</span></span>
|<span data-ttu-id="a3608-108">方法</span><span class="sxs-lookup"><span data-stu-id="a3608-108">Method</span></span>|<span data-ttu-id="a3608-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a3608-109">Return Type</span></span>|<span data-ttu-id="a3608-110">说明</span><span class="sxs-lookup"><span data-stu-id="a3608-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a3608-111">获取 windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="a3608-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-shared-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="a3608-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="a3608-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="a3608-113">读取[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a3608-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="a3608-114">分配操作</span><span class="sxs-lookup"><span data-stu-id="a3608-114">assign action</span></span>](../api/intune-shared-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="a3608-115">无</span><span class="sxs-lookup"><span data-stu-id="a3608-115">None</span></span>|<span data-ttu-id="a3608-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a3608-116">Not yet documented</span></span>|
|<span data-ttu-id="a3608-117">**策略集**</span><span class="sxs-lookup"><span data-stu-id="a3608-117">**Policy Set**</span></span>|
|[<span data-ttu-id="a3608-118">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="a3608-118">hasPayloadLinks action</span></span>](../api/intune-shared-windowsautopilotdeploymentprofile-haspayloadlinks.md)|<span data-ttu-id="a3608-119">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="a3608-119">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="a3608-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a3608-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a3608-121">属性</span><span class="sxs-lookup"><span data-stu-id="a3608-121">Properties</span></span>
|<span data-ttu-id="a3608-122">属性</span><span class="sxs-lookup"><span data-stu-id="a3608-122">Property</span></span>|<span data-ttu-id="a3608-123">类型</span><span class="sxs-lookup"><span data-stu-id="a3608-123">Type</span></span>|<span data-ttu-id="a3608-124">说明</span><span class="sxs-lookup"><span data-stu-id="a3608-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3608-125">id</span><span class="sxs-lookup"><span data-stu-id="a3608-125">id</span></span>|<span data-ttu-id="a3608-126">字符串</span><span class="sxs-lookup"><span data-stu-id="a3608-126">String</span></span>|<span data-ttu-id="a3608-127">配置文件键</span><span class="sxs-lookup"><span data-stu-id="a3608-127">Profile Key</span></span>|
|<span data-ttu-id="a3608-128">displayName</span><span class="sxs-lookup"><span data-stu-id="a3608-128">displayName</span></span>|<span data-ttu-id="a3608-129">字符串</span><span class="sxs-lookup"><span data-stu-id="a3608-129">String</span></span>|<span data-ttu-id="a3608-130">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="a3608-130">Name of the profile</span></span>|
|<span data-ttu-id="a3608-131">说明</span><span class="sxs-lookup"><span data-stu-id="a3608-131">description</span></span>|<span data-ttu-id="a3608-132">String</span><span class="sxs-lookup"><span data-stu-id="a3608-132">String</span></span>|<span data-ttu-id="a3608-133">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="a3608-133">Description of the profile</span></span>|
|<span data-ttu-id="a3608-134">language</span><span class="sxs-lookup"><span data-stu-id="a3608-134">language</span></span>|<span data-ttu-id="a3608-135">String</span><span class="sxs-lookup"><span data-stu-id="a3608-135">String</span></span>|<span data-ttu-id="a3608-136">在设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="a3608-136">Language configured on the device</span></span>|
|<span data-ttu-id="a3608-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3608-137">createdDateTime</span></span>|<span data-ttu-id="a3608-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3608-138">DateTimeOffset</span></span>|<span data-ttu-id="a3608-139">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="a3608-139">Profile creation time</span></span>|
|<span data-ttu-id="a3608-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3608-140">lastModifiedDateTime</span></span>|<span data-ttu-id="a3608-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3608-141">DateTimeOffset</span></span>|<span data-ttu-id="a3608-142">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="a3608-142">Profile last modified time</span></span>|
|<span data-ttu-id="a3608-143">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="a3608-143">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="a3608-144">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="a3608-144">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="a3608-145">"开箱即用体验" 设置</span><span class="sxs-lookup"><span data-stu-id="a3608-145">Out of box experience setting</span></span>|
|<span data-ttu-id="a3608-146">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="a3608-146">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="a3608-147">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="a3608-147">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="a3608-148">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="a3608-148">Enrollment status screen setting</span></span>|
|<span data-ttu-id="a3608-149">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="a3608-149">extractHardwareHash</span></span>|<span data-ttu-id="a3608-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3608-150">Boolean</span></span>|<span data-ttu-id="a3608-151">配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="a3608-151">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="a3608-152">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="a3608-152">deviceNameTemplate</span></span>|<span data-ttu-id="a3608-153">字符串</span><span class="sxs-lookup"><span data-stu-id="a3608-153">String</span></span>|<span data-ttu-id="a3608-154">用于命名 AutoPilot 设备的模板。</span><span class="sxs-lookup"><span data-stu-id="a3608-154">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="a3608-155">它可以是自定义文本，也可以包含设备的序列号或随机生成的数字。</span><span class="sxs-lookup"><span data-stu-id="a3608-155">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="a3608-156">模板生成的文本的总长度不能超过15个字符。</span><span class="sxs-lookup"><span data-stu-id="a3608-156">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="a3608-157">deviceType</span><span class="sxs-lookup"><span data-stu-id="a3608-157">deviceType</span></span>|[<span data-ttu-id="a3608-158">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="a3608-158">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="a3608-159">此配置文件适用的 AutoPilot 设备类型。</span><span class="sxs-lookup"><span data-stu-id="a3608-159">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="a3608-160">可取值为：`windowsPc`、`surfaceHub2`。</span><span class="sxs-lookup"><span data-stu-id="a3608-160">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="a3608-161">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="a3608-161">enableWhiteGlove</span></span>|<span data-ttu-id="a3608-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a3608-162">Boolean</span></span>|<span data-ttu-id="a3608-163">为配置文件启用 Autopilot 白色 Glove。</span><span class="sxs-lookup"><span data-stu-id="a3608-163">Enable Autopilot White Glove for the profile.</span></span>|
|<span data-ttu-id="a3608-164">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a3608-164">roleScopeTagIds</span></span>|<span data-ttu-id="a3608-165">String 集合</span><span class="sxs-lookup"><span data-stu-id="a3608-165">String collection</span></span>|<span data-ttu-id="a3608-166">配置文件的范围标记。</span><span class="sxs-lookup"><span data-stu-id="a3608-166">Scope tags for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3608-167">关系</span><span class="sxs-lookup"><span data-stu-id="a3608-167">Relationships</span></span>
|<span data-ttu-id="a3608-168">关系</span><span class="sxs-lookup"><span data-stu-id="a3608-168">Relationship</span></span>|<span data-ttu-id="a3608-169">类型</span><span class="sxs-lookup"><span data-stu-id="a3608-169">Type</span></span>|<span data-ttu-id="a3608-170">说明</span><span class="sxs-lookup"><span data-stu-id="a3608-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3608-171">**开户**</span><span class="sxs-lookup"><span data-stu-id="a3608-171">**Enrollment**</span></span>|
|<span data-ttu-id="a3608-172">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="a3608-172">assignedDevices</span></span>|<span data-ttu-id="a3608-173">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="a3608-173">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="a3608-174">配置文件的已分配设备的列表。</span><span class="sxs-lookup"><span data-stu-id="a3608-174">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="a3608-175">assignments</span><span class="sxs-lookup"><span data-stu-id="a3608-175">assignments</span></span>|<span data-ttu-id="a3608-176">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="a3608-176">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="a3608-177">配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="a3608-177">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3608-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3608-178">JSON Representation</span></span>
<span data-ttu-id="a3608-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3608-179">Here is a JSON representation of the resource.</span></span>
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



