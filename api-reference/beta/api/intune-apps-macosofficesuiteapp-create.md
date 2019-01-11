---
title: 创建 macOSOfficeSuiteApp
description: 创建新的 macOSOfficeSuiteApp 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f82ebbaa3b7a5936d45f36a56a929eb6472600a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824134"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="d9e2b-103">创建 macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="d9e2b-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="d9e2b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9e2b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9e2b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9e2b-107">创建新的 [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-107">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9e2b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d9e2b-108">Prerequisites</span></span>
<span data-ttu-id="d9e2b-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d9e2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9e2b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9e2b-111">Permission type</span></span>|<span data-ttu-id="d9e2b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d9e2b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9e2b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9e2b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9e2b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9e2b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d9e2b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9e2b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9e2b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-116">Not supported.</span></span>|
|<span data-ttu-id="d9e2b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9e2b-117">Application</span></span>|<span data-ttu-id="d9e2b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9e2b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9e2b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d9e2b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9e2b-120">Request headers</span></span>
|<span data-ttu-id="d9e2b-121">标头</span><span class="sxs-lookup"><span data-stu-id="d9e2b-121">Header</span></span>|<span data-ttu-id="d9e2b-122">值</span><span class="sxs-lookup"><span data-stu-id="d9e2b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9e2b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9e2b-123">Authorization</span></span>|<span data-ttu-id="d9e2b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9e2b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d9e2b-125">Accept</span></span>|<span data-ttu-id="d9e2b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d9e2b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9e2b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9e2b-127">Request body</span></span>
<span data-ttu-id="d9e2b-128">在请求正文中，提供 macOSOfficeSuiteApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-128">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="d9e2b-129">下表显示创建 macOSOfficeSuiteApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-129">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="d9e2b-130">属性</span><span class="sxs-lookup"><span data-stu-id="d9e2b-130">Property</span></span>|<span data-ttu-id="d9e2b-131">类型</span><span class="sxs-lookup"><span data-stu-id="d9e2b-131">Type</span></span>|<span data-ttu-id="d9e2b-132">说明</span><span class="sxs-lookup"><span data-stu-id="d9e2b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9e2b-133">id</span><span class="sxs-lookup"><span data-stu-id="d9e2b-133">id</span></span>|<span data-ttu-id="d9e2b-134">String</span><span class="sxs-lookup"><span data-stu-id="d9e2b-134">String</span></span>|<span data-ttu-id="d9e2b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-135">Key of the entity.</span></span> <span data-ttu-id="d9e2b-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e2b-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e2b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d9e2b-137">displayName</span></span>|<span data-ttu-id="d9e2b-138">String</span><span class="sxs-lookup"><span data-stu-id="d9e2b-138">String</span></span>|<span data-ttu-id="d9e2b-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d9e2b-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e2b-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e2b-141">description</span><span class="sxs-lookup"><span data-stu-id="d9e2b-141">description</span></span>|<span data-ttu-id="d9e2b-142">String</span><span class="sxs-lookup"><span data-stu-id="d9e2b-142">String</span></span>|<span data-ttu-id="d9e2b-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-143">The description of the app.</span></span> <span data-ttu-id="d9e2b-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e2b-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e2b-145">publisher</span><span class="sxs-lookup"><span data-stu-id="d9e2b-145">publisher</span></span>|<span data-ttu-id="d9e2b-146">String</span><span class="sxs-lookup"><span data-stu-id="d9e2b-146">String</span></span>|<span data-ttu-id="d9e2b-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-147">The publisher of the app.</span></span> <span data-ttu-id="d9e2b-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e2b-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e2b-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d9e2b-149">largeIcon</span></span>|[<span data-ttu-id="d9e2b-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d9e2b-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d9e2b-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d9e2b-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e2b-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e2b-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9e2b-153">createdDateTime</span></span>|<span data-ttu-id="d9e2b-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9e2b-154">DateTimeOffset</span></span>|<span data-ttu-id="d9e2b-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-155">The date and time the app was created.</span></span> <span data-ttu-id="d9e2b-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e2b-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e2b-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d9e2b-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d9e2b-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9e2b-158">DateTimeOffset</span></span>|<span data-ttu-id="d9e2b-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d9e2b-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e2b-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e2b-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d9e2b-161">isFeatured</span></span>|<span data-ttu-id="d9e2b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9e2b-162">Boolean</span></span>|<span data-ttu-id="d9e2b-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e2b-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e2b-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d9e2b-164">privacyInformationUrl</span></span>|<span data-ttu-id="d9e2b-165">String</span><span class="sxs-lookup"><span data-stu-id="d9e2b-165">String</span></span>|<span data-ttu-id="d9e2b-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-166">The privacy statement Url.</span></span> <span data-ttu-id="d9e2b-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e2b-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e2b-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d9e2b-168">informationUrl</span></span>|<span data-ttu-id="d9e2b-169">String</span><span class="sxs-lookup"><span data-stu-id="d9e2b-169">String</span></span>|<span data-ttu-id="d9e2b-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-170">The more information Url.</span></span> <span data-ttu-id="d9e2b-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e2b-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e2b-172">owner</span><span class="sxs-lookup"><span data-stu-id="d9e2b-172">owner</span></span>|<span data-ttu-id="d9e2b-173">String</span><span class="sxs-lookup"><span data-stu-id="d9e2b-173">String</span></span>|<span data-ttu-id="d9e2b-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-174">The owner of the app.</span></span> <span data-ttu-id="d9e2b-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e2b-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e2b-176">developer</span><span class="sxs-lookup"><span data-stu-id="d9e2b-176">developer</span></span>|<span data-ttu-id="d9e2b-177">String</span><span class="sxs-lookup"><span data-stu-id="d9e2b-177">String</span></span>|<span data-ttu-id="d9e2b-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-178">The developer of the app.</span></span> <span data-ttu-id="d9e2b-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e2b-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e2b-180">notes</span><span class="sxs-lookup"><span data-stu-id="d9e2b-180">notes</span></span>|<span data-ttu-id="d9e2b-181">String</span><span class="sxs-lookup"><span data-stu-id="d9e2b-181">String</span></span>|<span data-ttu-id="d9e2b-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-182">Notes for the app.</span></span> <span data-ttu-id="d9e2b-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e2b-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e2b-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d9e2b-184">uploadState</span></span>|<span data-ttu-id="d9e2b-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d9e2b-185">Int32</span></span>|<span data-ttu-id="d9e2b-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-186">The upload state.</span></span> <span data-ttu-id="d9e2b-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d9e2b-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d9e2b-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="d9e2b-188">publishingState</span></span>|[<span data-ttu-id="d9e2b-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d9e2b-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d9e2b-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-190">The publishing state for the app.</span></span> <span data-ttu-id="d9e2b-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d9e2b-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d9e2b-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="d9e2b-194">响应</span><span class="sxs-lookup"><span data-stu-id="d9e2b-194">Response</span></span>
<span data-ttu-id="d9e2b-195">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-195">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9e2b-196">示例</span><span class="sxs-lookup"><span data-stu-id="d9e2b-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="d9e2b-197">请求</span><span class="sxs-lookup"><span data-stu-id="d9e2b-197">Request</span></span>
<span data-ttu-id="d9e2b-198">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 670

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="d9e2b-199">响应</span><span class="sxs-lookup"><span data-stu-id="d9e2b-199">Response</span></span>
<span data-ttu-id="d9e2b-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9e2b-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 778

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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
  "publishingState": "processing"
}
```





