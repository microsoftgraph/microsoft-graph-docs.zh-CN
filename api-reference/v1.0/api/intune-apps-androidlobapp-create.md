---
title: 创建 androidLobApp
description: 创建新的 androidLobApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f20b79f14f9dfd92a9615a5f1d65e073f20d069
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974207"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="93326-103">创建 androidLobApp</span><span class="sxs-lookup"><span data-stu-id="93326-103">Create androidLobApp</span></span>

> <span data-ttu-id="93326-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="93326-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93326-105">创建新的 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="93326-105">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93326-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="93326-106">Prerequisites</span></span>
<span data-ttu-id="93326-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93326-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93326-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="93326-109">Permission type</span></span>|<span data-ttu-id="93326-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="93326-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93326-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93326-111">Delegated (work or school account)</span></span>|<span data-ttu-id="93326-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93326-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="93326-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93326-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93326-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="93326-114">Not supported.</span></span>|
|<span data-ttu-id="93326-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="93326-115">Application</span></span>|<span data-ttu-id="93326-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="93326-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93326-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93326-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="93326-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="93326-118">Request headers</span></span>
|<span data-ttu-id="93326-119">标头</span><span class="sxs-lookup"><span data-stu-id="93326-119">Header</span></span>|<span data-ttu-id="93326-120">值</span><span class="sxs-lookup"><span data-stu-id="93326-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93326-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="93326-121">Authorization</span></span>|<span data-ttu-id="93326-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="93326-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93326-123">接受</span><span class="sxs-lookup"><span data-stu-id="93326-123">Accept</span></span>|<span data-ttu-id="93326-124">application/json</span><span class="sxs-lookup"><span data-stu-id="93326-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93326-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="93326-125">Request body</span></span>
<span data-ttu-id="93326-126">在请求正文中，提供 androidLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93326-126">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="93326-127">下表显示了创建 androidLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="93326-127">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="93326-128">属性</span><span class="sxs-lookup"><span data-stu-id="93326-128">Property</span></span>|<span data-ttu-id="93326-129">类型</span><span class="sxs-lookup"><span data-stu-id="93326-129">Type</span></span>|<span data-ttu-id="93326-130">说明</span><span class="sxs-lookup"><span data-stu-id="93326-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93326-131">id</span><span class="sxs-lookup"><span data-stu-id="93326-131">id</span></span>|<span data-ttu-id="93326-132">String</span><span class="sxs-lookup"><span data-stu-id="93326-132">String</span></span>|<span data-ttu-id="93326-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="93326-133">Key of the entity.</span></span> <span data-ttu-id="93326-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93326-135">displayName</span><span class="sxs-lookup"><span data-stu-id="93326-135">displayName</span></span>|<span data-ttu-id="93326-136">String</span><span class="sxs-lookup"><span data-stu-id="93326-136">String</span></span>|<span data-ttu-id="93326-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="93326-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="93326-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93326-139">description</span><span class="sxs-lookup"><span data-stu-id="93326-139">description</span></span>|<span data-ttu-id="93326-140">String</span><span class="sxs-lookup"><span data-stu-id="93326-140">String</span></span>|<span data-ttu-id="93326-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="93326-141">The description of the app.</span></span> <span data-ttu-id="93326-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93326-143">publisher</span><span class="sxs-lookup"><span data-stu-id="93326-143">publisher</span></span>|<span data-ttu-id="93326-144">String</span><span class="sxs-lookup"><span data-stu-id="93326-144">String</span></span>|<span data-ttu-id="93326-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="93326-145">The publisher of the app.</span></span> <span data-ttu-id="93326-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93326-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="93326-147">largeIcon</span></span>|[<span data-ttu-id="93326-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="93326-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="93326-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="93326-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="93326-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93326-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93326-151">createdDateTime</span></span>|<span data-ttu-id="93326-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93326-152">DateTimeOffset</span></span>|<span data-ttu-id="93326-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="93326-153">The date and time the app was created.</span></span> <span data-ttu-id="93326-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93326-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93326-155">lastModifiedDateTime</span></span>|<span data-ttu-id="93326-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93326-156">DateTimeOffset</span></span>|<span data-ttu-id="93326-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="93326-157">The date and time the app was last modified.</span></span> <span data-ttu-id="93326-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93326-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="93326-159">isFeatured</span></span>|<span data-ttu-id="93326-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="93326-160">Boolean</span></span>|<span data-ttu-id="93326-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93326-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="93326-162">privacyInformationUrl</span></span>|<span data-ttu-id="93326-163">String</span><span class="sxs-lookup"><span data-stu-id="93326-163">String</span></span>|<span data-ttu-id="93326-164">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="93326-164">The privacy statement Url.</span></span> <span data-ttu-id="93326-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93326-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="93326-166">informationUrl</span></span>|<span data-ttu-id="93326-167">String</span><span class="sxs-lookup"><span data-stu-id="93326-167">String</span></span>|<span data-ttu-id="93326-168">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="93326-168">The more information Url.</span></span> <span data-ttu-id="93326-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93326-170">owner</span><span class="sxs-lookup"><span data-stu-id="93326-170">owner</span></span>|<span data-ttu-id="93326-171">字符串</span><span class="sxs-lookup"><span data-stu-id="93326-171">String</span></span>|<span data-ttu-id="93326-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="93326-172">The owner of the app.</span></span> <span data-ttu-id="93326-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93326-174">developer</span><span class="sxs-lookup"><span data-stu-id="93326-174">developer</span></span>|<span data-ttu-id="93326-175">String</span><span class="sxs-lookup"><span data-stu-id="93326-175">String</span></span>|<span data-ttu-id="93326-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="93326-176">The developer of the app.</span></span> <span data-ttu-id="93326-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93326-178">notes</span><span class="sxs-lookup"><span data-stu-id="93326-178">notes</span></span>|<span data-ttu-id="93326-179">String</span><span class="sxs-lookup"><span data-stu-id="93326-179">String</span></span>|<span data-ttu-id="93326-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="93326-180">Notes for the app.</span></span> <span data-ttu-id="93326-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="93326-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="93326-182">publishingState</span></span>|[<span data-ttu-id="93326-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="93326-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="93326-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="93326-184">The publishing state for the app.</span></span> <span data-ttu-id="93326-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="93326-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="93326-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="93326-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="93326-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="93326-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="93326-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="93326-188">committedContentVersion</span></span>|<span data-ttu-id="93326-189">String</span><span class="sxs-lookup"><span data-stu-id="93326-189">String</span></span>|<span data-ttu-id="93326-190">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="93326-190">The internal committed content version.</span></span> <span data-ttu-id="93326-191">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="93326-192">fileName</span><span class="sxs-lookup"><span data-stu-id="93326-192">fileName</span></span>|<span data-ttu-id="93326-193">String</span><span class="sxs-lookup"><span data-stu-id="93326-193">String</span></span>|<span data-ttu-id="93326-194">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="93326-194">The name of the main Lob application file.</span></span> <span data-ttu-id="93326-195">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="93326-196">size</span><span class="sxs-lookup"><span data-stu-id="93326-196">size</span></span>|<span data-ttu-id="93326-197">Int64</span><span class="sxs-lookup"><span data-stu-id="93326-197">Int64</span></span>|<span data-ttu-id="93326-198">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="93326-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="93326-199">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="93326-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="93326-200">packageId</span><span class="sxs-lookup"><span data-stu-id="93326-200">packageId</span></span>|<span data-ttu-id="93326-201">String</span><span class="sxs-lookup"><span data-stu-id="93326-201">String</span></span>|<span data-ttu-id="93326-202">包标识符。</span><span class="sxs-lookup"><span data-stu-id="93326-202">The package identifier.</span></span>|
|<span data-ttu-id="93326-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="93326-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="93326-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="93326-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="93326-205">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="93326-205">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="93326-206">versionName</span><span class="sxs-lookup"><span data-stu-id="93326-206">versionName</span></span>|<span data-ttu-id="93326-207">String</span><span class="sxs-lookup"><span data-stu-id="93326-207">String</span></span>|<span data-ttu-id="93326-208">Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="93326-208">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="93326-209">versionCode</span><span class="sxs-lookup"><span data-stu-id="93326-209">versionCode</span></span>|<span data-ttu-id="93326-210">String</span><span class="sxs-lookup"><span data-stu-id="93326-210">String</span></span>|<span data-ttu-id="93326-211">Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="93326-211">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="93326-212">响应</span><span class="sxs-lookup"><span data-stu-id="93326-212">Response</span></span>
<span data-ttu-id="93326-213">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="93326-213">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93326-214">示例</span><span class="sxs-lookup"><span data-stu-id="93326-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="93326-215">请求</span><span class="sxs-lookup"><span data-stu-id="93326-215">Request</span></span>
<span data-ttu-id="93326-216">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="93326-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1075

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="93326-217">响应</span><span class="sxs-lookup"><span data-stu-id="93326-217">Response</span></span>
<span data-ttu-id="93326-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="93326-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1247

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```



