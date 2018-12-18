---
title: 创建 iosLobApp
description: 创建新的 iosLobApp 对象。
author: tfitzmac
ms.openlocfilehash: 8ea8c1637f963fa25c8afa20c21720870b63a462
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320732"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="3dfce-103">创建 iosLobApp</span><span class="sxs-lookup"><span data-stu-id="3dfce-103">Create iosLobApp</span></span>

> <span data-ttu-id="3dfce-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3dfce-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3dfce-105">创建新的 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3dfce-105">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3dfce-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="3dfce-106">Prerequisites</span></span>
<span data-ttu-id="3dfce-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="3dfce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3dfce-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3dfce-109">Permission type</span></span>|<span data-ttu-id="3dfce-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3dfce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3dfce-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3dfce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3dfce-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dfce-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3dfce-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3dfce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3dfce-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dfce-114">Not supported.</span></span>|
|<span data-ttu-id="3dfce-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3dfce-115">Application</span></span>|<span data-ttu-id="3dfce-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dfce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3dfce-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3dfce-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3dfce-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3dfce-118">Request headers</span></span>
|<span data-ttu-id="3dfce-119">标头</span><span class="sxs-lookup"><span data-stu-id="3dfce-119">Header</span></span>|<span data-ttu-id="3dfce-120">值</span><span class="sxs-lookup"><span data-stu-id="3dfce-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3dfce-121">授权</span><span class="sxs-lookup"><span data-stu-id="3dfce-121">Authorization</span></span>|<span data-ttu-id="3dfce-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3dfce-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3dfce-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3dfce-123">Accept</span></span>|<span data-ttu-id="3dfce-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3dfce-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3dfce-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3dfce-125">Request body</span></span>
<span data-ttu-id="3dfce-126">在请求正文中，提供 iosLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3dfce-126">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="3dfce-127">下表显示了创建 iosLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3dfce-127">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="3dfce-128">属性</span><span class="sxs-lookup"><span data-stu-id="3dfce-128">Property</span></span>|<span data-ttu-id="3dfce-129">类型</span><span class="sxs-lookup"><span data-stu-id="3dfce-129">Type</span></span>|<span data-ttu-id="3dfce-130">说明</span><span class="sxs-lookup"><span data-stu-id="3dfce-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dfce-131">id</span><span class="sxs-lookup"><span data-stu-id="3dfce-131">id</span></span>|<span data-ttu-id="3dfce-132">String</span><span class="sxs-lookup"><span data-stu-id="3dfce-132">String</span></span>|<span data-ttu-id="3dfce-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3dfce-133">Key of the entity.</span></span> <span data-ttu-id="3dfce-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3dfce-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3dfce-135">displayName</span></span>|<span data-ttu-id="3dfce-136">String</span><span class="sxs-lookup"><span data-stu-id="3dfce-136">String</span></span>|<span data-ttu-id="3dfce-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="3dfce-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3dfce-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3dfce-139">description</span><span class="sxs-lookup"><span data-stu-id="3dfce-139">description</span></span>|<span data-ttu-id="3dfce-140">String</span><span class="sxs-lookup"><span data-stu-id="3dfce-140">String</span></span>|<span data-ttu-id="3dfce-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="3dfce-141">The description of the app.</span></span> <span data-ttu-id="3dfce-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3dfce-143">publisher</span><span class="sxs-lookup"><span data-stu-id="3dfce-143">publisher</span></span>|<span data-ttu-id="3dfce-144">String</span><span class="sxs-lookup"><span data-stu-id="3dfce-144">String</span></span>|<span data-ttu-id="3dfce-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="3dfce-145">The publisher of the app.</span></span> <span data-ttu-id="3dfce-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3dfce-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3dfce-147">largeIcon</span></span>|[<span data-ttu-id="3dfce-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3dfce-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3dfce-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="3dfce-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3dfce-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3dfce-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3dfce-151">createdDateTime</span></span>|<span data-ttu-id="3dfce-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dfce-152">DateTimeOffset</span></span>|<span data-ttu-id="3dfce-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3dfce-153">The date and time the app was created.</span></span> <span data-ttu-id="3dfce-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3dfce-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3dfce-155">lastModifiedDateTime</span></span>|<span data-ttu-id="3dfce-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dfce-156">DateTimeOffset</span></span>|<span data-ttu-id="3dfce-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3dfce-157">The date and time the app was last modified.</span></span> <span data-ttu-id="3dfce-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3dfce-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3dfce-159">isFeatured</span></span>|<span data-ttu-id="3dfce-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfce-160">Boolean</span></span>|<span data-ttu-id="3dfce-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3dfce-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3dfce-162">privacyInformationUrl</span></span>|<span data-ttu-id="3dfce-163">String</span><span class="sxs-lookup"><span data-stu-id="3dfce-163">String</span></span>|<span data-ttu-id="3dfce-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="3dfce-164">The privacy statement Url.</span></span> <span data-ttu-id="3dfce-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3dfce-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3dfce-166">informationUrl</span></span>|<span data-ttu-id="3dfce-167">String</span><span class="sxs-lookup"><span data-stu-id="3dfce-167">String</span></span>|<span data-ttu-id="3dfce-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="3dfce-168">The more information Url.</span></span> <span data-ttu-id="3dfce-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3dfce-170">owner</span><span class="sxs-lookup"><span data-stu-id="3dfce-170">owner</span></span>|<span data-ttu-id="3dfce-171">String</span><span class="sxs-lookup"><span data-stu-id="3dfce-171">String</span></span>|<span data-ttu-id="3dfce-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="3dfce-172">The owner of the app.</span></span> <span data-ttu-id="3dfce-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3dfce-174">developer</span><span class="sxs-lookup"><span data-stu-id="3dfce-174">developer</span></span>|<span data-ttu-id="3dfce-175">String</span><span class="sxs-lookup"><span data-stu-id="3dfce-175">String</span></span>|<span data-ttu-id="3dfce-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="3dfce-176">The developer of the app.</span></span> <span data-ttu-id="3dfce-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3dfce-178">notes</span><span class="sxs-lookup"><span data-stu-id="3dfce-178">notes</span></span>|<span data-ttu-id="3dfce-179">String</span><span class="sxs-lookup"><span data-stu-id="3dfce-179">String</span></span>|<span data-ttu-id="3dfce-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="3dfce-180">Notes for the app.</span></span> <span data-ttu-id="3dfce-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3dfce-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="3dfce-182">publishingState</span></span>|[<span data-ttu-id="3dfce-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3dfce-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3dfce-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="3dfce-184">The publishing state for the app.</span></span> <span data-ttu-id="3dfce-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="3dfce-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3dfce-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="3dfce-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3dfce-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="3dfce-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3dfce-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="3dfce-188">committedContentVersion</span></span>|<span data-ttu-id="3dfce-189">String</span><span class="sxs-lookup"><span data-stu-id="3dfce-189">String</span></span>|<span data-ttu-id="3dfce-190">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="3dfce-190">The internal committed content version.</span></span> <span data-ttu-id="3dfce-191">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3dfce-192">fileName</span><span class="sxs-lookup"><span data-stu-id="3dfce-192">fileName</span></span>|<span data-ttu-id="3dfce-193">String</span><span class="sxs-lookup"><span data-stu-id="3dfce-193">String</span></span>|<span data-ttu-id="3dfce-194">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="3dfce-194">The name of the main Lob application file.</span></span> <span data-ttu-id="3dfce-195">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3dfce-196">size</span><span class="sxs-lookup"><span data-stu-id="3dfce-196">size</span></span>|<span data-ttu-id="3dfce-197">Int64</span><span class="sxs-lookup"><span data-stu-id="3dfce-197">Int64</span></span>|<span data-ttu-id="3dfce-198">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="3dfce-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="3dfce-199">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3dfce-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3dfce-200">bundleId</span><span class="sxs-lookup"><span data-stu-id="3dfce-200">bundleId</span></span>|<span data-ttu-id="3dfce-201">String</span><span class="sxs-lookup"><span data-stu-id="3dfce-201">String</span></span>|<span data-ttu-id="3dfce-202">标识名称。</span><span class="sxs-lookup"><span data-stu-id="3dfce-202">The Identity Name.</span></span>|
|<span data-ttu-id="3dfce-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="3dfce-203">applicableDeviceType</span></span>|[<span data-ttu-id="3dfce-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="3dfce-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="3dfce-205">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="3dfce-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="3dfce-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3dfce-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3dfce-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3dfce-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="3dfce-208">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="3dfce-208">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="3dfce-209">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3dfce-209">expirationDateTime</span></span>|<span data-ttu-id="3dfce-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dfce-210">DateTimeOffset</span></span>|<span data-ttu-id="3dfce-211">过期时间。</span><span class="sxs-lookup"><span data-stu-id="3dfce-211">The expiration time.</span></span>|
|<span data-ttu-id="3dfce-212">versionNumber</span><span class="sxs-lookup"><span data-stu-id="3dfce-212">versionNumber</span></span>|<span data-ttu-id="3dfce-213">String</span><span class="sxs-lookup"><span data-stu-id="3dfce-213">String</span></span>|<span data-ttu-id="3dfce-214">iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="3dfce-214">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3dfce-215">buildNumber</span><span class="sxs-lookup"><span data-stu-id="3dfce-215">buildNumber</span></span>|<span data-ttu-id="3dfce-216">String</span><span class="sxs-lookup"><span data-stu-id="3dfce-216">String</span></span>|<span data-ttu-id="3dfce-217">iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="3dfce-217">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="3dfce-218">响应</span><span class="sxs-lookup"><span data-stu-id="3dfce-218">Response</span></span>
<span data-ttu-id="3dfce-219">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3dfce-219">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dfce-220">示例</span><span class="sxs-lookup"><span data-stu-id="3dfce-220">Example</span></span>
### <a name="request"></a><span data-ttu-id="3dfce-221">请求</span><span class="sxs-lookup"><span data-stu-id="3dfce-221">Request</span></span>
<span data-ttu-id="3dfce-222">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3dfce-222">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="3dfce-223">响应</span><span class="sxs-lookup"><span data-stu-id="3dfce-223">Response</span></span>
<span data-ttu-id="3dfce-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3dfce-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



