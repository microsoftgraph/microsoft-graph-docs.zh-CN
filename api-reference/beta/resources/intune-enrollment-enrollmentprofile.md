---
title: enrollmentProfile 资源类型
description: enrollmentProfile 资源表示必须提供预注册的配置的集合, 以便能够注册已预暂存其标识的某些设备。 预暂存的设备标识分配给此类型的配置文件, 以便在注册相应设备时应用配置文件的配置。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: abc00f27ef65cdddfef30a06bef55a8fa44e488a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805521"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="94478-104">enrollmentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="94478-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="94478-105">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="94478-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94478-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94478-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94478-107">enrollmentProfile 资源表示必须提供预注册的配置的集合, 以便能够注册已预暂存其标识的某些设备。</span><span class="sxs-lookup"><span data-stu-id="94478-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="94478-108">预暂存的设备标识分配给此类型的配置文件, 以便在注册相应设备时应用配置文件的配置。</span><span class="sxs-lookup"><span data-stu-id="94478-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="94478-109">方法</span><span class="sxs-lookup"><span data-stu-id="94478-109">Methods</span></span>
|<span data-ttu-id="94478-110">方法</span><span class="sxs-lookup"><span data-stu-id="94478-110">Method</span></span>|<span data-ttu-id="94478-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="94478-111">Return Type</span></span>|<span data-ttu-id="94478-112">说明</span><span class="sxs-lookup"><span data-stu-id="94478-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="94478-113">列出 enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="94478-113">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="94478-114">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="94478-114">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="94478-115">列出[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94478-115">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="94478-116">获取 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="94478-116">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="94478-117">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="94478-117">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="94478-118">读取[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94478-118">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="94478-119">创建 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="94478-119">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="94478-120">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="94478-120">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="94478-121">创建新的[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="94478-121">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="94478-122">删除 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="94478-122">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="94478-123">无</span><span class="sxs-lookup"><span data-stu-id="94478-123">None</span></span>|<span data-ttu-id="94478-124">删除[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="94478-124">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="94478-125">更新 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="94478-125">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="94478-126">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="94478-126">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="94478-127">更新[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94478-127">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="94478-128">setDefaultProfile 操作</span><span class="sxs-lookup"><span data-stu-id="94478-128">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="94478-129">无</span><span class="sxs-lookup"><span data-stu-id="94478-129">None</span></span>|<span data-ttu-id="94478-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94478-130">Not yet documented</span></span>|
|[<span data-ttu-id="94478-131">exportMobileConfig 函数</span><span class="sxs-lookup"><span data-stu-id="94478-131">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="94478-132">String</span><span class="sxs-lookup"><span data-stu-id="94478-132">String</span></span>|<span data-ttu-id="94478-133">导出移动配置</span><span class="sxs-lookup"><span data-stu-id="94478-133">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="94478-134">updateDeviceProfileAssignment 操作</span><span class="sxs-lookup"><span data-stu-id="94478-134">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="94478-135">无</span><span class="sxs-lookup"><span data-stu-id="94478-135">None</span></span>|<span data-ttu-id="94478-136">尚未记录</span><span class="sxs-lookup"><span data-stu-id="94478-136">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="94478-137">属性</span><span class="sxs-lookup"><span data-stu-id="94478-137">Properties</span></span>
|<span data-ttu-id="94478-138">属性</span><span class="sxs-lookup"><span data-stu-id="94478-138">Property</span></span>|<span data-ttu-id="94478-139">类型</span><span class="sxs-lookup"><span data-stu-id="94478-139">Type</span></span>|<span data-ttu-id="94478-140">说明</span><span class="sxs-lookup"><span data-stu-id="94478-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94478-141">id</span><span class="sxs-lookup"><span data-stu-id="94478-141">id</span></span>|<span data-ttu-id="94478-142">字符串</span><span class="sxs-lookup"><span data-stu-id="94478-142">String</span></span>|<span data-ttu-id="94478-143">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="94478-143">The GUID for the object</span></span>|
|<span data-ttu-id="94478-144">displayName</span><span class="sxs-lookup"><span data-stu-id="94478-144">displayName</span></span>|<span data-ttu-id="94478-145">String</span><span class="sxs-lookup"><span data-stu-id="94478-145">String</span></span>|<span data-ttu-id="94478-146">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="94478-146">Name of the profile</span></span>|
|<span data-ttu-id="94478-147">description</span><span class="sxs-lookup"><span data-stu-id="94478-147">description</span></span>|<span data-ttu-id="94478-148">String</span><span class="sxs-lookup"><span data-stu-id="94478-148">String</span></span>|<span data-ttu-id="94478-149">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="94478-149">Description of the profile</span></span>|
|<span data-ttu-id="94478-150">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="94478-150">requiresUserAuthentication</span></span>|<span data-ttu-id="94478-151">布尔值</span><span class="sxs-lookup"><span data-stu-id="94478-151">Boolean</span></span>|<span data-ttu-id="94478-152">指示配置文件是否需要用户身份验证</span><span class="sxs-lookup"><span data-stu-id="94478-152">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="94478-153">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="94478-153">configurationEndpointUrl</span></span>|<span data-ttu-id="94478-154">String</span><span class="sxs-lookup"><span data-stu-id="94478-154">String</span></span>|<span data-ttu-id="94478-155">用于注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="94478-155">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="94478-156">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="94478-156">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="94478-157">布尔值</span><span class="sxs-lookup"><span data-stu-id="94478-157">Boolean</span></span>|<span data-ttu-id="94478-158">指示使用 Apple Setup 助理 (而不是公司门户) 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="94478-158">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="94478-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="94478-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="94478-160">布尔值</span><span class="sxs-lookup"><span data-stu-id="94478-160">Boolean</span></span>|<span data-ttu-id="94478-161">指示在安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="94478-161">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="94478-162">关系</span><span class="sxs-lookup"><span data-stu-id="94478-162">Relationships</span></span>
<span data-ttu-id="94478-163">无</span><span class="sxs-lookup"><span data-stu-id="94478-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94478-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94478-164">JSON Representation</span></span>
<span data-ttu-id="94478-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94478-165">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```





