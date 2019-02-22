---
title: windowsAutopilotDeploymentProfile 资源类型
description: Windows Autopilot 部署配置文件
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b3b815e0184ab9969af348338c07c3fabf0b0597
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168871"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="25cc1-103">windowsAutopilotDeploymentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="25cc1-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="25cc1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="25cc1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25cc1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25cc1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25cc1-106">Windows Autopilot 部署配置文件</span><span class="sxs-lookup"><span data-stu-id="25cc1-106">Windows Autopilot Deployment Profile</span></span>

## <a name="methods"></a><span data-ttu-id="25cc1-107">方法</span><span class="sxs-lookup"><span data-stu-id="25cc1-107">Methods</span></span>
|<span data-ttu-id="25cc1-108">方法</span><span class="sxs-lookup"><span data-stu-id="25cc1-108">Method</span></span>|<span data-ttu-id="25cc1-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="25cc1-109">Return Type</span></span>|<span data-ttu-id="25cc1-110">说明</span><span class="sxs-lookup"><span data-stu-id="25cc1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="25cc1-111">获取 windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="25cc1-111">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="25cc1-112">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="25cc1-112">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="25cc1-113">读取[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="25cc1-113">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="25cc1-114">assign 操作</span><span class="sxs-lookup"><span data-stu-id="25cc1-114">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="25cc1-115">无</span><span class="sxs-lookup"><span data-stu-id="25cc1-115">None</span></span>|<span data-ttu-id="25cc1-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="25cc1-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="25cc1-117">属性</span><span class="sxs-lookup"><span data-stu-id="25cc1-117">Properties</span></span>
|<span data-ttu-id="25cc1-118">属性</span><span class="sxs-lookup"><span data-stu-id="25cc1-118">Property</span></span>|<span data-ttu-id="25cc1-119">类型</span><span class="sxs-lookup"><span data-stu-id="25cc1-119">Type</span></span>|<span data-ttu-id="25cc1-120">说明</span><span class="sxs-lookup"><span data-stu-id="25cc1-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25cc1-121">id</span><span class="sxs-lookup"><span data-stu-id="25cc1-121">id</span></span>|<span data-ttu-id="25cc1-122">字串符号</span><span class="sxs-lookup"><span data-stu-id="25cc1-122">String</span></span>|<span data-ttu-id="25cc1-123">配置文件键</span><span class="sxs-lookup"><span data-stu-id="25cc1-123">Profile Key</span></span>|
|<span data-ttu-id="25cc1-124">displayName</span><span class="sxs-lookup"><span data-stu-id="25cc1-124">displayName</span></span>|<span data-ttu-id="25cc1-125">字符串</span><span class="sxs-lookup"><span data-stu-id="25cc1-125">String</span></span>|<span data-ttu-id="25cc1-126">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="25cc1-126">Name of the profile</span></span>|
|<span data-ttu-id="25cc1-127">说明</span><span class="sxs-lookup"><span data-stu-id="25cc1-127">description</span></span>|<span data-ttu-id="25cc1-128">字符串</span><span class="sxs-lookup"><span data-stu-id="25cc1-128">String</span></span>|<span data-ttu-id="25cc1-129">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="25cc1-129">Description of the profile</span></span>|
|<span data-ttu-id="25cc1-130">language</span><span class="sxs-lookup"><span data-stu-id="25cc1-130">language</span></span>|<span data-ttu-id="25cc1-131">String</span><span class="sxs-lookup"><span data-stu-id="25cc1-131">String</span></span>|<span data-ttu-id="25cc1-132">在设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="25cc1-132">Language configured on the device</span></span>|
|<span data-ttu-id="25cc1-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25cc1-133">createdDateTime</span></span>|<span data-ttu-id="25cc1-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25cc1-134">DateTimeOffset</span></span>|<span data-ttu-id="25cc1-135">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="25cc1-135">Profile creation time</span></span>|
|<span data-ttu-id="25cc1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25cc1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="25cc1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25cc1-137">DateTimeOffset</span></span>|<span data-ttu-id="25cc1-138">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="25cc1-138">Profile last modified time</span></span>|
|<span data-ttu-id="25cc1-139">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="25cc1-139">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="25cc1-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="25cc1-140">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="25cc1-141">"开箱即用体验" 设置</span><span class="sxs-lookup"><span data-stu-id="25cc1-141">Out of box experience setting</span></span>|
|<span data-ttu-id="25cc1-142">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="25cc1-142">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="25cc1-143">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="25cc1-143">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="25cc1-144">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="25cc1-144">Enrollment status screen setting</span></span>|
|<span data-ttu-id="25cc1-145">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="25cc1-145">extractHardwareHash</span></span>|<span data-ttu-id="25cc1-146">布尔</span><span class="sxs-lookup"><span data-stu-id="25cc1-146">Boolean</span></span>|<span data-ttu-id="25cc1-147">配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="25cc1-147">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="25cc1-148">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="25cc1-148">deviceNameTemplate</span></span>|<span data-ttu-id="25cc1-149">字符串</span><span class="sxs-lookup"><span data-stu-id="25cc1-149">String</span></span>|<span data-ttu-id="25cc1-150">用于命名 AutoPilot 设备的模板。</span><span class="sxs-lookup"><span data-stu-id="25cc1-150">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="25cc1-151">它可以是自定义文本, 也可以包含设备的序列号或随机生成的数字。</span><span class="sxs-lookup"><span data-stu-id="25cc1-151">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="25cc1-152">模板生成的文本的总长度不能超过15个字符。</span><span class="sxs-lookup"><span data-stu-id="25cc1-152">The total length of the text generated by the template can be no more than 15 characters.</span></span>|
|<span data-ttu-id="25cc1-153">enableWhiteGlove</span><span class="sxs-lookup"><span data-stu-id="25cc1-153">enableWhiteGlove</span></span>|<span data-ttu-id="25cc1-154">布尔</span><span class="sxs-lookup"><span data-stu-id="25cc1-154">Boolean</span></span>|<span data-ttu-id="25cc1-155">为配置文件启用 Autopilot 白色 Glove。</span><span class="sxs-lookup"><span data-stu-id="25cc1-155">Enable Autopilot White Glove for the profile.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25cc1-156">关系</span><span class="sxs-lookup"><span data-stu-id="25cc1-156">Relationships</span></span>
|<span data-ttu-id="25cc1-157">关系</span><span class="sxs-lookup"><span data-stu-id="25cc1-157">Relationship</span></span>|<span data-ttu-id="25cc1-158">类型</span><span class="sxs-lookup"><span data-stu-id="25cc1-158">Type</span></span>|<span data-ttu-id="25cc1-159">说明</span><span class="sxs-lookup"><span data-stu-id="25cc1-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25cc1-160">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="25cc1-160">assignedDevices</span></span>|<span data-ttu-id="25cc1-161">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="25cc1-161">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="25cc1-162">配置文件的已分配设备的列表。</span><span class="sxs-lookup"><span data-stu-id="25cc1-162">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="25cc1-163">assignments</span><span class="sxs-lookup"><span data-stu-id="25cc1-163">assignments</span></span>|<span data-ttu-id="25cc1-164">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="25cc1-164">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="25cc1-165">配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="25cc1-165">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25cc1-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25cc1-166">JSON Representation</span></span>
<span data-ttu-id="25cc1-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25cc1-167">Here is a JSON representation of the resource.</span></span>
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
  "enableWhiteGlove": true
}
```




