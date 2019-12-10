---
title: 更新 androidLobApp
description: 更新 androidLobApp 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 74143d7ebfbf8c621ef294eee326200f4cc1b633
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39922298"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="efb62-103">更新 androidLobApp</span><span class="sxs-lookup"><span data-stu-id="efb62-103">Update androidLobApp</span></span>

> <span data-ttu-id="efb62-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="efb62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efb62-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="efb62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efb62-106">更新 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="efb62-106">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="efb62-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="efb62-107">Prerequisites</span></span>
<span data-ttu-id="efb62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="efb62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="efb62-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="efb62-110">Permission type</span></span>|<span data-ttu-id="efb62-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="efb62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="efb62-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="efb62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="efb62-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efb62-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="efb62-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="efb62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="efb62-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="efb62-115">Not supported.</span></span>|
|<span data-ttu-id="efb62-116">Application</span><span class="sxs-lookup"><span data-stu-id="efb62-116">Application</span></span>|<span data-ttu-id="efb62-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="efb62-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="efb62-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="efb62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="efb62-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="efb62-119">Request headers</span></span>
|<span data-ttu-id="efb62-120">标头</span><span class="sxs-lookup"><span data-stu-id="efb62-120">Header</span></span>|<span data-ttu-id="efb62-121">值</span><span class="sxs-lookup"><span data-stu-id="efb62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="efb62-122">授权</span><span class="sxs-lookup"><span data-stu-id="efb62-122">Authorization</span></span>|<span data-ttu-id="efb62-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="efb62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="efb62-124">接受</span><span class="sxs-lookup"><span data-stu-id="efb62-124">Accept</span></span>|<span data-ttu-id="efb62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="efb62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="efb62-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="efb62-126">Request body</span></span>
<span data-ttu-id="efb62-127">在请求正文中，提供 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efb62-127">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="efb62-128">下表显示了创建 [androidLobApp](../resources/intune-apps-androidlobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="efb62-128">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="efb62-129">属性</span><span class="sxs-lookup"><span data-stu-id="efb62-129">Property</span></span>|<span data-ttu-id="efb62-130">类型</span><span class="sxs-lookup"><span data-stu-id="efb62-130">Type</span></span>|<span data-ttu-id="efb62-131">说明</span><span class="sxs-lookup"><span data-stu-id="efb62-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efb62-132">id</span><span class="sxs-lookup"><span data-stu-id="efb62-132">id</span></span>|<span data-ttu-id="efb62-133">字符串</span><span class="sxs-lookup"><span data-stu-id="efb62-133">String</span></span>|<span data-ttu-id="efb62-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="efb62-134">Key of the entity.</span></span> <span data-ttu-id="efb62-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-136">displayName</span><span class="sxs-lookup"><span data-stu-id="efb62-136">displayName</span></span>|<span data-ttu-id="efb62-137">字符串</span><span class="sxs-lookup"><span data-stu-id="efb62-137">String</span></span>|<span data-ttu-id="efb62-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="efb62-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="efb62-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-140">说明</span><span class="sxs-lookup"><span data-stu-id="efb62-140">description</span></span>|<span data-ttu-id="efb62-141">字符串</span><span class="sxs-lookup"><span data-stu-id="efb62-141">String</span></span>|<span data-ttu-id="efb62-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="efb62-142">The description of the app.</span></span> <span data-ttu-id="efb62-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-144">publisher</span><span class="sxs-lookup"><span data-stu-id="efb62-144">publisher</span></span>|<span data-ttu-id="efb62-145">字符串</span><span class="sxs-lookup"><span data-stu-id="efb62-145">String</span></span>|<span data-ttu-id="efb62-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="efb62-146">The publisher of the app.</span></span> <span data-ttu-id="efb62-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="efb62-148">largeIcon</span></span>|[<span data-ttu-id="efb62-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="efb62-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="efb62-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="efb62-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="efb62-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="efb62-152">createdDateTime</span></span>|<span data-ttu-id="efb62-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efb62-153">DateTimeOffset</span></span>|<span data-ttu-id="efb62-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="efb62-154">The date and time the app was created.</span></span> <span data-ttu-id="efb62-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="efb62-156">lastModifiedDateTime</span></span>|<span data-ttu-id="efb62-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efb62-157">DateTimeOffset</span></span>|<span data-ttu-id="efb62-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="efb62-158">The date and time the app was last modified.</span></span> <span data-ttu-id="efb62-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="efb62-160">isFeatured</span></span>|<span data-ttu-id="efb62-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="efb62-161">Boolean</span></span>|<span data-ttu-id="efb62-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="efb62-163">privacyInformationUrl</span></span>|<span data-ttu-id="efb62-164">字符串</span><span class="sxs-lookup"><span data-stu-id="efb62-164">String</span></span>|<span data-ttu-id="efb62-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="efb62-165">The privacy statement Url.</span></span> <span data-ttu-id="efb62-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="efb62-167">informationUrl</span></span>|<span data-ttu-id="efb62-168">字符串</span><span class="sxs-lookup"><span data-stu-id="efb62-168">String</span></span>|<span data-ttu-id="efb62-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="efb62-169">The more information Url.</span></span> <span data-ttu-id="efb62-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-171">owner</span><span class="sxs-lookup"><span data-stu-id="efb62-171">owner</span></span>|<span data-ttu-id="efb62-172">String</span><span class="sxs-lookup"><span data-stu-id="efb62-172">String</span></span>|<span data-ttu-id="efb62-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="efb62-173">The owner of the app.</span></span> <span data-ttu-id="efb62-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-175">developer</span><span class="sxs-lookup"><span data-stu-id="efb62-175">developer</span></span>|<span data-ttu-id="efb62-176">字符串</span><span class="sxs-lookup"><span data-stu-id="efb62-176">String</span></span>|<span data-ttu-id="efb62-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="efb62-177">The developer of the app.</span></span> <span data-ttu-id="efb62-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-179">notes</span><span class="sxs-lookup"><span data-stu-id="efb62-179">notes</span></span>|<span data-ttu-id="efb62-180">字符串</span><span class="sxs-lookup"><span data-stu-id="efb62-180">String</span></span>|<span data-ttu-id="efb62-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="efb62-181">Notes for the app.</span></span> <span data-ttu-id="efb62-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="efb62-183">uploadState</span></span>|<span data-ttu-id="efb62-184">Int32</span><span class="sxs-lookup"><span data-stu-id="efb62-184">Int32</span></span>|<span data-ttu-id="efb62-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="efb62-185">The upload state.</span></span> <span data-ttu-id="efb62-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="efb62-187">publishingState</span></span>|[<span data-ttu-id="efb62-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="efb62-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="efb62-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="efb62-189">The publishing state for the app.</span></span> <span data-ttu-id="efb62-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="efb62-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="efb62-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="efb62-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="efb62-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="efb62-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="efb62-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="efb62-193">isAssigned</span></span>|<span data-ttu-id="efb62-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="efb62-194">Boolean</span></span>|<span data-ttu-id="efb62-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="efb62-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="efb62-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="efb62-197">roleScopeTagIds</span></span>|<span data-ttu-id="efb62-198">String collection</span><span class="sxs-lookup"><span data-stu-id="efb62-198">String collection</span></span>|<span data-ttu-id="efb62-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="efb62-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="efb62-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="efb62-201">dependentAppCount</span></span>|<span data-ttu-id="efb62-202">Int32</span><span class="sxs-lookup"><span data-stu-id="efb62-202">Int32</span></span>|<span data-ttu-id="efb62-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="efb62-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="efb62-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="efb62-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="efb62-205">committedContentVersion</span></span>|<span data-ttu-id="efb62-206">字符串</span><span class="sxs-lookup"><span data-stu-id="efb62-206">String</span></span>|<span data-ttu-id="efb62-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="efb62-207">The internal committed content version.</span></span> <span data-ttu-id="efb62-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="efb62-209">fileName</span><span class="sxs-lookup"><span data-stu-id="efb62-209">fileName</span></span>|<span data-ttu-id="efb62-210">字符串</span><span class="sxs-lookup"><span data-stu-id="efb62-210">String</span></span>|<span data-ttu-id="efb62-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="efb62-211">The name of the main Lob application file.</span></span> <span data-ttu-id="efb62-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="efb62-213">size</span><span class="sxs-lookup"><span data-stu-id="efb62-213">size</span></span>|<span data-ttu-id="efb62-214">Int64</span><span class="sxs-lookup"><span data-stu-id="efb62-214">Int64</span></span>|<span data-ttu-id="efb62-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="efb62-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="efb62-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="efb62-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="efb62-217">packageId</span><span class="sxs-lookup"><span data-stu-id="efb62-217">packageId</span></span>|<span data-ttu-id="efb62-218">字符串</span><span class="sxs-lookup"><span data-stu-id="efb62-218">String</span></span>|<span data-ttu-id="efb62-219">包标识符。</span><span class="sxs-lookup"><span data-stu-id="efb62-219">The package identifier.</span></span>|
|<span data-ttu-id="efb62-220">identityName</span><span class="sxs-lookup"><span data-stu-id="efb62-220">identityName</span></span>|<span data-ttu-id="efb62-221">String</span><span class="sxs-lookup"><span data-stu-id="efb62-221">String</span></span>|<span data-ttu-id="efb62-222">标识名称。</span><span class="sxs-lookup"><span data-stu-id="efb62-222">The Identity Name.</span></span>|
|<span data-ttu-id="efb62-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="efb62-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="efb62-224">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="efb62-224">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="efb62-225">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="efb62-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="efb62-226">versionName</span><span class="sxs-lookup"><span data-stu-id="efb62-226">versionName</span></span>|<span data-ttu-id="efb62-227">字符串</span><span class="sxs-lookup"><span data-stu-id="efb62-227">String</span></span>|<span data-ttu-id="efb62-228">Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="efb62-228">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="efb62-229">versionCode</span><span class="sxs-lookup"><span data-stu-id="efb62-229">versionCode</span></span>|<span data-ttu-id="efb62-230">字符串</span><span class="sxs-lookup"><span data-stu-id="efb62-230">String</span></span>|<span data-ttu-id="efb62-231">Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="efb62-231">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="efb62-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="efb62-232">identityVersion</span></span>|<span data-ttu-id="efb62-233">String</span><span class="sxs-lookup"><span data-stu-id="efb62-233">String</span></span>|<span data-ttu-id="efb62-234">标识版本。</span><span class="sxs-lookup"><span data-stu-id="efb62-234">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="efb62-235">响应</span><span class="sxs-lookup"><span data-stu-id="efb62-235">Response</span></span>
<span data-ttu-id="efb62-236">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidLobApp](../resources/intune-apps-androidlobapp.md)  对象。</span><span class="sxs-lookup"><span data-stu-id="efb62-236">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="efb62-237">示例</span><span class="sxs-lookup"><span data-stu-id="efb62-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="efb62-238">请求</span><span class="sxs-lookup"><span data-stu-id="efb62-238">Request</span></span>
<span data-ttu-id="efb62-239">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="efb62-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1413

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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="efb62-240">响应</span><span class="sxs-lookup"><span data-stu-id="efb62-240">Response</span></span>
<span data-ttu-id="efb62-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="efb62-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1585

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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```





