---
title: 创建 androidLobApp
description: 创建新的 androidLobApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b701d1b501f89a177801c7de3219b8efbe297d63
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757729"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="ce8bd-103">创建 androidLobApp</span><span class="sxs-lookup"><span data-stu-id="ce8bd-103">Create androidLobApp</span></span>

<span data-ttu-id="ce8bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce8bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce8bd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce8bd-106">创建新的 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-106">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce8bd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ce8bd-107">Prerequisites</span></span>
<span data-ttu-id="ce8bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce8bd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce8bd-110">Permission type</span></span>|<span data-ttu-id="ce8bd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce8bd-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce8bd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce8bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce8bd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce8bd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ce8bd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce8bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce8bd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-115">Not supported.</span></span>|
|<span data-ttu-id="ce8bd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce8bd-116">Application</span></span>|<span data-ttu-id="ce8bd-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce8bd-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce8bd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce8bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ce8bd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce8bd-119">Request headers</span></span>
|<span data-ttu-id="ce8bd-120">标头</span><span class="sxs-lookup"><span data-stu-id="ce8bd-120">Header</span></span>|<span data-ttu-id="ce8bd-121">值</span><span class="sxs-lookup"><span data-stu-id="ce8bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce8bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce8bd-122">Authorization</span></span>|<span data-ttu-id="ce8bd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce8bd-124">接受</span><span class="sxs-lookup"><span data-stu-id="ce8bd-124">Accept</span></span>|<span data-ttu-id="ce8bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ce8bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce8bd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce8bd-126">Request body</span></span>
<span data-ttu-id="ce8bd-127">在请求正文中，提供 androidLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-127">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="ce8bd-128">下表显示了创建 androidLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-128">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="ce8bd-129">属性</span><span class="sxs-lookup"><span data-stu-id="ce8bd-129">Property</span></span>|<span data-ttu-id="ce8bd-130">类型</span><span class="sxs-lookup"><span data-stu-id="ce8bd-130">Type</span></span>|<span data-ttu-id="ce8bd-131">说明</span><span class="sxs-lookup"><span data-stu-id="ce8bd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce8bd-132">id</span><span class="sxs-lookup"><span data-stu-id="ce8bd-132">id</span></span>|<span data-ttu-id="ce8bd-133">String</span><span class="sxs-lookup"><span data-stu-id="ce8bd-133">String</span></span>|<span data-ttu-id="ce8bd-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-134">Key of the entity.</span></span> <span data-ttu-id="ce8bd-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce8bd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ce8bd-136">displayName</span></span>|<span data-ttu-id="ce8bd-137">String</span><span class="sxs-lookup"><span data-stu-id="ce8bd-137">String</span></span>|<span data-ttu-id="ce8bd-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ce8bd-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce8bd-140">说明</span><span class="sxs-lookup"><span data-stu-id="ce8bd-140">description</span></span>|<span data-ttu-id="ce8bd-141">String</span><span class="sxs-lookup"><span data-stu-id="ce8bd-141">String</span></span>|<span data-ttu-id="ce8bd-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-142">The description of the app.</span></span> <span data-ttu-id="ce8bd-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce8bd-144">publisher</span><span class="sxs-lookup"><span data-stu-id="ce8bd-144">publisher</span></span>|<span data-ttu-id="ce8bd-145">String</span><span class="sxs-lookup"><span data-stu-id="ce8bd-145">String</span></span>|<span data-ttu-id="ce8bd-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-146">The publisher of the app.</span></span> <span data-ttu-id="ce8bd-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce8bd-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ce8bd-148">largeIcon</span></span>|[<span data-ttu-id="ce8bd-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ce8bd-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ce8bd-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ce8bd-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce8bd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce8bd-152">createdDateTime</span></span>|<span data-ttu-id="ce8bd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce8bd-153">DateTimeOffset</span></span>|<span data-ttu-id="ce8bd-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-154">The date and time the app was created.</span></span> <span data-ttu-id="ce8bd-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce8bd-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce8bd-156">lastModifiedDateTime</span></span>|<span data-ttu-id="ce8bd-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce8bd-157">DateTimeOffset</span></span>|<span data-ttu-id="ce8bd-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-158">The date and time the app was last modified.</span></span> <span data-ttu-id="ce8bd-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce8bd-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ce8bd-160">isFeatured</span></span>|<span data-ttu-id="ce8bd-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce8bd-161">Boolean</span></span>|<span data-ttu-id="ce8bd-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce8bd-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ce8bd-163">privacyInformationUrl</span></span>|<span data-ttu-id="ce8bd-164">String</span><span class="sxs-lookup"><span data-stu-id="ce8bd-164">String</span></span>|<span data-ttu-id="ce8bd-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-165">The privacy statement Url.</span></span> <span data-ttu-id="ce8bd-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce8bd-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ce8bd-167">informationUrl</span></span>|<span data-ttu-id="ce8bd-168">String</span><span class="sxs-lookup"><span data-stu-id="ce8bd-168">String</span></span>|<span data-ttu-id="ce8bd-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-169">The more information Url.</span></span> <span data-ttu-id="ce8bd-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce8bd-171">所有者</span><span class="sxs-lookup"><span data-stu-id="ce8bd-171">owner</span></span>|<span data-ttu-id="ce8bd-172">String</span><span class="sxs-lookup"><span data-stu-id="ce8bd-172">String</span></span>|<span data-ttu-id="ce8bd-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-173">The owner of the app.</span></span> <span data-ttu-id="ce8bd-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce8bd-175">developer</span><span class="sxs-lookup"><span data-stu-id="ce8bd-175">developer</span></span>|<span data-ttu-id="ce8bd-176">String</span><span class="sxs-lookup"><span data-stu-id="ce8bd-176">String</span></span>|<span data-ttu-id="ce8bd-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-177">The developer of the app.</span></span> <span data-ttu-id="ce8bd-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce8bd-179">notes</span><span class="sxs-lookup"><span data-stu-id="ce8bd-179">notes</span></span>|<span data-ttu-id="ce8bd-180">String</span><span class="sxs-lookup"><span data-stu-id="ce8bd-180">String</span></span>|<span data-ttu-id="ce8bd-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-181">Notes for the app.</span></span> <span data-ttu-id="ce8bd-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce8bd-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="ce8bd-183">publishingState</span></span>|[<span data-ttu-id="ce8bd-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ce8bd-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ce8bd-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-185">The publishing state for the app.</span></span> <span data-ttu-id="ce8bd-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ce8bd-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ce8bd-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ce8bd-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ce8bd-189">committedContentVersion</span></span>|<span data-ttu-id="ce8bd-190">String</span><span class="sxs-lookup"><span data-stu-id="ce8bd-190">String</span></span>|<span data-ttu-id="ce8bd-191">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-191">The internal committed content version.</span></span> <span data-ttu-id="ce8bd-192">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ce8bd-193">fileName</span><span class="sxs-lookup"><span data-stu-id="ce8bd-193">fileName</span></span>|<span data-ttu-id="ce8bd-194">String</span><span class="sxs-lookup"><span data-stu-id="ce8bd-194">String</span></span>|<span data-ttu-id="ce8bd-195">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-195">The name of the main Lob application file.</span></span> <span data-ttu-id="ce8bd-196">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ce8bd-197">size</span><span class="sxs-lookup"><span data-stu-id="ce8bd-197">size</span></span>|<span data-ttu-id="ce8bd-198">Int64</span><span class="sxs-lookup"><span data-stu-id="ce8bd-198">Int64</span></span>|<span data-ttu-id="ce8bd-199">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="ce8bd-200">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ce8bd-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ce8bd-201">packageId</span><span class="sxs-lookup"><span data-stu-id="ce8bd-201">packageId</span></span>|<span data-ttu-id="ce8bd-202">String</span><span class="sxs-lookup"><span data-stu-id="ce8bd-202">String</span></span>|<span data-ttu-id="ce8bd-203">包标识符。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-203">The package identifier.</span></span>|
|<span data-ttu-id="ce8bd-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ce8bd-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ce8bd-205">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ce8bd-205">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="ce8bd-206">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-206">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ce8bd-207">versionName</span><span class="sxs-lookup"><span data-stu-id="ce8bd-207">versionName</span></span>|<span data-ttu-id="ce8bd-208">String</span><span class="sxs-lookup"><span data-stu-id="ce8bd-208">String</span></span>|<span data-ttu-id="ce8bd-209">Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-209">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ce8bd-210">versionCode</span><span class="sxs-lookup"><span data-stu-id="ce8bd-210">versionCode</span></span>|<span data-ttu-id="ce8bd-211">String</span><span class="sxs-lookup"><span data-stu-id="ce8bd-211">String</span></span>|<span data-ttu-id="ce8bd-212">Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-212">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="ce8bd-213">响应</span><span class="sxs-lookup"><span data-stu-id="ce8bd-213">Response</span></span>
<span data-ttu-id="ce8bd-214">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-214">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce8bd-215">示例</span><span class="sxs-lookup"><span data-stu-id="ce8bd-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce8bd-216">请求</span><span class="sxs-lookup"><span data-stu-id="ce8bd-216">Request</span></span>
<span data-ttu-id="ce8bd-217">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1115

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
    "v5_1": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="ce8bd-218">响应</span><span class="sxs-lookup"><span data-stu-id="ce8bd-218">Response</span></span>
<span data-ttu-id="ce8bd-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ce8bd-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1287

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
    "v5_1": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```




