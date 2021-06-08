---
title: 创建 windowsMobileMSI
description: 创建新的 windowsMobileMSI 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 083692d7d7b35d2e29e2525eb9bee87c45b262bd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759663"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="0fb89-103">创建 windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="0fb89-103">Create windowsMobileMSI</span></span>

<span data-ttu-id="0fb89-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fb89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fb89-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0fb89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fb89-106">创建新的 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0fb89-106">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fb89-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0fb89-107">Prerequisites</span></span>
<span data-ttu-id="0fb89-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0fb89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fb89-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0fb89-110">Permission type</span></span>|<span data-ttu-id="0fb89-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0fb89-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fb89-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0fb89-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0fb89-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fb89-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0fb89-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0fb89-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fb89-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0fb89-115">Not supported.</span></span>|
|<span data-ttu-id="0fb89-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0fb89-116">Application</span></span>|<span data-ttu-id="0fb89-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fb89-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fb89-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0fb89-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0fb89-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0fb89-119">Request headers</span></span>
|<span data-ttu-id="0fb89-120">标头</span><span class="sxs-lookup"><span data-stu-id="0fb89-120">Header</span></span>|<span data-ttu-id="0fb89-121">值</span><span class="sxs-lookup"><span data-stu-id="0fb89-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fb89-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fb89-122">Authorization</span></span>|<span data-ttu-id="0fb89-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0fb89-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fb89-124">接受</span><span class="sxs-lookup"><span data-stu-id="0fb89-124">Accept</span></span>|<span data-ttu-id="0fb89-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0fb89-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fb89-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0fb89-126">Request body</span></span>
<span data-ttu-id="0fb89-127">在请求正文中，提供 windowsMobileMSI 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fb89-127">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="0fb89-128">下表显示创建 windowsMobileMSI 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0fb89-128">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="0fb89-129">属性</span><span class="sxs-lookup"><span data-stu-id="0fb89-129">Property</span></span>|<span data-ttu-id="0fb89-130">类型</span><span class="sxs-lookup"><span data-stu-id="0fb89-130">Type</span></span>|<span data-ttu-id="0fb89-131">说明</span><span class="sxs-lookup"><span data-stu-id="0fb89-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fb89-132">id</span><span class="sxs-lookup"><span data-stu-id="0fb89-132">id</span></span>|<span data-ttu-id="0fb89-133">String</span><span class="sxs-lookup"><span data-stu-id="0fb89-133">String</span></span>|<span data-ttu-id="0fb89-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0fb89-134">Key of the entity.</span></span> <span data-ttu-id="0fb89-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0fb89-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0fb89-136">displayName</span></span>|<span data-ttu-id="0fb89-137">String</span><span class="sxs-lookup"><span data-stu-id="0fb89-137">String</span></span>|<span data-ttu-id="0fb89-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="0fb89-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0fb89-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0fb89-140">description</span><span class="sxs-lookup"><span data-stu-id="0fb89-140">description</span></span>|<span data-ttu-id="0fb89-141">String</span><span class="sxs-lookup"><span data-stu-id="0fb89-141">String</span></span>|<span data-ttu-id="0fb89-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="0fb89-142">The description of the app.</span></span> <span data-ttu-id="0fb89-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0fb89-144">publisher</span><span class="sxs-lookup"><span data-stu-id="0fb89-144">publisher</span></span>|<span data-ttu-id="0fb89-145">String</span><span class="sxs-lookup"><span data-stu-id="0fb89-145">String</span></span>|<span data-ttu-id="0fb89-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="0fb89-146">The publisher of the app.</span></span> <span data-ttu-id="0fb89-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0fb89-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0fb89-148">largeIcon</span></span>|[<span data-ttu-id="0fb89-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0fb89-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0fb89-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="0fb89-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0fb89-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0fb89-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fb89-152">createdDateTime</span></span>|<span data-ttu-id="0fb89-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fb89-153">DateTimeOffset</span></span>|<span data-ttu-id="0fb89-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0fb89-154">The date and time the app was created.</span></span> <span data-ttu-id="0fb89-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0fb89-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0fb89-156">lastModifiedDateTime</span></span>|<span data-ttu-id="0fb89-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fb89-157">DateTimeOffset</span></span>|<span data-ttu-id="0fb89-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0fb89-158">The date and time the app was last modified.</span></span> <span data-ttu-id="0fb89-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0fb89-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0fb89-160">isFeatured</span></span>|<span data-ttu-id="0fb89-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fb89-161">Boolean</span></span>|<span data-ttu-id="0fb89-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0fb89-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0fb89-163">privacyInformationUrl</span></span>|<span data-ttu-id="0fb89-164">String</span><span class="sxs-lookup"><span data-stu-id="0fb89-164">String</span></span>|<span data-ttu-id="0fb89-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="0fb89-165">The privacy statement Url.</span></span> <span data-ttu-id="0fb89-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0fb89-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0fb89-167">informationUrl</span></span>|<span data-ttu-id="0fb89-168">String</span><span class="sxs-lookup"><span data-stu-id="0fb89-168">String</span></span>|<span data-ttu-id="0fb89-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="0fb89-169">The more information Url.</span></span> <span data-ttu-id="0fb89-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0fb89-171">所有者</span><span class="sxs-lookup"><span data-stu-id="0fb89-171">owner</span></span>|<span data-ttu-id="0fb89-172">String</span><span class="sxs-lookup"><span data-stu-id="0fb89-172">String</span></span>|<span data-ttu-id="0fb89-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="0fb89-173">The owner of the app.</span></span> <span data-ttu-id="0fb89-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0fb89-175">developer</span><span class="sxs-lookup"><span data-stu-id="0fb89-175">developer</span></span>|<span data-ttu-id="0fb89-176">String</span><span class="sxs-lookup"><span data-stu-id="0fb89-176">String</span></span>|<span data-ttu-id="0fb89-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="0fb89-177">The developer of the app.</span></span> <span data-ttu-id="0fb89-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0fb89-179">notes</span><span class="sxs-lookup"><span data-stu-id="0fb89-179">notes</span></span>|<span data-ttu-id="0fb89-180">String</span><span class="sxs-lookup"><span data-stu-id="0fb89-180">String</span></span>|<span data-ttu-id="0fb89-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="0fb89-181">Notes for the app.</span></span> <span data-ttu-id="0fb89-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0fb89-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="0fb89-183">publishingState</span></span>|[<span data-ttu-id="0fb89-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0fb89-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0fb89-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="0fb89-185">The publishing state for the app.</span></span> <span data-ttu-id="0fb89-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="0fb89-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0fb89-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="0fb89-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0fb89-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="0fb89-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0fb89-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="0fb89-189">committedContentVersion</span></span>|<span data-ttu-id="0fb89-190">String</span><span class="sxs-lookup"><span data-stu-id="0fb89-190">String</span></span>|<span data-ttu-id="0fb89-191">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="0fb89-191">The internal committed content version.</span></span> <span data-ttu-id="0fb89-192">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0fb89-193">fileName</span><span class="sxs-lookup"><span data-stu-id="0fb89-193">fileName</span></span>|<span data-ttu-id="0fb89-194">String</span><span class="sxs-lookup"><span data-stu-id="0fb89-194">String</span></span>|<span data-ttu-id="0fb89-195">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="0fb89-195">The name of the main Lob application file.</span></span> <span data-ttu-id="0fb89-196">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0fb89-197">size</span><span class="sxs-lookup"><span data-stu-id="0fb89-197">size</span></span>|<span data-ttu-id="0fb89-198">Int64</span><span class="sxs-lookup"><span data-stu-id="0fb89-198">Int64</span></span>|<span data-ttu-id="0fb89-199">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="0fb89-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="0fb89-200">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="0fb89-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0fb89-201">commandLine</span><span class="sxs-lookup"><span data-stu-id="0fb89-201">commandLine</span></span>|<span data-ttu-id="0fb89-202">String</span><span class="sxs-lookup"><span data-stu-id="0fb89-202">String</span></span>|<span data-ttu-id="0fb89-203">命令行。</span><span class="sxs-lookup"><span data-stu-id="0fb89-203">The command line.</span></span>|
|<span data-ttu-id="0fb89-204">productCode</span><span class="sxs-lookup"><span data-stu-id="0fb89-204">productCode</span></span>|<span data-ttu-id="0fb89-205">String</span><span class="sxs-lookup"><span data-stu-id="0fb89-205">String</span></span>|<span data-ttu-id="0fb89-206">产品代码。</span><span class="sxs-lookup"><span data-stu-id="0fb89-206">The product code.</span></span>|
|<span data-ttu-id="0fb89-207">productVersion</span><span class="sxs-lookup"><span data-stu-id="0fb89-207">productVersion</span></span>|<span data-ttu-id="0fb89-208">String</span><span class="sxs-lookup"><span data-stu-id="0fb89-208">String</span></span>|<span data-ttu-id="0fb89-209">Windows Mobile MSI 业务线 (LoB) 应用的产品版本。</span><span class="sxs-lookup"><span data-stu-id="0fb89-209">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="0fb89-210">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="0fb89-210">ignoreVersionDetection</span></span>|<span data-ttu-id="0fb89-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fb89-211">Boolean</span></span>|<span data-ttu-id="0fb89-212">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="0fb89-212">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="0fb89-213">对于使用自更新功能的 Windows Mobile MSI 业务线 (LoB) 应用，将此值设置为 true。</span><span class="sxs-lookup"><span data-stu-id="0fb89-213">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="0fb89-214">响应</span><span class="sxs-lookup"><span data-stu-id="0fb89-214">Response</span></span>
<span data-ttu-id="0fb89-215">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0fb89-215">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fb89-216">示例</span><span class="sxs-lookup"><span data-stu-id="0fb89-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fb89-217">请求</span><span class="sxs-lookup"><span data-stu-id="0fb89-217">Request</span></span>
<span data-ttu-id="0fb89-218">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0fb89-218">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 855

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="0fb89-219">响应</span><span class="sxs-lookup"><span data-stu-id="0fb89-219">Response</span></span>
<span data-ttu-id="0fb89-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0fb89-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1027

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```




