---
title: depEnrollmentBaseProfile 资源类型
description: DepEnrollmentBaseProfile 资源表示 Apple 设备注册程序 (DEP) 注册配置文件。 相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号
author: tfitzmac
ms.openlocfilehash: 26335fd3d35494b815dd43531ad54b4796dc861c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308370"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="2bb29-104">depEnrollmentBaseProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="2bb29-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="2bb29-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2bb29-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2bb29-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2bb29-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2bb29-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2bb29-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2bb29-108">DepEnrollmentBaseProfile 资源表示 Apple 设备注册程序 (DEP) 注册配置文件。</span><span class="sxs-lookup"><span data-stu-id="2bb29-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="2bb29-109">相应的设备可以通过部署注册之前，必须将此类型的配置文件分配给 Apple DEP 序列号</span><span class="sxs-lookup"><span data-stu-id="2bb29-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>

<span data-ttu-id="2bb29-110">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2bb29-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2bb29-111">方法</span><span class="sxs-lookup"><span data-stu-id="2bb29-111">Methods</span></span>
|<span data-ttu-id="2bb29-112">方法</span><span class="sxs-lookup"><span data-stu-id="2bb29-112">Method</span></span>|<span data-ttu-id="2bb29-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="2bb29-113">Return Type</span></span>|<span data-ttu-id="2bb29-114">说明</span><span class="sxs-lookup"><span data-stu-id="2bb29-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2bb29-115">列表 depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="2bb29-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="2bb29-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="2bb29-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="2bb29-117">列出属性和[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="2bb29-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="2bb29-118">获取 depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="2bb29-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="2bb29-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="2bb29-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="2bb29-120">读取属性和[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="2bb29-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2bb29-121">属性</span><span class="sxs-lookup"><span data-stu-id="2bb29-121">Properties</span></span>
|<span data-ttu-id="2bb29-122">属性</span><span class="sxs-lookup"><span data-stu-id="2bb29-122">Property</span></span>|<span data-ttu-id="2bb29-123">类型</span><span class="sxs-lookup"><span data-stu-id="2bb29-123">Type</span></span>|<span data-ttu-id="2bb29-124">说明</span><span class="sxs-lookup"><span data-stu-id="2bb29-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bb29-125">id</span><span class="sxs-lookup"><span data-stu-id="2bb29-125">id</span></span>|<span data-ttu-id="2bb29-126">字符串</span><span class="sxs-lookup"><span data-stu-id="2bb29-126">String</span></span>|<span data-ttu-id="2bb29-127">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)对象继承的 GUID</span><span class="sxs-lookup"><span data-stu-id="2bb29-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2bb29-128">displayName</span><span class="sxs-lookup"><span data-stu-id="2bb29-128">displayName</span></span>|<span data-ttu-id="2bb29-129">字符串</span><span class="sxs-lookup"><span data-stu-id="2bb29-129">String</span></span>|<span data-ttu-id="2bb29-130">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="2bb29-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2bb29-131">说明</span><span class="sxs-lookup"><span data-stu-id="2bb29-131">description</span></span>|<span data-ttu-id="2bb29-132">字符串</span><span class="sxs-lookup"><span data-stu-id="2bb29-132">String</span></span>|<span data-ttu-id="2bb29-133">从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)的继承配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="2bb29-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2bb29-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="2bb29-134">requiresUserAuthentication</span></span>|<span data-ttu-id="2bb29-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-135">Boolean</span></span>|<span data-ttu-id="2bb29-136">指示该配置文件是否要求来自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)用户身份验证继承</span><span class="sxs-lookup"><span data-stu-id="2bb29-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2bb29-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="2bb29-137">configurationEndpointUrl</span></span>|<span data-ttu-id="2bb29-138">字符串</span><span class="sxs-lookup"><span data-stu-id="2bb29-138">String</span></span>|<span data-ttu-id="2bb29-139">配置终结点 url，用于注册继承从[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2bb29-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2bb29-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="2bb29-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="2bb29-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-141">Boolean</span></span>|<span data-ttu-id="2bb29-142">指示要通过 Apple Setup Assistant 而不是的公司门户进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="2bb29-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="2bb29-143">继承自[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="2bb29-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="2bb29-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="2bb29-144">isDefault</span></span>|<span data-ttu-id="2bb29-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-145">Boolean</span></span>|<span data-ttu-id="2bb29-146">指示是否这是默认配置文件</span><span class="sxs-lookup"><span data-stu-id="2bb29-146">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="2bb29-147">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="2bb29-147">supervisedModeEnabled</span></span>|<span data-ttu-id="2bb29-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-148">Boolean</span></span>|<span data-ttu-id="2bb29-149">监管模式下，设置为 True 可启用，false 否则。</span><span class="sxs-lookup"><span data-stu-id="2bb29-149">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="2bb29-150">请参阅https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune的其他信息。</span><span class="sxs-lookup"><span data-stu-id="2bb29-150">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="2bb29-151">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="2bb29-151">supportDepartment</span></span>|<span data-ttu-id="2bb29-152">字符串</span><span class="sxs-lookup"><span data-stu-id="2bb29-152">String</span></span>|<span data-ttu-id="2bb29-153">支持部门信息</span><span class="sxs-lookup"><span data-stu-id="2bb29-153">Support department information</span></span>|
|<span data-ttu-id="2bb29-154">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="2bb29-154">passCodeDisabled</span></span>|<span data-ttu-id="2bb29-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-155">Boolean</span></span>|<span data-ttu-id="2bb29-156">指示是否密码设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="2bb29-156">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="2bb29-157">isMandatory</span><span class="sxs-lookup"><span data-stu-id="2bb29-157">isMandatory</span></span>|<span data-ttu-id="2bb29-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-158">Boolean</span></span>|<span data-ttu-id="2bb29-159">指示是否强制配置文件</span><span class="sxs-lookup"><span data-stu-id="2bb29-159">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="2bb29-160">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="2bb29-160">locationDisabled</span></span>|<span data-ttu-id="2bb29-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-161">Boolean</span></span>|<span data-ttu-id="2bb29-162">指示是否位置服务设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="2bb29-162">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="2bb29-163">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="2bb29-163">supportPhoneNumber</span></span>|<span data-ttu-id="2bb29-164">字符串</span><span class="sxs-lookup"><span data-stu-id="2bb29-164">String</span></span>|<span data-ttu-id="2bb29-165">支持电话号码</span><span class="sxs-lookup"><span data-stu-id="2bb29-165">Support phone number</span></span>|
|<span data-ttu-id="2bb29-166">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="2bb29-166">profileRemovalDisabled</span></span>|<span data-ttu-id="2bb29-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-167">Boolean</span></span>|<span data-ttu-id="2bb29-168">指示是否已禁用配置文件删除选项</span><span class="sxs-lookup"><span data-stu-id="2bb29-168">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="2bb29-169">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="2bb29-169">restoreBlocked</span></span>|<span data-ttu-id="2bb29-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-170">Boolean</span></span>|<span data-ttu-id="2bb29-171">指示是否还原设置窗格被阻止</span><span class="sxs-lookup"><span data-stu-id="2bb29-171">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="2bb29-172">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="2bb29-172">appleIdDisabled</span></span>|<span data-ttu-id="2bb29-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-173">Boolean</span></span>|<span data-ttu-id="2bb29-174">指示是否 Apple id 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="2bb29-174">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="2bb29-175">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="2bb29-175">termsAndConditionsDisabled</span></span>|<span data-ttu-id="2bb29-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-176">Boolean</span></span>|<span data-ttu-id="2bb29-177">指示是否已禁用条款和条件设置窗格</span><span class="sxs-lookup"><span data-stu-id="2bb29-177">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="2bb29-178">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="2bb29-178">touchIdDisabled</span></span>|<span data-ttu-id="2bb29-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-179">Boolean</span></span>|<span data-ttu-id="2bb29-180">指示是否触摸 id 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="2bb29-180">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="2bb29-181">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="2bb29-181">applePayDisabled</span></span>|<span data-ttu-id="2bb29-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-182">Boolean</span></span>|<span data-ttu-id="2bb29-183">指示是否 Apple 付薪设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="2bb29-183">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="2bb29-184">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="2bb29-184">zoomDisabled</span></span>|<span data-ttu-id="2bb29-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-185">Boolean</span></span>|<span data-ttu-id="2bb29-186">指示是否缩放设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="2bb29-186">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="2bb29-187">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="2bb29-187">siriDisabled</span></span>|<span data-ttu-id="2bb29-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-188">Boolean</span></span>|<span data-ttu-id="2bb29-189">指示是否 siri 设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="2bb29-189">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="2bb29-190">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="2bb29-190">diagnosticsDisabled</span></span>|<span data-ttu-id="2bb29-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bb29-191">Boolean</span></span>|<span data-ttu-id="2bb29-192">指示是否诊断设置窗格被禁用</span><span class="sxs-lookup"><span data-stu-id="2bb29-192">Indicates if diagnostics setup pane is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bb29-193">Relationships</span><span class="sxs-lookup"><span data-stu-id="2bb29-193">Relationships</span></span>
<span data-ttu-id="2bb29-194">无</span><span class="sxs-lookup"><span data-stu-id="2bb29-194">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2bb29-195">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2bb29-195">JSON Representation</span></span>
<span data-ttu-id="2bb29-196">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bb29-196">Here is a JSON representation of the resource.</span></span>
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





