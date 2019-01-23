---
title: enrollmentProfile 资源类型
description: EnrollmentProfile 资源表示它必须提供预注册启用注册其标识已预暂存某些设备配置的集合。 预暂存的设备标识分配给此类型的配置文件，以应用在相应的设备的注册的配置文件的配置。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a7ce4aac1e22610d539419dd6a63d124616b83f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396838"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="e2b4e-104">enrollmentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2b4e-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="e2b4e-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e2b4e-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e2b4e-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e2b4e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2b4e-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2b4e-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2b4e-108">EnrollmentProfile 资源表示它必须提供预注册启用注册其标识已预暂存某些设备配置的集合。</span><span class="sxs-lookup"><span data-stu-id="e2b4e-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="e2b4e-109">预暂存的设备标识分配给此类型的配置文件，以应用在相应的设备的注册的配置文件的配置。</span><span class="sxs-lookup"><span data-stu-id="e2b4e-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="e2b4e-110">方法</span><span class="sxs-lookup"><span data-stu-id="e2b4e-110">Methods</span></span>
|<span data-ttu-id="e2b4e-111">方法</span><span class="sxs-lookup"><span data-stu-id="e2b4e-111">Method</span></span>|<span data-ttu-id="e2b4e-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="e2b4e-112">Return Type</span></span>|<span data-ttu-id="e2b4e-113">说明</span><span class="sxs-lookup"><span data-stu-id="e2b4e-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e2b4e-114">列表 enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="e2b4e-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="e2b4e-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="e2b4e-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="e2b4e-116">列出属性和[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="e2b4e-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="e2b4e-117">获取 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e2b4e-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="e2b4e-118">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e2b4e-118">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="e2b4e-119">读取属性和[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="e2b4e-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="e2b4e-120">创建 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e2b4e-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="e2b4e-121">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e2b4e-121">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="e2b4e-122">创建新的[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e2b4e-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="e2b4e-123">删除 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e2b4e-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="e2b4e-124">无</span><span class="sxs-lookup"><span data-stu-id="e2b4e-124">None</span></span>|<span data-ttu-id="e2b4e-125">删除[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="e2b4e-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="e2b4e-126">更新 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e2b4e-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="e2b4e-127">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e2b4e-127">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="e2b4e-128">更新[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e2b4e-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="e2b4e-129">setDefaultProfile 操作</span><span class="sxs-lookup"><span data-stu-id="e2b4e-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="e2b4e-130">无</span><span class="sxs-lookup"><span data-stu-id="e2b4e-130">None</span></span>|<span data-ttu-id="e2b4e-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e2b4e-131">Not yet documented</span></span>|
|[<span data-ttu-id="e2b4e-132">exportMobileConfig 函数</span><span class="sxs-lookup"><span data-stu-id="e2b4e-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="e2b4e-133">String</span><span class="sxs-lookup"><span data-stu-id="e2b4e-133">String</span></span>|<span data-ttu-id="e2b4e-134">导出移动配置</span><span class="sxs-lookup"><span data-stu-id="e2b4e-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="e2b4e-135">updateDeviceProfileAssignment 操作</span><span class="sxs-lookup"><span data-stu-id="e2b4e-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="e2b4e-136">无</span><span class="sxs-lookup"><span data-stu-id="e2b4e-136">None</span></span>|<span data-ttu-id="e2b4e-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e2b4e-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e2b4e-138">属性</span><span class="sxs-lookup"><span data-stu-id="e2b4e-138">Properties</span></span>
|<span data-ttu-id="e2b4e-139">属性</span><span class="sxs-lookup"><span data-stu-id="e2b4e-139">Property</span></span>|<span data-ttu-id="e2b4e-140">类型</span><span class="sxs-lookup"><span data-stu-id="e2b4e-140">Type</span></span>|<span data-ttu-id="e2b4e-141">说明</span><span class="sxs-lookup"><span data-stu-id="e2b4e-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2b4e-142">id</span><span class="sxs-lookup"><span data-stu-id="e2b4e-142">id</span></span>|<span data-ttu-id="e2b4e-143">String</span><span class="sxs-lookup"><span data-stu-id="e2b4e-143">String</span></span>|<span data-ttu-id="e2b4e-144">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="e2b4e-144">The GUID for the object</span></span>|
|<span data-ttu-id="e2b4e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e2b4e-145">displayName</span></span>|<span data-ttu-id="e2b4e-146">String</span><span class="sxs-lookup"><span data-stu-id="e2b4e-146">String</span></span>|<span data-ttu-id="e2b4e-147">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="e2b4e-147">Name of the profile</span></span>|
|<span data-ttu-id="e2b4e-148">说明</span><span class="sxs-lookup"><span data-stu-id="e2b4e-148">description</span></span>|<span data-ttu-id="e2b4e-149">String</span><span class="sxs-lookup"><span data-stu-id="e2b4e-149">String</span></span>|<span data-ttu-id="e2b4e-150">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="e2b4e-150">Description of the profile</span></span>|
|<span data-ttu-id="e2b4e-151">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="e2b4e-151">requiresUserAuthentication</span></span>|<span data-ttu-id="e2b4e-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b4e-152">Boolean</span></span>|<span data-ttu-id="e2b4e-153">指示该配置文件是否要求用户身份验证</span><span class="sxs-lookup"><span data-stu-id="e2b4e-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="e2b4e-154">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="e2b4e-154">configurationEndpointUrl</span></span>|<span data-ttu-id="e2b4e-155">String</span><span class="sxs-lookup"><span data-stu-id="e2b4e-155">String</span></span>|<span data-ttu-id="e2b4e-156">配置用于注册的终结点 url</span><span class="sxs-lookup"><span data-stu-id="e2b4e-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="e2b4e-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="e2b4e-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="e2b4e-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b4e-158">Boolean</span></span>|<span data-ttu-id="e2b4e-159">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e2b4e-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="e2b4e-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="e2b4e-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="e2b4e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2b4e-161">Boolean</span></span>|<span data-ttu-id="e2b4e-162">表示安装程序注册的助手设备上必须的公司门户</span><span class="sxs-lookup"><span data-stu-id="e2b4e-162">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2b4e-163">关系</span><span class="sxs-lookup"><span data-stu-id="e2b4e-163">Relationships</span></span>
<span data-ttu-id="e2b4e-164">无</span><span class="sxs-lookup"><span data-stu-id="e2b4e-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2b4e-165">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2b4e-165">JSON Representation</span></span>
<span data-ttu-id="e2b4e-166">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2b4e-166">Here is a JSON representation of the resource.</span></span>
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




