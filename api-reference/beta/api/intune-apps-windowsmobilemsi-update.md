---
title: 更新 windowsMobileMSI
description: 更新 windowsMobileMSI 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad7bd8beb2572fa6c9f92976ab9a33f46b99fd70
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934703"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="186f7-103">更新 windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="186f7-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="186f7-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="186f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="186f7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="186f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="186f7-106">更新 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="186f7-106">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="186f7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="186f7-107">Prerequisites</span></span>
<span data-ttu-id="186f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="186f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="186f7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="186f7-110">Permission type</span></span>|<span data-ttu-id="186f7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="186f7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="186f7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="186f7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="186f7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="186f7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="186f7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="186f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="186f7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="186f7-115">Not supported.</span></span>|
|<span data-ttu-id="186f7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="186f7-116">Application</span></span>|<span data-ttu-id="186f7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="186f7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="186f7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="186f7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="186f7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="186f7-119">Request headers</span></span>
|<span data-ttu-id="186f7-120">标头</span><span class="sxs-lookup"><span data-stu-id="186f7-120">Header</span></span>|<span data-ttu-id="186f7-121">值</span><span class="sxs-lookup"><span data-stu-id="186f7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="186f7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="186f7-122">Authorization</span></span>|<span data-ttu-id="186f7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="186f7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="186f7-124">接受</span><span class="sxs-lookup"><span data-stu-id="186f7-124">Accept</span></span>|<span data-ttu-id="186f7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="186f7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="186f7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="186f7-126">Request body</span></span>
<span data-ttu-id="186f7-127">在请求正文中，提供 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="186f7-127">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="186f7-128">下表显示创建 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="186f7-128">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="186f7-129">属性</span><span class="sxs-lookup"><span data-stu-id="186f7-129">Property</span></span>|<span data-ttu-id="186f7-130">类型</span><span class="sxs-lookup"><span data-stu-id="186f7-130">Type</span></span>|<span data-ttu-id="186f7-131">说明</span><span class="sxs-lookup"><span data-stu-id="186f7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="186f7-132">id</span><span class="sxs-lookup"><span data-stu-id="186f7-132">id</span></span>|<span data-ttu-id="186f7-133">字符串</span><span class="sxs-lookup"><span data-stu-id="186f7-133">String</span></span>|<span data-ttu-id="186f7-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="186f7-134">Key of the entity.</span></span> <span data-ttu-id="186f7-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="186f7-136">displayName</span></span>|<span data-ttu-id="186f7-137">String</span><span class="sxs-lookup"><span data-stu-id="186f7-137">String</span></span>|<span data-ttu-id="186f7-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="186f7-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="186f7-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-140">说明</span><span class="sxs-lookup"><span data-stu-id="186f7-140">description</span></span>|<span data-ttu-id="186f7-141">字符串</span><span class="sxs-lookup"><span data-stu-id="186f7-141">String</span></span>|<span data-ttu-id="186f7-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="186f7-142">The description of the app.</span></span> <span data-ttu-id="186f7-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-144">publisher</span><span class="sxs-lookup"><span data-stu-id="186f7-144">publisher</span></span>|<span data-ttu-id="186f7-145">String</span><span class="sxs-lookup"><span data-stu-id="186f7-145">String</span></span>|<span data-ttu-id="186f7-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="186f7-146">The publisher of the app.</span></span> <span data-ttu-id="186f7-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="186f7-148">largeIcon</span></span>|[<span data-ttu-id="186f7-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="186f7-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="186f7-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="186f7-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="186f7-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="186f7-152">createdDateTime</span></span>|<span data-ttu-id="186f7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="186f7-153">DateTimeOffset</span></span>|<span data-ttu-id="186f7-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="186f7-154">The date and time the app was created.</span></span> <span data-ttu-id="186f7-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="186f7-156">lastModifiedDateTime</span></span>|<span data-ttu-id="186f7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="186f7-157">DateTimeOffset</span></span>|<span data-ttu-id="186f7-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="186f7-158">The date and time the app was last modified.</span></span> <span data-ttu-id="186f7-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="186f7-160">isFeatured</span></span>|<span data-ttu-id="186f7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="186f7-161">Boolean</span></span>|<span data-ttu-id="186f7-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="186f7-163">privacyInformationUrl</span></span>|<span data-ttu-id="186f7-164">String</span><span class="sxs-lookup"><span data-stu-id="186f7-164">String</span></span>|<span data-ttu-id="186f7-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="186f7-165">The privacy statement Url.</span></span> <span data-ttu-id="186f7-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="186f7-167">informationUrl</span></span>|<span data-ttu-id="186f7-168">String</span><span class="sxs-lookup"><span data-stu-id="186f7-168">String</span></span>|<span data-ttu-id="186f7-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="186f7-169">The more information Url.</span></span> <span data-ttu-id="186f7-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-171">owner</span><span class="sxs-lookup"><span data-stu-id="186f7-171">owner</span></span>|<span data-ttu-id="186f7-172">String</span><span class="sxs-lookup"><span data-stu-id="186f7-172">String</span></span>|<span data-ttu-id="186f7-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="186f7-173">The owner of the app.</span></span> <span data-ttu-id="186f7-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-175">developer</span><span class="sxs-lookup"><span data-stu-id="186f7-175">developer</span></span>|<span data-ttu-id="186f7-176">String</span><span class="sxs-lookup"><span data-stu-id="186f7-176">String</span></span>|<span data-ttu-id="186f7-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="186f7-177">The developer of the app.</span></span> <span data-ttu-id="186f7-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-179">notes</span><span class="sxs-lookup"><span data-stu-id="186f7-179">notes</span></span>|<span data-ttu-id="186f7-180">String</span><span class="sxs-lookup"><span data-stu-id="186f7-180">String</span></span>|<span data-ttu-id="186f7-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="186f7-181">Notes for the app.</span></span> <span data-ttu-id="186f7-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="186f7-183">uploadState</span></span>|<span data-ttu-id="186f7-184">Int32</span><span class="sxs-lookup"><span data-stu-id="186f7-184">Int32</span></span>|<span data-ttu-id="186f7-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="186f7-185">The upload state.</span></span> <span data-ttu-id="186f7-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="186f7-187">publishingState</span></span>|[<span data-ttu-id="186f7-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="186f7-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="186f7-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="186f7-189">The publishing state for the app.</span></span> <span data-ttu-id="186f7-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="186f7-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="186f7-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="186f7-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="186f7-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="186f7-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="186f7-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="186f7-193">isAssigned</span></span>|<span data-ttu-id="186f7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="186f7-194">Boolean</span></span>|<span data-ttu-id="186f7-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="186f7-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="186f7-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="186f7-197">roleScopeTagIds</span></span>|<span data-ttu-id="186f7-198">String collection</span><span class="sxs-lookup"><span data-stu-id="186f7-198">String collection</span></span>|<span data-ttu-id="186f7-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="186f7-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="186f7-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="186f7-201">dependentAppCount</span></span>|<span data-ttu-id="186f7-202">Int32</span><span class="sxs-lookup"><span data-stu-id="186f7-202">Int32</span></span>|<span data-ttu-id="186f7-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="186f7-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="186f7-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="186f7-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="186f7-205">committedContentVersion</span></span>|<span data-ttu-id="186f7-206">String</span><span class="sxs-lookup"><span data-stu-id="186f7-206">String</span></span>|<span data-ttu-id="186f7-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="186f7-207">The internal committed content version.</span></span> <span data-ttu-id="186f7-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="186f7-209">fileName</span><span class="sxs-lookup"><span data-stu-id="186f7-209">fileName</span></span>|<span data-ttu-id="186f7-210">String</span><span class="sxs-lookup"><span data-stu-id="186f7-210">String</span></span>|<span data-ttu-id="186f7-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="186f7-211">The name of the main Lob application file.</span></span> <span data-ttu-id="186f7-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="186f7-213">size</span><span class="sxs-lookup"><span data-stu-id="186f7-213">size</span></span>|<span data-ttu-id="186f7-214">Int64</span><span class="sxs-lookup"><span data-stu-id="186f7-214">Int64</span></span>|<span data-ttu-id="186f7-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="186f7-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="186f7-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="186f7-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="186f7-217">commandLine</span><span class="sxs-lookup"><span data-stu-id="186f7-217">commandLine</span></span>|<span data-ttu-id="186f7-218">String</span><span class="sxs-lookup"><span data-stu-id="186f7-218">String</span></span>|<span data-ttu-id="186f7-219">命令行。</span><span class="sxs-lookup"><span data-stu-id="186f7-219">The command line.</span></span>|
|<span data-ttu-id="186f7-220">productCode</span><span class="sxs-lookup"><span data-stu-id="186f7-220">productCode</span></span>|<span data-ttu-id="186f7-221">String</span><span class="sxs-lookup"><span data-stu-id="186f7-221">String</span></span>|<span data-ttu-id="186f7-222">产品代码。</span><span class="sxs-lookup"><span data-stu-id="186f7-222">The product code.</span></span>|
|<span data-ttu-id="186f7-223">productVersion</span><span class="sxs-lookup"><span data-stu-id="186f7-223">productVersion</span></span>|<span data-ttu-id="186f7-224">String</span><span class="sxs-lookup"><span data-stu-id="186f7-224">String</span></span>|<span data-ttu-id="186f7-225">Windows Mobile MSI 业务线 (LoB) 应用的产品版本。</span><span class="sxs-lookup"><span data-stu-id="186f7-225">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="186f7-226">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="186f7-226">ignoreVersionDetection</span></span>|<span data-ttu-id="186f7-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="186f7-227">Boolean</span></span>|<span data-ttu-id="186f7-228">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="186f7-228">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="186f7-229">对于使用自更新功能的 Windows Mobile MSI 业务线 (LoB) 应用，将此值设置为 true。</span><span class="sxs-lookup"><span data-stu-id="186f7-229">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="186f7-230">identityVersion</span><span class="sxs-lookup"><span data-stu-id="186f7-230">identityVersion</span></span>|<span data-ttu-id="186f7-231">String</span><span class="sxs-lookup"><span data-stu-id="186f7-231">String</span></span>|<span data-ttu-id="186f7-232">标识版本。</span><span class="sxs-lookup"><span data-stu-id="186f7-232">The identity version.</span></span>|
|<span data-ttu-id="186f7-233">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="186f7-233">useDeviceContext</span></span>|<span data-ttu-id="186f7-234">布尔值</span><span class="sxs-lookup"><span data-stu-id="186f7-234">Boolean</span></span>|<span data-ttu-id="186f7-235">指示是否在设备上下文中安装双模式 MSI。</span><span class="sxs-lookup"><span data-stu-id="186f7-235">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="186f7-236">如果为 true, 则将为所有用户安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="186f7-236">If true, app will be installed for all users.</span></span> <span data-ttu-id="186f7-237">如果为 false, 将按用户安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="186f7-237">If false, app will be installed per-user.</span></span> <span data-ttu-id="186f7-238">如果为 null, 服务将使用 MSI 包的默认安装上下文。</span><span class="sxs-lookup"><span data-stu-id="186f7-238">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="186f7-239">在双模式 MSI 的情况下, 此默认值将为每个用户。</span><span class="sxs-lookup"><span data-stu-id="186f7-239">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="186f7-240">不能为非双重模式的应用程序进行设置。</span><span class="sxs-lookup"><span data-stu-id="186f7-240">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="186f7-241">在首次创建应用程序后, 不能更改。</span><span class="sxs-lookup"><span data-stu-id="186f7-241">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="186f7-242">响应</span><span class="sxs-lookup"><span data-stu-id="186f7-242">Response</span></span>
<span data-ttu-id="186f7-243">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="186f7-243">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="186f7-244">示例</span><span class="sxs-lookup"><span data-stu-id="186f7-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="186f7-245">请求</span><span class="sxs-lookup"><span data-stu-id="186f7-245">Request</span></span>
<span data-ttu-id="186f7-246">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="186f7-246">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1066

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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="186f7-247">响应</span><span class="sxs-lookup"><span data-stu-id="186f7-247">Response</span></span>
<span data-ttu-id="186f7-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="186f7-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1238

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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```




