---
title: windowsAutopilotDeploymentProfile 资源类型
description: Windows 自动执行某些操作部署配置文件
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1538497dc5105dcd2e7f0c9ff7fdf83c3ddec56e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892195"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="a0e2e-103">windowsAutopilotDeploymentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0e2e-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="a0e2e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a0e2e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0e2e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a0e2e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0e2e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a0e2e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0e2e-107">Windows 自动执行某些操作部署配置文件</span><span class="sxs-lookup"><span data-stu-id="a0e2e-107">Windows Autopilot Deployment Profile</span></span>
## <a name="methods"></a><span data-ttu-id="a0e2e-108">方法</span><span class="sxs-lookup"><span data-stu-id="a0e2e-108">Methods</span></span>
|<span data-ttu-id="a0e2e-109">方法</span><span class="sxs-lookup"><span data-stu-id="a0e2e-109">Method</span></span>|<span data-ttu-id="a0e2e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a0e2e-110">Return Type</span></span>|<span data-ttu-id="a0e2e-111">说明</span><span class="sxs-lookup"><span data-stu-id="a0e2e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a0e2e-112">获取 windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="a0e2e-112">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="a0e2e-113">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="a0e2e-113">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="a0e2e-114">读取属性和[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a0e2e-114">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="a0e2e-115">assign 操作</span><span class="sxs-lookup"><span data-stu-id="a0e2e-115">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="a0e2e-116">无</span><span class="sxs-lookup"><span data-stu-id="a0e2e-116">None</span></span>|<span data-ttu-id="a0e2e-117">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a0e2e-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a0e2e-118">属性</span><span class="sxs-lookup"><span data-stu-id="a0e2e-118">Properties</span></span>
|<span data-ttu-id="a0e2e-119">属性</span><span class="sxs-lookup"><span data-stu-id="a0e2e-119">Property</span></span>|<span data-ttu-id="a0e2e-120">类型</span><span class="sxs-lookup"><span data-stu-id="a0e2e-120">Type</span></span>|<span data-ttu-id="a0e2e-121">说明</span><span class="sxs-lookup"><span data-stu-id="a0e2e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0e2e-122">id</span><span class="sxs-lookup"><span data-stu-id="a0e2e-122">id</span></span>|<span data-ttu-id="a0e2e-123">字符串</span><span class="sxs-lookup"><span data-stu-id="a0e2e-123">String</span></span>|<span data-ttu-id="a0e2e-124">配置文件密钥</span><span class="sxs-lookup"><span data-stu-id="a0e2e-124">Profile Key</span></span>|
|<span data-ttu-id="a0e2e-125">displayName</span><span class="sxs-lookup"><span data-stu-id="a0e2e-125">displayName</span></span>|<span data-ttu-id="a0e2e-126">字符串</span><span class="sxs-lookup"><span data-stu-id="a0e2e-126">String</span></span>|<span data-ttu-id="a0e2e-127">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="a0e2e-127">Name of the profile</span></span>|
|<span data-ttu-id="a0e2e-128">说明</span><span class="sxs-lookup"><span data-stu-id="a0e2e-128">description</span></span>|<span data-ttu-id="a0e2e-129">字符串</span><span class="sxs-lookup"><span data-stu-id="a0e2e-129">String</span></span>|<span data-ttu-id="a0e2e-130">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="a0e2e-130">Description of the profile</span></span>|
|<span data-ttu-id="a0e2e-131">language</span><span class="sxs-lookup"><span data-stu-id="a0e2e-131">language</span></span>|<span data-ttu-id="a0e2e-132">String</span><span class="sxs-lookup"><span data-stu-id="a0e2e-132">String</span></span>|<span data-ttu-id="a0e2e-133">在设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="a0e2e-133">Language configured on the device</span></span>|
|<span data-ttu-id="a0e2e-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0e2e-134">createdDateTime</span></span>|<span data-ttu-id="a0e2e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0e2e-135">DateTimeOffset</span></span>|<span data-ttu-id="a0e2e-136">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="a0e2e-136">Profile creation time</span></span>|
|<span data-ttu-id="a0e2e-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0e2e-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a0e2e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0e2e-138">DateTimeOffset</span></span>|<span data-ttu-id="a0e2e-139">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="a0e2e-139">Profile last modified time</span></span>|
|<span data-ttu-id="a0e2e-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="a0e2e-140">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="a0e2e-141">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="a0e2e-141">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="a0e2e-142">即开体验设置</span><span class="sxs-lookup"><span data-stu-id="a0e2e-142">Out of box experience setting</span></span>|
|<span data-ttu-id="a0e2e-143">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="a0e2e-143">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="a0e2e-144">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="a0e2e-144">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="a0e2e-145">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="a0e2e-145">Enrollment status screen setting</span></span>|
|<span data-ttu-id="a0e2e-146">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="a0e2e-146">extractHardwareHash</span></span>|<span data-ttu-id="a0e2e-147">布尔</span><span class="sxs-lookup"><span data-stu-id="a0e2e-147">Boolean</span></span>|<span data-ttu-id="a0e2e-148">配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="a0e2e-148">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="a0e2e-149">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="a0e2e-149">deviceNameTemplate</span></span>|<span data-ttu-id="a0e2e-150">字符串</span><span class="sxs-lookup"><span data-stu-id="a0e2e-150">String</span></span>|<span data-ttu-id="a0e2e-151">用于自动执行某些操作设备命名的模板。</span><span class="sxs-lookup"><span data-stu-id="a0e2e-151">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="a0e2e-152">这可以是自定义文本，并且还可以包含该设备，序列号或随机生成的编号。</span><span class="sxs-lookup"><span data-stu-id="a0e2e-152">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="a0e2e-153">由模板生成的文本的总长度可不超过 15 个字符。</span><span class="sxs-lookup"><span data-stu-id="a0e2e-153">The total length of the text generated by the template can be no more than 15 characters.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0e2e-154">Relationships</span><span class="sxs-lookup"><span data-stu-id="a0e2e-154">Relationships</span></span>
|<span data-ttu-id="a0e2e-155">关系</span><span class="sxs-lookup"><span data-stu-id="a0e2e-155">Relationship</span></span>|<span data-ttu-id="a0e2e-156">类型</span><span class="sxs-lookup"><span data-stu-id="a0e2e-156">Type</span></span>|<span data-ttu-id="a0e2e-157">Description</span><span class="sxs-lookup"><span data-stu-id="a0e2e-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0e2e-158">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="a0e2e-158">assignedDevices</span></span>|<span data-ttu-id="a0e2e-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="a0e2e-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="a0e2e-160">配置文件分配设备的列表。</span><span class="sxs-lookup"><span data-stu-id="a0e2e-160">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="a0e2e-161">assignments</span><span class="sxs-lookup"><span data-stu-id="a0e2e-161">assignments</span></span>|<span data-ttu-id="a0e2e-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="a0e2e-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="a0e2e-163">配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="a0e2e-163">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0e2e-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0e2e-164">JSON Representation</span></span>
<span data-ttu-id="a0e2e-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0e2e-165">Here is a JSON representation of the resource.</span></span>
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
  "deviceNameTemplate": "String"
}
```





