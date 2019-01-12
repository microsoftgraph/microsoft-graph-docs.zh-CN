---
title: 创建 macOSOfficeSuiteApp
description: 创建新的 macOSOfficeSuiteApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2f31345b70d8faec304dd91497af677386fdb43e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931620"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="bd276-103">创建 macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="bd276-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="bd276-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bd276-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd276-105">创建新的 [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bd276-105">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd276-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="bd276-106">Prerequisites</span></span>
<span data-ttu-id="bd276-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="bd276-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd276-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd276-109">Permission type</span></span>|<span data-ttu-id="bd276-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bd276-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd276-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd276-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bd276-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd276-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bd276-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd276-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd276-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd276-114">Not supported.</span></span>|
|<span data-ttu-id="bd276-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd276-115">Application</span></span>|<span data-ttu-id="bd276-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd276-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd276-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd276-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bd276-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd276-118">Request headers</span></span>
|<span data-ttu-id="bd276-119">标头</span><span class="sxs-lookup"><span data-stu-id="bd276-119">Header</span></span>|<span data-ttu-id="bd276-120">值</span><span class="sxs-lookup"><span data-stu-id="bd276-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd276-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd276-121">Authorization</span></span>|<span data-ttu-id="bd276-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bd276-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd276-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bd276-123">Accept</span></span>|<span data-ttu-id="bd276-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bd276-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd276-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd276-125">Request body</span></span>
<span data-ttu-id="bd276-126">在请求正文中，提供 macOSOfficeSuiteApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd276-126">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="bd276-127">下表显示创建 macOSOfficeSuiteApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bd276-127">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="bd276-128">属性</span><span class="sxs-lookup"><span data-stu-id="bd276-128">Property</span></span>|<span data-ttu-id="bd276-129">类型</span><span class="sxs-lookup"><span data-stu-id="bd276-129">Type</span></span>|<span data-ttu-id="bd276-130">说明</span><span class="sxs-lookup"><span data-stu-id="bd276-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd276-131">id</span><span class="sxs-lookup"><span data-stu-id="bd276-131">id</span></span>|<span data-ttu-id="bd276-132">String</span><span class="sxs-lookup"><span data-stu-id="bd276-132">String</span></span>|<span data-ttu-id="bd276-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bd276-133">Key of the entity.</span></span> <span data-ttu-id="bd276-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd276-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd276-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bd276-135">displayName</span></span>|<span data-ttu-id="bd276-136">String</span><span class="sxs-lookup"><span data-stu-id="bd276-136">String</span></span>|<span data-ttu-id="bd276-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="bd276-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bd276-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd276-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd276-139">description</span><span class="sxs-lookup"><span data-stu-id="bd276-139">description</span></span>|<span data-ttu-id="bd276-140">String</span><span class="sxs-lookup"><span data-stu-id="bd276-140">String</span></span>|<span data-ttu-id="bd276-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="bd276-141">The description of the app.</span></span> <span data-ttu-id="bd276-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd276-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd276-143">publisher</span><span class="sxs-lookup"><span data-stu-id="bd276-143">publisher</span></span>|<span data-ttu-id="bd276-144">String</span><span class="sxs-lookup"><span data-stu-id="bd276-144">String</span></span>|<span data-ttu-id="bd276-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="bd276-145">The publisher of the app.</span></span> <span data-ttu-id="bd276-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd276-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd276-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bd276-147">largeIcon</span></span>|[<span data-ttu-id="bd276-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bd276-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bd276-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="bd276-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bd276-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd276-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd276-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd276-151">createdDateTime</span></span>|<span data-ttu-id="bd276-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd276-152">DateTimeOffset</span></span>|<span data-ttu-id="bd276-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bd276-153">The date and time the app was created.</span></span> <span data-ttu-id="bd276-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd276-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd276-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd276-155">lastModifiedDateTime</span></span>|<span data-ttu-id="bd276-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd276-156">DateTimeOffset</span></span>|<span data-ttu-id="bd276-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bd276-157">The date and time the app was last modified.</span></span> <span data-ttu-id="bd276-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd276-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd276-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bd276-159">isFeatured</span></span>|<span data-ttu-id="bd276-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd276-160">Boolean</span></span>|<span data-ttu-id="bd276-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd276-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd276-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bd276-162">privacyInformationUrl</span></span>|<span data-ttu-id="bd276-163">String</span><span class="sxs-lookup"><span data-stu-id="bd276-163">String</span></span>|<span data-ttu-id="bd276-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="bd276-164">The privacy statement Url.</span></span> <span data-ttu-id="bd276-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd276-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd276-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bd276-166">informationUrl</span></span>|<span data-ttu-id="bd276-167">String</span><span class="sxs-lookup"><span data-stu-id="bd276-167">String</span></span>|<span data-ttu-id="bd276-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="bd276-168">The more information Url.</span></span> <span data-ttu-id="bd276-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd276-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd276-170">owner</span><span class="sxs-lookup"><span data-stu-id="bd276-170">owner</span></span>|<span data-ttu-id="bd276-171">String</span><span class="sxs-lookup"><span data-stu-id="bd276-171">String</span></span>|<span data-ttu-id="bd276-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="bd276-172">The owner of the app.</span></span> <span data-ttu-id="bd276-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd276-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd276-174">developer</span><span class="sxs-lookup"><span data-stu-id="bd276-174">developer</span></span>|<span data-ttu-id="bd276-175">String</span><span class="sxs-lookup"><span data-stu-id="bd276-175">String</span></span>|<span data-ttu-id="bd276-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="bd276-176">The developer of the app.</span></span> <span data-ttu-id="bd276-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd276-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd276-178">notes</span><span class="sxs-lookup"><span data-stu-id="bd276-178">notes</span></span>|<span data-ttu-id="bd276-179">String</span><span class="sxs-lookup"><span data-stu-id="bd276-179">String</span></span>|<span data-ttu-id="bd276-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="bd276-180">Notes for the app.</span></span> <span data-ttu-id="bd276-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bd276-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bd276-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="bd276-182">publishingState</span></span>|[<span data-ttu-id="bd276-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bd276-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bd276-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="bd276-184">The publishing state for the app.</span></span> <span data-ttu-id="bd276-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="bd276-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bd276-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="bd276-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="bd276-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="bd276-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="bd276-188">响应</span><span class="sxs-lookup"><span data-stu-id="bd276-188">Response</span></span>
<span data-ttu-id="bd276-189">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bd276-189">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd276-190">示例</span><span class="sxs-lookup"><span data-stu-id="bd276-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="bd276-191">请求</span><span class="sxs-lookup"><span data-stu-id="bd276-191">Request</span></span>
<span data-ttu-id="bd276-192">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bd276-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bd276-193">响应</span><span class="sxs-lookup"><span data-stu-id="bd276-193">Response</span></span>
<span data-ttu-id="bd276-p115">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bd276-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



