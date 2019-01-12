---
title: 创建 macOSLobApp
description: 创建新的 macOSLobApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4a7b3b0a6bfc9a201ba274ab66a83932f760a809
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931676"
---
# <a name="create-macoslobapp"></a><span data-ttu-id="ea179-103">创建 macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="ea179-103">Create macOSLobApp</span></span>

> <span data-ttu-id="ea179-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ea179-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea179-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ea179-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea179-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ea179-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea179-107">创建新的[macOSLobApp](../resources/intune-apps-macoslobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ea179-107">Create a new [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea179-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ea179-108">Prerequisites</span></span>
<span data-ttu-id="ea179-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ea179-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea179-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea179-111">Permission type</span></span>|<span data-ttu-id="ea179-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ea179-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea179-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea179-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ea179-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea179-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ea179-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea179-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea179-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea179-116">Not supported.</span></span>|
|<span data-ttu-id="ea179-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea179-117">Application</span></span>|<span data-ttu-id="ea179-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea179-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea179-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea179-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ea179-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea179-120">Request headers</span></span>
|<span data-ttu-id="ea179-121">标头</span><span class="sxs-lookup"><span data-stu-id="ea179-121">Header</span></span>|<span data-ttu-id="ea179-122">值</span><span class="sxs-lookup"><span data-stu-id="ea179-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea179-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea179-123">Authorization</span></span>|<span data-ttu-id="ea179-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ea179-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea179-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ea179-125">Accept</span></span>|<span data-ttu-id="ea179-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ea179-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea179-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea179-127">Request body</span></span>
<span data-ttu-id="ea179-128">在请求正文中，提供 macOSLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea179-128">In the request body, supply a JSON representation for the macOSLobApp object.</span></span>

<span data-ttu-id="ea179-129">下表显示时创建 macOSLobApp 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ea179-129">The following table shows the properties that are required when you create the macOSLobApp.</span></span>

|<span data-ttu-id="ea179-130">属性</span><span class="sxs-lookup"><span data-stu-id="ea179-130">Property</span></span>|<span data-ttu-id="ea179-131">类型</span><span class="sxs-lookup"><span data-stu-id="ea179-131">Type</span></span>|<span data-ttu-id="ea179-132">说明</span><span class="sxs-lookup"><span data-stu-id="ea179-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea179-133">id</span><span class="sxs-lookup"><span data-stu-id="ea179-133">id</span></span>|<span data-ttu-id="ea179-134">String</span><span class="sxs-lookup"><span data-stu-id="ea179-134">String</span></span>|<span data-ttu-id="ea179-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ea179-135">Key of the entity.</span></span> <span data-ttu-id="ea179-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea179-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ea179-137">displayName</span></span>|<span data-ttu-id="ea179-138">String</span><span class="sxs-lookup"><span data-stu-id="ea179-138">String</span></span>|<span data-ttu-id="ea179-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="ea179-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ea179-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea179-141">description</span><span class="sxs-lookup"><span data-stu-id="ea179-141">description</span></span>|<span data-ttu-id="ea179-142">String</span><span class="sxs-lookup"><span data-stu-id="ea179-142">String</span></span>|<span data-ttu-id="ea179-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="ea179-143">The description of the app.</span></span> <span data-ttu-id="ea179-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea179-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ea179-145">publisher</span></span>|<span data-ttu-id="ea179-146">String</span><span class="sxs-lookup"><span data-stu-id="ea179-146">String</span></span>|<span data-ttu-id="ea179-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="ea179-147">The publisher of the app.</span></span> <span data-ttu-id="ea179-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea179-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ea179-149">largeIcon</span></span>|[<span data-ttu-id="ea179-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ea179-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ea179-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="ea179-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ea179-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea179-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea179-153">createdDateTime</span></span>|<span data-ttu-id="ea179-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea179-154">DateTimeOffset</span></span>|<span data-ttu-id="ea179-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ea179-155">The date and time the app was created.</span></span> <span data-ttu-id="ea179-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea179-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea179-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ea179-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea179-158">DateTimeOffset</span></span>|<span data-ttu-id="ea179-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ea179-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ea179-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea179-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ea179-161">isFeatured</span></span>|<span data-ttu-id="ea179-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea179-162">Boolean</span></span>|<span data-ttu-id="ea179-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea179-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ea179-164">privacyInformationUrl</span></span>|<span data-ttu-id="ea179-165">String</span><span class="sxs-lookup"><span data-stu-id="ea179-165">String</span></span>|<span data-ttu-id="ea179-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="ea179-166">The privacy statement Url.</span></span> <span data-ttu-id="ea179-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea179-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ea179-168">informationUrl</span></span>|<span data-ttu-id="ea179-169">String</span><span class="sxs-lookup"><span data-stu-id="ea179-169">String</span></span>|<span data-ttu-id="ea179-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="ea179-170">The more information Url.</span></span> <span data-ttu-id="ea179-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea179-172">owner</span><span class="sxs-lookup"><span data-stu-id="ea179-172">owner</span></span>|<span data-ttu-id="ea179-173">String</span><span class="sxs-lookup"><span data-stu-id="ea179-173">String</span></span>|<span data-ttu-id="ea179-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="ea179-174">The owner of the app.</span></span> <span data-ttu-id="ea179-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea179-176">developer</span><span class="sxs-lookup"><span data-stu-id="ea179-176">developer</span></span>|<span data-ttu-id="ea179-177">String</span><span class="sxs-lookup"><span data-stu-id="ea179-177">String</span></span>|<span data-ttu-id="ea179-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="ea179-178">The developer of the app.</span></span> <span data-ttu-id="ea179-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea179-180">notes</span><span class="sxs-lookup"><span data-stu-id="ea179-180">notes</span></span>|<span data-ttu-id="ea179-181">String</span><span class="sxs-lookup"><span data-stu-id="ea179-181">String</span></span>|<span data-ttu-id="ea179-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="ea179-182">Notes for the app.</span></span> <span data-ttu-id="ea179-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea179-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ea179-184">uploadState</span></span>|<span data-ttu-id="ea179-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ea179-185">Int32</span></span>|<span data-ttu-id="ea179-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="ea179-186">The upload state.</span></span> <span data-ttu-id="ea179-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ea179-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="ea179-188">publishingState</span></span>|[<span data-ttu-id="ea179-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ea179-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ea179-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="ea179-190">The publishing state for the app.</span></span> <span data-ttu-id="ea179-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="ea179-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ea179-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="ea179-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ea179-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="ea179-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ea179-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ea179-194">committedContentVersion</span></span>|<span data-ttu-id="ea179-195">String</span><span class="sxs-lookup"><span data-stu-id="ea179-195">String</span></span>|<span data-ttu-id="ea179-196">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="ea179-196">The internal committed content version.</span></span> <span data-ttu-id="ea179-197">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ea179-198">fileName</span><span class="sxs-lookup"><span data-stu-id="ea179-198">fileName</span></span>|<span data-ttu-id="ea179-199">String</span><span class="sxs-lookup"><span data-stu-id="ea179-199">String</span></span>|<span data-ttu-id="ea179-200">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="ea179-200">The name of the main Lob application file.</span></span> <span data-ttu-id="ea179-201">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ea179-202">size</span><span class="sxs-lookup"><span data-stu-id="ea179-202">size</span></span>|<span data-ttu-id="ea179-203">Int64</span><span class="sxs-lookup"><span data-stu-id="ea179-203">Int64</span></span>|<span data-ttu-id="ea179-204">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="ea179-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="ea179-205">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ea179-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ea179-206">bundleId</span><span class="sxs-lookup"><span data-stu-id="ea179-206">bundleId</span></span>|<span data-ttu-id="ea179-207">String</span><span class="sxs-lookup"><span data-stu-id="ea179-207">String</span></span>|<span data-ttu-id="ea179-208">绑定 id。</span><span class="sxs-lookup"><span data-stu-id="ea179-208">The bundle id.</span></span>|
|<span data-ttu-id="ea179-209">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ea179-209">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ea179-210">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ea179-210">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="ea179-211">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="ea179-211">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ea179-212">buildNumber</span><span class="sxs-lookup"><span data-stu-id="ea179-212">buildNumber</span></span>|<span data-ttu-id="ea179-213">String</span><span class="sxs-lookup"><span data-stu-id="ea179-213">String</span></span>|<span data-ttu-id="ea179-214">MacOS 行业务 (LoB) 应用程序的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="ea179-214">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ea179-215">versionNumber</span><span class="sxs-lookup"><span data-stu-id="ea179-215">versionNumber</span></span>|<span data-ttu-id="ea179-216">String</span><span class="sxs-lookup"><span data-stu-id="ea179-216">String</span></span>|<span data-ttu-id="ea179-217">MacOS 线 (LoB) 企业应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="ea179-217">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ea179-218">childApps</span><span class="sxs-lookup"><span data-stu-id="ea179-218">childApps</span></span>|<span data-ttu-id="ea179-219">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="ea179-219">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="ea179-220">此绑定程序包中应用程序列表</span><span class="sxs-lookup"><span data-stu-id="ea179-220">The app list in this bundle package</span></span>|
|<span data-ttu-id="ea179-221">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ea179-221">identityVersion</span></span>|<span data-ttu-id="ea179-222">String</span><span class="sxs-lookup"><span data-stu-id="ea179-222">String</span></span>|<span data-ttu-id="ea179-223">标识版本。</span><span class="sxs-lookup"><span data-stu-id="ea179-223">The identity version.</span></span>|
|<span data-ttu-id="ea179-224">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="ea179-224">md5HashChunkSize</span></span>|<span data-ttu-id="ea179-225">Int32</span><span class="sxs-lookup"><span data-stu-id="ea179-225">Int32</span></span>|<span data-ttu-id="ea179-226">MD5 哈希块区大小</span><span class="sxs-lookup"><span data-stu-id="ea179-226">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="ea179-227">md5Hash</span><span class="sxs-lookup"><span data-stu-id="ea179-227">md5Hash</span></span>|<span data-ttu-id="ea179-228">String 集合</span><span class="sxs-lookup"><span data-stu-id="ea179-228">String collection</span></span>|<span data-ttu-id="ea179-229">MD5 哈希代码</span><span class="sxs-lookup"><span data-stu-id="ea179-229">The MD5 hash codes</span></span>|
|<span data-ttu-id="ea179-230">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="ea179-230">ignoreVersionDetection</span></span>|<span data-ttu-id="ea179-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea179-231">Boolean</span></span>|<span data-ttu-id="ea179-232">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="ea179-232">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="ea179-233">将其设置为 true macOS 使用自我更新功能的业务线 (LoB) 应用程序。</span><span class="sxs-lookup"><span data-stu-id="ea179-233">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="ea179-234">响应</span><span class="sxs-lookup"><span data-stu-id="ea179-234">Response</span></span>
<span data-ttu-id="ea179-235">如果成功，此方法返回`201 Created`响应代码和响应正文中的[macOSLobApp](../resources/intune-apps-macoslobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ea179-235">If successful, this method returns a `201 Created` response code and a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea179-236">示例</span><span class="sxs-lookup"><span data-stu-id="ea179-236">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea179-237">请求</span><span class="sxs-lookup"><span data-stu-id="ea179-237">Request</span></span>
<span data-ttu-id="ea179-238">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea179-238">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1526

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="ea179-239">响应</span><span class="sxs-lookup"><span data-stu-id="ea179-239">Response</span></span>
<span data-ttu-id="ea179-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea179-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1634

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
  "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```





