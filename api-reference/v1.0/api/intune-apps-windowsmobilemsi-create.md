---
title: 创建 windowsMobileMSI
description: 创建新的 windowsMobileMSI 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9fa4fd686c870a2f649c8a8af5b3f7fb909ece90
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952914"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="c9124-103">创建 windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="c9124-103">Create windowsMobileMSI</span></span>

> <span data-ttu-id="c9124-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c9124-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9124-105">创建新的 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c9124-105">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9124-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="c9124-106">Prerequisites</span></span>
<span data-ttu-id="c9124-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c9124-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9124-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9124-109">Permission type</span></span>|<span data-ttu-id="c9124-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c9124-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9124-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9124-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c9124-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9124-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c9124-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9124-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9124-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9124-114">Not supported.</span></span>|
|<span data-ttu-id="c9124-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9124-115">Application</span></span>|<span data-ttu-id="c9124-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9124-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9124-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9124-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c9124-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9124-118">Request headers</span></span>
|<span data-ttu-id="c9124-119">标头</span><span class="sxs-lookup"><span data-stu-id="c9124-119">Header</span></span>|<span data-ttu-id="c9124-120">值</span><span class="sxs-lookup"><span data-stu-id="c9124-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9124-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9124-121">Authorization</span></span>|<span data-ttu-id="c9124-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c9124-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9124-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c9124-123">Accept</span></span>|<span data-ttu-id="c9124-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c9124-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9124-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9124-125">Request body</span></span>
<span data-ttu-id="c9124-126">在请求正文中，提供 windowsMobileMSI 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9124-126">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="c9124-127">下表显示创建 windowsMobileMSI 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c9124-127">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="c9124-128">属性</span><span class="sxs-lookup"><span data-stu-id="c9124-128">Property</span></span>|<span data-ttu-id="c9124-129">类型</span><span class="sxs-lookup"><span data-stu-id="c9124-129">Type</span></span>|<span data-ttu-id="c9124-130">说明</span><span class="sxs-lookup"><span data-stu-id="c9124-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9124-131">id</span><span class="sxs-lookup"><span data-stu-id="c9124-131">id</span></span>|<span data-ttu-id="c9124-132">String</span><span class="sxs-lookup"><span data-stu-id="c9124-132">String</span></span>|<span data-ttu-id="c9124-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c9124-133">Key of the entity.</span></span> <span data-ttu-id="c9124-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9124-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c9124-135">displayName</span></span>|<span data-ttu-id="c9124-136">String</span><span class="sxs-lookup"><span data-stu-id="c9124-136">String</span></span>|<span data-ttu-id="c9124-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="c9124-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c9124-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9124-139">description</span><span class="sxs-lookup"><span data-stu-id="c9124-139">description</span></span>|<span data-ttu-id="c9124-140">String</span><span class="sxs-lookup"><span data-stu-id="c9124-140">String</span></span>|<span data-ttu-id="c9124-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="c9124-141">The description of the app.</span></span> <span data-ttu-id="c9124-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9124-143">publisher</span><span class="sxs-lookup"><span data-stu-id="c9124-143">publisher</span></span>|<span data-ttu-id="c9124-144">String</span><span class="sxs-lookup"><span data-stu-id="c9124-144">String</span></span>|<span data-ttu-id="c9124-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="c9124-145">The publisher of the app.</span></span> <span data-ttu-id="c9124-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9124-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c9124-147">largeIcon</span></span>|[<span data-ttu-id="c9124-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c9124-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c9124-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="c9124-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c9124-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9124-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9124-151">createdDateTime</span></span>|<span data-ttu-id="c9124-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9124-152">DateTimeOffset</span></span>|<span data-ttu-id="c9124-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c9124-153">The date and time the app was created.</span></span> <span data-ttu-id="c9124-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9124-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9124-155">lastModifiedDateTime</span></span>|<span data-ttu-id="c9124-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9124-156">DateTimeOffset</span></span>|<span data-ttu-id="c9124-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c9124-157">The date and time the app was last modified.</span></span> <span data-ttu-id="c9124-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9124-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c9124-159">isFeatured</span></span>|<span data-ttu-id="c9124-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9124-160">Boolean</span></span>|<span data-ttu-id="c9124-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9124-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c9124-162">privacyInformationUrl</span></span>|<span data-ttu-id="c9124-163">String</span><span class="sxs-lookup"><span data-stu-id="c9124-163">String</span></span>|<span data-ttu-id="c9124-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="c9124-164">The privacy statement Url.</span></span> <span data-ttu-id="c9124-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9124-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c9124-166">informationUrl</span></span>|<span data-ttu-id="c9124-167">String</span><span class="sxs-lookup"><span data-stu-id="c9124-167">String</span></span>|<span data-ttu-id="c9124-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="c9124-168">The more information Url.</span></span> <span data-ttu-id="c9124-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9124-170">owner</span><span class="sxs-lookup"><span data-stu-id="c9124-170">owner</span></span>|<span data-ttu-id="c9124-171">String</span><span class="sxs-lookup"><span data-stu-id="c9124-171">String</span></span>|<span data-ttu-id="c9124-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="c9124-172">The owner of the app.</span></span> <span data-ttu-id="c9124-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9124-174">developer</span><span class="sxs-lookup"><span data-stu-id="c9124-174">developer</span></span>|<span data-ttu-id="c9124-175">String</span><span class="sxs-lookup"><span data-stu-id="c9124-175">String</span></span>|<span data-ttu-id="c9124-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="c9124-176">The developer of the app.</span></span> <span data-ttu-id="c9124-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9124-178">notes</span><span class="sxs-lookup"><span data-stu-id="c9124-178">notes</span></span>|<span data-ttu-id="c9124-179">String</span><span class="sxs-lookup"><span data-stu-id="c9124-179">String</span></span>|<span data-ttu-id="c9124-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="c9124-180">Notes for the app.</span></span> <span data-ttu-id="c9124-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c9124-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="c9124-182">publishingState</span></span>|[<span data-ttu-id="c9124-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c9124-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c9124-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="c9124-184">The publishing state for the app.</span></span> <span data-ttu-id="c9124-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="c9124-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c9124-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="c9124-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c9124-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="c9124-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c9124-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="c9124-188">committedContentVersion</span></span>|<span data-ttu-id="c9124-189">String</span><span class="sxs-lookup"><span data-stu-id="c9124-189">String</span></span>|<span data-ttu-id="c9124-190">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="c9124-190">The internal committed content version.</span></span> <span data-ttu-id="c9124-191">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c9124-192">fileName</span><span class="sxs-lookup"><span data-stu-id="c9124-192">fileName</span></span>|<span data-ttu-id="c9124-193">String</span><span class="sxs-lookup"><span data-stu-id="c9124-193">String</span></span>|<span data-ttu-id="c9124-194">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="c9124-194">The name of the main Lob application file.</span></span> <span data-ttu-id="c9124-195">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c9124-196">size</span><span class="sxs-lookup"><span data-stu-id="c9124-196">size</span></span>|<span data-ttu-id="c9124-197">Int64</span><span class="sxs-lookup"><span data-stu-id="c9124-197">Int64</span></span>|<span data-ttu-id="c9124-198">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="c9124-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="c9124-199">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c9124-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c9124-200">commandLine</span><span class="sxs-lookup"><span data-stu-id="c9124-200">commandLine</span></span>|<span data-ttu-id="c9124-201">String</span><span class="sxs-lookup"><span data-stu-id="c9124-201">String</span></span>|<span data-ttu-id="c9124-202">命令行。</span><span class="sxs-lookup"><span data-stu-id="c9124-202">The command line.</span></span>|
|<span data-ttu-id="c9124-203">productCode</span><span class="sxs-lookup"><span data-stu-id="c9124-203">productCode</span></span>|<span data-ttu-id="c9124-204">String</span><span class="sxs-lookup"><span data-stu-id="c9124-204">String</span></span>|<span data-ttu-id="c9124-205">产品代码。</span><span class="sxs-lookup"><span data-stu-id="c9124-205">The product code.</span></span>|
|<span data-ttu-id="c9124-206">productVersion</span><span class="sxs-lookup"><span data-stu-id="c9124-206">productVersion</span></span>|<span data-ttu-id="c9124-207">String</span><span class="sxs-lookup"><span data-stu-id="c9124-207">String</span></span>|<span data-ttu-id="c9124-208">Windows Mobile MSI 业务线 (LoB) 应用的产品版本。</span><span class="sxs-lookup"><span data-stu-id="c9124-208">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c9124-209">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="c9124-209">ignoreVersionDetection</span></span>|<span data-ttu-id="c9124-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9124-210">Boolean</span></span>|<span data-ttu-id="c9124-211">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="c9124-211">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="c9124-212">对于使用自更新功能的 Windows Mobile MSI 业务线 (LoB) 应用，将此值设置为 true。</span><span class="sxs-lookup"><span data-stu-id="c9124-212">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="c9124-213">响应</span><span class="sxs-lookup"><span data-stu-id="c9124-213">Response</span></span>
<span data-ttu-id="c9124-214">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c9124-214">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9124-215">示例</span><span class="sxs-lookup"><span data-stu-id="c9124-215">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9124-216">请求</span><span class="sxs-lookup"><span data-stu-id="c9124-216">Request</span></span>
<span data-ttu-id="c9124-217">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c9124-217">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c9124-218">响应</span><span class="sxs-lookup"><span data-stu-id="c9124-218">Response</span></span>
<span data-ttu-id="c9124-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c9124-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



