---
title: windowsAutopilotDeploymentProfile 资源类型
description: Windows 自动执行某些操作部署配置文件
ms.openlocfilehash: ed109af370d73d22d46198b206ba42dc4ebab2da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042843"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="c83b7-103">windowsAutopilotDeploymentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="c83b7-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="c83b7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c83b7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c83b7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c83b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c83b7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c83b7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c83b7-107">Windows 自动执行某些操作部署配置文件</span><span class="sxs-lookup"><span data-stu-id="c83b7-107">Windows Autopilot Deployment Profile</span></span>
## <a name="methods"></a><span data-ttu-id="c83b7-108">方法</span><span class="sxs-lookup"><span data-stu-id="c83b7-108">Methods</span></span>
|<span data-ttu-id="c83b7-109">方法</span><span class="sxs-lookup"><span data-stu-id="c83b7-109">Method</span></span>|<span data-ttu-id="c83b7-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c83b7-110">Return Type</span></span>|<span data-ttu-id="c83b7-111">说明</span><span class="sxs-lookup"><span data-stu-id="c83b7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c83b7-112">获取 windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="c83b7-112">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="c83b7-113">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="c83b7-113">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="c83b7-114">读取属性和[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="c83b7-114">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="c83b7-115">assign 操作</span><span class="sxs-lookup"><span data-stu-id="c83b7-115">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="c83b7-116">无</span><span class="sxs-lookup"><span data-stu-id="c83b7-116">None</span></span>|<span data-ttu-id="c83b7-117">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c83b7-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c83b7-118">属性</span><span class="sxs-lookup"><span data-stu-id="c83b7-118">Properties</span></span>
|<span data-ttu-id="c83b7-119">属性</span><span class="sxs-lookup"><span data-stu-id="c83b7-119">Property</span></span>|<span data-ttu-id="c83b7-120">类型</span><span class="sxs-lookup"><span data-stu-id="c83b7-120">Type</span></span>|<span data-ttu-id="c83b7-121">说明</span><span class="sxs-lookup"><span data-stu-id="c83b7-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c83b7-122">id</span><span class="sxs-lookup"><span data-stu-id="c83b7-122">id</span></span>|<span data-ttu-id="c83b7-123">字符串</span><span class="sxs-lookup"><span data-stu-id="c83b7-123">String</span></span>|<span data-ttu-id="c83b7-124">配置文件密钥</span><span class="sxs-lookup"><span data-stu-id="c83b7-124">Profile Key</span></span>|
|<span data-ttu-id="c83b7-125">displayName</span><span class="sxs-lookup"><span data-stu-id="c83b7-125">displayName</span></span>|<span data-ttu-id="c83b7-126">字符串</span><span class="sxs-lookup"><span data-stu-id="c83b7-126">String</span></span>|<span data-ttu-id="c83b7-127">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="c83b7-127">Name of the profile</span></span>|
|<span data-ttu-id="c83b7-128">说明</span><span class="sxs-lookup"><span data-stu-id="c83b7-128">description</span></span>|<span data-ttu-id="c83b7-129">字符串</span><span class="sxs-lookup"><span data-stu-id="c83b7-129">String</span></span>|<span data-ttu-id="c83b7-130">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="c83b7-130">Description of the profile</span></span>|
|<span data-ttu-id="c83b7-131">language</span><span class="sxs-lookup"><span data-stu-id="c83b7-131">language</span></span>|<span data-ttu-id="c83b7-132">String</span><span class="sxs-lookup"><span data-stu-id="c83b7-132">String</span></span>|<span data-ttu-id="c83b7-133">在设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="c83b7-133">Language configured on the device</span></span>|
|<span data-ttu-id="c83b7-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c83b7-134">createdDateTime</span></span>|<span data-ttu-id="c83b7-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c83b7-135">DateTimeOffset</span></span>|<span data-ttu-id="c83b7-136">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="c83b7-136">Profile creation time</span></span>|
|<span data-ttu-id="c83b7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c83b7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c83b7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c83b7-138">DateTimeOffset</span></span>|<span data-ttu-id="c83b7-139">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="c83b7-139">Profile last modified time</span></span>|
|<span data-ttu-id="c83b7-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="c83b7-140">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="c83b7-141">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="c83b7-141">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="c83b7-142">即开体验设置</span><span class="sxs-lookup"><span data-stu-id="c83b7-142">Out of box experience setting</span></span>|
|<span data-ttu-id="c83b7-143">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="c83b7-143">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="c83b7-144">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="c83b7-144">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="c83b7-145">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="c83b7-145">Enrollment status screen setting</span></span>|
|<span data-ttu-id="c83b7-146">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="c83b7-146">extractHardwareHash</span></span>|<span data-ttu-id="c83b7-147">布尔</span><span class="sxs-lookup"><span data-stu-id="c83b7-147">Boolean</span></span>|<span data-ttu-id="c83b7-148">配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="c83b7-148">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="c83b7-149">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="c83b7-149">deviceNameTemplate</span></span>|<span data-ttu-id="c83b7-150">字符串</span><span class="sxs-lookup"><span data-stu-id="c83b7-150">String</span></span>|<span data-ttu-id="c83b7-151">用于自动执行某些操作设备命名的模板。</span><span class="sxs-lookup"><span data-stu-id="c83b7-151">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="c83b7-152">这可以是自定义文本，并且还可以包含该设备，序列号或随机生成的编号。</span><span class="sxs-lookup"><span data-stu-id="c83b7-152">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="c83b7-153">由模板生成的文本的总长度可不超过 15 个字符。</span><span class="sxs-lookup"><span data-stu-id="c83b7-153">The total length of the text generated by the template can be no more than 15 characters.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c83b7-154">Relationships</span><span class="sxs-lookup"><span data-stu-id="c83b7-154">Relationships</span></span>
|<span data-ttu-id="c83b7-155">关系</span><span class="sxs-lookup"><span data-stu-id="c83b7-155">Relationship</span></span>|<span data-ttu-id="c83b7-156">类型</span><span class="sxs-lookup"><span data-stu-id="c83b7-156">Type</span></span>|<span data-ttu-id="c83b7-157">说明</span><span class="sxs-lookup"><span data-stu-id="c83b7-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c83b7-158">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="c83b7-158">assignedDevices</span></span>|<span data-ttu-id="c83b7-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="c83b7-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="c83b7-160">配置文件分配设备的列表。</span><span class="sxs-lookup"><span data-stu-id="c83b7-160">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="c83b7-161">assignments</span><span class="sxs-lookup"><span data-stu-id="c83b7-161">assignments</span></span>|<span data-ttu-id="c83b7-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="c83b7-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="c83b7-163">配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="c83b7-163">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c83b7-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c83b7-164">JSON Representation</span></span>
<span data-ttu-id="c83b7-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c83b7-165">Here is a JSON representation of the resource.</span></span>
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





