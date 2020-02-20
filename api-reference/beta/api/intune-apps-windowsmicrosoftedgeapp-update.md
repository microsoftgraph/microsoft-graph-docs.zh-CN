---
title: 更新 windowsMicrosoftEdgeApp
description: 更新 windowsMicrosoftEdgeApp 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e5d0d57987ce7638fa75d39fbe12cfa4d6c062ef
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160296"
---
# <a name="update-windowsmicrosoftedgeapp"></a><span data-ttu-id="0eb01-103">更新 windowsMicrosoftEdgeApp</span><span class="sxs-lookup"><span data-stu-id="0eb01-103">Update windowsMicrosoftEdgeApp</span></span>

> <span data-ttu-id="0eb01-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0eb01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0eb01-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0eb01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0eb01-106">更新[windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0eb01-106">Update the properties of a [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0eb01-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0eb01-107">Prerequisites</span></span>
<span data-ttu-id="0eb01-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0eb01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0eb01-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0eb01-110">Permission type</span></span>|<span data-ttu-id="0eb01-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0eb01-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0eb01-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0eb01-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0eb01-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eb01-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0eb01-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0eb01-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0eb01-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0eb01-115">Not supported.</span></span>|
|<span data-ttu-id="0eb01-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0eb01-116">Application</span></span>|<span data-ttu-id="0eb01-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0eb01-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0eb01-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0eb01-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="0eb01-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0eb01-119">Request headers</span></span>
|<span data-ttu-id="0eb01-120">标头</span><span class="sxs-lookup"><span data-stu-id="0eb01-120">Header</span></span>|<span data-ttu-id="0eb01-121">值</span><span class="sxs-lookup"><span data-stu-id="0eb01-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0eb01-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0eb01-122">Authorization</span></span>|<span data-ttu-id="0eb01-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0eb01-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0eb01-124">接受</span><span class="sxs-lookup"><span data-stu-id="0eb01-124">Accept</span></span>|<span data-ttu-id="0eb01-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0eb01-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0eb01-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0eb01-126">Request body</span></span>
<span data-ttu-id="0eb01-127">在请求正文中，提供[windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0eb01-127">In the request body, supply a JSON representation for the [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object.</span></span>

<span data-ttu-id="0eb01-128">下表显示创建[windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0eb01-128">The following table shows the properties that are required when you create the [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md).</span></span>

|<span data-ttu-id="0eb01-129">属性</span><span class="sxs-lookup"><span data-stu-id="0eb01-129">Property</span></span>|<span data-ttu-id="0eb01-130">类型</span><span class="sxs-lookup"><span data-stu-id="0eb01-130">Type</span></span>|<span data-ttu-id="0eb01-131">说明</span><span class="sxs-lookup"><span data-stu-id="0eb01-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0eb01-132">id</span><span class="sxs-lookup"><span data-stu-id="0eb01-132">id</span></span>|<span data-ttu-id="0eb01-133">字符串</span><span class="sxs-lookup"><span data-stu-id="0eb01-133">String</span></span>|<span data-ttu-id="0eb01-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0eb01-134">Key of the entity.</span></span> <span data-ttu-id="0eb01-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0eb01-136">displayName</span></span>|<span data-ttu-id="0eb01-137">String</span><span class="sxs-lookup"><span data-stu-id="0eb01-137">String</span></span>|<span data-ttu-id="0eb01-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="0eb01-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0eb01-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-140">说明</span><span class="sxs-lookup"><span data-stu-id="0eb01-140">description</span></span>|<span data-ttu-id="0eb01-141">字符串</span><span class="sxs-lookup"><span data-stu-id="0eb01-141">String</span></span>|<span data-ttu-id="0eb01-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="0eb01-142">The description of the app.</span></span> <span data-ttu-id="0eb01-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-144">publisher</span><span class="sxs-lookup"><span data-stu-id="0eb01-144">publisher</span></span>|<span data-ttu-id="0eb01-145">String</span><span class="sxs-lookup"><span data-stu-id="0eb01-145">String</span></span>|<span data-ttu-id="0eb01-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="0eb01-146">The publisher of the app.</span></span> <span data-ttu-id="0eb01-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0eb01-148">largeIcon</span></span>|[<span data-ttu-id="0eb01-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0eb01-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0eb01-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="0eb01-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0eb01-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0eb01-152">createdDateTime</span></span>|<span data-ttu-id="0eb01-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0eb01-153">DateTimeOffset</span></span>|<span data-ttu-id="0eb01-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0eb01-154">The date and time the app was created.</span></span> <span data-ttu-id="0eb01-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0eb01-156">lastModifiedDateTime</span></span>|<span data-ttu-id="0eb01-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0eb01-157">DateTimeOffset</span></span>|<span data-ttu-id="0eb01-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0eb01-158">The date and time the app was last modified.</span></span> <span data-ttu-id="0eb01-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0eb01-160">isFeatured</span></span>|<span data-ttu-id="0eb01-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb01-161">Boolean</span></span>|<span data-ttu-id="0eb01-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0eb01-163">privacyInformationUrl</span></span>|<span data-ttu-id="0eb01-164">String</span><span class="sxs-lookup"><span data-stu-id="0eb01-164">String</span></span>|<span data-ttu-id="0eb01-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="0eb01-165">The privacy statement Url.</span></span> <span data-ttu-id="0eb01-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0eb01-167">informationUrl</span></span>|<span data-ttu-id="0eb01-168">String</span><span class="sxs-lookup"><span data-stu-id="0eb01-168">String</span></span>|<span data-ttu-id="0eb01-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="0eb01-169">The more information Url.</span></span> <span data-ttu-id="0eb01-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-171">owner</span><span class="sxs-lookup"><span data-stu-id="0eb01-171">owner</span></span>|<span data-ttu-id="0eb01-172">String</span><span class="sxs-lookup"><span data-stu-id="0eb01-172">String</span></span>|<span data-ttu-id="0eb01-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="0eb01-173">The owner of the app.</span></span> <span data-ttu-id="0eb01-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-175">developer</span><span class="sxs-lookup"><span data-stu-id="0eb01-175">developer</span></span>|<span data-ttu-id="0eb01-176">String</span><span class="sxs-lookup"><span data-stu-id="0eb01-176">String</span></span>|<span data-ttu-id="0eb01-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="0eb01-177">The developer of the app.</span></span> <span data-ttu-id="0eb01-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-179">notes</span><span class="sxs-lookup"><span data-stu-id="0eb01-179">notes</span></span>|<span data-ttu-id="0eb01-180">String</span><span class="sxs-lookup"><span data-stu-id="0eb01-180">String</span></span>|<span data-ttu-id="0eb01-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="0eb01-181">Notes for the app.</span></span> <span data-ttu-id="0eb01-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="0eb01-183">uploadState</span></span>|<span data-ttu-id="0eb01-184">Int32</span><span class="sxs-lookup"><span data-stu-id="0eb01-184">Int32</span></span>|<span data-ttu-id="0eb01-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="0eb01-185">The upload state.</span></span> <span data-ttu-id="0eb01-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="0eb01-187">publishingState</span></span>|[<span data-ttu-id="0eb01-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0eb01-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0eb01-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="0eb01-189">The publishing state for the app.</span></span> <span data-ttu-id="0eb01-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="0eb01-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0eb01-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="0eb01-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="0eb01-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="0eb01-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0eb01-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0eb01-193">isAssigned</span></span>|<span data-ttu-id="0eb01-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="0eb01-194">Boolean</span></span>|<span data-ttu-id="0eb01-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="0eb01-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="0eb01-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0eb01-197">roleScopeTagIds</span></span>|<span data-ttu-id="0eb01-198">String collection</span><span class="sxs-lookup"><span data-stu-id="0eb01-198">String collection</span></span>|<span data-ttu-id="0eb01-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="0eb01-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="0eb01-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="0eb01-201">dependentAppCount</span></span>|<span data-ttu-id="0eb01-202">Int32</span><span class="sxs-lookup"><span data-stu-id="0eb01-202">Int32</span></span>|<span data-ttu-id="0eb01-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="0eb01-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="0eb01-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="0eb01-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="0eb01-205">信道</span><span class="sxs-lookup"><span data-stu-id="0eb01-205">channel</span></span>|[<span data-ttu-id="0eb01-206">microsoftEdgeChannel</span><span class="sxs-lookup"><span data-stu-id="0eb01-206">microsoftEdgeChannel</span></span>](../resources/intune-apps-microsoftedgechannel.md)|<span data-ttu-id="0eb01-207">要在目标设备上安装的通道。</span><span class="sxs-lookup"><span data-stu-id="0eb01-207">The channel to install on target devices.</span></span> <span data-ttu-id="0eb01-208">可取值为：`dev`、`beta`、`stable`。</span><span class="sxs-lookup"><span data-stu-id="0eb01-208">Possible values are: `dev`, `beta`, `stable`.</span></span>|
|<span data-ttu-id="0eb01-209">displayLanguageLocale</span><span class="sxs-lookup"><span data-stu-id="0eb01-209">displayLanguageLocale</span></span>|<span data-ttu-id="0eb01-210">String</span><span class="sxs-lookup"><span data-stu-id="0eb01-210">String</span></span>|<span data-ttu-id="0eb01-211">边缘应用向用户显示文本时要使用的语言区域设置。</span><span class="sxs-lookup"><span data-stu-id="0eb01-211">The language locale to use when the Edge app displays text to the user.</span></span>|



## <a name="response"></a><span data-ttu-id="0eb01-212">响应</span><span class="sxs-lookup"><span data-stu-id="0eb01-212">Response</span></span>
<span data-ttu-id="0eb01-213">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0eb01-213">If successful, this method returns a `200 OK` response code and an updated [windowsMicrosoftEdgeApp](../resources/intune-apps-windowsmicrosoftedgeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0eb01-214">示例</span><span class="sxs-lookup"><span data-stu-id="0eb01-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="0eb01-215">请求</span><span class="sxs-lookup"><span data-stu-id="0eb01-215">Request</span></span>
<span data-ttu-id="0eb01-216">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0eb01-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 805

{
  "@odata.type": "#microsoft.graph.windowsMicrosoftEdgeApp",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "channel": "beta",
  "displayLanguageLocale": "Display Language Locale value"
}
```

### <a name="response"></a><span data-ttu-id="0eb01-217">响应</span><span class="sxs-lookup"><span data-stu-id="0eb01-217">Response</span></span>
<span data-ttu-id="0eb01-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0eb01-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "@odata.type": "#microsoft.graph.windowsMicrosoftEdgeApp",
  "id": "a4d4a316-a316-a4d4-16a3-d4a416a3d4a4",
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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "channel": "beta",
  "displayLanguageLocale": "Display Language Locale value"
}
```





