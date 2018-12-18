---
title: 创建 managedIOSStoreApp
description: 创建新的 managedIOSStoreApp 对象。
author: tfitzmac
ms.openlocfilehash: cfc72ef6fa4de29d8e6d48ef4786dd19a7ada3d1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335726"
---
# <a name="create-managediosstoreapp"></a><span data-ttu-id="c12f4-103">创建 managedIOSStoreApp</span><span class="sxs-lookup"><span data-stu-id="c12f4-103">Create managedIOSStoreApp</span></span>

> <span data-ttu-id="c12f4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c12f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c12f4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c12f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c12f4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c12f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c12f4-107">创建新的 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c12f4-107">Create a new [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c12f4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c12f4-108">Prerequisites</span></span>
<span data-ttu-id="c12f4-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c12f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c12f4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c12f4-111">Permission type</span></span>|<span data-ttu-id="c12f4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c12f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c12f4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c12f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c12f4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c12f4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c12f4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c12f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c12f4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c12f4-116">Not supported.</span></span>|
|<span data-ttu-id="c12f4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c12f4-117">Application</span></span>|<span data-ttu-id="c12f4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c12f4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c12f4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c12f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c12f4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c12f4-120">Request headers</span></span>
|<span data-ttu-id="c12f4-121">标头</span><span class="sxs-lookup"><span data-stu-id="c12f4-121">Header</span></span>|<span data-ttu-id="c12f4-122">值</span><span class="sxs-lookup"><span data-stu-id="c12f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c12f4-123">授权</span><span class="sxs-lookup"><span data-stu-id="c12f4-123">Authorization</span></span>|<span data-ttu-id="c12f4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c12f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c12f4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c12f4-125">Accept</span></span>|<span data-ttu-id="c12f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c12f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c12f4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c12f4-127">Request body</span></span>
<span data-ttu-id="c12f4-128">在请求正文中，提供 managedIOSStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c12f4-128">In the request body, supply a JSON representation for the managedIOSStoreApp object.</span></span>

<span data-ttu-id="c12f4-129">下表显示创建 managedIOSStoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c12f4-129">The following table shows the properties that are required when you create the managedIOSStoreApp.</span></span>

