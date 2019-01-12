---
title: windowsAutopilotDeploymentProfile 资源类型
description: Windows 自动执行某些操作部署配置文件
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 60d72a63cfd4e062c312aeda89a37937b7e03041
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949393"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a><span data-ttu-id="da5fc-103">windowsAutopilotDeploymentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="da5fc-103">windowsAutopilotDeploymentProfile resource type</span></span>

> <span data-ttu-id="da5fc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="da5fc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da5fc-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="da5fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da5fc-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="da5fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da5fc-107">Windows 自动执行某些操作部署配置文件</span><span class="sxs-lookup"><span data-stu-id="da5fc-107">Windows Autopilot Deployment Profile</span></span>
## <a name="methods"></a><span data-ttu-id="da5fc-108">方法</span><span class="sxs-lookup"><span data-stu-id="da5fc-108">Methods</span></span>
|<span data-ttu-id="da5fc-109">方法</span><span class="sxs-lookup"><span data-stu-id="da5fc-109">Method</span></span>|<span data-ttu-id="da5fc-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="da5fc-110">Return Type</span></span>|<span data-ttu-id="da5fc-111">说明</span><span class="sxs-lookup"><span data-stu-id="da5fc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="da5fc-112">获取 windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="da5fc-112">Get windowsAutopilotDeploymentProfile</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[<span data-ttu-id="da5fc-113">windowsAutopilotDeploymentProfile</span><span class="sxs-lookup"><span data-stu-id="da5fc-113">windowsAutopilotDeploymentProfile</span></span>](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|<span data-ttu-id="da5fc-114">读取属性和[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="da5fc-114">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>|
|[<span data-ttu-id="da5fc-115">assign 操作</span><span class="sxs-lookup"><span data-stu-id="da5fc-115">assign action</span></span>](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|<span data-ttu-id="da5fc-116">无</span><span class="sxs-lookup"><span data-stu-id="da5fc-116">None</span></span>|<span data-ttu-id="da5fc-117">尚未记录</span><span class="sxs-lookup"><span data-stu-id="da5fc-117">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="da5fc-118">属性</span><span class="sxs-lookup"><span data-stu-id="da5fc-118">Properties</span></span>
|<span data-ttu-id="da5fc-119">属性</span><span class="sxs-lookup"><span data-stu-id="da5fc-119">Property</span></span>|<span data-ttu-id="da5fc-120">类型</span><span class="sxs-lookup"><span data-stu-id="da5fc-120">Type</span></span>|<span data-ttu-id="da5fc-121">说明</span><span class="sxs-lookup"><span data-stu-id="da5fc-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da5fc-122">id</span><span class="sxs-lookup"><span data-stu-id="da5fc-122">id</span></span>|<span data-ttu-id="da5fc-123">字符串</span><span class="sxs-lookup"><span data-stu-id="da5fc-123">String</span></span>|<span data-ttu-id="da5fc-124">配置文件密钥</span><span class="sxs-lookup"><span data-stu-id="da5fc-124">Profile Key</span></span>|
|<span data-ttu-id="da5fc-125">displayName</span><span class="sxs-lookup"><span data-stu-id="da5fc-125">displayName</span></span>|<span data-ttu-id="da5fc-126">字符串</span><span class="sxs-lookup"><span data-stu-id="da5fc-126">String</span></span>|<span data-ttu-id="da5fc-127">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="da5fc-127">Name of the profile</span></span>|
|<span data-ttu-id="da5fc-128">说明</span><span class="sxs-lookup"><span data-stu-id="da5fc-128">description</span></span>|<span data-ttu-id="da5fc-129">字符串</span><span class="sxs-lookup"><span data-stu-id="da5fc-129">String</span></span>|<span data-ttu-id="da5fc-130">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="da5fc-130">Description of the profile</span></span>|
|<span data-ttu-id="da5fc-131">language</span><span class="sxs-lookup"><span data-stu-id="da5fc-131">language</span></span>|<span data-ttu-id="da5fc-132">String</span><span class="sxs-lookup"><span data-stu-id="da5fc-132">String</span></span>|<span data-ttu-id="da5fc-133">在设备上配置的语言</span><span class="sxs-lookup"><span data-stu-id="da5fc-133">Language configured on the device</span></span>|
|<span data-ttu-id="da5fc-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da5fc-134">createdDateTime</span></span>|<span data-ttu-id="da5fc-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da5fc-135">DateTimeOffset</span></span>|<span data-ttu-id="da5fc-136">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="da5fc-136">Profile creation time</span></span>|
|<span data-ttu-id="da5fc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da5fc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="da5fc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da5fc-138">DateTimeOffset</span></span>|<span data-ttu-id="da5fc-139">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="da5fc-139">Profile last modified time</span></span>|
|<span data-ttu-id="da5fc-140">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="da5fc-140">outOfBoxExperienceSettings</span></span>|[<span data-ttu-id="da5fc-141">outOfBoxExperienceSettings</span><span class="sxs-lookup"><span data-stu-id="da5fc-141">outOfBoxExperienceSettings</span></span>](../resources/intune-enrollment-outofboxexperiencesettings.md)|<span data-ttu-id="da5fc-142">即开体验设置</span><span class="sxs-lookup"><span data-stu-id="da5fc-142">Out of box experience setting</span></span>|
|<span data-ttu-id="da5fc-143">enrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="da5fc-143">enrollmentStatusScreenSettings</span></span>|[<span data-ttu-id="da5fc-144">windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="da5fc-144">windowsEnrollmentStatusScreenSettings</span></span>](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|<span data-ttu-id="da5fc-145">注册状态屏幕设置</span><span class="sxs-lookup"><span data-stu-id="da5fc-145">Enrollment status screen setting</span></span>|
|<span data-ttu-id="da5fc-146">extractHardwareHash</span><span class="sxs-lookup"><span data-stu-id="da5fc-146">extractHardwareHash</span></span>|<span data-ttu-id="da5fc-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="da5fc-147">Boolean</span></span>|<span data-ttu-id="da5fc-148">配置文件的 HardwareHash 提取</span><span class="sxs-lookup"><span data-stu-id="da5fc-148">HardwareHash Extraction for the profile</span></span>|
|<span data-ttu-id="da5fc-149">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="da5fc-149">deviceNameTemplate</span></span>|<span data-ttu-id="da5fc-150">字符串</span><span class="sxs-lookup"><span data-stu-id="da5fc-150">String</span></span>|<span data-ttu-id="da5fc-151">用于自动执行某些操作设备命名的模板。</span><span class="sxs-lookup"><span data-stu-id="da5fc-151">The template used to name the AutoPilot Device.</span></span> <span data-ttu-id="da5fc-152">这可以是自定义文本，并且还可以包含该设备，序列号或随机生成的编号。</span><span class="sxs-lookup"><span data-stu-id="da5fc-152">This can be a custom text and can also contain either the serial number of the device, or a randomly generated number.</span></span> <span data-ttu-id="da5fc-153">由模板生成的文本的总长度可不超过 15 个字符。</span><span class="sxs-lookup"><span data-stu-id="da5fc-153">The total length of the text generated by the template can be no more than 15 characters.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da5fc-154">Relationships</span><span class="sxs-lookup"><span data-stu-id="da5fc-154">Relationships</span></span>
|<span data-ttu-id="da5fc-155">关系</span><span class="sxs-lookup"><span data-stu-id="da5fc-155">Relationship</span></span>|<span data-ttu-id="da5fc-156">类型</span><span class="sxs-lookup"><span data-stu-id="da5fc-156">Type</span></span>|<span data-ttu-id="da5fc-157">说明</span><span class="sxs-lookup"><span data-stu-id="da5fc-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da5fc-158">assignedDevices</span><span class="sxs-lookup"><span data-stu-id="da5fc-158">assignedDevices</span></span>|<span data-ttu-id="da5fc-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="da5fc-159">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="da5fc-160">配置文件分配设备的列表。</span><span class="sxs-lookup"><span data-stu-id="da5fc-160">The list of assigned devices for the profile.</span></span>|
|<span data-ttu-id="da5fc-161">assignments</span><span class="sxs-lookup"><span data-stu-id="da5fc-161">assignments</span></span>|<span data-ttu-id="da5fc-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="da5fc-162">[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) collection</span></span>|<span data-ttu-id="da5fc-163">配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="da5fc-163">The list of group assignments for the profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="da5fc-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da5fc-164">JSON Representation</span></span>
<span data-ttu-id="da5fc-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da5fc-165">Here is a JSON representation of the resource.</span></span>
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





