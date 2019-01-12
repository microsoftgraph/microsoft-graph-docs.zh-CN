---
title: enrollmentProfile 资源类型
description: EnrollmentProfile 资源表示它必须提供预注册启用注册其标识已预暂存某些设备配置的集合。 预暂存的设备标识分配给此类型的配置文件，以应用在相应的设备的注册的配置文件的配置。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: b88745c060e71e32199a96b23f94fa0d3229d451
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935589"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="d2eef-104">enrollmentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2eef-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="d2eef-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d2eef-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2eef-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d2eef-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2eef-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d2eef-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2eef-108">EnrollmentProfile 资源表示它必须提供预注册启用注册其标识已预暂存某些设备配置的集合。</span><span class="sxs-lookup"><span data-stu-id="d2eef-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="d2eef-109">预暂存的设备标识分配给此类型的配置文件，以应用在相应的设备的注册的配置文件的配置。</span><span class="sxs-lookup"><span data-stu-id="d2eef-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>
## <a name="methods"></a><span data-ttu-id="d2eef-110">方法</span><span class="sxs-lookup"><span data-stu-id="d2eef-110">Methods</span></span>
|<span data-ttu-id="d2eef-111">方法</span><span class="sxs-lookup"><span data-stu-id="d2eef-111">Method</span></span>|<span data-ttu-id="d2eef-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2eef-112">Return Type</span></span>|<span data-ttu-id="d2eef-113">说明</span><span class="sxs-lookup"><span data-stu-id="d2eef-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2eef-114">列表 enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="d2eef-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="d2eef-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="d2eef-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="d2eef-116">列出属性和[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="d2eef-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="d2eef-117">获取 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d2eef-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="d2eef-118">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d2eef-118">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="d2eef-119">读取属性和[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="d2eef-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="d2eef-120">创建 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d2eef-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="d2eef-121">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d2eef-121">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="d2eef-122">创建新的[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d2eef-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="d2eef-123">删除 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d2eef-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="d2eef-124">无</span><span class="sxs-lookup"><span data-stu-id="d2eef-124">None</span></span>|<span data-ttu-id="d2eef-125">删除[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="d2eef-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="d2eef-126">更新 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d2eef-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="d2eef-127">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d2eef-127">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="d2eef-128">更新[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d2eef-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="d2eef-129">setDefaultProfile 操作</span><span class="sxs-lookup"><span data-stu-id="d2eef-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="d2eef-130">无</span><span class="sxs-lookup"><span data-stu-id="d2eef-130">None</span></span>|<span data-ttu-id="d2eef-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d2eef-131">Not yet documented</span></span>|
|[<span data-ttu-id="d2eef-132">exportMobileConfig 函数</span><span class="sxs-lookup"><span data-stu-id="d2eef-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="d2eef-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d2eef-133">String</span></span>|<span data-ttu-id="d2eef-134">导出移动配置</span><span class="sxs-lookup"><span data-stu-id="d2eef-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="d2eef-135">updateDeviceProfileAssignment 操作</span><span class="sxs-lookup"><span data-stu-id="d2eef-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="d2eef-136">无</span><span class="sxs-lookup"><span data-stu-id="d2eef-136">None</span></span>|<span data-ttu-id="d2eef-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d2eef-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d2eef-138">属性</span><span class="sxs-lookup"><span data-stu-id="d2eef-138">Properties</span></span>
|<span data-ttu-id="d2eef-139">属性</span><span class="sxs-lookup"><span data-stu-id="d2eef-139">Property</span></span>|<span data-ttu-id="d2eef-140">类型</span><span class="sxs-lookup"><span data-stu-id="d2eef-140">Type</span></span>|<span data-ttu-id="d2eef-141">说明</span><span class="sxs-lookup"><span data-stu-id="d2eef-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2eef-142">id</span><span class="sxs-lookup"><span data-stu-id="d2eef-142">id</span></span>|<span data-ttu-id="d2eef-143">字符串</span><span class="sxs-lookup"><span data-stu-id="d2eef-143">String</span></span>|<span data-ttu-id="d2eef-144">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="d2eef-144">The GUID for the object</span></span>|
|<span data-ttu-id="d2eef-145">displayName</span><span class="sxs-lookup"><span data-stu-id="d2eef-145">displayName</span></span>|<span data-ttu-id="d2eef-146">字符串</span><span class="sxs-lookup"><span data-stu-id="d2eef-146">String</span></span>|<span data-ttu-id="d2eef-147">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="d2eef-147">Name of the profile</span></span>|
|<span data-ttu-id="d2eef-148">说明</span><span class="sxs-lookup"><span data-stu-id="d2eef-148">description</span></span>|<span data-ttu-id="d2eef-149">字符串</span><span class="sxs-lookup"><span data-stu-id="d2eef-149">String</span></span>|<span data-ttu-id="d2eef-150">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="d2eef-150">Description of the profile</span></span>|
|<span data-ttu-id="d2eef-151">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="d2eef-151">requiresUserAuthentication</span></span>|<span data-ttu-id="d2eef-152">布尔</span><span class="sxs-lookup"><span data-stu-id="d2eef-152">Boolean</span></span>|<span data-ttu-id="d2eef-153">指示该配置文件是否要求用户身份验证</span><span class="sxs-lookup"><span data-stu-id="d2eef-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="d2eef-154">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="d2eef-154">configurationEndpointUrl</span></span>|<span data-ttu-id="d2eef-155">字符串</span><span class="sxs-lookup"><span data-stu-id="d2eef-155">String</span></span>|<span data-ttu-id="d2eef-156">配置用于注册的终结点 url</span><span class="sxs-lookup"><span data-stu-id="d2eef-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="d2eef-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="d2eef-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="d2eef-158">布尔</span><span class="sxs-lookup"><span data-stu-id="d2eef-158">Boolean</span></span>|<span data-ttu-id="d2eef-159">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="d2eef-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2eef-160">Relationships</span><span class="sxs-lookup"><span data-stu-id="d2eef-160">Relationships</span></span>
<span data-ttu-id="d2eef-161">无</span><span class="sxs-lookup"><span data-stu-id="d2eef-161">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d2eef-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2eef-162">JSON Representation</span></span>
<span data-ttu-id="d2eef-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2eef-163">Here is a JSON representation of the resource.</span></span>
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
  "enableAuthenticationViaCompanyPortal": true
}
```





