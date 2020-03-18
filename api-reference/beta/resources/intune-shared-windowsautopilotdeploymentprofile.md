---
title: windowsAutopilotDeploymentProfile 资源类型
description: Windows Autopilot 部署配置文件
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 981cd4d9b1eb50982c56e59d146a876f4f52ce8f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42766824"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="d914c-103">windowsAutopilotDeploymentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="d914c-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="d914c-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d914c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d914c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d914c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d914c-106">Windows Autopilot 部署配置文件</span><span class="sxs-lookup"><span data-stu-id="d914c-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="d914c-107">方法</span><span class="sxs-lookup"><span data-stu-id="d914c-107">Methods</span></span>
|<span data-ttu-id="d914c-108">方法</span><span class="sxs-lookup"><span data-stu-id="d914c-108">Method</span></span>|<span data-ttu-id="d914c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d914c-109">Return Type</span></span>|<span data-ttu-id="d914c-110">说明</span><span class="sxs-lookup"><span data-stu-id="d914c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d914c-111">获取 windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="d914c-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-shared-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="d914c-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="d914c-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-shared-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="d914c-113">读取[windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d914c-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-shared-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="d914c-114">分配操作</span><span class="sxs-lookup"><span data-stu-id="d914c-114">assign action</span></span>](../api/intune-shared-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="d914c-115">无</span><span class="sxs-lookup"><span data-stu-id="d914c-115">None</span></span>|<span data-ttu-id="d914c-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d914c-116">Not yet documented</span></span>|
|<span data-ttu-id="d914c-117">**策略集**</span><span class="sxs-lookup"><span data-stu-id="d914c-117">**Policy Set**</span></span>|
|[<span data-ttu-id="d914c-118">hasPayloadLinks 操作</span><span class="sxs-lookup"><span data-stu-id="d914c-118">hasPayloadLinks action</span></span>](../api/intune-shared-windowsautopilotdeploymentprofile-haspayloadlinks.md)|<span data-ttu-id="d914c-119">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="d914c-119">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="d914c-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d914c-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d914c-121">属性</span><span class="sxs-lookup"><span data-stu-id="d914c-121">Properties</span></span>
|<span data-ttu-id="d914c-122">属性</span><span class="sxs-lookup"><span data-stu-id="d914c-122">Property</span></span>|<span data-ttu-id="d914c-123">类型</span><span class="sxs-lookup"><span data-stu-id="d914c-123">Type</span></span>|<span data-ttu-id="d914c-124">说明</span><span class="sxs-lookup"><span data-stu-id="d914c-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d914c-125">id</span><span class="sxs-lookup"><span data-stu-id="d914c-125">id</span></span>|<span data-ttu-id="d914c-126">字符串</span><span class="sxs-lookup"><span data-stu-id="d914c-126">String</span></span>|<span data-ttu-id="d914c-127">配置文件键</span><span class="sxs-lookup"><span data-stu-id="d914c-127">Profile Key</span></span>|
|<span data-ttu-id="d914c-128">displayName</span><span class="sxs-lookup"><span data-stu-id="d914c-128">displayName</span></span>|<span data-ttu-id="d914c-129">字符串</span><span class="sxs-lookup"><span data-stu-id="d914c-129">String</span></span>|<span data-ttu-id="d914c-130">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="d914c-130">Name of the profile</span></span>|
|<span data-ttu-id="d914c-131">说明</span><span class="sxs-lookup"><span data-stu-id="d914c-131">description</span></span>|<span data-ttu-id="d914c-132">String</span><span class="sxs-lookup"><span data-stu-id="d914c-132">String</span></span>|<span data-ttu-id="d914c-133">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="d914c-133">Description of the profile</span></span>|
|<span data-ttu-id="d914c-134">language</span><span class="sxs-lookup"><span data-stu-id="d914c-134">language</span></span>|<span data-ttu-id="d914c-135">String</span><span class="sxs-lookup"><span data-stu-id="d914c-135">String</span></span>|<span data-ttu-id="d914c-136">在设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="d914c-136">Language configured on the device</span></span>|
|<span data-ttu-id="d914c-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d914c-137">createdDateTime</span></span>|<span data-ttu-id="d914c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d914c-138">DateTimeOffset</span></span>|<span data-ttu-id="d914c-139">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="d914c-139">Profile creation time</span></span>|
|<span data-ttu-id="d914c-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d914c-140">lastModifiedDateTime</span></span>|<span data-ttu-id="d914c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d914c-141">DateTimeOffset</span></span>|<span data-ttu-id="d914c-142">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="d914c-142">Profile last modified time</span></span>|
|<span data-ttu-id="d914c-143">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="d914c-143">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="d914c-144">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="d914c-144">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="d914c-145">"开箱即用体验" 设置</span><span class="sxs-lookup"><span data-stu-id="d914c-145">Out of box experience setting</span></span>|
|<span data-ttu-id="d914c-146">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="d914c-146">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="d914c-147">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="d914c-147">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="d914c-148">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="d914c-148">Enrollment status screen setting</span></span>|
|<span data-ttu-id="d914c-149">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="d914c-149">extractHardwareHash</span></span>|<span data-ttu-id="d914c-150">布尔值</span><span class="sxs-lookup"><span data-stu-id="d914c-150">Boolean</span></span>|<span data-ttu-id="d914c-151">配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="d914c-151">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="d914c-152">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="d914c-152">deviceNameTemplate</span></span>|<span data-ttu-id="d914c-153">String</span><span class="sxs-lookup"><span data-stu-id="d914c-153">String</span></span>|<span data-ttu-id="d914c-154">用于命名 AutoPilot 设备的模板。</span><span class="sxs-lookup"><span data-stu-id="d914c-154">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="d914c-155">它可以是自定义文本，也可以包含设备的序列号或随机生成的数字。</span><span class="sxs-lookup"><span data-stu-id="d914c-155">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="d914c-156">模板生成的文本的总长度不能超过15个字符。</span><span class="sxs-lookup"><span data-stu-id="d914c-156">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="d914c-157">deviceType</span><span class="sxs-lookup"><span data-stu-id="d914c-157">deviceType</span></span>|[<span data-ttu-id="d914c-158">windowsAutopilotDeviceType</span><span class="sxs-lookup"><span data-stu-id="d914c-158">windowsAutopilotDeviceType</span></span>](../resources/intune-enrollment-windowsautopilotdevicetype.md)|<span data-ttu-id="d914c-159">此配置文件适用的 AutoPilot 设备类型。</span><span class="sxs-lookup"><span data-stu-id="d914c-159">The AutoPilot device type that this profile is applicable to.</span></span> <span data-ttu-id="d914c-160">可取值为：`windowsPc`、`surfaceHub2`。</span><span class="sxs-lookup"><span data-stu-id="d914c-160">Possible values are: `windowsPc`, `surfaceHub2`.</span></span>|
|<span data-ttu-id="d914c-161">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="d914c-161">enableWhiteGlove</span></span>|<span data-ttu-id="d914c-162">布尔值</span><span class="sxs-lookup"><span data-stu-id="d914c-162">Boolean</span></span>|<span data-ttu-id="d914c-163">为配置文件启用 Autopilot 白色 Glove。</span><span class="sxs-lookup"><span data-stu-id="d914c-163">Enable Autopilot White Glove for the profile.</span></span>|
|<span data-ttu-id="d914c-164">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d914c-164">roleScopeTagIds</span></span>|<span data-ttu-id="d914c-165">String collection</span><span class="sxs-lookup"><span data-stu-id="d914c-165">String collection</span></span>|<span data-ttu-id="d914c-166">配置文件的范围标记。</span><span class="sxs-lookup"><span data-stu-id="d914c-166">Scope tags for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d914c-167">关系</span><span class="sxs-lookup"><span data-stu-id="d914c-167">Relationships</span></span>
|<span data-ttu-id="d914c-168">关系</span><span class="sxs-lookup"><span data-stu-id="d914c-168">Relationship</span></span>|<span data-ttu-id="d914c-169">类型</span><span class="sxs-lookup"><span data-stu-id="d914c-169">Type</span></span>|<span data-ttu-id="d914c-170">说明</span><span class="sxs-lookup"><span data-stu-id="d914c-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d914c-171">**开户**</span><span class="sxs-lookup"><span data-stu-id="d914c-171">**Enrollment**</span></span>|
|<span data-ttu-id="d914c-172">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="d914c-172">assignedDevices</span></span>|<span data-ttu-id="d914c-173">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="d914c-173">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="d914c-174">配置文件的已分配设备的列表。</span><span class="sxs-lookup"><span data-stu-id="d914c-174">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="d914c-175">assignments</span><span class="sxs-lookup"><span data-stu-id="d914c-175">assignments</span></span>|<span data-ttu-id="d914c-176">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="d914c-176">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="d914c-177">配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="d914c-177">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d914c-178">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d914c-178">JSON Representation</span></span>
<span data-ttu-id="d914c-179">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d914c-179">Here is a JSON representation of the resource.</span></span>
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



