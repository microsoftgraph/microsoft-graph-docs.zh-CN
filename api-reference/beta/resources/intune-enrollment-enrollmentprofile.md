---
title: enrollmentProfile 资源类型
description: EnrollmentProfile 资源表示必须提供预注册的配置的集合，以便能够注册已预暂存其标识的某些设备。 预暂存的设备标识分配给此类型的配置文件，以便在注册相应设备时应用配置文件的配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f848ca73088a360ed098a612338d8e52e5078518
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528304"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="26a8f-104">enrollmentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="26a8f-104">enrollmentProfile resource type</span></span>

<span data-ttu-id="26a8f-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="26a8f-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="26a8f-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="26a8f-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26a8f-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26a8f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26a8f-108">EnrollmentProfile 资源表示必须提供预注册的配置的集合，以便能够注册已预暂存其标识的某些设备。</span><span class="sxs-lookup"><span data-stu-id="26a8f-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="26a8f-109">预暂存的设备标识分配给此类型的配置文件，以便在注册相应设备时应用配置文件的配置。</span><span class="sxs-lookup"><span data-stu-id="26a8f-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="26a8f-110">方法</span><span class="sxs-lookup"><span data-stu-id="26a8f-110">Methods</span></span>
|<span data-ttu-id="26a8f-111">方法</span><span class="sxs-lookup"><span data-stu-id="26a8f-111">Method</span></span>|<span data-ttu-id="26a8f-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="26a8f-112">Return Type</span></span>|<span data-ttu-id="26a8f-113">说明</span><span class="sxs-lookup"><span data-stu-id="26a8f-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="26a8f-114">列出 enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="26a8f-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="26a8f-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="26a8f-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="26a8f-116">列出[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="26a8f-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="26a8f-117">获取 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="26a8f-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="26a8f-118">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="26a8f-118">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="26a8f-119">读取[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="26a8f-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="26a8f-120">创建 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="26a8f-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="26a8f-121">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="26a8f-121">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="26a8f-122">创建新的[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="26a8f-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="26a8f-123">删除 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="26a8f-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="26a8f-124">无</span><span class="sxs-lookup"><span data-stu-id="26a8f-124">None</span></span>|<span data-ttu-id="26a8f-125">删除[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="26a8f-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="26a8f-126">更新 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="26a8f-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="26a8f-127">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="26a8f-127">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="26a8f-128">更新[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="26a8f-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="26a8f-129">setDefaultProfile 操作</span><span class="sxs-lookup"><span data-stu-id="26a8f-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="26a8f-130">无</span><span class="sxs-lookup"><span data-stu-id="26a8f-130">None</span></span>|<span data-ttu-id="26a8f-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="26a8f-131">Not yet documented</span></span>|
|[<span data-ttu-id="26a8f-132">exportMobileConfig 函数</span><span class="sxs-lookup"><span data-stu-id="26a8f-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="26a8f-133">String</span><span class="sxs-lookup"><span data-stu-id="26a8f-133">String</span></span>|<span data-ttu-id="26a8f-134">导出移动配置</span><span class="sxs-lookup"><span data-stu-id="26a8f-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="26a8f-135">updateDeviceProfileAssignment 操作</span><span class="sxs-lookup"><span data-stu-id="26a8f-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="26a8f-136">无</span><span class="sxs-lookup"><span data-stu-id="26a8f-136">None</span></span>|<span data-ttu-id="26a8f-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="26a8f-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="26a8f-138">属性</span><span class="sxs-lookup"><span data-stu-id="26a8f-138">Properties</span></span>
|<span data-ttu-id="26a8f-139">属性</span><span class="sxs-lookup"><span data-stu-id="26a8f-139">Property</span></span>|<span data-ttu-id="26a8f-140">类型</span><span class="sxs-lookup"><span data-stu-id="26a8f-140">Type</span></span>|<span data-ttu-id="26a8f-141">说明</span><span class="sxs-lookup"><span data-stu-id="26a8f-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26a8f-142">id</span><span class="sxs-lookup"><span data-stu-id="26a8f-142">id</span></span>|<span data-ttu-id="26a8f-143">字符串</span><span class="sxs-lookup"><span data-stu-id="26a8f-143">String</span></span>|<span data-ttu-id="26a8f-144">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="26a8f-144">The GUID for the object</span></span>|
|<span data-ttu-id="26a8f-145">displayName</span><span class="sxs-lookup"><span data-stu-id="26a8f-145">displayName</span></span>|<span data-ttu-id="26a8f-146">String</span><span class="sxs-lookup"><span data-stu-id="26a8f-146">String</span></span>|<span data-ttu-id="26a8f-147">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="26a8f-147">Name of the profile</span></span>|
|<span data-ttu-id="26a8f-148">说明</span><span class="sxs-lookup"><span data-stu-id="26a8f-148">description</span></span>|<span data-ttu-id="26a8f-149">String</span><span class="sxs-lookup"><span data-stu-id="26a8f-149">String</span></span>|<span data-ttu-id="26a8f-150">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="26a8f-150">Description of the profile</span></span>|
|<span data-ttu-id="26a8f-151">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="26a8f-151">requiresUserAuthentication</span></span>|<span data-ttu-id="26a8f-152">布尔</span><span class="sxs-lookup"><span data-stu-id="26a8f-152">Boolean</span></span>|<span data-ttu-id="26a8f-153">指示配置文件是否需要用户身份验证</span><span class="sxs-lookup"><span data-stu-id="26a8f-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="26a8f-154">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="26a8f-154">configurationEndpointUrl</span></span>|<span data-ttu-id="26a8f-155">String</span><span class="sxs-lookup"><span data-stu-id="26a8f-155">String</span></span>|<span data-ttu-id="26a8f-156">用于注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="26a8f-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="26a8f-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="26a8f-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="26a8f-158">布尔</span><span class="sxs-lookup"><span data-stu-id="26a8f-158">Boolean</span></span>|<span data-ttu-id="26a8f-159">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="26a8f-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="26a8f-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="26a8f-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="26a8f-161">布尔</span><span class="sxs-lookup"><span data-stu-id="26a8f-161">Boolean</span></span>|<span data-ttu-id="26a8f-162">指示在安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="26a8f-162">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="26a8f-163">关系</span><span class="sxs-lookup"><span data-stu-id="26a8f-163">Relationships</span></span>
<span data-ttu-id="26a8f-164">无</span><span class="sxs-lookup"><span data-stu-id="26a8f-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26a8f-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26a8f-165">JSON Representation</span></span>
<span data-ttu-id="26a8f-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26a8f-166">Here is a JSON representation of the resource.</span></span>
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



