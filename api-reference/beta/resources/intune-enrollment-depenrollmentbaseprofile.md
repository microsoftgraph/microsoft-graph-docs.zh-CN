---
title: depEnrollmentBaseProfile 资源类型
description: DepEnrollmentBaseProfile 资源表示 Apple 设备注册程序 (DEP) 注册配置文件。 相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f8b820959e5515a575e4f074a2762794a15e7f5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423753"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="a26a7-104">depEnrollmentBaseProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="a26a7-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="a26a7-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a26a7-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a26a7-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a26a7-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a26a7-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a26a7-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a26a7-108">DepEnrollmentBaseProfile 资源表示 Apple 设备注册程序 (DEP) 注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="a26a7-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="a26a7-109">相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号</span><span class="sxs-lookup"><span data-stu-id="a26a7-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="a26a7-110">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a26a7-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a26a7-111">方法</span><span class="sxs-lookup"><span data-stu-id="a26a7-111">Methods</span></span>
|<span data-ttu-id="a26a7-112">方法</span><span class="sxs-lookup"><span data-stu-id="a26a7-112">Method</span></span>|<span data-ttu-id="a26a7-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="a26a7-113">Return Type</span></span>|<span data-ttu-id="a26a7-114">说明</span><span class="sxs-lookup"><span data-stu-id="a26a7-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a26a7-115">列表 depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="a26a7-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="a26a7-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="a26a7-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="a26a7-117">列出属性和[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="a26a7-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="a26a7-118">获取 depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="a26a7-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="a26a7-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="a26a7-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="a26a7-120">读取属性和[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a26a7-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a26a7-121">属性</span><span class="sxs-lookup"><span data-stu-id="a26a7-121">Properties</span></span>
|<span data-ttu-id="a26a7-122">属性</span><span class="sxs-lookup"><span data-stu-id="a26a7-122">Property</span></span>|<span data-ttu-id="a26a7-123">类型</span><span class="sxs-lookup"><span data-stu-id="a26a7-123">Type</span></span>|<span data-ttu-id="a26a7-124">说明</span><span class="sxs-lookup"><span data-stu-id="a26a7-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a26a7-125">id</span><span class="sxs-lookup"><span data-stu-id="a26a7-125">id</span></span>|<span data-ttu-id="a26a7-126">String</span><span class="sxs-lookup"><span data-stu-id="a26a7-126">String</span></span>|<span data-ttu-id="a26a7-127">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象继承的 GUID</span><span class="sxs-lookup"><span data-stu-id="a26a7-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a26a7-128">displayName</span><span class="sxs-lookup"><span data-stu-id="a26a7-128">displayName</span></span>|<span data-ttu-id="a26a7-129">String</span><span class="sxs-lookup"><span data-stu-id="a26a7-129">String</span></span>|<span data-ttu-id="a26a7-130">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="a26a7-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a26a7-131">说明</span><span class="sxs-lookup"><span data-stu-id="a26a7-131">description</span></span>|<span data-ttu-id="a26a7-132">String</span><span class="sxs-lookup"><span data-stu-id="a26a7-132">String</span></span>|<span data-ttu-id="a26a7-133">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="a26a7-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a26a7-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="a26a7-134">requiresUserAuthentication</span></span>|<span data-ttu-id="a26a7-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-135">Boolean</span></span>|<span data-ttu-id="a26a7-136">指示该配置文件是否要求来自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)用户身份验证继承</span><span class="sxs-lookup"><span data-stu-id="a26a7-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a26a7-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="a26a7-137">configurationEndpointUrl</span></span>|<span data-ttu-id="a26a7-138">String</span><span class="sxs-lookup"><span data-stu-id="a26a7-138">String</span></span>|<span data-ttu-id="a26a7-139">配置终结点 url，用于注册继承从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a26a7-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a26a7-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="a26a7-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="a26a7-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-141">Boolean</span></span>|<span data-ttu-id="a26a7-142">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="a26a7-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="a26a7-143">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a26a7-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a26a7-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="a26a7-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="a26a7-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-145">Boolean</span></span>|<span data-ttu-id="a26a7-146">指示安装程序注册的助手设备继承[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) ，需要的公司门户</span><span class="sxs-lookup"><span data-stu-id="a26a7-146">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a26a7-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="a26a7-147">isDefault</span></span>|<span data-ttu-id="a26a7-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-148">Boolean</span></span>|<span data-ttu-id="a26a7-149">指示是否这是默认配置文件</span><span class="sxs-lookup"><span data-stu-id="a26a7-149">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="a26a7-150">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="a26a7-150">supervisedModeEnabled</span></span>|<span data-ttu-id="a26a7-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-151">Boolean</span></span>|<span data-ttu-id="a26a7-152">监管模式下，设置为 True 可启用，false 否则。</span><span class="sxs-lookup"><span data-stu-id="a26a7-152">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="a26a7-153">请参阅https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune的其他信息。</span><span class="sxs-lookup"><span data-stu-id="a26a7-153">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="a26a7-154">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="a26a7-154">supportDepartment</span></span>|<span data-ttu-id="a26a7-155">String</span><span class="sxs-lookup"><span data-stu-id="a26a7-155">String</span></span>|<span data-ttu-id="a26a7-156">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="a26a7-156">Support department information</span></span>|
|<span data-ttu-id="a26a7-157">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="a26a7-157">passCodeDisabled</span></span>|<span data-ttu-id="a26a7-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-158">Boolean</span></span>|<span data-ttu-id="a26a7-159">指示是否密码设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="a26a7-159">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="a26a7-160">isMandatory</span><span class="sxs-lookup"><span data-stu-id="a26a7-160">isMandatory</span></span>|<span data-ttu-id="a26a7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-161">Boolean</span></span>|<span data-ttu-id="a26a7-162">指示是否强制配置文件</span><span class="sxs-lookup"><span data-stu-id="a26a7-162">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="a26a7-163">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="a26a7-163">locationDisabled</span></span>|<span data-ttu-id="a26a7-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-164">Boolean</span></span>|<span data-ttu-id="a26a7-165">指示是否位置服务设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="a26a7-165">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="a26a7-166">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="a26a7-166">supportPhoneNumber</span></span>|<span data-ttu-id="a26a7-167">String</span><span class="sxs-lookup"><span data-stu-id="a26a7-167">String</span></span>|<span data-ttu-id="a26a7-168">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="a26a7-168">Support phone number</span></span>|
|<span data-ttu-id="a26a7-169">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="a26a7-169">profileRemovalDisabled</span></span>|<span data-ttu-id="a26a7-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-170">Boolean</span></span>|<span data-ttu-id="a26a7-171">指示是否已禁用配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="a26a7-171">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="a26a7-172">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="a26a7-172">restoreBlocked</span></span>|<span data-ttu-id="a26a7-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-173">Boolean</span></span>|<span data-ttu-id="a26a7-174">指示是否还原设置窗格被阻止</span><span class="sxs-lookup"><span data-stu-id="a26a7-174">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="a26a7-175">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="a26a7-175">appleIdDisabled</span></span>|<span data-ttu-id="a26a7-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-176">Boolean</span></span>|<span data-ttu-id="a26a7-177">指示是否 Apple id 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="a26a7-177">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="a26a7-178">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="a26a7-178">termsAndConditionsDisabled</span></span>|<span data-ttu-id="a26a7-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-179">Boolean</span></span>|<span data-ttu-id="a26a7-180">指示是否已禁用条款和条件设置窗格</span><span class="sxs-lookup"><span data-stu-id="a26a7-180">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="a26a7-181">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="a26a7-181">touchIdDisabled</span></span>|<span data-ttu-id="a26a7-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-182">Boolean</span></span>|<span data-ttu-id="a26a7-183">指示是否触摸 id 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="a26a7-183">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="a26a7-184">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="a26a7-184">applePayDisabled</span></span>|<span data-ttu-id="a26a7-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-185">Boolean</span></span>|<span data-ttu-id="a26a7-186">指示是否 Apple 付薪设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="a26a7-186">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="a26a7-187">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="a26a7-187">zoomDisabled</span></span>|<span data-ttu-id="a26a7-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-188">Boolean</span></span>|<span data-ttu-id="a26a7-189">指示是否缩放设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="a26a7-189">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="a26a7-190">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="a26a7-190">siriDisabled</span></span>|<span data-ttu-id="a26a7-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-191">Boolean</span></span>|<span data-ttu-id="a26a7-192">指示是否 siri 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="a26a7-192">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="a26a7-193">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="a26a7-193">diagnosticsDisabled</span></span>|<span data-ttu-id="a26a7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-194">Boolean</span></span>|<span data-ttu-id="a26a7-195">指示是否诊断设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="a26a7-195">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="a26a7-196">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="a26a7-196">displayToneSetupDisabled</span></span>|<span data-ttu-id="a26a7-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-197">Boolean</span></span>|<span data-ttu-id="a26a7-198">指示是否禁用 displaytone 设置屏幕</span><span class="sxs-lookup"><span data-stu-id="a26a7-198">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="a26a7-199">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="a26a7-199">privacyPaneDisabled</span></span>|<span data-ttu-id="a26a7-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="a26a7-200">Boolean</span></span>|<span data-ttu-id="a26a7-201">指示是否禁用隐私屏幕</span><span class="sxs-lookup"><span data-stu-id="a26a7-201">Indicates if privacy screen is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="a26a7-202">关系</span><span class="sxs-lookup"><span data-stu-id="a26a7-202">Relationships</span></span>
<span data-ttu-id="a26a7-203">无</span><span class="sxs-lookup"><span data-stu-id="a26a7-203">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a26a7-204">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a26a7-204">JSON Representation</span></span>
<span data-ttu-id="a26a7-205">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a26a7-205">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentBaseProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true
}
```




