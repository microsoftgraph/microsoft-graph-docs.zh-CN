---
title: 更新了 windowsphone81appxbundle
description: 更新了 windowsphone81appxbundle 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2f030ac687d585d65c2ed1f0c3e19605e1e11f47
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37176917"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="9c1f1-103">更新了 windowsphone81appxbundle</span><span class="sxs-lookup"><span data-stu-id="9c1f1-103">Update windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="9c1f1-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c1f1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c1f1-106">更新[了 windowsphone81appxbundle](../resources/intune-apps-windowsphone81appxbundle.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-106">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c1f1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9c1f1-107">Prerequisites</span></span>
<span data-ttu-id="9c1f1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c1f1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c1f1-110">Permission type</span></span>|<span data-ttu-id="9c1f1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9c1f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c1f1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c1f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9c1f1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c1f1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9c1f1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c1f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c1f1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-115">Not supported.</span></span>|
|<span data-ttu-id="9c1f1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c1f1-116">Application</span></span>|<span data-ttu-id="9c1f1-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c1f1-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c1f1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c1f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9c1f1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c1f1-119">Request headers</span></span>
|<span data-ttu-id="9c1f1-120">标头</span><span class="sxs-lookup"><span data-stu-id="9c1f1-120">Header</span></span>|<span data-ttu-id="9c1f1-121">值</span><span class="sxs-lookup"><span data-stu-id="9c1f1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c1f1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c1f1-122">Authorization</span></span>|<span data-ttu-id="9c1f1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c1f1-124">接受</span><span class="sxs-lookup"><span data-stu-id="9c1f1-124">Accept</span></span>|<span data-ttu-id="9c1f1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9c1f1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c1f1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c1f1-126">Request body</span></span>
<span data-ttu-id="9c1f1-127">在请求正文中，提供[了 windowsphone81appxbundle](../resources/intune-apps-windowsphone81appxbundle.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-127">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="9c1f1-128">下表显示创建[了 windowsphone81appxbundle](../resources/intune-apps-windowsphone81appxbundle.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-128">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="9c1f1-129">属性</span><span class="sxs-lookup"><span data-stu-id="9c1f1-129">Property</span></span>|<span data-ttu-id="9c1f1-130">类型</span><span class="sxs-lookup"><span data-stu-id="9c1f1-130">Type</span></span>|<span data-ttu-id="9c1f1-131">说明</span><span class="sxs-lookup"><span data-stu-id="9c1f1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c1f1-132">id</span><span class="sxs-lookup"><span data-stu-id="9c1f1-132">id</span></span>|<span data-ttu-id="9c1f1-133">字符串</span><span class="sxs-lookup"><span data-stu-id="9c1f1-133">String</span></span>|<span data-ttu-id="9c1f1-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-134">Key of the entity.</span></span> <span data-ttu-id="9c1f1-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9c1f1-136">displayName</span></span>|<span data-ttu-id="9c1f1-137">String</span><span class="sxs-lookup"><span data-stu-id="9c1f1-137">String</span></span>|<span data-ttu-id="9c1f1-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9c1f1-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-140">说明</span><span class="sxs-lookup"><span data-stu-id="9c1f1-140">description</span></span>|<span data-ttu-id="9c1f1-141">字符串</span><span class="sxs-lookup"><span data-stu-id="9c1f1-141">String</span></span>|<span data-ttu-id="9c1f1-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-142">The description of the app.</span></span> <span data-ttu-id="9c1f1-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-144">publisher</span><span class="sxs-lookup"><span data-stu-id="9c1f1-144">publisher</span></span>|<span data-ttu-id="9c1f1-145">String</span><span class="sxs-lookup"><span data-stu-id="9c1f1-145">String</span></span>|<span data-ttu-id="9c1f1-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-146">The publisher of the app.</span></span> <span data-ttu-id="9c1f1-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9c1f1-148">largeIcon</span></span>|[<span data-ttu-id="9c1f1-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9c1f1-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9c1f1-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9c1f1-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c1f1-152">createdDateTime</span></span>|<span data-ttu-id="9c1f1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c1f1-153">DateTimeOffset</span></span>|<span data-ttu-id="9c1f1-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-154">The date and time the app was created.</span></span> <span data-ttu-id="9c1f1-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c1f1-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9c1f1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c1f1-157">DateTimeOffset</span></span>|<span data-ttu-id="9c1f1-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-158">The date and time the app was last modified.</span></span> <span data-ttu-id="9c1f1-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9c1f1-160">isFeatured</span></span>|<span data-ttu-id="9c1f1-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c1f1-161">Boolean</span></span>|<span data-ttu-id="9c1f1-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9c1f1-163">privacyInformationUrl</span></span>|<span data-ttu-id="9c1f1-164">String</span><span class="sxs-lookup"><span data-stu-id="9c1f1-164">String</span></span>|<span data-ttu-id="9c1f1-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-165">The privacy statement Url.</span></span> <span data-ttu-id="9c1f1-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9c1f1-167">informationUrl</span></span>|<span data-ttu-id="9c1f1-168">String</span><span class="sxs-lookup"><span data-stu-id="9c1f1-168">String</span></span>|<span data-ttu-id="9c1f1-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-169">The more information Url.</span></span> <span data-ttu-id="9c1f1-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-171">owner</span><span class="sxs-lookup"><span data-stu-id="9c1f1-171">owner</span></span>|<span data-ttu-id="9c1f1-172">String</span><span class="sxs-lookup"><span data-stu-id="9c1f1-172">String</span></span>|<span data-ttu-id="9c1f1-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-173">The owner of the app.</span></span> <span data-ttu-id="9c1f1-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-175">developer</span><span class="sxs-lookup"><span data-stu-id="9c1f1-175">developer</span></span>|<span data-ttu-id="9c1f1-176">String</span><span class="sxs-lookup"><span data-stu-id="9c1f1-176">String</span></span>|<span data-ttu-id="9c1f1-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-177">The developer of the app.</span></span> <span data-ttu-id="9c1f1-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-179">notes</span><span class="sxs-lookup"><span data-stu-id="9c1f1-179">notes</span></span>|<span data-ttu-id="9c1f1-180">String</span><span class="sxs-lookup"><span data-stu-id="9c1f1-180">String</span></span>|<span data-ttu-id="9c1f1-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-181">Notes for the app.</span></span> <span data-ttu-id="9c1f1-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="9c1f1-183">uploadState</span></span>|<span data-ttu-id="9c1f1-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9c1f1-184">Int32</span></span>|<span data-ttu-id="9c1f1-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-185">The upload state.</span></span> <span data-ttu-id="9c1f1-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="9c1f1-187">publishingState</span></span>|[<span data-ttu-id="9c1f1-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9c1f1-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9c1f1-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-189">The publishing state for the app.</span></span> <span data-ttu-id="9c1f1-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9c1f1-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="9c1f1-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9c1f1-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9c1f1-193">isAssigned</span></span>|<span data-ttu-id="9c1f1-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c1f1-194">Boolean</span></span>|<span data-ttu-id="9c1f1-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9c1f1-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9c1f1-197">roleScopeTagIds</span></span>|<span data-ttu-id="9c1f1-198">String collection</span><span class="sxs-lookup"><span data-stu-id="9c1f1-198">String collection</span></span>|<span data-ttu-id="9c1f1-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9c1f1-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="9c1f1-201">dependentAppCount</span></span>|<span data-ttu-id="9c1f1-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9c1f1-202">Int32</span></span>|<span data-ttu-id="9c1f1-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9c1f1-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9c1f1-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9c1f1-205">committedContentVersion</span></span>|<span data-ttu-id="9c1f1-206">String</span><span class="sxs-lookup"><span data-stu-id="9c1f1-206">String</span></span>|<span data-ttu-id="9c1f1-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-207">The internal committed content version.</span></span> <span data-ttu-id="9c1f1-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9c1f1-209">fileName</span><span class="sxs-lookup"><span data-stu-id="9c1f1-209">fileName</span></span>|<span data-ttu-id="9c1f1-210">String</span><span class="sxs-lookup"><span data-stu-id="9c1f1-210">String</span></span>|<span data-ttu-id="9c1f1-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-211">The name of the main Lob application file.</span></span> <span data-ttu-id="9c1f1-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9c1f1-213">size</span><span class="sxs-lookup"><span data-stu-id="9c1f1-213">size</span></span>|<span data-ttu-id="9c1f1-214">Int64</span><span class="sxs-lookup"><span data-stu-id="9c1f1-214">Int64</span></span>|<span data-ttu-id="9c1f1-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="9c1f1-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9c1f1-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="9c1f1-217">applicableArchitectures</span></span>|[<span data-ttu-id="9c1f1-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="9c1f1-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="9c1f1-219">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="9c1f1-220">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-220">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="9c1f1-221">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="9c1f1-222">identityName</span><span class="sxs-lookup"><span data-stu-id="9c1f1-222">identityName</span></span>|<span data-ttu-id="9c1f1-223">String</span><span class="sxs-lookup"><span data-stu-id="9c1f1-223">String</span></span>|<span data-ttu-id="9c1f1-224">标识名称。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-224">The Identity Name.</span></span> <span data-ttu-id="9c1f1-225">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="9c1f1-226">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="9c1f1-226">identityPublisherHash</span></span>|<span data-ttu-id="9c1f1-227">String</span><span class="sxs-lookup"><span data-stu-id="9c1f1-227">String</span></span>|<span data-ttu-id="9c1f1-228">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-228">The Identity Publisher Hash.</span></span> <span data-ttu-id="9c1f1-229">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="9c1f1-230">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="9c1f1-230">identityResourceIdentifier</span></span>|<span data-ttu-id="9c1f1-231">String</span><span class="sxs-lookup"><span data-stu-id="9c1f1-231">String</span></span>|<span data-ttu-id="9c1f1-232">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-232">The Identity Resource Identifier.</span></span> <span data-ttu-id="9c1f1-233">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="9c1f1-234">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9c1f1-234">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9c1f1-235">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9c1f1-235">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="9c1f1-236">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-236">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="9c1f1-237">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="9c1f1-238">将 phoneproductidentifier</span><span class="sxs-lookup"><span data-stu-id="9c1f1-238">phoneProductIdentifier</span></span>|<span data-ttu-id="9c1f1-239">String</span><span class="sxs-lookup"><span data-stu-id="9c1f1-239">String</span></span>|<span data-ttu-id="9c1f1-240">电话产品标识符。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-240">The Phone Product Identifier.</span></span> <span data-ttu-id="9c1f1-241">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-241">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="9c1f1-242">将 phonepublisherid</span><span class="sxs-lookup"><span data-stu-id="9c1f1-242">phonePublisherId</span></span>|<span data-ttu-id="9c1f1-243">String</span><span class="sxs-lookup"><span data-stu-id="9c1f1-243">String</span></span>|<span data-ttu-id="9c1f1-244">电话发布者 Id。继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-244">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="9c1f1-245">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9c1f1-245">identityVersion</span></span>|<span data-ttu-id="9c1f1-246">String</span><span class="sxs-lookup"><span data-stu-id="9c1f1-246">String</span></span>|<span data-ttu-id="9c1f1-247">标识版本。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-247">The identity version.</span></span> <span data-ttu-id="9c1f1-248">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="9c1f1-248">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="9c1f1-249">将 appxpackageinformationlist</span><span class="sxs-lookup"><span data-stu-id="9c1f1-249">appXPackageInformationList</span></span>|<span data-ttu-id="9c1f1-250">[了 windowspackageinformation](../resources/intune-apps-windowspackageinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="9c1f1-250">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="9c1f1-251">AppX 包信息的列表。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-251">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="9c1f1-252">响应</span><span class="sxs-lookup"><span data-stu-id="9c1f1-252">Response</span></span>
<span data-ttu-id="9c1f1-253">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[了 windowsphone81appxbundle](../resources/intune-apps-windowsphone81appxbundle.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-253">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c1f1-254">示例</span><span class="sxs-lookup"><span data-stu-id="9c1f1-254">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c1f1-255">请求</span><span class="sxs-lookup"><span data-stu-id="9c1f1-255">Request</span></span>
<span data-ttu-id="9c1f1-256">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-256">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2311

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true,
        "v10_1809": true,
        "v10_1903": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="9c1f1-257">响应</span><span class="sxs-lookup"><span data-stu-id="9c1f1-257">Response</span></span>
<span data-ttu-id="9c1f1-p129">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c1f1-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2483

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true,
        "v10_1809": true,
        "v10_1903": true
      }
    }
  ]
}
```