|<span data-ttu-id="c12f4-130">属性</span><span class="sxs-lookup"><span data-stu-id="c12f4-130">Property</span></span>|<span data-ttu-id="c12f4-131">类型</span><span class="sxs-lookup"><span data-stu-id="c12f4-131">Type</span></span>|<span data-ttu-id="c12f4-132">说明</span><span class="sxs-lookup"><span data-stu-id="c12f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c12f4-133">id</span><span class="sxs-lookup"><span data-stu-id="c12f4-133">id</span></span>|<span data-ttu-id="c12f4-134">String</span><span class="sxs-lookup"><span data-stu-id="c12f4-134">String</span></span>|<span data-ttu-id="c12f4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c12f4-135">Key of the entity.</span></span> <span data-ttu-id="c12f4-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c12f4-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c12f4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c12f4-137">displayName</span></span>|<span data-ttu-id="c12f4-138">String</span><span class="sxs-lookup"><span data-stu-id="c12f4-138">String</span></span>|<span data-ttu-id="c12f4-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="c12f4-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c12f4-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c12f4-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c12f4-141">description</span><span class="sxs-lookup"><span data-stu-id="c12f4-141">description</span></span>|<span data-ttu-id="c12f4-142">String</span><span class="sxs-lookup"><span data-stu-id="c12f4-142">String</span></span>|<span data-ttu-id="c12f4-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="c12f4-143">The description of the app.</span></span> <span data-ttu-id="c12f4-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c12f4-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c12f4-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c12f4-145">publisher</span></span>|<span data-ttu-id="c12f4-146">String</span><span class="sxs-lookup"><span data-stu-id="c12f4-146">String</span></span>|<span data-ttu-id="c12f4-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="c12f4-147">The publisher of the app.</span></span> <span data-ttu-id="c12f4-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c12f4-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c12f4-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c12f4-149">largeIcon</span></span>|[<span data-ttu-id="c12f4-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c12f4-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c12f4-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="c12f4-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c12f4-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c12f4-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c12f4-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c12f4-153">createdDateTime</span></span>|<span data-ttu-id="c12f4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c12f4-154">DateTimeOffset</span></span>|<span data-ttu-id="c12f4-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c12f4-155">The date and time the app was created.</span></span> <span data-ttu-id="c12f4-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c12f4-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c12f4-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c12f4-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c12f4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c12f4-158">DateTimeOffset</span></span>|<span data-ttu-id="c12f4-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c12f4-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c12f4-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c12f4-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c12f4-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c12f4-161">isFeatured</span></span>|<span data-ttu-id="c12f4-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c12f4-162">Boolean</span></span>|<span data-ttu-id="c12f4-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c12f4-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c12f4-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c12f4-164">privacyInformationUrl</span></span>|<span data-ttu-id="c12f4-165">String</span><span class="sxs-lookup"><span data-stu-id="c12f4-165">String</span></span>|<span data-ttu-id="c12f4-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="c12f4-166">The privacy statement Url.</span></span> <span data-ttu-id="c12f4-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c12f4-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c12f4-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c12f4-168">informationUrl</span></span>|<span data-ttu-id="c12f4-169">String</span><span class="sxs-lookup"><span data-stu-id="c12f4-169">String</span></span>|<span data-ttu-id="c12f4-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="c12f4-170">The more information Url.</span></span> <span data-ttu-id="c12f4-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c12f4-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c12f4-172">owner</span><span class="sxs-lookup"><span data-stu-id="c12f4-172">owner</span></span>|<span data-ttu-id="c12f4-173">String</span><span class="sxs-lookup"><span data-stu-id="c12f4-173">String</span></span>|<span data-ttu-id="c12f4-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="c12f4-174">The owner of the app.</span></span> <span data-ttu-id="c12f4-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c12f4-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c12f4-176">developer</span><span class="sxs-lookup"><span data-stu-id="c12f4-176">developer</span></span>|<span data-ttu-id="c12f4-177">String</span><span class="sxs-lookup"><span data-stu-id="c12f4-177">String</span></span>|<span data-ttu-id="c12f4-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="c12f4-178">The developer of the app.</span></span> <span data-ttu-id="c12f4-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c12f4-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c12f4-180">notes</span><span class="sxs-lookup"><span data-stu-id="c12f4-180">notes</span></span>|<span data-ttu-id="c12f4-181">String</span><span class="sxs-lookup"><span data-stu-id="c12f4-181">String</span></span>|<span data-ttu-id="c12f4-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="c12f4-182">Notes for the app.</span></span> <span data-ttu-id="c12f4-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c12f4-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c12f4-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c12f4-184">uploadState</span></span>|<span data-ttu-id="c12f4-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c12f4-185">Int32</span></span>|<span data-ttu-id="c12f4-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="c12f4-186">The upload state.</span></span> <span data-ttu-id="c12f4-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c12f4-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c12f4-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="c12f4-188">publishingState</span></span>|[<span data-ttu-id="c12f4-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c12f4-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c12f4-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="c12f4-190">The publishing state for the app.</span></span> <span data-ttu-id="c12f4-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="c12f4-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c12f4-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="c12f4-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c12f4-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="c12f4-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c12f4-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="c12f4-194">appAvailability</span></span>|[<span data-ttu-id="c12f4-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="c12f4-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="c12f4-196">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="c12f4-196">The Application's availability.</span></span> <span data-ttu-id="c12f4-197">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="c12f4-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="c12f4-198">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="c12f4-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="c12f4-199">version</span><span class="sxs-lookup"><span data-stu-id="c12f4-199">version</span></span>|<span data-ttu-id="c12f4-200">String</span><span class="sxs-lookup"><span data-stu-id="c12f4-200">String</span></span>|<span data-ttu-id="c12f4-201">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="c12f4-201">The Application's version.</span></span> <span data-ttu-id="c12f4-202">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c12f4-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="c12f4-203">bundleId</span><span class="sxs-lookup"><span data-stu-id="c12f4-203">bundleId</span></span>|<span data-ttu-id="c12f4-204">String</span><span class="sxs-lookup"><span data-stu-id="c12f4-204">String</span></span>|<span data-ttu-id="c12f4-205">应用的捆绑 ID。</span><span class="sxs-lookup"><span data-stu-id="c12f4-205">The app's Bundle ID.</span></span>|
|<span data-ttu-id="c12f4-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c12f4-206">appStoreUrl</span></span>|<span data-ttu-id="c12f4-207">String</span><span class="sxs-lookup"><span data-stu-id="c12f4-207">String</span></span>|<span data-ttu-id="c12f4-208">Apple AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="c12f4-208">The Apple AppStoreUrl.</span></span>|
|<span data-ttu-id="c12f4-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="c12f4-209">applicableDeviceType</span></span>|[<span data-ttu-id="c12f4-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="c12f4-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="c12f4-211">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="c12f4-211">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="c12f4-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c12f4-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c12f4-213">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c12f4-213">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="c12f4-214">最低受支持操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="c12f4-214">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="c12f4-215">响应</span><span class="sxs-lookup"><span data-stu-id="c12f4-215">Response</span></span>
<span data-ttu-id="c12f4-216">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c12f4-216">If successful, this method returns a `201 Created` response code and a [managedIOSStoreApp](../resources/intune-apps-managediosstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c12f4-217">示例</span><span class="sxs-lookup"><span data-stu-id="c12f4-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="c12f4-218">请求</span><span class="sxs-lookup"><span data-stu-id="c12f4-218">Request</span></span>
<span data-ttu-id="c12f4-219">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c12f4-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1170

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="c12f4-220">响应</span><span class="sxs-lookup"><span data-stu-id="c12f4-220">Response</span></span>
<span data-ttu-id="c12f4-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c12f4-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1278

{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
  "id": "51b9830f-830f-51b9-0f83-b9510f83b951",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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





