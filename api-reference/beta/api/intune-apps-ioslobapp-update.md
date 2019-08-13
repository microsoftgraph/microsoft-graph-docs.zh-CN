---
title: 更新 iosLobApp
description: 更新 iosLobApp 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0bdb91b12e0f314e0bcb2ed749c9b1514584da88
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330851"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="cee64-103">更新 iosLobApp</span><span class="sxs-lookup"><span data-stu-id="cee64-103">Update iosLobApp</span></span>

> <span data-ttu-id="cee64-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cee64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cee64-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cee64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cee64-106">更新 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cee64-106">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cee64-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cee64-107">Prerequisites</span></span>
<span data-ttu-id="cee64-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cee64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cee64-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cee64-110">Permission type</span></span>|<span data-ttu-id="cee64-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cee64-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cee64-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cee64-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cee64-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cee64-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cee64-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cee64-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cee64-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cee64-115">Not supported.</span></span>|
|<span data-ttu-id="cee64-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cee64-116">Application</span></span>|<span data-ttu-id="cee64-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cee64-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cee64-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cee64-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="cee64-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cee64-119">Request headers</span></span>
|<span data-ttu-id="cee64-120">标头</span><span class="sxs-lookup"><span data-stu-id="cee64-120">Header</span></span>|<span data-ttu-id="cee64-121">值</span><span class="sxs-lookup"><span data-stu-id="cee64-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cee64-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cee64-122">Authorization</span></span>|<span data-ttu-id="cee64-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cee64-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cee64-124">接受</span><span class="sxs-lookup"><span data-stu-id="cee64-124">Accept</span></span>|<span data-ttu-id="cee64-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cee64-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cee64-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cee64-126">Request body</span></span>
<span data-ttu-id="cee64-127">在请求正文中，提供 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cee64-127">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="cee64-128">下表显示了创建 [iosLobApp](../resources/intune-apps-ioslobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cee64-128">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="cee64-129">属性</span><span class="sxs-lookup"><span data-stu-id="cee64-129">Property</span></span>|<span data-ttu-id="cee64-130">类型</span><span class="sxs-lookup"><span data-stu-id="cee64-130">Type</span></span>|<span data-ttu-id="cee64-131">说明</span><span class="sxs-lookup"><span data-stu-id="cee64-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cee64-132">id</span><span class="sxs-lookup"><span data-stu-id="cee64-132">id</span></span>|<span data-ttu-id="cee64-133">字符串</span><span class="sxs-lookup"><span data-stu-id="cee64-133">String</span></span>|<span data-ttu-id="cee64-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cee64-134">Key of the entity.</span></span> <span data-ttu-id="cee64-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cee64-136">displayName</span></span>|<span data-ttu-id="cee64-137">String</span><span class="sxs-lookup"><span data-stu-id="cee64-137">String</span></span>|<span data-ttu-id="cee64-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="cee64-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cee64-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-140">说明</span><span class="sxs-lookup"><span data-stu-id="cee64-140">description</span></span>|<span data-ttu-id="cee64-141">字符串</span><span class="sxs-lookup"><span data-stu-id="cee64-141">String</span></span>|<span data-ttu-id="cee64-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="cee64-142">The description of the app.</span></span> <span data-ttu-id="cee64-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-144">publisher</span><span class="sxs-lookup"><span data-stu-id="cee64-144">publisher</span></span>|<span data-ttu-id="cee64-145">String</span><span class="sxs-lookup"><span data-stu-id="cee64-145">String</span></span>|<span data-ttu-id="cee64-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="cee64-146">The publisher of the app.</span></span> <span data-ttu-id="cee64-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cee64-148">largeIcon</span></span>|[<span data-ttu-id="cee64-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cee64-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cee64-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="cee64-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cee64-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cee64-152">createdDateTime</span></span>|<span data-ttu-id="cee64-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cee64-153">DateTimeOffset</span></span>|<span data-ttu-id="cee64-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cee64-154">The date and time the app was created.</span></span> <span data-ttu-id="cee64-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cee64-156">lastModifiedDateTime</span></span>|<span data-ttu-id="cee64-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cee64-157">DateTimeOffset</span></span>|<span data-ttu-id="cee64-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cee64-158">The date and time the app was last modified.</span></span> <span data-ttu-id="cee64-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cee64-160">isFeatured</span></span>|<span data-ttu-id="cee64-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="cee64-161">Boolean</span></span>|<span data-ttu-id="cee64-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cee64-163">privacyInformationUrl</span></span>|<span data-ttu-id="cee64-164">String</span><span class="sxs-lookup"><span data-stu-id="cee64-164">String</span></span>|<span data-ttu-id="cee64-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="cee64-165">The privacy statement Url.</span></span> <span data-ttu-id="cee64-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cee64-167">informationUrl</span></span>|<span data-ttu-id="cee64-168">String</span><span class="sxs-lookup"><span data-stu-id="cee64-168">String</span></span>|<span data-ttu-id="cee64-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="cee64-169">The more information Url.</span></span> <span data-ttu-id="cee64-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-171">owner</span><span class="sxs-lookup"><span data-stu-id="cee64-171">owner</span></span>|<span data-ttu-id="cee64-172">String</span><span class="sxs-lookup"><span data-stu-id="cee64-172">String</span></span>|<span data-ttu-id="cee64-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="cee64-173">The owner of the app.</span></span> <span data-ttu-id="cee64-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-175">developer</span><span class="sxs-lookup"><span data-stu-id="cee64-175">developer</span></span>|<span data-ttu-id="cee64-176">String</span><span class="sxs-lookup"><span data-stu-id="cee64-176">String</span></span>|<span data-ttu-id="cee64-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="cee64-177">The developer of the app.</span></span> <span data-ttu-id="cee64-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-179">notes</span><span class="sxs-lookup"><span data-stu-id="cee64-179">notes</span></span>|<span data-ttu-id="cee64-180">String</span><span class="sxs-lookup"><span data-stu-id="cee64-180">String</span></span>|<span data-ttu-id="cee64-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="cee64-181">Notes for the app.</span></span> <span data-ttu-id="cee64-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="cee64-183">uploadState</span></span>|<span data-ttu-id="cee64-184">Int32</span><span class="sxs-lookup"><span data-stu-id="cee64-184">Int32</span></span>|<span data-ttu-id="cee64-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="cee64-185">The upload state.</span></span> <span data-ttu-id="cee64-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="cee64-187">publishingState</span></span>|[<span data-ttu-id="cee64-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cee64-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cee64-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="cee64-189">The publishing state for the app.</span></span> <span data-ttu-id="cee64-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="cee64-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cee64-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="cee64-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="cee64-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="cee64-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cee64-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="cee64-193">isAssigned</span></span>|<span data-ttu-id="cee64-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="cee64-194">Boolean</span></span>|<span data-ttu-id="cee64-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="cee64-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="cee64-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cee64-197">roleScopeTagIds</span></span>|<span data-ttu-id="cee64-198">String collection</span><span class="sxs-lookup"><span data-stu-id="cee64-198">String collection</span></span>|<span data-ttu-id="cee64-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="cee64-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="cee64-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="cee64-201">dependentAppCount</span></span>|<span data-ttu-id="cee64-202">Int32</span><span class="sxs-lookup"><span data-stu-id="cee64-202">Int32</span></span>|<span data-ttu-id="cee64-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="cee64-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="cee64-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cee64-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="cee64-205">committedContentVersion</span></span>|<span data-ttu-id="cee64-206">String</span><span class="sxs-lookup"><span data-stu-id="cee64-206">String</span></span>|<span data-ttu-id="cee64-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="cee64-207">The internal committed content version.</span></span> <span data-ttu-id="cee64-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cee64-209">fileName</span><span class="sxs-lookup"><span data-stu-id="cee64-209">fileName</span></span>|<span data-ttu-id="cee64-210">String</span><span class="sxs-lookup"><span data-stu-id="cee64-210">String</span></span>|<span data-ttu-id="cee64-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="cee64-211">The name of the main Lob application file.</span></span> <span data-ttu-id="cee64-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cee64-213">size</span><span class="sxs-lookup"><span data-stu-id="cee64-213">size</span></span>|<span data-ttu-id="cee64-214">Int64</span><span class="sxs-lookup"><span data-stu-id="cee64-214">Int64</span></span>|<span data-ttu-id="cee64-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="cee64-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="cee64-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cee64-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="cee64-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="cee64-217">bundleId</span></span>|<span data-ttu-id="cee64-218">String</span><span class="sxs-lookup"><span data-stu-id="cee64-218">String</span></span>|<span data-ttu-id="cee64-219">标识名称。</span><span class="sxs-lookup"><span data-stu-id="cee64-219">The Identity Name.</span></span>|
|<span data-ttu-id="cee64-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="cee64-220">applicableDeviceType</span></span>|[<span data-ttu-id="cee64-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="cee64-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="cee64-222">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="cee64-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="cee64-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cee64-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cee64-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cee64-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="cee64-225">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="cee64-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="cee64-226">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cee64-226">expirationDateTime</span></span>|<span data-ttu-id="cee64-227">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cee64-227">DateTimeOffset</span></span>|<span data-ttu-id="cee64-228">过期时间。</span><span class="sxs-lookup"><span data-stu-id="cee64-228">The expiration time.</span></span>|
|<span data-ttu-id="cee64-229">versionNumber</span><span class="sxs-lookup"><span data-stu-id="cee64-229">versionNumber</span></span>|<span data-ttu-id="cee64-230">String</span><span class="sxs-lookup"><span data-stu-id="cee64-230">String</span></span>|<span data-ttu-id="cee64-231">iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="cee64-231">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="cee64-232">buildNumber</span><span class="sxs-lookup"><span data-stu-id="cee64-232">buildNumber</span></span>|<span data-ttu-id="cee64-233">String</span><span class="sxs-lookup"><span data-stu-id="cee64-233">String</span></span>|<span data-ttu-id="cee64-234">iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="cee64-234">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="cee64-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="cee64-235">identityVersion</span></span>|<span data-ttu-id="cee64-236">String</span><span class="sxs-lookup"><span data-stu-id="cee64-236">String</span></span>|<span data-ttu-id="cee64-237">标识版本。</span><span class="sxs-lookup"><span data-stu-id="cee64-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="cee64-238">响应</span><span class="sxs-lookup"><span data-stu-id="cee64-238">Response</span></span>
<span data-ttu-id="cee64-239">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cee64-239">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cee64-240">示例</span><span class="sxs-lookup"><span data-stu-id="cee64-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="cee64-241">请求</span><span class="sxs-lookup"><span data-stu-id="cee64-241">Request</span></span>
<span data-ttu-id="cee64-242">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cee64-242">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1391

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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
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
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="cee64-243">响应</span><span class="sxs-lookup"><span data-stu-id="cee64-243">Response</span></span>
<span data-ttu-id="cee64-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cee64-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1563

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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
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
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```






