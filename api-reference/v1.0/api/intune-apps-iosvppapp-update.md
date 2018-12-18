---
title: 更新 iosVppApp
description: 更新 iosVppApp 对象的属性。
author: tfitzmac
ms.openlocfilehash: 05da16de7fc9d9cf5c556fd48f29d327bd6cd6eb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348004"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="1ccde-103">更新 iosVppApp</span><span class="sxs-lookup"><span data-stu-id="1ccde-103">Update iosVppApp</span></span>

> <span data-ttu-id="1ccde-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1ccde-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ccde-105">更新 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1ccde-105">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ccde-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1ccde-106">Prerequisites</span></span>
<span data-ttu-id="1ccde-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1ccde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ccde-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ccde-109">Permission type</span></span>|<span data-ttu-id="1ccde-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1ccde-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ccde-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ccde-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1ccde-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ccde-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1ccde-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ccde-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ccde-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ccde-114">Not supported.</span></span>|
|<span data-ttu-id="1ccde-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ccde-115">Application</span></span>|<span data-ttu-id="1ccde-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ccde-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ccde-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ccde-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="1ccde-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ccde-118">Request headers</span></span>
|<span data-ttu-id="1ccde-119">标头</span><span class="sxs-lookup"><span data-stu-id="1ccde-119">Header</span></span>|<span data-ttu-id="1ccde-120">值</span><span class="sxs-lookup"><span data-stu-id="1ccde-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ccde-121">授权</span><span class="sxs-lookup"><span data-stu-id="1ccde-121">Authorization</span></span>|<span data-ttu-id="1ccde-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1ccde-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ccde-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1ccde-123">Accept</span></span>|<span data-ttu-id="1ccde-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1ccde-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ccde-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ccde-125">Request body</span></span>
<span data-ttu-id="1ccde-126">在请求正文中，提供 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ccde-126">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="1ccde-127">下表显示了创建 [iosVppApp](../resources/intune-apps-iosvppapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1ccde-127">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="1ccde-128">属性</span><span class="sxs-lookup"><span data-stu-id="1ccde-128">Property</span></span>|<span data-ttu-id="1ccde-129">类型</span><span class="sxs-lookup"><span data-stu-id="1ccde-129">Type</span></span>|<span data-ttu-id="1ccde-130">说明</span><span class="sxs-lookup"><span data-stu-id="1ccde-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ccde-131">id</span><span class="sxs-lookup"><span data-stu-id="1ccde-131">id</span></span>|<span data-ttu-id="1ccde-132">String</span><span class="sxs-lookup"><span data-stu-id="1ccde-132">String</span></span>|<span data-ttu-id="1ccde-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1ccde-133">Key of the entity.</span></span> <span data-ttu-id="1ccde-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ccde-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ccde-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1ccde-135">displayName</span></span>|<span data-ttu-id="1ccde-136">String</span><span class="sxs-lookup"><span data-stu-id="1ccde-136">String</span></span>|<span data-ttu-id="1ccde-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="1ccde-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1ccde-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ccde-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ccde-139">description</span><span class="sxs-lookup"><span data-stu-id="1ccde-139">description</span></span>|<span data-ttu-id="1ccde-140">String</span><span class="sxs-lookup"><span data-stu-id="1ccde-140">String</span></span>|<span data-ttu-id="1ccde-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="1ccde-141">The description of the app.</span></span> <span data-ttu-id="1ccde-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ccde-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ccde-143">publisher</span><span class="sxs-lookup"><span data-stu-id="1ccde-143">publisher</span></span>|<span data-ttu-id="1ccde-144">String</span><span class="sxs-lookup"><span data-stu-id="1ccde-144">String</span></span>|<span data-ttu-id="1ccde-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="1ccde-145">The publisher of the app.</span></span> <span data-ttu-id="1ccde-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ccde-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ccde-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1ccde-147">largeIcon</span></span>|[<span data-ttu-id="1ccde-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1ccde-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1ccde-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="1ccde-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1ccde-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ccde-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ccde-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ccde-151">createdDateTime</span></span>|<span data-ttu-id="1ccde-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ccde-152">DateTimeOffset</span></span>|<span data-ttu-id="1ccde-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1ccde-153">The date and time the app was created.</span></span> <span data-ttu-id="1ccde-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ccde-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ccde-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ccde-155">lastModifiedDateTime</span></span>|<span data-ttu-id="1ccde-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ccde-156">DateTimeOffset</span></span>|<span data-ttu-id="1ccde-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1ccde-157">The date and time the app was last modified.</span></span> <span data-ttu-id="1ccde-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ccde-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ccde-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1ccde-159">isFeatured</span></span>|<span data-ttu-id="1ccde-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ccde-160">Boolean</span></span>|<span data-ttu-id="1ccde-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ccde-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ccde-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1ccde-162">privacyInformationUrl</span></span>|<span data-ttu-id="1ccde-163">String</span><span class="sxs-lookup"><span data-stu-id="1ccde-163">String</span></span>|<span data-ttu-id="1ccde-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="1ccde-164">The privacy statement Url.</span></span> <span data-ttu-id="1ccde-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ccde-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ccde-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1ccde-166">informationUrl</span></span>|<span data-ttu-id="1ccde-167">String</span><span class="sxs-lookup"><span data-stu-id="1ccde-167">String</span></span>|<span data-ttu-id="1ccde-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="1ccde-168">The more information Url.</span></span> <span data-ttu-id="1ccde-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ccde-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ccde-170">owner</span><span class="sxs-lookup"><span data-stu-id="1ccde-170">owner</span></span>|<span data-ttu-id="1ccde-171">String</span><span class="sxs-lookup"><span data-stu-id="1ccde-171">String</span></span>|<span data-ttu-id="1ccde-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="1ccde-172">The owner of the app.</span></span> <span data-ttu-id="1ccde-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ccde-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ccde-174">developer</span><span class="sxs-lookup"><span data-stu-id="1ccde-174">developer</span></span>|<span data-ttu-id="1ccde-175">String</span><span class="sxs-lookup"><span data-stu-id="1ccde-175">String</span></span>|<span data-ttu-id="1ccde-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="1ccde-176">The developer of the app.</span></span> <span data-ttu-id="1ccde-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ccde-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ccde-178">notes</span><span class="sxs-lookup"><span data-stu-id="1ccde-178">notes</span></span>|<span data-ttu-id="1ccde-179">String</span><span class="sxs-lookup"><span data-stu-id="1ccde-179">String</span></span>|<span data-ttu-id="1ccde-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="1ccde-180">Notes for the app.</span></span> <span data-ttu-id="1ccde-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1ccde-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ccde-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="1ccde-182">publishingState</span></span>|[<span data-ttu-id="1ccde-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1ccde-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1ccde-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="1ccde-184">The publishing state for the app.</span></span> <span data-ttu-id="1ccde-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="1ccde-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1ccde-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="1ccde-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1ccde-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="1ccde-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1ccde-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1ccde-188">usedLicenseCount</span></span>|<span data-ttu-id="1ccde-189">Int32</span><span class="sxs-lookup"><span data-stu-id="1ccde-189">Int32</span></span>|<span data-ttu-id="1ccde-190">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="1ccde-190">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="1ccde-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="1ccde-191">totalLicenseCount</span></span>|<span data-ttu-id="1ccde-192">Int32</span><span class="sxs-lookup"><span data-stu-id="1ccde-192">Int32</span></span>|<span data-ttu-id="1ccde-193">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="1ccde-193">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="1ccde-194">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="1ccde-194">releaseDateTime</span></span>|<span data-ttu-id="1ccde-195">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ccde-195">DateTimeOffset</span></span>|<span data-ttu-id="1ccde-196">VPP 应用程序的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1ccde-196">The VPP application release date and time.</span></span>|
|<span data-ttu-id="1ccde-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="1ccde-197">appStoreUrl</span></span>|<span data-ttu-id="1ccde-198">String</span><span class="sxs-lookup"><span data-stu-id="1ccde-198">String</span></span>|<span data-ttu-id="1ccde-199">存储 URL。</span><span class="sxs-lookup"><span data-stu-id="1ccde-199">The store URL.</span></span>|
|<span data-ttu-id="1ccde-200">licensingType</span><span class="sxs-lookup"><span data-stu-id="1ccde-200">licensingType</span></span>|[<span data-ttu-id="1ccde-201">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="1ccde-201">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="1ccde-202">受支持的许可证类型。</span><span class="sxs-lookup"><span data-stu-id="1ccde-202">The supported License Type.</span></span>|
|<span data-ttu-id="1ccde-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="1ccde-203">applicableDeviceType</span></span>|[<span data-ttu-id="1ccde-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="1ccde-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="1ccde-205">适用的 iOS 设备类型。</span><span class="sxs-lookup"><span data-stu-id="1ccde-205">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="1ccde-206">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="1ccde-206">vppTokenOrganizationName</span></span>|<span data-ttu-id="1ccde-207">String</span><span class="sxs-lookup"><span data-stu-id="1ccde-207">String</span></span>|<span data-ttu-id="1ccde-208">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="1ccde-208">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="1ccde-209">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="1ccde-209">vppTokenAccountType</span></span>|[<span data-ttu-id="1ccde-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="1ccde-210">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="1ccde-211">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="1ccde-211">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="1ccde-212">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="1ccde-212">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="1ccde-213">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="1ccde-213">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="1ccde-214">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="1ccde-214">vppTokenAppleId</span></span>|<span data-ttu-id="1ccde-215">String</span><span class="sxs-lookup"><span data-stu-id="1ccde-215">String</span></span>|<span data-ttu-id="1ccde-216">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="1ccde-216">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="1ccde-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="1ccde-217">bundleId</span></span>|<span data-ttu-id="1ccde-218">String</span><span class="sxs-lookup"><span data-stu-id="1ccde-218">String</span></span>|<span data-ttu-id="1ccde-219">标识名称。</span><span class="sxs-lookup"><span data-stu-id="1ccde-219">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="1ccde-220">响应</span><span class="sxs-lookup"><span data-stu-id="1ccde-220">Response</span></span>
<span data-ttu-id="1ccde-221">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1ccde-221">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ccde-222">示例</span><span class="sxs-lookup"><span data-stu-id="1ccde-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ccde-223">请求</span><span class="sxs-lookup"><span data-stu-id="1ccde-223">Request</span></span>
<span data-ttu-id="1ccde-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ccde-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1222

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```

### <a name="response"></a><span data-ttu-id="1ccde-225">响应</span><span class="sxs-lookup"><span data-stu-id="1ccde-225">Response</span></span>
<span data-ttu-id="1ccde-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1ccde-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1394

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```



