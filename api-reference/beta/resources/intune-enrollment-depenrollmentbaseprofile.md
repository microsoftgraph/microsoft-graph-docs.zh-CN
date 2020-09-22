---
title: depEnrollmentBaseProfile 资源类型
description: DepEnrollmentBaseProfile 资源表示 Apple 设备注册计划 (DEP) 注册配置文件。 在相应的设备可以通过 DEP 进行注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3878177d847cd4c98908345f8e1de66b22218bb3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080346"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="57cf5-104">depEnrollmentBaseProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="57cf5-104">depEnrollmentBaseProfile resource type</span></span>

<span data-ttu-id="57cf5-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57cf5-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57cf5-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="57cf5-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57cf5-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57cf5-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57cf5-108">DepEnrollmentBaseProfile 资源表示 Apple 设备注册计划 (DEP) 注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="57cf5-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="57cf5-109">在相应的设备可以通过 DEP 进行注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号。</span><span class="sxs-lookup"><span data-stu-id="57cf5-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="57cf5-110">继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="57cf5-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="57cf5-111">方法</span><span class="sxs-lookup"><span data-stu-id="57cf5-111">Methods</span></span>
|<span data-ttu-id="57cf5-112">方法</span><span class="sxs-lookup"><span data-stu-id="57cf5-112">Method</span></span>|<span data-ttu-id="57cf5-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="57cf5-113">Return Type</span></span>|<span data-ttu-id="57cf5-114">说明</span><span class="sxs-lookup"><span data-stu-id="57cf5-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="57cf5-115">列出 depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="57cf5-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="57cf5-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="57cf5-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="57cf5-117">列出 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="57cf5-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="57cf5-118">获取 depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="57cf5-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="57cf5-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="57cf5-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="57cf5-120">读取 [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="57cf5-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="57cf5-121">属性</span><span class="sxs-lookup"><span data-stu-id="57cf5-121">Properties</span></span>
|<span data-ttu-id="57cf5-122">属性</span><span class="sxs-lookup"><span data-stu-id="57cf5-122">Property</span></span>|<span data-ttu-id="57cf5-123">类型</span><span class="sxs-lookup"><span data-stu-id="57cf5-123">Type</span></span>|<span data-ttu-id="57cf5-124">说明</span><span class="sxs-lookup"><span data-stu-id="57cf5-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57cf5-125">id</span><span class="sxs-lookup"><span data-stu-id="57cf5-125">id</span></span>|<span data-ttu-id="57cf5-126">String</span><span class="sxs-lookup"><span data-stu-id="57cf5-126">String</span></span>|<span data-ttu-id="57cf5-127">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="57cf5-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="57cf5-128">displayName</span><span class="sxs-lookup"><span data-stu-id="57cf5-128">displayName</span></span>|<span data-ttu-id="57cf5-129">String</span><span class="sxs-lookup"><span data-stu-id="57cf5-129">String</span></span>|<span data-ttu-id="57cf5-130">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="57cf5-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="57cf5-131">说明</span><span class="sxs-lookup"><span data-stu-id="57cf5-131">description</span></span>|<span data-ttu-id="57cf5-132">String</span><span class="sxs-lookup"><span data-stu-id="57cf5-132">String</span></span>|<span data-ttu-id="57cf5-133">从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="57cf5-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="57cf5-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="57cf5-134">requiresUserAuthentication</span></span>|<span data-ttu-id="57cf5-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-135">Boolean</span></span>|<span data-ttu-id="57cf5-136">指示配置文件是否需要从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的用户身份验证</span><span class="sxs-lookup"><span data-stu-id="57cf5-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="57cf5-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="57cf5-137">configurationEndpointUrl</span></span>|<span data-ttu-id="57cf5-138">String</span><span class="sxs-lookup"><span data-stu-id="57cf5-138">String</span></span>|<span data-ttu-id="57cf5-139">用于从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的注册的配置终结点 url</span><span class="sxs-lookup"><span data-stu-id="57cf5-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="57cf5-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="57cf5-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="57cf5-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-141">Boolean</span></span>|<span data-ttu-id="57cf5-142">指示使用 Apple Setup 助理（而不是公司门户）进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="57cf5-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="57cf5-143">继承自 [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="57cf5-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="57cf5-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="57cf5-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="57cf5-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-145">Boolean</span></span>|<span data-ttu-id="57cf5-146">指示在从[EnrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)继承的安装助理注册设备上需要公司门户</span><span class="sxs-lookup"><span data-stu-id="57cf5-146">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="57cf5-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="57cf5-147">isDefault</span></span>|<span data-ttu-id="57cf5-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-148">Boolean</span></span>|<span data-ttu-id="57cf5-149">指示这是否为默认配置文件</span><span class="sxs-lookup"><span data-stu-id="57cf5-149">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="57cf5-150">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="57cf5-150">supervisedModeEnabled</span></span>|<span data-ttu-id="57cf5-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-151">Boolean</span></span>|<span data-ttu-id="57cf5-152">监督模式，如果启用，则为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="57cf5-152">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="57cf5-153">https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune有关详细信息，请参阅。</span><span class="sxs-lookup"><span data-stu-id="57cf5-153">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="57cf5-154">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="57cf5-154">supportDepartment</span></span>|<span data-ttu-id="57cf5-155">String</span><span class="sxs-lookup"><span data-stu-id="57cf5-155">String</span></span>|<span data-ttu-id="57cf5-156">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="57cf5-156">Support department information</span></span>|
|<span data-ttu-id="57cf5-157">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="57cf5-157">passCodeDisabled</span></span>|<span data-ttu-id="57cf5-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-158">Boolean</span></span>|<span data-ttu-id="57cf5-159">指示是否禁用密码设置窗格</span><span class="sxs-lookup"><span data-stu-id="57cf5-159">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="57cf5-160">isMandatory</span><span class="sxs-lookup"><span data-stu-id="57cf5-160">isMandatory</span></span>|<span data-ttu-id="57cf5-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-161">Boolean</span></span>|<span data-ttu-id="57cf5-162">指示配置文件是否是必需的</span><span class="sxs-lookup"><span data-stu-id="57cf5-162">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="57cf5-163">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="57cf5-163">locationDisabled</span></span>|<span data-ttu-id="57cf5-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-164">Boolean</span></span>|<span data-ttu-id="57cf5-165">指示是否禁用位置服务设置窗格</span><span class="sxs-lookup"><span data-stu-id="57cf5-165">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="57cf5-166">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="57cf5-166">supportPhoneNumber</span></span>|<span data-ttu-id="57cf5-167">String</span><span class="sxs-lookup"><span data-stu-id="57cf5-167">String</span></span>|<span data-ttu-id="57cf5-168">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="57cf5-168">Support phone number</span></span>|
|<span data-ttu-id="57cf5-169">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="57cf5-169">profileRemovalDisabled</span></span>|<span data-ttu-id="57cf5-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-170">Boolean</span></span>|<span data-ttu-id="57cf5-171">指示是否禁用了配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="57cf5-171">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="57cf5-172">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="57cf5-172">restoreBlocked</span></span>|<span data-ttu-id="57cf5-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-173">Boolean</span></span>|<span data-ttu-id="57cf5-174">指示是否阻止还原安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="57cf5-174">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="57cf5-175">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="57cf5-175">appleIdDisabled</span></span>|<span data-ttu-id="57cf5-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-176">Boolean</span></span>|<span data-ttu-id="57cf5-177">指示是否禁用 Apple id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="57cf5-177">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="57cf5-178">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="57cf5-178">termsAndConditionsDisabled</span></span>|<span data-ttu-id="57cf5-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-179">Boolean</span></span>|<span data-ttu-id="57cf5-180">指示是否已禁用 "条款和条件" 安装窗格</span><span class="sxs-lookup"><span data-stu-id="57cf5-180">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="57cf5-181">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="57cf5-181">touchIdDisabled</span></span>|<span data-ttu-id="57cf5-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-182">Boolean</span></span>|<span data-ttu-id="57cf5-183">指示是否禁用了触控 id 设置窗格</span><span class="sxs-lookup"><span data-stu-id="57cf5-183">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="57cf5-184">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="57cf5-184">applePayDisabled</span></span>|<span data-ttu-id="57cf5-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-185">Boolean</span></span>|<span data-ttu-id="57cf5-186">指示是否禁用 Apple 付费设置窗格</span><span class="sxs-lookup"><span data-stu-id="57cf5-186">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="57cf5-187">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="57cf5-187">zoomDisabled</span></span>|<span data-ttu-id="57cf5-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-188">Boolean</span></span>|<span data-ttu-id="57cf5-189">指示是否禁用缩放设置窗格</span><span class="sxs-lookup"><span data-stu-id="57cf5-189">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="57cf5-190">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="57cf5-190">siriDisabled</span></span>|<span data-ttu-id="57cf5-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-191">Boolean</span></span>|<span data-ttu-id="57cf5-192">指示是否禁用 siri 安装程序窗格</span><span class="sxs-lookup"><span data-stu-id="57cf5-192">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="57cf5-193">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="57cf5-193">diagnosticsDisabled</span></span>|<span data-ttu-id="57cf5-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-194">Boolean</span></span>|<span data-ttu-id="57cf5-195">指示是否禁用诊断设置窗格</span><span class="sxs-lookup"><span data-stu-id="57cf5-195">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="57cf5-196">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="57cf5-196">displayToneSetupDisabled</span></span>|<span data-ttu-id="57cf5-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-197">Boolean</span></span>|<span data-ttu-id="57cf5-198">指示是否禁用 displaytone 安装程序屏幕</span><span class="sxs-lookup"><span data-stu-id="57cf5-198">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="57cf5-199">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="57cf5-199">privacyPaneDisabled</span></span>|<span data-ttu-id="57cf5-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-200">Boolean</span></span>|<span data-ttu-id="57cf5-201">指示是否禁用隐私屏幕</span><span class="sxs-lookup"><span data-stu-id="57cf5-201">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="57cf5-202">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="57cf5-202">screenTimeScreenDisabled</span></span>|<span data-ttu-id="57cf5-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-203">Boolean</span></span>|<span data-ttu-id="57cf5-204">指示是否禁用屏幕超时设置</span><span class="sxs-lookup"><span data-stu-id="57cf5-204">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="57cf5-205">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="57cf5-205">deviceNameTemplate</span></span>|<span data-ttu-id="57cf5-206">String</span><span class="sxs-lookup"><span data-stu-id="57cf5-206">String</span></span>|<span data-ttu-id="57cf5-207">设置文本或名称模式。</span><span class="sxs-lookup"><span data-stu-id="57cf5-207">Sets a literal or name pattern.</span></span>|
|<span data-ttu-id="57cf5-208">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="57cf5-208">configurationWebUrl</span></span>|<span data-ttu-id="57cf5-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="57cf5-209">Boolean</span></span>|<span data-ttu-id="57cf5-210">设置助理登录 URL</span><span class="sxs-lookup"><span data-stu-id="57cf5-210">URL for setup assistant login</span></span>|

## <a name="relationships"></a><span data-ttu-id="57cf5-211">关系</span><span class="sxs-lookup"><span data-stu-id="57cf5-211">Relationships</span></span>
<span data-ttu-id="57cf5-212">无</span><span class="sxs-lookup"><span data-stu-id="57cf5-212">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57cf5-213">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57cf5-213">JSON Representation</span></span>
<span data-ttu-id="57cf5-214">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57cf5-214">Here is a JSON representation of the resource.</span></span>
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
  "deviceNameTemplate": "String",
  "configurationWebUrl": true
}
```






