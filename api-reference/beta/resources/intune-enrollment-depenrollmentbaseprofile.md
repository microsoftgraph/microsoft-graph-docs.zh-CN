---
title: depEnrollmentBaseProfile 资源类型
description: DepEnrollmentBaseProfile 资源表示 Apple 设备注册计划 (DEP) 注册配置文件。 在相应的设备可以通过 DEP 进行注册之前, 必须将此类型的配置文件分配给 Apple DEP 序列号。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0b33d4c8ed70c5391d1bc5f85761dfac6f61a76
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941658"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="1fff5-104">depEnrollmentBaseProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="1fff5-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="1fff5-105">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1fff5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fff5-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1fff5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fff5-107">DepEnrollmentBaseProfile 资源表示 Apple 设备注册计划 (DEP) 注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="1fff5-107">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="1fff5-108">在相应的设备可以通过 DEP 进行注册之前, 必须将此类型的配置文件分配给 Apple DEP 序列号。</span><span class="sxs-lookup"><span data-stu-id="1fff5-108">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="1fff5-109">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1fff5-109">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1fff5-110">方法</span><span class="sxs-lookup"><span data-stu-id="1fff5-110">Methods</span></span>
|<span data-ttu-id="1fff5-111">方法</span><span class="sxs-lookup"><span data-stu-id="1fff5-111">Method</span></span>|<span data-ttu-id="1fff5-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="1fff5-112">Return Type</span></span>|<span data-ttu-id="1fff5-113">说明</span><span class="sxs-lookup"><span data-stu-id="1fff5-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1fff5-114">列出 depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="1fff5-114">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="1fff5-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="1fff5-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="1fff5-116">列出[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1fff5-116">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="1fff5-117">获取 depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="1fff5-117">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="1fff5-118">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="1fff5-118">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="1fff5-119">读取[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1fff5-119">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1fff5-120">属性</span><span class="sxs-lookup"><span data-stu-id="1fff5-120">Properties</span></span>
|<span data-ttu-id="1fff5-121">属性</span><span class="sxs-lookup"><span data-stu-id="1fff5-121">Property</span></span>|<span data-ttu-id="1fff5-122">类型</span><span class="sxs-lookup"><span data-stu-id="1fff5-122">Type</span></span>|<span data-ttu-id="1fff5-123">说明</span><span class="sxs-lookup"><span data-stu-id="1fff5-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fff5-124">id</span><span class="sxs-lookup"><span data-stu-id="1fff5-124">id</span></span>|<span data-ttu-id="1fff5-125">字符串</span><span class="sxs-lookup"><span data-stu-id="1fff5-125">String</span></span>|<span data-ttu-id="1fff5-126">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="1fff5-126">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fff5-127">displayName</span><span class="sxs-lookup"><span data-stu-id="1fff5-127">displayName</span></span>|<span data-ttu-id="1fff5-128">String</span><span class="sxs-lookup"><span data-stu-id="1fff5-128">String</span></span>|<span data-ttu-id="1fff5-129">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="1fff5-129">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fff5-130">说明</span><span class="sxs-lookup"><span data-stu-id="1fff5-130">description</span></span>|<span data-ttu-id="1fff5-131">String</span><span class="sxs-lookup"><span data-stu-id="1fff5-131">String</span></span>|<span data-ttu-id="1fff5-132">从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="1fff5-132">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fff5-133">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="1fff5-133">requiresUserAuthentication</span></span>|<span data-ttu-id="1fff5-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-134">Boolean</span></span>|<span data-ttu-id="1fff5-135">指示配置文件是否需要从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="1fff5-135">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fff5-136">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="1fff5-136">configurationEndpointUrl</span></span>|<span data-ttu-id="1fff5-137">String</span><span class="sxs-lookup"><span data-stu-id="1fff5-137">String</span></span>|<span data-ttu-id="1fff5-138">用于从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="1fff5-138">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fff5-139">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="1fff5-139">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="1fff5-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-140">Boolean</span></span>|<span data-ttu-id="1fff5-141">指示使用 Apple Setup 助理 (而不是公司门户) 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="1fff5-141">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="1fff5-142">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1fff5-142">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fff5-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="1fff5-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="1fff5-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-144">Boolean</span></span>|<span data-ttu-id="1fff5-145">指示在从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="1fff5-145">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1fff5-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="1fff5-146">isDefault</span></span>|<span data-ttu-id="1fff5-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-147">Boolean</span></span>|<span data-ttu-id="1fff5-148">指示这是否为默认配置文件</span><span class="sxs-lookup"><span data-stu-id="1fff5-148">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="1fff5-149">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="1fff5-149">supervisedModeEnabled</span></span>|<span data-ttu-id="1fff5-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-150">Boolean</span></span>|<span data-ttu-id="1fff5-151">监督模式, 如果启用, 则为 True, 否则为 false。</span><span class="sxs-lookup"><span data-stu-id="1fff5-151">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="1fff5-152">有关https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune详细信息, 请参阅。</span><span class="sxs-lookup"><span data-stu-id="1fff5-152">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="1fff5-153">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="1fff5-153">supportDepartment</span></span>|<span data-ttu-id="1fff5-154">String</span><span class="sxs-lookup"><span data-stu-id="1fff5-154">String</span></span>|<span data-ttu-id="1fff5-155">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="1fff5-155">Support department information</span></span>|
|<span data-ttu-id="1fff5-156">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="1fff5-156">passCodeDisabled</span></span>|<span data-ttu-id="1fff5-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-157">Boolean</span></span>|<span data-ttu-id="1fff5-158">指示是否禁用密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="1fff5-158">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="1fff5-159">isMandatory</span><span class="sxs-lookup"><span data-stu-id="1fff5-159">isMandatory</span></span>|<span data-ttu-id="1fff5-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-160">Boolean</span></span>|<span data-ttu-id="1fff5-161">指示配置文件是否是必需的</span><span class="sxs-lookup"><span data-stu-id="1fff5-161">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="1fff5-162">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="1fff5-162">locationDisabled</span></span>|<span data-ttu-id="1fff5-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-163">Boolean</span></span>|<span data-ttu-id="1fff5-164">指示是否禁用位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="1fff5-164">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="1fff5-165">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="1fff5-165">supportPhoneNumber</span></span>|<span data-ttu-id="1fff5-166">String</span><span class="sxs-lookup"><span data-stu-id="1fff5-166">String</span></span>|<span data-ttu-id="1fff5-167">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="1fff5-167">Support phone number</span></span>|
|<span data-ttu-id="1fff5-168">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="1fff5-168">profileRemovalDisabled</span></span>|<span data-ttu-id="1fff5-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-169">Boolean</span></span>|<span data-ttu-id="1fff5-170">指示是否禁用了配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="1fff5-170">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="1fff5-171">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="1fff5-171">restoreBlocked</span></span>|<span data-ttu-id="1fff5-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-172">Boolean</span></span>|<span data-ttu-id="1fff5-173">指示是否阻止还原安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="1fff5-173">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="1fff5-174">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="1fff5-174">appleIdDisabled</span></span>|<span data-ttu-id="1fff5-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-175">Boolean</span></span>|<span data-ttu-id="1fff5-176">指示是否禁用 Apple id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="1fff5-176">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="1fff5-177">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="1fff5-177">termsAndConditionsDisabled</span></span>|<span data-ttu-id="1fff5-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-178">Boolean</span></span>|<span data-ttu-id="1fff5-179">指示是否已禁用 "条款和条件" 安装窗格</span><span class="sxs-lookup"><span data-stu-id="1fff5-179">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="1fff5-180">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="1fff5-180">touchIdDisabled</span></span>|<span data-ttu-id="1fff5-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-181">Boolean</span></span>|<span data-ttu-id="1fff5-182">指示是否禁用了触控 id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="1fff5-182">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="1fff5-183">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="1fff5-183">applePayDisabled</span></span>|<span data-ttu-id="1fff5-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-184">Boolean</span></span>|<span data-ttu-id="1fff5-185">指示是否禁用 Apple 付费设置窗格</span><span class="sxs-lookup"><span data-stu-id="1fff5-185">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="1fff5-186">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="1fff5-186">zoomDisabled</span></span>|<span data-ttu-id="1fff5-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-187">Boolean</span></span>|<span data-ttu-id="1fff5-188">指示是否禁用缩放设置窗格</span><span class="sxs-lookup"><span data-stu-id="1fff5-188">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="1fff5-189">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="1fff5-189">siriDisabled</span></span>|<span data-ttu-id="1fff5-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-190">Boolean</span></span>|<span data-ttu-id="1fff5-191">指示是否禁用 siri 安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="1fff5-191">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="1fff5-192">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="1fff5-192">diagnosticsDisabled</span></span>|<span data-ttu-id="1fff5-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-193">Boolean</span></span>|<span data-ttu-id="1fff5-194">指示是否禁用诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="1fff5-194">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="1fff5-195">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="1fff5-195">displayToneSetupDisabled</span></span>|<span data-ttu-id="1fff5-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-196">Boolean</span></span>|<span data-ttu-id="1fff5-197">指示是否禁用 displaytone 安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="1fff5-197">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="1fff5-198">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="1fff5-198">privacyPaneDisabled</span></span>|<span data-ttu-id="1fff5-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fff5-199">Boolean</span></span>|<span data-ttu-id="1fff5-200">指示是否禁用隐私屏幕</span><span class="sxs-lookup"><span data-stu-id="1fff5-200">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="1fff5-201">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="1fff5-201">deviceNameTemplate</span></span>|<span data-ttu-id="1fff5-202">String</span><span class="sxs-lookup"><span data-stu-id="1fff5-202">String</span></span>|<span data-ttu-id="1fff5-203">设置文本或名称模式。</span><span class="sxs-lookup"><span data-stu-id="1fff5-203">Sets a literal or name pattern.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fff5-204">关系</span><span class="sxs-lookup"><span data-stu-id="1fff5-204">Relationships</span></span>
<span data-ttu-id="1fff5-205">无</span><span class="sxs-lookup"><span data-stu-id="1fff5-205">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1fff5-206">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1fff5-206">JSON Representation</span></span>
<span data-ttu-id="1fff5-207">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fff5-207">Here is a JSON representation of the resource.</span></span>
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
  "deviceNameTemplate": "String"
}
```




