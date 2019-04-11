---
title: 更新 iosStoreApp
description: 更新 iosStoreApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c7015b269b0b8d3e2107097b59561bd6680dab11
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780621"
---
# <a name="update-iosstoreapp"></a><span data-ttu-id="2bffd-103">更新 iosStoreApp</span><span class="sxs-lookup"><span data-stu-id="2bffd-103">Update iosStoreApp</span></span>

> <span data-ttu-id="2bffd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2bffd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bffd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2bffd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bffd-106">更新 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2bffd-106">Update the properties of a [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bffd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2bffd-107">Prerequisites</span></span>
<span data-ttu-id="2bffd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2bffd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bffd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2bffd-110">Permission type</span></span>|<span data-ttu-id="2bffd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2bffd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bffd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2bffd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2bffd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bffd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2bffd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2bffd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bffd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2bffd-115">Not supported.</span></span>|
|<span data-ttu-id="2bffd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2bffd-116">Application</span></span>|<span data-ttu-id="2bffd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2bffd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bffd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2bffd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="2bffd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2bffd-119">Request headers</span></span>
|<span data-ttu-id="2bffd-120">标头</span><span class="sxs-lookup"><span data-stu-id="2bffd-120">Header</span></span>|<span data-ttu-id="2bffd-121">值</span><span class="sxs-lookup"><span data-stu-id="2bffd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bffd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bffd-122">Authorization</span></span>|<span data-ttu-id="2bffd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2bffd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bffd-124">接受</span><span class="sxs-lookup"><span data-stu-id="2bffd-124">Accept</span></span>|<span data-ttu-id="2bffd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2bffd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bffd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2bffd-126">Request body</span></span>
<span data-ttu-id="2bffd-127">在请求正文中，提供 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bffd-127">In the request body, supply a JSON representation for the [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object.</span></span>

<span data-ttu-id="2bffd-128">下表显示了创建 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2bffd-128">The following table shows the properties that are required when you create the [iosStoreApp](../resources/intune-apps-iosstoreapp.md).</span></span>

