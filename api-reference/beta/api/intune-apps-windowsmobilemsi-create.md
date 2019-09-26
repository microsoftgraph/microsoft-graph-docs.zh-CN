---
title: 创建 windowsMobileMSI
description: 创建新的 windowsMobileMSI 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4438023f5041047c5947e0d75ade657d7c67231c
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37171972"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="bb266-103">创建 windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="bb266-103">Create windowsMobileMSI</span></span>

> <span data-ttu-id="bb266-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb266-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb266-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb266-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb266-106">创建新的 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb266-106">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb266-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bb266-107">Prerequisites</span></span>
<span data-ttu-id="bb266-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb266-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb266-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb266-110">Permission type</span></span>|<span data-ttu-id="bb266-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bb266-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb266-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb266-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb266-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb266-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bb266-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb266-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb266-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb266-115">Not supported.</span></span>|
|<span data-ttu-id="bb266-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb266-116">Application</span></span>|<span data-ttu-id="bb266-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb266-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb266-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb266-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bb266-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb266-119">Request headers</span></span>
|<span data-ttu-id="bb266-120">标头</span><span class="sxs-lookup"><span data-stu-id="bb266-120">Header</span></span>|<span data-ttu-id="bb266-121">值</span><span class="sxs-lookup"><span data-stu-id="bb266-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb266-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb266-122">Authorization</span></span>|<span data-ttu-id="bb266-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bb266-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb266-124">接受</span><span class="sxs-lookup"><span data-stu-id="bb266-124">Accept</span></span>|<span data-ttu-id="bb266-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb266-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb266-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb266-126">Request body</span></span>
<span data-ttu-id="bb266-127">在请求正文中，提供 windowsMobileMSI 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb266-127">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="bb266-128">下表显示创建 windowsMobileMSI 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bb266-128">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="bb266-129">属性</span><span class="sxs-lookup"><span data-stu-id="bb266-129">Property</span></span>|<span data-ttu-id="bb266-130">类型</span><span class="sxs-lookup"><span data-stu-id="bb266-130">Type</span></span>|<span data-ttu-id="bb266-131">说明</span><span class="sxs-lookup"><span data-stu-id="bb266-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb266-132">id</span><span class="sxs-lookup"><span data-stu-id="bb266-132">id</span></span>|<span data-ttu-id="bb266-133">字符串</span><span class="sxs-lookup"><span data-stu-id="bb266-133">String</span></span>|<span data-ttu-id="bb266-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bb266-134">Key of the entity.</span></span> <span data-ttu-id="bb266-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bb266-136">displayName</span></span>|<span data-ttu-id="bb266-137">String</span><span class="sxs-lookup"><span data-stu-id="bb266-137">String</span></span>|<span data-ttu-id="bb266-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="bb266-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bb266-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-140">说明</span><span class="sxs-lookup"><span data-stu-id="bb266-140">description</span></span>|<span data-ttu-id="bb266-141">字符串</span><span class="sxs-lookup"><span data-stu-id="bb266-141">String</span></span>|<span data-ttu-id="bb266-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="bb266-142">The description of the app.</span></span> <span data-ttu-id="bb266-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-144">publisher</span><span class="sxs-lookup"><span data-stu-id="bb266-144">publisher</span></span>|<span data-ttu-id="bb266-145">String</span><span class="sxs-lookup"><span data-stu-id="bb266-145">String</span></span>|<span data-ttu-id="bb266-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="bb266-146">The publisher of the app.</span></span> <span data-ttu-id="bb266-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bb266-148">largeIcon</span></span>|[<span data-ttu-id="bb266-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bb266-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bb266-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="bb266-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bb266-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb266-152">createdDateTime</span></span>|<span data-ttu-id="bb266-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb266-153">DateTimeOffset</span></span>|<span data-ttu-id="bb266-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bb266-154">The date and time the app was created.</span></span> <span data-ttu-id="bb266-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb266-156">lastModifiedDateTime</span></span>|<span data-ttu-id="bb266-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb266-157">DateTimeOffset</span></span>|<span data-ttu-id="bb266-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bb266-158">The date and time the app was last modified.</span></span> <span data-ttu-id="bb266-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bb266-160">isFeatured</span></span>|<span data-ttu-id="bb266-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb266-161">Boolean</span></span>|<span data-ttu-id="bb266-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bb266-163">privacyInformationUrl</span></span>|<span data-ttu-id="bb266-164">String</span><span class="sxs-lookup"><span data-stu-id="bb266-164">String</span></span>|<span data-ttu-id="bb266-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="bb266-165">The privacy statement Url.</span></span> <span data-ttu-id="bb266-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bb266-167">informationUrl</span></span>|<span data-ttu-id="bb266-168">String</span><span class="sxs-lookup"><span data-stu-id="bb266-168">String</span></span>|<span data-ttu-id="bb266-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="bb266-169">The more information Url.</span></span> <span data-ttu-id="bb266-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-171">owner</span><span class="sxs-lookup"><span data-stu-id="bb266-171">owner</span></span>|<span data-ttu-id="bb266-172">String</span><span class="sxs-lookup"><span data-stu-id="bb266-172">String</span></span>|<span data-ttu-id="bb266-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="bb266-173">The owner of the app.</span></span> <span data-ttu-id="bb266-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-175">developer</span><span class="sxs-lookup"><span data-stu-id="bb266-175">developer</span></span>|<span data-ttu-id="bb266-176">String</span><span class="sxs-lookup"><span data-stu-id="bb266-176">String</span></span>|<span data-ttu-id="bb266-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="bb266-177">The developer of the app.</span></span> <span data-ttu-id="bb266-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-179">notes</span><span class="sxs-lookup"><span data-stu-id="bb266-179">notes</span></span>|<span data-ttu-id="bb266-180">String</span><span class="sxs-lookup"><span data-stu-id="bb266-180">String</span></span>|<span data-ttu-id="bb266-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="bb266-181">Notes for the app.</span></span> <span data-ttu-id="bb266-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="bb266-183">uploadState</span></span>|<span data-ttu-id="bb266-184">Int32</span><span class="sxs-lookup"><span data-stu-id="bb266-184">Int32</span></span>|<span data-ttu-id="bb266-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="bb266-185">The upload state.</span></span> <span data-ttu-id="bb266-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="bb266-187">publishingState</span></span>|[<span data-ttu-id="bb266-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bb266-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bb266-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="bb266-189">The publishing state for the app.</span></span> <span data-ttu-id="bb266-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="bb266-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bb266-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="bb266-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="bb266-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="bb266-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bb266-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bb266-193">isAssigned</span></span>|<span data-ttu-id="bb266-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb266-194">Boolean</span></span>|<span data-ttu-id="bb266-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="bb266-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="bb266-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bb266-197">roleScopeTagIds</span></span>|<span data-ttu-id="bb266-198">String collection</span><span class="sxs-lookup"><span data-stu-id="bb266-198">String collection</span></span>|<span data-ttu-id="bb266-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="bb266-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="bb266-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="bb266-201">dependentAppCount</span></span>|<span data-ttu-id="bb266-202">Int32</span><span class="sxs-lookup"><span data-stu-id="bb266-202">Int32</span></span>|<span data-ttu-id="bb266-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="bb266-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="bb266-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bb266-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="bb266-205">committedContentVersion</span></span>|<span data-ttu-id="bb266-206">String</span><span class="sxs-lookup"><span data-stu-id="bb266-206">String</span></span>|<span data-ttu-id="bb266-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="bb266-207">The internal committed content version.</span></span> <span data-ttu-id="bb266-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bb266-209">fileName</span><span class="sxs-lookup"><span data-stu-id="bb266-209">fileName</span></span>|<span data-ttu-id="bb266-210">String</span><span class="sxs-lookup"><span data-stu-id="bb266-210">String</span></span>|<span data-ttu-id="bb266-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="bb266-211">The name of the main Lob application file.</span></span> <span data-ttu-id="bb266-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bb266-213">size</span><span class="sxs-lookup"><span data-stu-id="bb266-213">size</span></span>|<span data-ttu-id="bb266-214">Int64</span><span class="sxs-lookup"><span data-stu-id="bb266-214">Int64</span></span>|<span data-ttu-id="bb266-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="bb266-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="bb266-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb266-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bb266-217">commandLine</span><span class="sxs-lookup"><span data-stu-id="bb266-217">commandLine</span></span>|<span data-ttu-id="bb266-218">String</span><span class="sxs-lookup"><span data-stu-id="bb266-218">String</span></span>|<span data-ttu-id="bb266-219">命令行。</span><span class="sxs-lookup"><span data-stu-id="bb266-219">The command line.</span></span>|
|<span data-ttu-id="bb266-220">productCode</span><span class="sxs-lookup"><span data-stu-id="bb266-220">productCode</span></span>|<span data-ttu-id="bb266-221">String</span><span class="sxs-lookup"><span data-stu-id="bb266-221">String</span></span>|<span data-ttu-id="bb266-222">产品代码。</span><span class="sxs-lookup"><span data-stu-id="bb266-222">The product code.</span></span>|
|<span data-ttu-id="bb266-223">productVersion</span><span class="sxs-lookup"><span data-stu-id="bb266-223">productVersion</span></span>|<span data-ttu-id="bb266-224">String</span><span class="sxs-lookup"><span data-stu-id="bb266-224">String</span></span>|<span data-ttu-id="bb266-225">Windows Mobile MSI 业务线 (LoB) 应用的产品版本。</span><span class="sxs-lookup"><span data-stu-id="bb266-225">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="bb266-226">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="bb266-226">ignoreVersionDetection</span></span>|<span data-ttu-id="bb266-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb266-227">Boolean</span></span>|<span data-ttu-id="bb266-228">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="bb266-228">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="bb266-229">对于使用自更新功能的 Windows Mobile MSI 业务线 (LoB) 应用，将此值设置为 true。</span><span class="sxs-lookup"><span data-stu-id="bb266-229">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="bb266-230">identityVersion</span><span class="sxs-lookup"><span data-stu-id="bb266-230">identityVersion</span></span>|<span data-ttu-id="bb266-231">String</span><span class="sxs-lookup"><span data-stu-id="bb266-231">String</span></span>|<span data-ttu-id="bb266-232">标识版本。</span><span class="sxs-lookup"><span data-stu-id="bb266-232">The identity version.</span></span>|
|<span data-ttu-id="bb266-233">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="bb266-233">useDeviceContext</span></span>|<span data-ttu-id="bb266-234">布尔值</span><span class="sxs-lookup"><span data-stu-id="bb266-234">Boolean</span></span>|<span data-ttu-id="bb266-235">指示是否在设备上下文中安装双模式 MSI。</span><span class="sxs-lookup"><span data-stu-id="bb266-235">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="bb266-236">如果为 true，则将为所有用户安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="bb266-236">If true, app will be installed for all users.</span></span> <span data-ttu-id="bb266-237">如果为 false，将按用户安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="bb266-237">If false, app will be installed per-user.</span></span> <span data-ttu-id="bb266-238">如果为 null，服务将使用 MSI 包的默认安装上下文。</span><span class="sxs-lookup"><span data-stu-id="bb266-238">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="bb266-239">在双模式 MSI 的情况下，此默认值将为每个用户。</span><span class="sxs-lookup"><span data-stu-id="bb266-239">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="bb266-240">不能为非双重模式的应用程序进行设置。</span><span class="sxs-lookup"><span data-stu-id="bb266-240">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="bb266-241">在首次创建应用程序后，不能更改。</span><span class="sxs-lookup"><span data-stu-id="bb266-241">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="bb266-242">响应</span><span class="sxs-lookup"><span data-stu-id="bb266-242">Response</span></span>
<span data-ttu-id="bb266-243">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb266-243">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb266-244">示例</span><span class="sxs-lookup"><span data-stu-id="bb266-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb266-245">请求</span><span class="sxs-lookup"><span data-stu-id="bb266-245">Request</span></span>
<span data-ttu-id="bb266-246">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb266-246">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="bb266-247">响应</span><span class="sxs-lookup"><span data-stu-id="bb266-247">Response</span></span>
<span data-ttu-id="bb266-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb266-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




