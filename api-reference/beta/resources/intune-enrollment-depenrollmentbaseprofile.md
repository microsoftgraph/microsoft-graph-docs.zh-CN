---
title: depEnrollmentBaseProfile 资源类型
description: DepEnrollmentBaseProfile 资源表示 Apple 设备注册程序 (DEP) 注册配置文件。 相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9e1383048b08a309ea0ecf60eb1ad07c2636e7e5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937668"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="e5dd2-104">depEnrollmentBaseProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5dd2-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="e5dd2-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e5dd2-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5dd2-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e5dd2-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5dd2-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e5dd2-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5dd2-108">DepEnrollmentBaseProfile 资源表示 Apple 设备注册程序 (DEP) 注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="e5dd2-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="e5dd2-109">相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号</span><span class="sxs-lookup"><span data-stu-id="e5dd2-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>

<span data-ttu-id="e5dd2-110">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e5dd2-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e5dd2-111">方法</span><span class="sxs-lookup"><span data-stu-id="e5dd2-111">Methods</span></span>
|<span data-ttu-id="e5dd2-112">方法</span><span class="sxs-lookup"><span data-stu-id="e5dd2-112">Method</span></span>|<span data-ttu-id="e5dd2-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="e5dd2-113">Return Type</span></span>|<span data-ttu-id="e5dd2-114">说明</span><span class="sxs-lookup"><span data-stu-id="e5dd2-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e5dd2-115">列表 depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="e5dd2-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="e5dd2-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="e5dd2-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="e5dd2-117">列出属性和[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="e5dd2-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="e5dd2-118">获取 depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="e5dd2-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="e5dd2-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="e5dd2-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="e5dd2-120">读取属性和[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="e5dd2-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5dd2-121">属性</span><span class="sxs-lookup"><span data-stu-id="e5dd2-121">Properties</span></span>
|<span data-ttu-id="e5dd2-122">属性</span><span class="sxs-lookup"><span data-stu-id="e5dd2-122">Property</span></span>|<span data-ttu-id="e5dd2-123">类型</span><span class="sxs-lookup"><span data-stu-id="e5dd2-123">Type</span></span>|<span data-ttu-id="e5dd2-124">说明</span><span class="sxs-lookup"><span data-stu-id="e5dd2-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5dd2-125">id</span><span class="sxs-lookup"><span data-stu-id="e5dd2-125">id</span></span>|<span data-ttu-id="e5dd2-126">字符串</span><span class="sxs-lookup"><span data-stu-id="e5dd2-126">String</span></span>|<span data-ttu-id="e5dd2-127">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象继承的 GUID</span><span class="sxs-lookup"><span data-stu-id="e5dd2-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e5dd2-128">displayName</span><span class="sxs-lookup"><span data-stu-id="e5dd2-128">displayName</span></span>|<span data-ttu-id="e5dd2-129">字符串</span><span class="sxs-lookup"><span data-stu-id="e5dd2-129">String</span></span>|<span data-ttu-id="e5dd2-130">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="e5dd2-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e5dd2-131">说明</span><span class="sxs-lookup"><span data-stu-id="e5dd2-131">description</span></span>|<span data-ttu-id="e5dd2-132">字符串</span><span class="sxs-lookup"><span data-stu-id="e5dd2-132">String</span></span>|<span data-ttu-id="e5dd2-133">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="e5dd2-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e5dd2-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="e5dd2-134">requiresUserAuthentication</span></span>|<span data-ttu-id="e5dd2-135">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-135">Boolean</span></span>|<span data-ttu-id="e5dd2-136">指示该配置文件是否要求来自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)用户身份验证继承</span><span class="sxs-lookup"><span data-stu-id="e5dd2-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e5dd2-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="e5dd2-137">configurationEndpointUrl</span></span>|<span data-ttu-id="e5dd2-138">字符串</span><span class="sxs-lookup"><span data-stu-id="e5dd2-138">String</span></span>|<span data-ttu-id="e5dd2-139">配置终结点 url，用于注册继承从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e5dd2-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e5dd2-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="e5dd2-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="e5dd2-141">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-141">Boolean</span></span>|<span data-ttu-id="e5dd2-142">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="e5dd2-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="e5dd2-143">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e5dd2-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e5dd2-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="e5dd2-144">isDefault</span></span>|<span data-ttu-id="e5dd2-145">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-145">Boolean</span></span>|<span data-ttu-id="e5dd2-146">指示是否这是默认配置文件</span><span class="sxs-lookup"><span data-stu-id="e5dd2-146">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="e5dd2-147">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="e5dd2-147">supervisedModeEnabled</span></span>|<span data-ttu-id="e5dd2-148">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-148">Boolean</span></span>|<span data-ttu-id="e5dd2-149">监管模式下，设置为 True 可启用，false 否则。</span><span class="sxs-lookup"><span data-stu-id="e5dd2-149">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="e5dd2-150">请参阅https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune的其他信息。</span><span class="sxs-lookup"><span data-stu-id="e5dd2-150">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="e5dd2-151">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="e5dd2-151">supportDepartment</span></span>|<span data-ttu-id="e5dd2-152">字符串</span><span class="sxs-lookup"><span data-stu-id="e5dd2-152">String</span></span>|<span data-ttu-id="e5dd2-153">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="e5dd2-153">Support department information</span></span>|
|<span data-ttu-id="e5dd2-154">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="e5dd2-154">passCodeDisabled</span></span>|<span data-ttu-id="e5dd2-155">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-155">Boolean</span></span>|<span data-ttu-id="e5dd2-156">指示是否密码设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="e5dd2-156">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="e5dd2-157">isMandatory</span><span class="sxs-lookup"><span data-stu-id="e5dd2-157">isMandatory</span></span>|<span data-ttu-id="e5dd2-158">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-158">Boolean</span></span>|<span data-ttu-id="e5dd2-159">指示是否强制配置文件</span><span class="sxs-lookup"><span data-stu-id="e5dd2-159">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="e5dd2-160">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="e5dd2-160">locationDisabled</span></span>|<span data-ttu-id="e5dd2-161">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-161">Boolean</span></span>|<span data-ttu-id="e5dd2-162">指示是否位置服务设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="e5dd2-162">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="e5dd2-163">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="e5dd2-163">supportPhoneNumber</span></span>|<span data-ttu-id="e5dd2-164">字符串</span><span class="sxs-lookup"><span data-stu-id="e5dd2-164">String</span></span>|<span data-ttu-id="e5dd2-165">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="e5dd2-165">Support phone number</span></span>|
|<span data-ttu-id="e5dd2-166">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="e5dd2-166">profileRemovalDisabled</span></span>|<span data-ttu-id="e5dd2-167">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-167">Boolean</span></span>|<span data-ttu-id="e5dd2-168">指示是否已禁用配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="e5dd2-168">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="e5dd2-169">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="e5dd2-169">restoreBlocked</span></span>|<span data-ttu-id="e5dd2-170">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-170">Boolean</span></span>|<span data-ttu-id="e5dd2-171">指示是否还原设置窗格被阻止</span><span class="sxs-lookup"><span data-stu-id="e5dd2-171">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="e5dd2-172">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="e5dd2-172">appleIdDisabled</span></span>|<span data-ttu-id="e5dd2-173">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-173">Boolean</span></span>|<span data-ttu-id="e5dd2-174">指示是否 Apple id 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="e5dd2-174">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="e5dd2-175">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="e5dd2-175">termsAndConditionsDisabled</span></span>|<span data-ttu-id="e5dd2-176">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-176">Boolean</span></span>|<span data-ttu-id="e5dd2-177">指示是否已禁用条款和条件设置窗格</span><span class="sxs-lookup"><span data-stu-id="e5dd2-177">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="e5dd2-178">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="e5dd2-178">touchIdDisabled</span></span>|<span data-ttu-id="e5dd2-179">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-179">Boolean</span></span>|<span data-ttu-id="e5dd2-180">指示是否触摸 id 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="e5dd2-180">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="e5dd2-181">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="e5dd2-181">applePayDisabled</span></span>|<span data-ttu-id="e5dd2-182">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-182">Boolean</span></span>|<span data-ttu-id="e5dd2-183">指示是否 Apple 付薪设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="e5dd2-183">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="e5dd2-184">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="e5dd2-184">zoomDisabled</span></span>|<span data-ttu-id="e5dd2-185">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-185">Boolean</span></span>|<span data-ttu-id="e5dd2-186">指示是否缩放设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="e5dd2-186">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="e5dd2-187">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="e5dd2-187">siriDisabled</span></span>|<span data-ttu-id="e5dd2-188">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-188">Boolean</span></span>|<span data-ttu-id="e5dd2-189">指示是否 siri 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="e5dd2-189">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="e5dd2-190">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="e5dd2-190">diagnosticsDisabled</span></span>|<span data-ttu-id="e5dd2-191">布尔</span><span class="sxs-lookup"><span data-stu-id="e5dd2-191">Boolean</span></span>|<span data-ttu-id="e5dd2-192">指示是否诊断设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="e5dd2-192">Indicates if diagnostics setup pane is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5dd2-193">Relationships</span><span class="sxs-lookup"><span data-stu-id="e5dd2-193">Relationships</span></span>
<span data-ttu-id="e5dd2-194">无</span><span class="sxs-lookup"><span data-stu-id="e5dd2-194">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e5dd2-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5dd2-195">JSON Representation</span></span>
<span data-ttu-id="e5dd2-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5dd2-196">Here is a JSON representation of the resource.</span></span>
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
  "diagnosticsDisabled": true
}
```





