---
title: 创建 macOSOfficeSuiteApp
description: 创建新的 macOSOfficeSuiteApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a97794b613a944021a5bc5bf4531a9cc758a58e0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456109"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="85cf0-103">创建 macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="85cf0-103">Create macOSOfficeSuiteApp</span></span>

<span data-ttu-id="85cf0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85cf0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85cf0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85cf0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85cf0-106">创建新的 [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="85cf0-106">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85cf0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="85cf0-107">Prerequisites</span></span>
<span data-ttu-id="85cf0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85cf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85cf0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="85cf0-110">Permission type</span></span>|<span data-ttu-id="85cf0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="85cf0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85cf0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85cf0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85cf0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85cf0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="85cf0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85cf0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85cf0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="85cf0-115">Not supported.</span></span>|
|<span data-ttu-id="85cf0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="85cf0-116">Application</span></span>|<span data-ttu-id="85cf0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="85cf0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="85cf0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85cf0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="85cf0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="85cf0-119">Request headers</span></span>
|<span data-ttu-id="85cf0-120">标头</span><span class="sxs-lookup"><span data-stu-id="85cf0-120">Header</span></span>|<span data-ttu-id="85cf0-121">值</span><span class="sxs-lookup"><span data-stu-id="85cf0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85cf0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="85cf0-122">Authorization</span></span>|<span data-ttu-id="85cf0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="85cf0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85cf0-124">接受</span><span class="sxs-lookup"><span data-stu-id="85cf0-124">Accept</span></span>|<span data-ttu-id="85cf0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85cf0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85cf0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="85cf0-126">Request body</span></span>
<span data-ttu-id="85cf0-127">在请求正文中，提供 macOSOfficeSuiteApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85cf0-127">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="85cf0-128">下表显示创建 macOSOfficeSuiteApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="85cf0-128">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="85cf0-129">属性</span><span class="sxs-lookup"><span data-stu-id="85cf0-129">Property</span></span>|<span data-ttu-id="85cf0-130">类型</span><span class="sxs-lookup"><span data-stu-id="85cf0-130">Type</span></span>|<span data-ttu-id="85cf0-131">说明</span><span class="sxs-lookup"><span data-stu-id="85cf0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85cf0-132">id</span><span class="sxs-lookup"><span data-stu-id="85cf0-132">id</span></span>|<span data-ttu-id="85cf0-133">字符串</span><span class="sxs-lookup"><span data-stu-id="85cf0-133">String</span></span>|<span data-ttu-id="85cf0-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="85cf0-134">Key of the entity.</span></span> <span data-ttu-id="85cf0-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85cf0-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85cf0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="85cf0-136">displayName</span></span>|<span data-ttu-id="85cf0-137">String</span><span class="sxs-lookup"><span data-stu-id="85cf0-137">String</span></span>|<span data-ttu-id="85cf0-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="85cf0-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="85cf0-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85cf0-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85cf0-140">description</span><span class="sxs-lookup"><span data-stu-id="85cf0-140">description</span></span>|<span data-ttu-id="85cf0-141">字符串</span><span class="sxs-lookup"><span data-stu-id="85cf0-141">String</span></span>|<span data-ttu-id="85cf0-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="85cf0-142">The description of the app.</span></span> <span data-ttu-id="85cf0-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85cf0-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85cf0-144">publisher</span><span class="sxs-lookup"><span data-stu-id="85cf0-144">publisher</span></span>|<span data-ttu-id="85cf0-145">String</span><span class="sxs-lookup"><span data-stu-id="85cf0-145">String</span></span>|<span data-ttu-id="85cf0-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="85cf0-146">The publisher of the app.</span></span> <span data-ttu-id="85cf0-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85cf0-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85cf0-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="85cf0-148">largeIcon</span></span>|[<span data-ttu-id="85cf0-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="85cf0-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="85cf0-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="85cf0-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="85cf0-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85cf0-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85cf0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85cf0-152">createdDateTime</span></span>|<span data-ttu-id="85cf0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85cf0-153">DateTimeOffset</span></span>|<span data-ttu-id="85cf0-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="85cf0-154">The date and time the app was created.</span></span> <span data-ttu-id="85cf0-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85cf0-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85cf0-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85cf0-156">lastModifiedDateTime</span></span>|<span data-ttu-id="85cf0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85cf0-157">DateTimeOffset</span></span>|<span data-ttu-id="85cf0-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="85cf0-158">The date and time the app was last modified.</span></span> <span data-ttu-id="85cf0-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85cf0-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85cf0-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="85cf0-160">isFeatured</span></span>|<span data-ttu-id="85cf0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="85cf0-161">Boolean</span></span>|<span data-ttu-id="85cf0-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85cf0-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85cf0-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="85cf0-163">privacyInformationUrl</span></span>|<span data-ttu-id="85cf0-164">String</span><span class="sxs-lookup"><span data-stu-id="85cf0-164">String</span></span>|<span data-ttu-id="85cf0-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="85cf0-165">The privacy statement Url.</span></span> <span data-ttu-id="85cf0-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85cf0-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85cf0-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="85cf0-167">informationUrl</span></span>|<span data-ttu-id="85cf0-168">String</span><span class="sxs-lookup"><span data-stu-id="85cf0-168">String</span></span>|<span data-ttu-id="85cf0-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="85cf0-169">The more information Url.</span></span> <span data-ttu-id="85cf0-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85cf0-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85cf0-171">owner</span><span class="sxs-lookup"><span data-stu-id="85cf0-171">owner</span></span>|<span data-ttu-id="85cf0-172">String</span><span class="sxs-lookup"><span data-stu-id="85cf0-172">String</span></span>|<span data-ttu-id="85cf0-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="85cf0-173">The owner of the app.</span></span> <span data-ttu-id="85cf0-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85cf0-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85cf0-175">developer</span><span class="sxs-lookup"><span data-stu-id="85cf0-175">developer</span></span>|<span data-ttu-id="85cf0-176">String</span><span class="sxs-lookup"><span data-stu-id="85cf0-176">String</span></span>|<span data-ttu-id="85cf0-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="85cf0-177">The developer of the app.</span></span> <span data-ttu-id="85cf0-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85cf0-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85cf0-179">notes</span><span class="sxs-lookup"><span data-stu-id="85cf0-179">notes</span></span>|<span data-ttu-id="85cf0-180">String</span><span class="sxs-lookup"><span data-stu-id="85cf0-180">String</span></span>|<span data-ttu-id="85cf0-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="85cf0-181">Notes for the app.</span></span> <span data-ttu-id="85cf0-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="85cf0-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="85cf0-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="85cf0-183">publishingState</span></span>|[<span data-ttu-id="85cf0-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="85cf0-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="85cf0-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="85cf0-185">The publishing state for the app.</span></span> <span data-ttu-id="85cf0-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="85cf0-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="85cf0-187">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="85cf0-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="85cf0-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="85cf0-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="85cf0-189">响应</span><span class="sxs-lookup"><span data-stu-id="85cf0-189">Response</span></span>
<span data-ttu-id="85cf0-190">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="85cf0-190">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85cf0-191">示例</span><span class="sxs-lookup"><span data-stu-id="85cf0-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="85cf0-192">请求</span><span class="sxs-lookup"><span data-stu-id="85cf0-192">Request</span></span>
<span data-ttu-id="85cf0-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="85cf0-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 584

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
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="85cf0-194">响应</span><span class="sxs-lookup"><span data-stu-id="85cf0-194">Response</span></span>
<span data-ttu-id="85cf0-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="85cf0-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 756

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
  "publishingState": "processing"
}
```






