---
title: 更新 iosVppApp
description: 更新 iosVppApp 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d302daf914fd8dbc32a2ebd40901dd8c81c10636
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516488"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="af7d6-103">更新 iosVppApp</span><span class="sxs-lookup"><span data-stu-id="af7d6-103">Update iosVppApp</span></span>

<span data-ttu-id="af7d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af7d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af7d6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="af7d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af7d6-106">更新 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="af7d6-106">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af7d6-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="af7d6-107">Prerequisites</span></span>
<span data-ttu-id="af7d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="af7d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af7d6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="af7d6-110">Permission type</span></span>|<span data-ttu-id="af7d6-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="af7d6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af7d6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="af7d6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af7d6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af7d6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="af7d6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="af7d6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af7d6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="af7d6-115">Not supported.</span></span>|
|<span data-ttu-id="af7d6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="af7d6-116">Application</span></span>|<span data-ttu-id="af7d6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="af7d6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af7d6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="af7d6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="af7d6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="af7d6-119">Request headers</span></span>
|<span data-ttu-id="af7d6-120">标头</span><span class="sxs-lookup"><span data-stu-id="af7d6-120">Header</span></span>|<span data-ttu-id="af7d6-121">值</span><span class="sxs-lookup"><span data-stu-id="af7d6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af7d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="af7d6-122">Authorization</span></span>|<span data-ttu-id="af7d6-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="af7d6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af7d6-124">接受</span><span class="sxs-lookup"><span data-stu-id="af7d6-124">Accept</span></span>|<span data-ttu-id="af7d6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af7d6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af7d6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="af7d6-126">Request body</span></span>
<span data-ttu-id="af7d6-127">在请求正文中，提供 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af7d6-127">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="af7d6-128">下表显示了创建 [iosVppApp](../resources/intune-apps-iosvppapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="af7d6-128">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="af7d6-129">属性</span><span class="sxs-lookup"><span data-stu-id="af7d6-129">Property</span></span>|<span data-ttu-id="af7d6-130">类型</span><span class="sxs-lookup"><span data-stu-id="af7d6-130">Type</span></span>|<span data-ttu-id="af7d6-131">说明</span><span class="sxs-lookup"><span data-stu-id="af7d6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af7d6-132">id</span><span class="sxs-lookup"><span data-stu-id="af7d6-132">id</span></span>|<span data-ttu-id="af7d6-133">字符串</span><span class="sxs-lookup"><span data-stu-id="af7d6-133">String</span></span>|<span data-ttu-id="af7d6-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="af7d6-134">Key of the entity.</span></span> <span data-ttu-id="af7d6-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af7d6-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af7d6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="af7d6-136">displayName</span></span>|<span data-ttu-id="af7d6-137">字符串</span><span class="sxs-lookup"><span data-stu-id="af7d6-137">String</span></span>|<span data-ttu-id="af7d6-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="af7d6-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="af7d6-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af7d6-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af7d6-140">说明</span><span class="sxs-lookup"><span data-stu-id="af7d6-140">description</span></span>|<span data-ttu-id="af7d6-141">字符串</span><span class="sxs-lookup"><span data-stu-id="af7d6-141">String</span></span>|<span data-ttu-id="af7d6-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="af7d6-142">The description of the app.</span></span> <span data-ttu-id="af7d6-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af7d6-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af7d6-144">publisher</span><span class="sxs-lookup"><span data-stu-id="af7d6-144">publisher</span></span>|<span data-ttu-id="af7d6-145">字符串</span><span class="sxs-lookup"><span data-stu-id="af7d6-145">String</span></span>|<span data-ttu-id="af7d6-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="af7d6-146">The publisher of the app.</span></span> <span data-ttu-id="af7d6-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af7d6-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af7d6-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="af7d6-148">largeIcon</span></span>|[<span data-ttu-id="af7d6-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="af7d6-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="af7d6-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="af7d6-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="af7d6-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af7d6-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af7d6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="af7d6-152">createdDateTime</span></span>|<span data-ttu-id="af7d6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af7d6-153">DateTimeOffset</span></span>|<span data-ttu-id="af7d6-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="af7d6-154">The date and time the app was created.</span></span> <span data-ttu-id="af7d6-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af7d6-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af7d6-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="af7d6-156">lastModifiedDateTime</span></span>|<span data-ttu-id="af7d6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af7d6-157">DateTimeOffset</span></span>|<span data-ttu-id="af7d6-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="af7d6-158">The date and time the app was last modified.</span></span> <span data-ttu-id="af7d6-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af7d6-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af7d6-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="af7d6-160">isFeatured</span></span>|<span data-ttu-id="af7d6-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="af7d6-161">Boolean</span></span>|<span data-ttu-id="af7d6-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af7d6-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af7d6-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="af7d6-163">privacyInformationUrl</span></span>|<span data-ttu-id="af7d6-164">字符串</span><span class="sxs-lookup"><span data-stu-id="af7d6-164">String</span></span>|<span data-ttu-id="af7d6-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="af7d6-165">The privacy statement Url.</span></span> <span data-ttu-id="af7d6-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af7d6-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af7d6-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="af7d6-167">informationUrl</span></span>|<span data-ttu-id="af7d6-168">字符串</span><span class="sxs-lookup"><span data-stu-id="af7d6-168">String</span></span>|<span data-ttu-id="af7d6-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="af7d6-169">The more information Url.</span></span> <span data-ttu-id="af7d6-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af7d6-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af7d6-171">owner</span><span class="sxs-lookup"><span data-stu-id="af7d6-171">owner</span></span>|<span data-ttu-id="af7d6-172">String</span><span class="sxs-lookup"><span data-stu-id="af7d6-172">String</span></span>|<span data-ttu-id="af7d6-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="af7d6-173">The owner of the app.</span></span> <span data-ttu-id="af7d6-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af7d6-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af7d6-175">developer</span><span class="sxs-lookup"><span data-stu-id="af7d6-175">developer</span></span>|<span data-ttu-id="af7d6-176">字符串</span><span class="sxs-lookup"><span data-stu-id="af7d6-176">String</span></span>|<span data-ttu-id="af7d6-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="af7d6-177">The developer of the app.</span></span> <span data-ttu-id="af7d6-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af7d6-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af7d6-179">notes</span><span class="sxs-lookup"><span data-stu-id="af7d6-179">notes</span></span>|<span data-ttu-id="af7d6-180">字符串</span><span class="sxs-lookup"><span data-stu-id="af7d6-180">String</span></span>|<span data-ttu-id="af7d6-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="af7d6-181">Notes for the app.</span></span> <span data-ttu-id="af7d6-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="af7d6-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="af7d6-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="af7d6-183">publishingState</span></span>|[<span data-ttu-id="af7d6-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="af7d6-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="af7d6-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="af7d6-185">The publishing state for the app.</span></span> <span data-ttu-id="af7d6-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="af7d6-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="af7d6-187">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="af7d6-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="af7d6-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="af7d6-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="af7d6-189">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="af7d6-189">usedLicenseCount</span></span>|<span data-ttu-id="af7d6-190">Int32</span><span class="sxs-lookup"><span data-stu-id="af7d6-190">Int32</span></span>|<span data-ttu-id="af7d6-191">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="af7d6-191">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="af7d6-192">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="af7d6-192">totalLicenseCount</span></span>|<span data-ttu-id="af7d6-193">Int32</span><span class="sxs-lookup"><span data-stu-id="af7d6-193">Int32</span></span>|<span data-ttu-id="af7d6-194">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="af7d6-194">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="af7d6-195">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="af7d6-195">releaseDateTime</span></span>|<span data-ttu-id="af7d6-196">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af7d6-196">DateTimeOffset</span></span>|<span data-ttu-id="af7d6-197">VPP 应用程序的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="af7d6-197">The VPP application release date and time.</span></span>|
|<span data-ttu-id="af7d6-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="af7d6-198">appStoreUrl</span></span>|<span data-ttu-id="af7d6-199">字符串</span><span class="sxs-lookup"><span data-stu-id="af7d6-199">String</span></span>|<span data-ttu-id="af7d6-200">存储 URL。</span><span class="sxs-lookup"><span data-stu-id="af7d6-200">The store URL.</span></span>|
|<span data-ttu-id="af7d6-201">licensingType</span><span class="sxs-lookup"><span data-stu-id="af7d6-201">licensingType</span></span>|[<span data-ttu-id="af7d6-202">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="af7d6-202">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="af7d6-203">受支持的许可证类型。</span><span class="sxs-lookup"><span data-stu-id="af7d6-203">The supported License Type.</span></span>|
|<span data-ttu-id="af7d6-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="af7d6-204">applicableDeviceType</span></span>|[<span data-ttu-id="af7d6-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="af7d6-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="af7d6-206">适用的 iOS 设备类型。</span><span class="sxs-lookup"><span data-stu-id="af7d6-206">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="af7d6-207">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="af7d6-207">vppTokenOrganizationName</span></span>|<span data-ttu-id="af7d6-208">字符串</span><span class="sxs-lookup"><span data-stu-id="af7d6-208">String</span></span>|<span data-ttu-id="af7d6-209">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="af7d6-209">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="af7d6-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="af7d6-210">vppTokenAccountType</span></span>|[<span data-ttu-id="af7d6-211">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="af7d6-211">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="af7d6-212">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="af7d6-212">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="af7d6-213">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="af7d6-213">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="af7d6-214">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="af7d6-214">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="af7d6-215">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="af7d6-215">vppTokenAppleId</span></span>|<span data-ttu-id="af7d6-216">String</span><span class="sxs-lookup"><span data-stu-id="af7d6-216">String</span></span>|<span data-ttu-id="af7d6-217">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="af7d6-217">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="af7d6-218">bundleId</span><span class="sxs-lookup"><span data-stu-id="af7d6-218">bundleId</span></span>|<span data-ttu-id="af7d6-219">字符串</span><span class="sxs-lookup"><span data-stu-id="af7d6-219">String</span></span>|<span data-ttu-id="af7d6-220">标识名称。</span><span class="sxs-lookup"><span data-stu-id="af7d6-220">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="af7d6-221">响应</span><span class="sxs-lookup"><span data-stu-id="af7d6-221">Response</span></span>
<span data-ttu-id="af7d6-222">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppApp](../resources/intune-apps-iosvppapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="af7d6-222">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af7d6-223">示例</span><span class="sxs-lookup"><span data-stu-id="af7d6-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="af7d6-224">请求</span><span class="sxs-lookup"><span data-stu-id="af7d6-224">Request</span></span>
<span data-ttu-id="af7d6-225">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="af7d6-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="af7d6-226">响应</span><span class="sxs-lookup"><span data-stu-id="af7d6-226">Response</span></span>
<span data-ttu-id="af7d6-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="af7d6-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




