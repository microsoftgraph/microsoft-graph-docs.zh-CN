---
title: 更新 iosLobApp
description: 更新 iosLobApp 对象的属性。
ms.openlocfilehash: 159bdb4091d5ab0005ad0e9c1ba1720ee85a775e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009802"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="fbace-103">更新 iosLobApp</span><span class="sxs-lookup"><span data-stu-id="fbace-103">Update iosLobApp</span></span>

> <span data-ttu-id="fbace-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fbace-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbace-105">更新 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fbace-105">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fbace-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="fbace-106">Prerequisites</span></span>
<span data-ttu-id="fbace-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fbace-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbace-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fbace-109">Permission type</span></span>|<span data-ttu-id="fbace-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fbace-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbace-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fbace-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fbace-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbace-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fbace-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fbace-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbace-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbace-114">Not supported.</span></span>|
|<span data-ttu-id="fbace-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fbace-115">Application</span></span>|<span data-ttu-id="fbace-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbace-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbace-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fbace-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="fbace-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fbace-118">Request headers</span></span>
|<span data-ttu-id="fbace-119">标头</span><span class="sxs-lookup"><span data-stu-id="fbace-119">Header</span></span>|<span data-ttu-id="fbace-120">值</span><span class="sxs-lookup"><span data-stu-id="fbace-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbace-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbace-121">Authorization</span></span>|<span data-ttu-id="fbace-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fbace-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbace-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fbace-123">Accept</span></span>|<span data-ttu-id="fbace-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fbace-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbace-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fbace-125">Request body</span></span>
<span data-ttu-id="fbace-126">在请求正文中，提供 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbace-126">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="fbace-127">下表显示了创建 [iosLobApp](../resources/intune-apps-ioslobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fbace-127">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="fbace-128">属性</span><span class="sxs-lookup"><span data-stu-id="fbace-128">Property</span></span>|<span data-ttu-id="fbace-129">类型</span><span class="sxs-lookup"><span data-stu-id="fbace-129">Type</span></span>|<span data-ttu-id="fbace-130">说明</span><span class="sxs-lookup"><span data-stu-id="fbace-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbace-131">id</span><span class="sxs-lookup"><span data-stu-id="fbace-131">id</span></span>|<span data-ttu-id="fbace-132">String</span><span class="sxs-lookup"><span data-stu-id="fbace-132">String</span></span>|<span data-ttu-id="fbace-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fbace-133">Key of the entity.</span></span> <span data-ttu-id="fbace-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbace-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fbace-135">displayName</span></span>|<span data-ttu-id="fbace-136">String</span><span class="sxs-lookup"><span data-stu-id="fbace-136">String</span></span>|<span data-ttu-id="fbace-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="fbace-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fbace-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbace-139">description</span><span class="sxs-lookup"><span data-stu-id="fbace-139">description</span></span>|<span data-ttu-id="fbace-140">String</span><span class="sxs-lookup"><span data-stu-id="fbace-140">String</span></span>|<span data-ttu-id="fbace-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="fbace-141">The description of the app.</span></span> <span data-ttu-id="fbace-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbace-143">publisher</span><span class="sxs-lookup"><span data-stu-id="fbace-143">publisher</span></span>|<span data-ttu-id="fbace-144">String</span><span class="sxs-lookup"><span data-stu-id="fbace-144">String</span></span>|<span data-ttu-id="fbace-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="fbace-145">The publisher of the app.</span></span> <span data-ttu-id="fbace-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbace-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fbace-147">largeIcon</span></span>|[<span data-ttu-id="fbace-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fbace-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fbace-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="fbace-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fbace-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbace-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbace-151">createdDateTime</span></span>|<span data-ttu-id="fbace-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbace-152">DateTimeOffset</span></span>|<span data-ttu-id="fbace-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fbace-153">The date and time the app was created.</span></span> <span data-ttu-id="fbace-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbace-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fbace-155">lastModifiedDateTime</span></span>|<span data-ttu-id="fbace-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbace-156">DateTimeOffset</span></span>|<span data-ttu-id="fbace-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fbace-157">The date and time the app was last modified.</span></span> <span data-ttu-id="fbace-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbace-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fbace-159">isFeatured</span></span>|<span data-ttu-id="fbace-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbace-160">Boolean</span></span>|<span data-ttu-id="fbace-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbace-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fbace-162">privacyInformationUrl</span></span>|<span data-ttu-id="fbace-163">String</span><span class="sxs-lookup"><span data-stu-id="fbace-163">String</span></span>|<span data-ttu-id="fbace-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="fbace-164">The privacy statement Url.</span></span> <span data-ttu-id="fbace-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbace-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fbace-166">informationUrl</span></span>|<span data-ttu-id="fbace-167">String</span><span class="sxs-lookup"><span data-stu-id="fbace-167">String</span></span>|<span data-ttu-id="fbace-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="fbace-168">The more information Url.</span></span> <span data-ttu-id="fbace-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbace-170">owner</span><span class="sxs-lookup"><span data-stu-id="fbace-170">owner</span></span>|<span data-ttu-id="fbace-171">String</span><span class="sxs-lookup"><span data-stu-id="fbace-171">String</span></span>|<span data-ttu-id="fbace-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="fbace-172">The owner of the app.</span></span> <span data-ttu-id="fbace-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbace-174">developer</span><span class="sxs-lookup"><span data-stu-id="fbace-174">developer</span></span>|<span data-ttu-id="fbace-175">String</span><span class="sxs-lookup"><span data-stu-id="fbace-175">String</span></span>|<span data-ttu-id="fbace-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="fbace-176">The developer of the app.</span></span> <span data-ttu-id="fbace-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbace-178">notes</span><span class="sxs-lookup"><span data-stu-id="fbace-178">notes</span></span>|<span data-ttu-id="fbace-179">String</span><span class="sxs-lookup"><span data-stu-id="fbace-179">String</span></span>|<span data-ttu-id="fbace-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="fbace-180">Notes for the app.</span></span> <span data-ttu-id="fbace-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fbace-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="fbace-182">publishingState</span></span>|[<span data-ttu-id="fbace-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fbace-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fbace-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="fbace-184">The publishing state for the app.</span></span> <span data-ttu-id="fbace-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="fbace-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fbace-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="fbace-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="fbace-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="fbace-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fbace-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="fbace-188">committedContentVersion</span></span>|<span data-ttu-id="fbace-189">String</span><span class="sxs-lookup"><span data-stu-id="fbace-189">String</span></span>|<span data-ttu-id="fbace-190">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="fbace-190">The internal committed content version.</span></span> <span data-ttu-id="fbace-191">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fbace-192">fileName</span><span class="sxs-lookup"><span data-stu-id="fbace-192">fileName</span></span>|<span data-ttu-id="fbace-193">String</span><span class="sxs-lookup"><span data-stu-id="fbace-193">String</span></span>|<span data-ttu-id="fbace-194">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="fbace-194">The name of the main Lob application file.</span></span> <span data-ttu-id="fbace-195">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fbace-196">size</span><span class="sxs-lookup"><span data-stu-id="fbace-196">size</span></span>|<span data-ttu-id="fbace-197">Int64</span><span class="sxs-lookup"><span data-stu-id="fbace-197">Int64</span></span>|<span data-ttu-id="fbace-198">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="fbace-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="fbace-199">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbace-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fbace-200">bundleId</span><span class="sxs-lookup"><span data-stu-id="fbace-200">bundleId</span></span>|<span data-ttu-id="fbace-201">String</span><span class="sxs-lookup"><span data-stu-id="fbace-201">String</span></span>|<span data-ttu-id="fbace-202">标识名称。</span><span class="sxs-lookup"><span data-stu-id="fbace-202">The Identity Name.</span></span>|
|<span data-ttu-id="fbace-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="fbace-203">applicableDeviceType</span></span>|[<span data-ttu-id="fbace-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="fbace-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="fbace-205">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="fbace-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="fbace-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fbace-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fbace-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fbace-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="fbace-208">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="fbace-208">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="fbace-209">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fbace-209">expirationDateTime</span></span>|<span data-ttu-id="fbace-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbace-210">DateTimeOffset</span></span>|<span data-ttu-id="fbace-211">过期时间。</span><span class="sxs-lookup"><span data-stu-id="fbace-211">The expiration time.</span></span>|
|<span data-ttu-id="fbace-212">versionNumber</span><span class="sxs-lookup"><span data-stu-id="fbace-212">versionNumber</span></span>|<span data-ttu-id="fbace-213">String</span><span class="sxs-lookup"><span data-stu-id="fbace-213">String</span></span>|<span data-ttu-id="fbace-214">iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="fbace-214">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="fbace-215">buildNumber</span><span class="sxs-lookup"><span data-stu-id="fbace-215">buildNumber</span></span>|<span data-ttu-id="fbace-216">String</span><span class="sxs-lookup"><span data-stu-id="fbace-216">String</span></span>|<span data-ttu-id="fbace-217">iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="fbace-217">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="fbace-218">响应</span><span class="sxs-lookup"><span data-stu-id="fbace-218">Response</span></span>
<span data-ttu-id="fbace-219">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fbace-219">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbace-220">示例</span><span class="sxs-lookup"><span data-stu-id="fbace-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="fbace-221">请求</span><span class="sxs-lookup"><span data-stu-id="fbace-221">Request</span></span>
<span data-ttu-id="fbace-222">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fbace-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1209

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
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
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
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="fbace-223">响应</span><span class="sxs-lookup"><span data-stu-id="fbace-223">Response</span></span>
<span data-ttu-id="fbace-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fbace-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1381

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
  "buildNumber": "Build Number value"
}
```



