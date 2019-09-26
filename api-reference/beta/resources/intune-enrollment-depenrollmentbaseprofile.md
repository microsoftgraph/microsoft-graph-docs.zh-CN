---
title: depEnrollmentBaseProfile 资源类型
description: DepEnrollmentBaseProfile 资源表示 Apple 设备注册计划（DEP）注册配置文件。 在相应的设备可以通过 DEP 进行注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0698380f3fb69323275a8c2db3725ddb741f2151
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196614"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="9266b-104">depEnrollmentBaseProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="9266b-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="9266b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9266b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9266b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9266b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9266b-107">DepEnrollmentBaseProfile 资源表示 Apple 设备注册计划（DEP）注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="9266b-107">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="9266b-108">在相应的设备可以通过 DEP 进行注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号。</span><span class="sxs-lookup"><span data-stu-id="9266b-108">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="9266b-109">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9266b-109">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9266b-110">方法</span><span class="sxs-lookup"><span data-stu-id="9266b-110">Methods</span></span>
|<span data-ttu-id="9266b-111">方法</span><span class="sxs-lookup"><span data-stu-id="9266b-111">Method</span></span>|<span data-ttu-id="9266b-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="9266b-112">Return Type</span></span>|<span data-ttu-id="9266b-113">说明</span><span class="sxs-lookup"><span data-stu-id="9266b-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9266b-114">列出 depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="9266b-114">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="9266b-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="9266b-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="9266b-116">列出[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9266b-116">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="9266b-117">获取 depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="9266b-117">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="9266b-118">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="9266b-118">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="9266b-119">读取[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9266b-119">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9266b-120">属性</span><span class="sxs-lookup"><span data-stu-id="9266b-120">Properties</span></span>
|<span data-ttu-id="9266b-121">属性</span><span class="sxs-lookup"><span data-stu-id="9266b-121">Property</span></span>|<span data-ttu-id="9266b-122">类型</span><span class="sxs-lookup"><span data-stu-id="9266b-122">Type</span></span>|<span data-ttu-id="9266b-123">说明</span><span class="sxs-lookup"><span data-stu-id="9266b-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9266b-124">id</span><span class="sxs-lookup"><span data-stu-id="9266b-124">id</span></span>|<span data-ttu-id="9266b-125">字符串</span><span class="sxs-lookup"><span data-stu-id="9266b-125">String</span></span>|<span data-ttu-id="9266b-126">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="9266b-126">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9266b-127">displayName</span><span class="sxs-lookup"><span data-stu-id="9266b-127">displayName</span></span>|<span data-ttu-id="9266b-128">String</span><span class="sxs-lookup"><span data-stu-id="9266b-128">String</span></span>|<span data-ttu-id="9266b-129">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="9266b-129">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9266b-130">说明</span><span class="sxs-lookup"><span data-stu-id="9266b-130">description</span></span>|<span data-ttu-id="9266b-131">String</span><span class="sxs-lookup"><span data-stu-id="9266b-131">String</span></span>|<span data-ttu-id="9266b-132">从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="9266b-132">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9266b-133">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="9266b-133">requiresUserAuthentication</span></span>|<span data-ttu-id="9266b-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-134">Boolean</span></span>|<span data-ttu-id="9266b-135">指示配置文件是否需要从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="9266b-135">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9266b-136">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="9266b-136">configurationEndpointUrl</span></span>|<span data-ttu-id="9266b-137">String</span><span class="sxs-lookup"><span data-stu-id="9266b-137">String</span></span>|<span data-ttu-id="9266b-138">用于从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="9266b-138">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9266b-139">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="9266b-139">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="9266b-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-140">Boolean</span></span>|<span data-ttu-id="9266b-141">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="9266b-141">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="9266b-142">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="9266b-142">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9266b-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="9266b-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="9266b-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-144">Boolean</span></span>|<span data-ttu-id="9266b-145">指示在从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="9266b-145">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="9266b-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="9266b-146">isDefault</span></span>|<span data-ttu-id="9266b-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-147">Boolean</span></span>|<span data-ttu-id="9266b-148">指示这是否为默认配置文件</span><span class="sxs-lookup"><span data-stu-id="9266b-148">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="9266b-149">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="9266b-149">supervisedModeEnabled</span></span>|<span data-ttu-id="9266b-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-150">Boolean</span></span>|<span data-ttu-id="9266b-151">监督模式，如果启用，则为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="9266b-151">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="9266b-152">有关https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息，请参阅。</span><span class="sxs-lookup"><span data-stu-id="9266b-152">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="9266b-153">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="9266b-153">supportDepartment</span></span>|<span data-ttu-id="9266b-154">String</span><span class="sxs-lookup"><span data-stu-id="9266b-154">String</span></span>|<span data-ttu-id="9266b-155">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="9266b-155">Support department information</span></span>|
|<span data-ttu-id="9266b-156">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="9266b-156">passCodeDisabled</span></span>|<span data-ttu-id="9266b-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-157">Boolean</span></span>|<span data-ttu-id="9266b-158">指示是否禁用密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="9266b-158">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="9266b-159">isMandatory</span><span class="sxs-lookup"><span data-stu-id="9266b-159">isMandatory</span></span>|<span data-ttu-id="9266b-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-160">Boolean</span></span>|<span data-ttu-id="9266b-161">指示配置文件是否是必需的</span><span class="sxs-lookup"><span data-stu-id="9266b-161">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="9266b-162">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="9266b-162">locationDisabled</span></span>|<span data-ttu-id="9266b-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-163">Boolean</span></span>|<span data-ttu-id="9266b-164">指示是否禁用位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="9266b-164">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="9266b-165">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="9266b-165">supportPhoneNumber</span></span>|<span data-ttu-id="9266b-166">String</span><span class="sxs-lookup"><span data-stu-id="9266b-166">String</span></span>|<span data-ttu-id="9266b-167">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="9266b-167">Support phone number</span></span>|
|<span data-ttu-id="9266b-168">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="9266b-168">profileRemovalDisabled</span></span>|<span data-ttu-id="9266b-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-169">Boolean</span></span>|<span data-ttu-id="9266b-170">指示是否禁用了配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="9266b-170">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="9266b-171">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="9266b-171">restoreBlocked</span></span>|<span data-ttu-id="9266b-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-172">Boolean</span></span>|<span data-ttu-id="9266b-173">指示是否阻止还原安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="9266b-173">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="9266b-174">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="9266b-174">appleIdDisabled</span></span>|<span data-ttu-id="9266b-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-175">Boolean</span></span>|<span data-ttu-id="9266b-176">指示是否禁用 Apple id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="9266b-176">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="9266b-177">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="9266b-177">termsAndConditionsDisabled</span></span>|<span data-ttu-id="9266b-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-178">Boolean</span></span>|<span data-ttu-id="9266b-179">指示是否已禁用 "条款和条件" 安装窗格</span><span class="sxs-lookup"><span data-stu-id="9266b-179">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="9266b-180">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="9266b-180">touchIdDisabled</span></span>|<span data-ttu-id="9266b-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-181">Boolean</span></span>|<span data-ttu-id="9266b-182">指示是否禁用了触控 id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="9266b-182">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="9266b-183">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="9266b-183">applePayDisabled</span></span>|<span data-ttu-id="9266b-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-184">Boolean</span></span>|<span data-ttu-id="9266b-185">指示是否禁用 Apple 付费设置窗格</span><span class="sxs-lookup"><span data-stu-id="9266b-185">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="9266b-186">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="9266b-186">zoomDisabled</span></span>|<span data-ttu-id="9266b-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-187">Boolean</span></span>|<span data-ttu-id="9266b-188">指示是否禁用缩放设置窗格</span><span class="sxs-lookup"><span data-stu-id="9266b-188">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="9266b-189">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="9266b-189">siriDisabled</span></span>|<span data-ttu-id="9266b-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-190">Boolean</span></span>|<span data-ttu-id="9266b-191">指示是否禁用 siri 安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="9266b-191">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="9266b-192">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="9266b-192">diagnosticsDisabled</span></span>|<span data-ttu-id="9266b-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-193">Boolean</span></span>|<span data-ttu-id="9266b-194">指示是否禁用诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="9266b-194">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="9266b-195">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="9266b-195">displayToneSetupDisabled</span></span>|<span data-ttu-id="9266b-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-196">Boolean</span></span>|<span data-ttu-id="9266b-197">指示是否禁用 displaytone 安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="9266b-197">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="9266b-198">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="9266b-198">privacyPaneDisabled</span></span>|<span data-ttu-id="9266b-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-199">Boolean</span></span>|<span data-ttu-id="9266b-200">指示是否禁用隐私屏幕</span><span class="sxs-lookup"><span data-stu-id="9266b-200">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="9266b-201">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="9266b-201">screenTimeScreenDisabled</span></span>|<span data-ttu-id="9266b-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="9266b-202">Boolean</span></span>|<span data-ttu-id="9266b-203">指示是否禁用屏幕超时设置</span><span class="sxs-lookup"><span data-stu-id="9266b-203">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="9266b-204">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="9266b-204">deviceNameTemplate</span></span>|<span data-ttu-id="9266b-205">String</span><span class="sxs-lookup"><span data-stu-id="9266b-205">String</span></span>|<span data-ttu-id="9266b-206">设置文本或名称模式。</span><span class="sxs-lookup"><span data-stu-id="9266b-206">Sets a literal or name pattern.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9266b-207">关系</span><span class="sxs-lookup"><span data-stu-id="9266b-207">Relationships</span></span>
<span data-ttu-id="9266b-208">无</span><span class="sxs-lookup"><span data-stu-id="9266b-208">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9266b-209">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9266b-209">JSON Representation</span></span>
<span data-ttu-id="9266b-210">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9266b-210">Here is a JSON representation of the resource.</span></span>
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
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "String"
}
```



