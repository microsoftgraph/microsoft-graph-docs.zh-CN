---
title: 创建 iosLobApp
description: 创建新的 iosLobApp 对象。
ms.openlocfilehash: 2720192b45dcc55f74881163c93205ad5fecb24c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042725"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="18def-103">创建 iosLobApp</span><span class="sxs-lookup"><span data-stu-id="18def-103">Create iosLobApp</span></span>

> <span data-ttu-id="18def-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="18def-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18def-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="18def-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18def-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="18def-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18def-107">创建新的 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18def-107">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="18def-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="18def-108">Prerequisites</span></span>
<span data-ttu-id="18def-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="18def-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18def-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="18def-111">Permission type</span></span>|<span data-ttu-id="18def-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="18def-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18def-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18def-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18def-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18def-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="18def-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18def-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18def-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="18def-116">Not supported.</span></span>|
|<span data-ttu-id="18def-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="18def-117">Application</span></span>|<span data-ttu-id="18def-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="18def-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18def-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18def-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="18def-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="18def-120">Request headers</span></span>
|<span data-ttu-id="18def-121">标头</span><span class="sxs-lookup"><span data-stu-id="18def-121">Header</span></span>|<span data-ttu-id="18def-122">值</span><span class="sxs-lookup"><span data-stu-id="18def-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18def-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18def-123">Authorization</span></span>|<span data-ttu-id="18def-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="18def-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18def-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18def-125">Accept</span></span>|<span data-ttu-id="18def-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18def-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18def-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="18def-127">Request body</span></span>
<span data-ttu-id="18def-128">在请求正文中，提供 iosLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18def-128">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="18def-129">下表显示了创建 iosLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="18def-129">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="18def-130">属性</span><span class="sxs-lookup"><span data-stu-id="18def-130">Property</span></span>|<span data-ttu-id="18def-131">类型</span><span class="sxs-lookup"><span data-stu-id="18def-131">Type</span></span>|<span data-ttu-id="18def-132">说明</span><span class="sxs-lookup"><span data-stu-id="18def-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18def-133">id</span><span class="sxs-lookup"><span data-stu-id="18def-133">id</span></span>|<span data-ttu-id="18def-134">String</span><span class="sxs-lookup"><span data-stu-id="18def-134">String</span></span>|<span data-ttu-id="18def-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="18def-135">Key of the entity.</span></span> <span data-ttu-id="18def-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18def-137">displayName</span><span class="sxs-lookup"><span data-stu-id="18def-137">displayName</span></span>|<span data-ttu-id="18def-138">String</span><span class="sxs-lookup"><span data-stu-id="18def-138">String</span></span>|<span data-ttu-id="18def-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="18def-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="18def-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18def-141">description</span><span class="sxs-lookup"><span data-stu-id="18def-141">description</span></span>|<span data-ttu-id="18def-142">String</span><span class="sxs-lookup"><span data-stu-id="18def-142">String</span></span>|<span data-ttu-id="18def-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="18def-143">The description of the app.</span></span> <span data-ttu-id="18def-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18def-145">publisher</span><span class="sxs-lookup"><span data-stu-id="18def-145">publisher</span></span>|<span data-ttu-id="18def-146">String</span><span class="sxs-lookup"><span data-stu-id="18def-146">String</span></span>|<span data-ttu-id="18def-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="18def-147">The publisher of the app.</span></span> <span data-ttu-id="18def-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18def-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="18def-149">largeIcon</span></span>|[<span data-ttu-id="18def-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="18def-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="18def-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="18def-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="18def-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18def-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18def-153">createdDateTime</span></span>|<span data-ttu-id="18def-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18def-154">DateTimeOffset</span></span>|<span data-ttu-id="18def-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="18def-155">The date and time the app was created.</span></span> <span data-ttu-id="18def-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18def-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18def-157">lastModifiedDateTime</span></span>|<span data-ttu-id="18def-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18def-158">DateTimeOffset</span></span>|<span data-ttu-id="18def-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="18def-159">The date and time the app was last modified.</span></span> <span data-ttu-id="18def-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18def-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="18def-161">isFeatured</span></span>|<span data-ttu-id="18def-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="18def-162">Boolean</span></span>|<span data-ttu-id="18def-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18def-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="18def-164">privacyInformationUrl</span></span>|<span data-ttu-id="18def-165">String</span><span class="sxs-lookup"><span data-stu-id="18def-165">String</span></span>|<span data-ttu-id="18def-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="18def-166">The privacy statement Url.</span></span> <span data-ttu-id="18def-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18def-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="18def-168">informationUrl</span></span>|<span data-ttu-id="18def-169">String</span><span class="sxs-lookup"><span data-stu-id="18def-169">String</span></span>|<span data-ttu-id="18def-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="18def-170">The more information Url.</span></span> <span data-ttu-id="18def-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18def-172">owner</span><span class="sxs-lookup"><span data-stu-id="18def-172">owner</span></span>|<span data-ttu-id="18def-173">String</span><span class="sxs-lookup"><span data-stu-id="18def-173">String</span></span>|<span data-ttu-id="18def-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="18def-174">The owner of the app.</span></span> <span data-ttu-id="18def-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18def-176">developer</span><span class="sxs-lookup"><span data-stu-id="18def-176">developer</span></span>|<span data-ttu-id="18def-177">String</span><span class="sxs-lookup"><span data-stu-id="18def-177">String</span></span>|<span data-ttu-id="18def-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="18def-178">The developer of the app.</span></span> <span data-ttu-id="18def-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18def-180">notes</span><span class="sxs-lookup"><span data-stu-id="18def-180">notes</span></span>|<span data-ttu-id="18def-181">String</span><span class="sxs-lookup"><span data-stu-id="18def-181">String</span></span>|<span data-ttu-id="18def-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="18def-182">Notes for the app.</span></span> <span data-ttu-id="18def-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18def-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="18def-184">uploadState</span></span>|<span data-ttu-id="18def-185">Int32</span><span class="sxs-lookup"><span data-stu-id="18def-185">Int32</span></span>|<span data-ttu-id="18def-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="18def-186">The upload state.</span></span> <span data-ttu-id="18def-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="18def-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="18def-188">publishingState</span></span>|[<span data-ttu-id="18def-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="18def-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="18def-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="18def-190">The publishing state for the app.</span></span> <span data-ttu-id="18def-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="18def-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="18def-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="18def-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="18def-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="18def-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="18def-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="18def-194">committedContentVersion</span></span>|<span data-ttu-id="18def-195">String</span><span class="sxs-lookup"><span data-stu-id="18def-195">String</span></span>|<span data-ttu-id="18def-196">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="18def-196">The internal committed content version.</span></span> <span data-ttu-id="18def-197">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="18def-198">fileName</span><span class="sxs-lookup"><span data-stu-id="18def-198">fileName</span></span>|<span data-ttu-id="18def-199">String</span><span class="sxs-lookup"><span data-stu-id="18def-199">String</span></span>|<span data-ttu-id="18def-200">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="18def-200">The name of the main Lob application file.</span></span> <span data-ttu-id="18def-201">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="18def-202">size</span><span class="sxs-lookup"><span data-stu-id="18def-202">size</span></span>|<span data-ttu-id="18def-203">Int64</span><span class="sxs-lookup"><span data-stu-id="18def-203">Int64</span></span>|<span data-ttu-id="18def-204">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="18def-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="18def-205">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="18def-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="18def-206">bundleId</span><span class="sxs-lookup"><span data-stu-id="18def-206">bundleId</span></span>|<span data-ttu-id="18def-207">String</span><span class="sxs-lookup"><span data-stu-id="18def-207">String</span></span>|<span data-ttu-id="18def-208">标识名称。</span><span class="sxs-lookup"><span data-stu-id="18def-208">The Identity Name.</span></span>|
|<span data-ttu-id="18def-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="18def-209">applicableDeviceType</span></span>|[<span data-ttu-id="18def-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="18def-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="18def-211">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="18def-211">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="18def-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="18def-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="18def-213">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="18def-213">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="18def-214">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="18def-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="18def-215">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="18def-215">expirationDateTime</span></span>|<span data-ttu-id="18def-216">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18def-216">DateTimeOffset</span></span>|<span data-ttu-id="18def-217">过期时间。</span><span class="sxs-lookup"><span data-stu-id="18def-217">The expiration time.</span></span>|
|<span data-ttu-id="18def-218">versionNumber</span><span class="sxs-lookup"><span data-stu-id="18def-218">versionNumber</span></span>|<span data-ttu-id="18def-219">String</span><span class="sxs-lookup"><span data-stu-id="18def-219">String</span></span>|<span data-ttu-id="18def-220">iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="18def-220">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="18def-221">buildNumber</span><span class="sxs-lookup"><span data-stu-id="18def-221">buildNumber</span></span>|<span data-ttu-id="18def-222">String</span><span class="sxs-lookup"><span data-stu-id="18def-222">String</span></span>|<span data-ttu-id="18def-223">iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="18def-223">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="18def-224">identityVersion</span><span class="sxs-lookup"><span data-stu-id="18def-224">identityVersion</span></span>|<span data-ttu-id="18def-225">String</span><span class="sxs-lookup"><span data-stu-id="18def-225">String</span></span>|<span data-ttu-id="18def-226">标识版本。</span><span class="sxs-lookup"><span data-stu-id="18def-226">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="18def-227">响应</span><span class="sxs-lookup"><span data-stu-id="18def-227">Response</span></span>
<span data-ttu-id="18def-228">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18def-228">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18def-229">示例</span><span class="sxs-lookup"><span data-stu-id="18def-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="18def-230">请求</span><span class="sxs-lookup"><span data-stu-id="18def-230">Request</span></span>
<span data-ttu-id="18def-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18def-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1343

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="18def-232">响应</span><span class="sxs-lookup"><span data-stu-id="18def-232">Response</span></span>
<span data-ttu-id="18def-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="18def-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1451

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
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
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```





