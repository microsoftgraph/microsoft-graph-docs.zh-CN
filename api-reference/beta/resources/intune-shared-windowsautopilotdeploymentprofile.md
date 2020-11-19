---
title: windowsAutopilotDeploymentProfile 资源类型
description: Windows Autopilot 部署配置文件
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 196355a03a6c86a62765bc2b513670315d3311c2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255579"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="cde54-103">windowsAutopilotDeploymentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="cde54-103">windowsAutopilotDeploymentProfile resource type</span></span>

<span data-ttu-id="cde54-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cde54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cde54-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cde54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cde54-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cde54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cde54-107">Windows Autopilot 部署配置文件</span><span class="sxs-lookup"><span data-stu-id="cde54-107">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="cde54-108">方法</span><span class="sxs-lookup"><span data-stu-id="cde54-108">Methods</span></span>
|<span data-ttu-id="cde54-109">方法</span><span class="sxs-lookup"><span data-stu-id="cde54-109">Method</span></span>|<span data-ttu-id="cde54-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cde54-110">Return Type</span></span>|<span data-ttu-id="cde54-111">说明</span><span class="sxs-lookup"><span data-stu-id="cde54-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cde54-112">获取 windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="cde54-112">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-shared-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="cde54-113">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="cde54-113">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="cde54-114">读取 [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cde54-114">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="cde54-115">分配操作</span><span class="sxs-lookup"><span data-stu-id="cde54-115">assign action</span></span>](../api/intune-shared-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="cde54-116">无</span><span class="sxs-lookup"><span data-stu-id="cde54-116">None</span></span>|<span data-ttu-id="cde54-117">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cde54-117">Not yet documented</span></span>|
|<span data-ttu-id="cde54-118">**策略集**</span><span class="sxs-lookup"><span data-stu-id="cde54-118">**Policy Set**</span></span>|
|[<span data-ttu-id="cde54-119">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="cde54-119">hasPayloadLinks action</span></span>](../api/intune-shared-windowsautopilotdeploymentprofile-haspayloadlinks.md)|<span data-ttu-id="cde54-120">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cde54-120">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="cde54-121">尚未记录</span><span class="sxs-lookup"><span data-stu-id="cde54-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cde54-122">属性</span><span class="sxs-lookup"><span data-stu-id="cde54-122">Properties</span></span>
|<span data-ttu-id="cde54-123">属性</span><span class="sxs-lookup"><span data-stu-id="cde54-123">Property</span></span>|<span data-ttu-id="cde54-124">类型</span><span class="sxs-lookup"><span data-stu-id="cde54-124">Type</span></span>|<span data-ttu-id="cde54-125">说明</span><span class="sxs-lookup"><span data-stu-id="cde54-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cde54-126">id</span><span class="sxs-lookup"><span data-stu-id="cde54-126">id</span></span>|<span data-ttu-id="cde54-127">String</span><span class="sxs-lookup"><span data-stu-id="cde54-127">String</span></span>|<span data-ttu-id="cde54-128">配置文件键</span><span class="sxs-lookup"><span data-stu-id="cde54-128">Profile Key</span></span>|
|<span data-ttu-id="cde54-129">displayName</span><span class="sxs-lookup"><span data-stu-id="cde54-129">displayName</span></span>|<span data-ttu-id="cde54-130">String</span><span class="sxs-lookup"><span data-stu-id="cde54-130">String</span></span>|<span data-ttu-id="cde54-131">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="cde54-131">Name of the profile</span></span>|
|<span data-ttu-id="cde54-132">description</span><span class="sxs-lookup"><span data-stu-id="cde54-132">description</span></span>|<span data-ttu-id="cde54-133">String</span><span class="sxs-lookup"><span data-stu-id="cde54-133">String</span></span>|<span data-ttu-id="cde54-134">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="cde54-134">Description of the profile</span></span>|
|<span data-ttu-id="cde54-135">language</span><span class="sxs-lookup"><span data-stu-id="cde54-135">language</span></span>|<span data-ttu-id="cde54-136">String</span><span class="sxs-lookup"><span data-stu-id="cde54-136">String</span></span>|<span data-ttu-id="cde54-137">在设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="cde54-137">Language configured on the device</span></span>|
|<span data-ttu-id="cde54-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cde54-138">createdDateTime</span></span>|<span data-ttu-id="cde54-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cde54-139">DateTimeOffset</span></span>|<span data-ttu-id="cde54-140">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="cde54-140">Profile creation time</span></span>|
|<span data-ttu-id="cde54-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cde54-141">lastModifiedDateTime</span></span>|<span data-ttu-id="cde54-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cde54-142">DateTimeOffset</span></span>|<span data-ttu-id="cde54-143">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="cde54-143">Profile last modified time</span></span>|
|<span data-ttu-id="cde54-144">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="cde54-144">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="cde54-145">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="cde54-145">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="cde54-146">"开箱即用体验" 设置</span><span class="sxs-lookup"><span data-stu-id="cde54-146">Out of box experience setting</span></span>|
|<span data-ttu-id="cde54-147">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="cde54-147">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="cde54-148">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="cde54-148">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="cde54-149">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="cde54-149">Enrollment status screen setting</span></span>|
|<span data-ttu-id="cde54-150">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="cde54-150">extractHardwareHash</span></span>|<span data-ttu-id="cde54-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="cde54-151">Boolean</span></span>|<span data-ttu-id="cde54-152">配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="cde54-152">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="cde54-153">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="cde54-153">deviceNameTemplate</span></span>|<span data-ttu-id="cde54-154">String</span><span class="sxs-lookup"><span data-stu-id="cde54-154">String</span></span>|<span data-ttu-id="cde54-155">用于命名 AutoPilot 设备的模板。</span><span class="sxs-lookup"><span data-stu-id="cde54-155">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="cde54-156">它可以是自定义文本，也可以包含设备的序列号或随机生成的数字。</span><span class="sxs-lookup"><span data-stu-id="cde54-156">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="cde54-157">模板生成的文本的总长度不能超过15个字符。</span><span class="sxs-lookup"><span data-stu-id="cde54-157">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="cde54-158">deviceType</span><span class="sxs-lookup"><span data-stu-id="cde54-158">deviceType</span></span>|[<span data-ttu-id="cde54-159">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="cde54-159">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="cde54-160">此配置文件适用的 AutoPilot 设备类型。</span><span class="sxs-lookup"><span data-stu-id="cde54-160">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="cde54-161">可取值为：`windowsPc`、`surfaceHub2`。</span><span class="sxs-lookup"><span data-stu-id="cde54-161">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="cde54-162">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="cde54-162">enableWhiteGlove</span></span>|<span data-ttu-id="cde54-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="cde54-163">Boolean</span></span>|<span data-ttu-id="cde54-164">为配置文件启用 Autopilot 白色 Glove。</span><span class="sxs-lookup"><span data-stu-id="cde54-164">Enable Autopilot White Glove for the profile.</span></span>|
|<span data-ttu-id="cde54-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cde54-165">roleScopeTagIds</span></span>|<span data-ttu-id="cde54-166">String 集合</span><span class="sxs-lookup"><span data-stu-id="cde54-166">String collection</span></span>|<span data-ttu-id="cde54-167">配置文件的范围标记。</span><span class="sxs-lookup"><span data-stu-id="cde54-167">Scope tags for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cde54-168">关系</span><span class="sxs-lookup"><span data-stu-id="cde54-168">Relationships</span></span>
|<span data-ttu-id="cde54-169">关系</span><span class="sxs-lookup"><span data-stu-id="cde54-169">Relationship</span></span>|<span data-ttu-id="cde54-170">类型</span><span class="sxs-lookup"><span data-stu-id="cde54-170">Type</span></span>|<span data-ttu-id="cde54-171">描述</span><span class="sxs-lookup"><span data-stu-id="cde54-171">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cde54-172">**开户**</span><span class="sxs-lookup"><span data-stu-id="cde54-172">**Enrollment**</span></span>|
|<span data-ttu-id="cde54-173">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="cde54-173">assignedDevices</span></span>|<span data-ttu-id="cde54-174">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cde54-174">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="cde54-175">配置文件的已分配设备的列表。</span><span class="sxs-lookup"><span data-stu-id="cde54-175">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="cde54-176">assignments</span><span class="sxs-lookup"><span data-stu-id="cde54-176">assignments</span></span>|<span data-ttu-id="cde54-177">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cde54-177">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="cde54-178">配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="cde54-178">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cde54-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cde54-179">JSON Representation</span></span>
<span data-ttu-id="cde54-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cde54-180">Here is a JSON representation of the resource.</span></span>
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




