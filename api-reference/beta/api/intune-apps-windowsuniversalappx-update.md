---
title: 更新 windowsUniversalAppX
description: 更新 windowsUniversalAppX 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 259bf7701536f6b215bcc65b31ea5b3cccd07802
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450438"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="9bdd5-103">更新 windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="9bdd5-103">Update windowsUniversalAppX</span></span>

<span data-ttu-id="9bdd5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9bdd5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9bdd5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bdd5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bdd5-107">更新 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-107">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9bdd5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9bdd5-108">Prerequisites</span></span>
<span data-ttu-id="9bdd5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bdd5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9bdd5-111">Permission type</span></span>|<span data-ttu-id="9bdd5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9bdd5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bdd5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9bdd5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9bdd5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bdd5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9bdd5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9bdd5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bdd5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-116">Not supported.</span></span>|
|<span data-ttu-id="9bdd5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9bdd5-117">Application</span></span>|<span data-ttu-id="9bdd5-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bdd5-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bdd5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9bdd5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="9bdd5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9bdd5-120">Request headers</span></span>
|<span data-ttu-id="9bdd5-121">标头</span><span class="sxs-lookup"><span data-stu-id="9bdd5-121">Header</span></span>|<span data-ttu-id="9bdd5-122">值</span><span class="sxs-lookup"><span data-stu-id="9bdd5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bdd5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bdd5-123">Authorization</span></span>|<span data-ttu-id="9bdd5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bdd5-125">接受</span><span class="sxs-lookup"><span data-stu-id="9bdd5-125">Accept</span></span>|<span data-ttu-id="9bdd5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9bdd5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bdd5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9bdd5-127">Request body</span></span>
<span data-ttu-id="9bdd5-128">在请求正文中，提供 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-128">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="9bdd5-129">下表显示创建 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-129">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="9bdd5-130">属性</span><span class="sxs-lookup"><span data-stu-id="9bdd5-130">Property</span></span>|<span data-ttu-id="9bdd5-131">类型</span><span class="sxs-lookup"><span data-stu-id="9bdd5-131">Type</span></span>|<span data-ttu-id="9bdd5-132">说明</span><span class="sxs-lookup"><span data-stu-id="9bdd5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bdd5-133">id</span><span class="sxs-lookup"><span data-stu-id="9bdd5-133">id</span></span>|<span data-ttu-id="9bdd5-134">字符串</span><span class="sxs-lookup"><span data-stu-id="9bdd5-134">String</span></span>|<span data-ttu-id="9bdd5-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-135">Key of the entity.</span></span> <span data-ttu-id="9bdd5-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9bdd5-137">displayName</span></span>|<span data-ttu-id="9bdd5-138">String</span><span class="sxs-lookup"><span data-stu-id="9bdd5-138">String</span></span>|<span data-ttu-id="9bdd5-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9bdd5-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-141">说明</span><span class="sxs-lookup"><span data-stu-id="9bdd5-141">description</span></span>|<span data-ttu-id="9bdd5-142">字符串</span><span class="sxs-lookup"><span data-stu-id="9bdd5-142">String</span></span>|<span data-ttu-id="9bdd5-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-143">The description of the app.</span></span> <span data-ttu-id="9bdd5-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-145">publisher</span><span class="sxs-lookup"><span data-stu-id="9bdd5-145">publisher</span></span>|<span data-ttu-id="9bdd5-146">String</span><span class="sxs-lookup"><span data-stu-id="9bdd5-146">String</span></span>|<span data-ttu-id="9bdd5-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-147">The publisher of the app.</span></span> <span data-ttu-id="9bdd5-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9bdd5-149">largeIcon</span></span>|[<span data-ttu-id="9bdd5-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9bdd5-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9bdd5-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9bdd5-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9bdd5-153">createdDateTime</span></span>|<span data-ttu-id="9bdd5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bdd5-154">DateTimeOffset</span></span>|<span data-ttu-id="9bdd5-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-155">The date and time the app was created.</span></span> <span data-ttu-id="9bdd5-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9bdd5-157">lastModifiedDateTime</span></span>|<span data-ttu-id="9bdd5-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bdd5-158">DateTimeOffset</span></span>|<span data-ttu-id="9bdd5-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-159">The date and time the app was last modified.</span></span> <span data-ttu-id="9bdd5-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9bdd5-161">isFeatured</span></span>|<span data-ttu-id="9bdd5-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bdd5-162">Boolean</span></span>|<span data-ttu-id="9bdd5-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9bdd5-164">privacyInformationUrl</span></span>|<span data-ttu-id="9bdd5-165">String</span><span class="sxs-lookup"><span data-stu-id="9bdd5-165">String</span></span>|<span data-ttu-id="9bdd5-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-166">The privacy statement Url.</span></span> <span data-ttu-id="9bdd5-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9bdd5-168">informationUrl</span></span>|<span data-ttu-id="9bdd5-169">String</span><span class="sxs-lookup"><span data-stu-id="9bdd5-169">String</span></span>|<span data-ttu-id="9bdd5-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-170">The more information Url.</span></span> <span data-ttu-id="9bdd5-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-172">owner</span><span class="sxs-lookup"><span data-stu-id="9bdd5-172">owner</span></span>|<span data-ttu-id="9bdd5-173">String</span><span class="sxs-lookup"><span data-stu-id="9bdd5-173">String</span></span>|<span data-ttu-id="9bdd5-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-174">The owner of the app.</span></span> <span data-ttu-id="9bdd5-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-176">developer</span><span class="sxs-lookup"><span data-stu-id="9bdd5-176">developer</span></span>|<span data-ttu-id="9bdd5-177">String</span><span class="sxs-lookup"><span data-stu-id="9bdd5-177">String</span></span>|<span data-ttu-id="9bdd5-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-178">The developer of the app.</span></span> <span data-ttu-id="9bdd5-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-180">notes</span><span class="sxs-lookup"><span data-stu-id="9bdd5-180">notes</span></span>|<span data-ttu-id="9bdd5-181">String</span><span class="sxs-lookup"><span data-stu-id="9bdd5-181">String</span></span>|<span data-ttu-id="9bdd5-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-182">Notes for the app.</span></span> <span data-ttu-id="9bdd5-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="9bdd5-184">uploadState</span></span>|<span data-ttu-id="9bdd5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="9bdd5-185">Int32</span></span>|<span data-ttu-id="9bdd5-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-186">The upload state.</span></span> <span data-ttu-id="9bdd5-187">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="9bdd5-188">publishingState</span></span>|[<span data-ttu-id="9bdd5-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9bdd5-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9bdd5-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-190">The publishing state for the app.</span></span> <span data-ttu-id="9bdd5-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9bdd5-192">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="9bdd5-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9bdd5-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9bdd5-194">isAssigned</span></span>|<span data-ttu-id="9bdd5-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bdd5-195">Boolean</span></span>|<span data-ttu-id="9bdd5-196">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9bdd5-197">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9bdd5-198">roleScopeTagIds</span></span>|<span data-ttu-id="9bdd5-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="9bdd5-199">String collection</span></span>|<span data-ttu-id="9bdd5-200">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9bdd5-201">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="9bdd5-202">dependentAppCount</span></span>|<span data-ttu-id="9bdd5-203">Int32</span><span class="sxs-lookup"><span data-stu-id="9bdd5-203">Int32</span></span>|<span data-ttu-id="9bdd5-204">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9bdd5-205">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="9bdd5-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9bdd5-206">committedContentVersion</span></span>|<span data-ttu-id="9bdd5-207">String</span><span class="sxs-lookup"><span data-stu-id="9bdd5-207">String</span></span>|<span data-ttu-id="9bdd5-208">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-208">The internal committed content version.</span></span> <span data-ttu-id="9bdd5-209">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9bdd5-210">fileName</span><span class="sxs-lookup"><span data-stu-id="9bdd5-210">fileName</span></span>|<span data-ttu-id="9bdd5-211">String</span><span class="sxs-lookup"><span data-stu-id="9bdd5-211">String</span></span>|<span data-ttu-id="9bdd5-212">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-212">The name of the main Lob application file.</span></span> <span data-ttu-id="9bdd5-213">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9bdd5-214">size</span><span class="sxs-lookup"><span data-stu-id="9bdd5-214">size</span></span>|<span data-ttu-id="9bdd5-215">Int64</span><span class="sxs-lookup"><span data-stu-id="9bdd5-215">Int64</span></span>|<span data-ttu-id="9bdd5-216">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="9bdd5-217">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9bdd5-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9bdd5-218">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="9bdd5-218">applicableArchitectures</span></span>|[<span data-ttu-id="9bdd5-219">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="9bdd5-219">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="9bdd5-220">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-220">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="9bdd5-221">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="9bdd5-222">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="9bdd5-222">applicableDeviceTypes</span></span>|[<span data-ttu-id="9bdd5-223">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="9bdd5-223">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="9bdd5-224">可运行此应用的 Windows 设备类型。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-224">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="9bdd5-225">可取值为：`none`、`desktop`、`mobile`、`holographic`、`team`。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-225">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="9bdd5-226">identityName</span><span class="sxs-lookup"><span data-stu-id="9bdd5-226">identityName</span></span>|<span data-ttu-id="9bdd5-227">String</span><span class="sxs-lookup"><span data-stu-id="9bdd5-227">String</span></span>|<span data-ttu-id="9bdd5-228">标识名称。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-228">The Identity Name.</span></span>|
|<span data-ttu-id="9bdd5-229">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="9bdd5-229">identityPublisherHash</span></span>|<span data-ttu-id="9bdd5-230">String</span><span class="sxs-lookup"><span data-stu-id="9bdd5-230">String</span></span>|<span data-ttu-id="9bdd5-231">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-231">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="9bdd5-232">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="9bdd5-232">identityResourceIdentifier</span></span>|<span data-ttu-id="9bdd5-233">String</span><span class="sxs-lookup"><span data-stu-id="9bdd5-233">String</span></span>|<span data-ttu-id="9bdd5-234">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-234">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="9bdd5-235">isBundle</span><span class="sxs-lookup"><span data-stu-id="9bdd5-235">isBundle</span></span>|<span data-ttu-id="9bdd5-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="9bdd5-236">Boolean</span></span>|<span data-ttu-id="9bdd5-237">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-237">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="9bdd5-238">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9bdd5-238">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9bdd5-239">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9bdd5-239">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="9bdd5-240">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-240">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9bdd5-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9bdd5-241">identityVersion</span></span>|<span data-ttu-id="9bdd5-242">String</span><span class="sxs-lookup"><span data-stu-id="9bdd5-242">String</span></span>|<span data-ttu-id="9bdd5-243">标识版本。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-243">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="9bdd5-244">响应</span><span class="sxs-lookup"><span data-stu-id="9bdd5-244">Response</span></span>
<span data-ttu-id="9bdd5-245">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-245">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bdd5-246">示例</span><span class="sxs-lookup"><span data-stu-id="9bdd5-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="9bdd5-247">请求</span><span class="sxs-lookup"><span data-stu-id="9bdd5-247">Request</span></span>
<span data-ttu-id="9bdd5-248">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1461

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="9bdd5-249">响应</span><span class="sxs-lookup"><span data-stu-id="9bdd5-249">Response</span></span>
<span data-ttu-id="9bdd5-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9bdd5-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```