|<span data-ttu-id="2bffd-129">属性</span><span class="sxs-lookup"><span data-stu-id="2bffd-129">Property</span></span>|<span data-ttu-id="2bffd-130">类型</span><span class="sxs-lookup"><span data-stu-id="2bffd-130">Type</span></span>|<span data-ttu-id="2bffd-131">说明</span><span class="sxs-lookup"><span data-stu-id="2bffd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bffd-132">id</span><span class="sxs-lookup"><span data-stu-id="2bffd-132">id</span></span>|<span data-ttu-id="2bffd-133">String</span><span class="sxs-lookup"><span data-stu-id="2bffd-133">String</span></span>|<span data-ttu-id="2bffd-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2bffd-134">Key of the entity.</span></span> <span data-ttu-id="2bffd-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2bffd-136">displayName</span></span>|<span data-ttu-id="2bffd-137">String</span><span class="sxs-lookup"><span data-stu-id="2bffd-137">String</span></span>|<span data-ttu-id="2bffd-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="2bffd-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2bffd-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-140">description</span><span class="sxs-lookup"><span data-stu-id="2bffd-140">description</span></span>|<span data-ttu-id="2bffd-141">String</span><span class="sxs-lookup"><span data-stu-id="2bffd-141">String</span></span>|<span data-ttu-id="2bffd-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="2bffd-142">The description of the app.</span></span> <span data-ttu-id="2bffd-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-144">publisher</span><span class="sxs-lookup"><span data-stu-id="2bffd-144">publisher</span></span>|<span data-ttu-id="2bffd-145">String</span><span class="sxs-lookup"><span data-stu-id="2bffd-145">String</span></span>|<span data-ttu-id="2bffd-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="2bffd-146">The publisher of the app.</span></span> <span data-ttu-id="2bffd-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2bffd-148">largeIcon</span></span>|[<span data-ttu-id="2bffd-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2bffd-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2bffd-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="2bffd-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2bffd-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2bffd-152">createdDateTime</span></span>|<span data-ttu-id="2bffd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bffd-153">DateTimeOffset</span></span>|<span data-ttu-id="2bffd-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2bffd-154">The date and time the app was created.</span></span> <span data-ttu-id="2bffd-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2bffd-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2bffd-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bffd-157">DateTimeOffset</span></span>|<span data-ttu-id="2bffd-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2bffd-158">The date and time the app was last modified.</span></span> <span data-ttu-id="2bffd-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2bffd-160">isFeatured</span></span>|<span data-ttu-id="2bffd-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bffd-161">Boolean</span></span>|<span data-ttu-id="2bffd-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2bffd-163">privacyInformationUrl</span></span>|<span data-ttu-id="2bffd-164">String</span><span class="sxs-lookup"><span data-stu-id="2bffd-164">String</span></span>|<span data-ttu-id="2bffd-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="2bffd-165">The privacy statement Url.</span></span> <span data-ttu-id="2bffd-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2bffd-167">informationUrl</span></span>|<span data-ttu-id="2bffd-168">String</span><span class="sxs-lookup"><span data-stu-id="2bffd-168">String</span></span>|<span data-ttu-id="2bffd-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="2bffd-169">The more information Url.</span></span> <span data-ttu-id="2bffd-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-171">owner</span><span class="sxs-lookup"><span data-stu-id="2bffd-171">owner</span></span>|<span data-ttu-id="2bffd-172">字符串</span><span class="sxs-lookup"><span data-stu-id="2bffd-172">String</span></span>|<span data-ttu-id="2bffd-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="2bffd-173">The owner of the app.</span></span> <span data-ttu-id="2bffd-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-175">developer</span><span class="sxs-lookup"><span data-stu-id="2bffd-175">developer</span></span>|<span data-ttu-id="2bffd-176">String</span><span class="sxs-lookup"><span data-stu-id="2bffd-176">String</span></span>|<span data-ttu-id="2bffd-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="2bffd-177">The developer of the app.</span></span> <span data-ttu-id="2bffd-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-179">notes</span><span class="sxs-lookup"><span data-stu-id="2bffd-179">notes</span></span>|<span data-ttu-id="2bffd-180">String</span><span class="sxs-lookup"><span data-stu-id="2bffd-180">String</span></span>|<span data-ttu-id="2bffd-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="2bffd-181">Notes for the app.</span></span> <span data-ttu-id="2bffd-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="2bffd-183">uploadState</span></span>|<span data-ttu-id="2bffd-184">Int32</span><span class="sxs-lookup"><span data-stu-id="2bffd-184">Int32</span></span>|<span data-ttu-id="2bffd-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="2bffd-185">The upload state.</span></span> <span data-ttu-id="2bffd-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="2bffd-187">publishingState</span></span>|[<span data-ttu-id="2bffd-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2bffd-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2bffd-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="2bffd-189">The publishing state for the app.</span></span> <span data-ttu-id="2bffd-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="2bffd-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2bffd-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="2bffd-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2bffd-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="2bffd-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2bffd-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2bffd-193">isAssigned</span></span>|<span data-ttu-id="2bffd-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bffd-194">Boolean</span></span>|<span data-ttu-id="2bffd-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="2bffd-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2bffd-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2bffd-197">roleScopeTagIds</span></span>|<span data-ttu-id="2bffd-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="2bffd-198">String collection</span></span>|<span data-ttu-id="2bffd-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="2bffd-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2bffd-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="2bffd-201">dependentAppCount</span></span>|<span data-ttu-id="2bffd-202">Int32</span><span class="sxs-lookup"><span data-stu-id="2bffd-202">Int32</span></span>|<span data-ttu-id="2bffd-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="2bffd-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="2bffd-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2bffd-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2bffd-205">bundleId</span><span class="sxs-lookup"><span data-stu-id="2bffd-205">bundleId</span></span>|<span data-ttu-id="2bffd-206">String</span><span class="sxs-lookup"><span data-stu-id="2bffd-206">String</span></span>|<span data-ttu-id="2bffd-207">标识名称。</span><span class="sxs-lookup"><span data-stu-id="2bffd-207">The Identity Name.</span></span>|
|<span data-ttu-id="2bffd-208">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2bffd-208">appStoreUrl</span></span>|<span data-ttu-id="2bffd-209">String</span><span class="sxs-lookup"><span data-stu-id="2bffd-209">String</span></span>|<span data-ttu-id="2bffd-210">Apple App Store URL</span><span class="sxs-lookup"><span data-stu-id="2bffd-210">The Apple App Store URL</span></span>|
|<span data-ttu-id="2bffd-211">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="2bffd-211">applicableDeviceType</span></span>|[<span data-ttu-id="2bffd-212">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="2bffd-212">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="2bffd-213">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="2bffd-213">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="2bffd-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2bffd-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2bffd-215">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2bffd-215">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="2bffd-216">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="2bffd-216">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="2bffd-217">响应</span><span class="sxs-lookup"><span data-stu-id="2bffd-217">Response</span></span>
<span data-ttu-id="2bffd-218">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [iosStoreApp](../resources/intune-apps-iosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2bffd-218">If successful, this method returns a `200 OK` response code and an updated [iosStoreApp](../resources/intune-apps-iosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bffd-219">示例</span><span class="sxs-lookup"><span data-stu-id="2bffd-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bffd-220">请求</span><span class="sxs-lookup"><span data-stu-id="2bffd-220">Request</span></span>
<span data-ttu-id="2bffd-221">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2bffd-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1140

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="2bffd-222">响应</span><span class="sxs-lookup"><span data-stu-id="2bffd-222">Response</span></span>
<span data-ttu-id="2bffd-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2bffd-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1312

{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "a04adbe2-dbe2-a04a-e2db-4aa0e2db4aa0",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "bundleId": "Bundle Id value",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  }
}
```





