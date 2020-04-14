---
title: 更新 win32LobApp
description: 更新 win32LobApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 60d20ea301f3553f041b55b5bce31856d81e5cdc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43393870"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="18cd5-103">更新 win32LobApp</span><span class="sxs-lookup"><span data-stu-id="18cd5-103">Update win32LobApp</span></span>

<span data-ttu-id="18cd5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18cd5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18cd5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="18cd5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18cd5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="18cd5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18cd5-107">更新[win32LobApp](../resources/intune-apps-win32lobapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="18cd5-107">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18cd5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="18cd5-108">Prerequisites</span></span>
<span data-ttu-id="18cd5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18cd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18cd5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="18cd5-111">Permission type</span></span>|<span data-ttu-id="18cd5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="18cd5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18cd5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18cd5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18cd5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18cd5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="18cd5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18cd5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18cd5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="18cd5-116">Not supported.</span></span>|
|<span data-ttu-id="18cd5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="18cd5-117">Application</span></span>|<span data-ttu-id="18cd5-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18cd5-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18cd5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18cd5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="18cd5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="18cd5-120">Request headers</span></span>
|<span data-ttu-id="18cd5-121">标头</span><span class="sxs-lookup"><span data-stu-id="18cd5-121">Header</span></span>|<span data-ttu-id="18cd5-122">值</span><span class="sxs-lookup"><span data-stu-id="18cd5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18cd5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18cd5-123">Authorization</span></span>|<span data-ttu-id="18cd5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="18cd5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18cd5-125">接受</span><span class="sxs-lookup"><span data-stu-id="18cd5-125">Accept</span></span>|<span data-ttu-id="18cd5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18cd5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18cd5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="18cd5-127">Request body</span></span>
<span data-ttu-id="18cd5-128">在请求正文中，提供[win32LobApp](../resources/intune-apps-win32lobapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18cd5-128">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="18cd5-129">下表显示创建[win32LobApp](../resources/intune-apps-win32lobapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="18cd5-129">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="18cd5-130">属性</span><span class="sxs-lookup"><span data-stu-id="18cd5-130">Property</span></span>|<span data-ttu-id="18cd5-131">类型</span><span class="sxs-lookup"><span data-stu-id="18cd5-131">Type</span></span>|<span data-ttu-id="18cd5-132">说明</span><span class="sxs-lookup"><span data-stu-id="18cd5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18cd5-133">id</span><span class="sxs-lookup"><span data-stu-id="18cd5-133">id</span></span>|<span data-ttu-id="18cd5-134">字符串</span><span class="sxs-lookup"><span data-stu-id="18cd5-134">String</span></span>|<span data-ttu-id="18cd5-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="18cd5-135">Key of the entity.</span></span> <span data-ttu-id="18cd5-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="18cd5-137">displayName</span></span>|<span data-ttu-id="18cd5-138">字符串</span><span class="sxs-lookup"><span data-stu-id="18cd5-138">String</span></span>|<span data-ttu-id="18cd5-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="18cd5-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="18cd5-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-141">description</span><span class="sxs-lookup"><span data-stu-id="18cd5-141">description</span></span>|<span data-ttu-id="18cd5-142">字符串</span><span class="sxs-lookup"><span data-stu-id="18cd5-142">String</span></span>|<span data-ttu-id="18cd5-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="18cd5-143">The description of the app.</span></span> <span data-ttu-id="18cd5-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-145">publisher</span><span class="sxs-lookup"><span data-stu-id="18cd5-145">publisher</span></span>|<span data-ttu-id="18cd5-146">字符串</span><span class="sxs-lookup"><span data-stu-id="18cd5-146">String</span></span>|<span data-ttu-id="18cd5-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="18cd5-147">The publisher of the app.</span></span> <span data-ttu-id="18cd5-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="18cd5-149">largeIcon</span></span>|[<span data-ttu-id="18cd5-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="18cd5-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="18cd5-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="18cd5-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="18cd5-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="18cd5-153">createdDateTime</span></span>|<span data-ttu-id="18cd5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18cd5-154">DateTimeOffset</span></span>|<span data-ttu-id="18cd5-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="18cd5-155">The date and time the app was created.</span></span> <span data-ttu-id="18cd5-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="18cd5-157">lastModifiedDateTime</span></span>|<span data-ttu-id="18cd5-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18cd5-158">DateTimeOffset</span></span>|<span data-ttu-id="18cd5-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="18cd5-159">The date and time the app was last modified.</span></span> <span data-ttu-id="18cd5-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="18cd5-161">isFeatured</span></span>|<span data-ttu-id="18cd5-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="18cd5-162">Boolean</span></span>|<span data-ttu-id="18cd5-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="18cd5-164">privacyInformationUrl</span></span>|<span data-ttu-id="18cd5-165">字符串</span><span class="sxs-lookup"><span data-stu-id="18cd5-165">String</span></span>|<span data-ttu-id="18cd5-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="18cd5-166">The privacy statement Url.</span></span> <span data-ttu-id="18cd5-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="18cd5-168">informationUrl</span></span>|<span data-ttu-id="18cd5-169">字符串</span><span class="sxs-lookup"><span data-stu-id="18cd5-169">String</span></span>|<span data-ttu-id="18cd5-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="18cd5-170">The more information Url.</span></span> <span data-ttu-id="18cd5-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-172">owner</span><span class="sxs-lookup"><span data-stu-id="18cd5-172">owner</span></span>|<span data-ttu-id="18cd5-173">String</span><span class="sxs-lookup"><span data-stu-id="18cd5-173">String</span></span>|<span data-ttu-id="18cd5-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="18cd5-174">The owner of the app.</span></span> <span data-ttu-id="18cd5-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-176">developer</span><span class="sxs-lookup"><span data-stu-id="18cd5-176">developer</span></span>|<span data-ttu-id="18cd5-177">字符串</span><span class="sxs-lookup"><span data-stu-id="18cd5-177">String</span></span>|<span data-ttu-id="18cd5-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="18cd5-178">The developer of the app.</span></span> <span data-ttu-id="18cd5-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-180">notes</span><span class="sxs-lookup"><span data-stu-id="18cd5-180">notes</span></span>|<span data-ttu-id="18cd5-181">字符串</span><span class="sxs-lookup"><span data-stu-id="18cd5-181">String</span></span>|<span data-ttu-id="18cd5-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="18cd5-182">Notes for the app.</span></span> <span data-ttu-id="18cd5-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="18cd5-184">uploadState</span></span>|<span data-ttu-id="18cd5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="18cd5-185">Int32</span></span>|<span data-ttu-id="18cd5-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="18cd5-186">The upload state.</span></span> <span data-ttu-id="18cd5-187">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="18cd5-188">publishingState</span></span>|[<span data-ttu-id="18cd5-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="18cd5-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="18cd5-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="18cd5-190">The publishing state for the app.</span></span> <span data-ttu-id="18cd5-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="18cd5-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="18cd5-192">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="18cd5-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="18cd5-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="18cd5-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="18cd5-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="18cd5-194">isAssigned</span></span>|<span data-ttu-id="18cd5-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="18cd5-195">Boolean</span></span>|<span data-ttu-id="18cd5-196">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="18cd5-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="18cd5-197">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="18cd5-198">roleScopeTagIds</span></span>|<span data-ttu-id="18cd5-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="18cd5-199">String collection</span></span>|<span data-ttu-id="18cd5-200">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="18cd5-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="18cd5-201">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="18cd5-202">dependentAppCount</span></span>|<span data-ttu-id="18cd5-203">Int32</span><span class="sxs-lookup"><span data-stu-id="18cd5-203">Int32</span></span>|<span data-ttu-id="18cd5-204">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="18cd5-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="18cd5-205">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="18cd5-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="18cd5-206">committedContentVersion</span></span>|<span data-ttu-id="18cd5-207">字符串</span><span class="sxs-lookup"><span data-stu-id="18cd5-207">String</span></span>|<span data-ttu-id="18cd5-208">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="18cd5-208">The internal committed content version.</span></span> <span data-ttu-id="18cd5-209">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="18cd5-210">fileName</span><span class="sxs-lookup"><span data-stu-id="18cd5-210">fileName</span></span>|<span data-ttu-id="18cd5-211">String</span><span class="sxs-lookup"><span data-stu-id="18cd5-211">String</span></span>|<span data-ttu-id="18cd5-212">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="18cd5-212">The name of the main Lob application file.</span></span> <span data-ttu-id="18cd5-213">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="18cd5-214">size</span><span class="sxs-lookup"><span data-stu-id="18cd5-214">size</span></span>|<span data-ttu-id="18cd5-215">Int64</span><span class="sxs-lookup"><span data-stu-id="18cd5-215">Int64</span></span>|<span data-ttu-id="18cd5-216">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="18cd5-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="18cd5-217">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="18cd5-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="18cd5-218">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="18cd5-218">installCommandLine</span></span>|<span data-ttu-id="18cd5-219">字符串</span><span class="sxs-lookup"><span data-stu-id="18cd5-219">String</span></span>|<span data-ttu-id="18cd5-220">要安装此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="18cd5-220">The command line to install this app</span></span>|
|<span data-ttu-id="18cd5-221">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="18cd5-221">uninstallCommandLine</span></span>|<span data-ttu-id="18cd5-222">字符串</span><span class="sxs-lookup"><span data-stu-id="18cd5-222">String</span></span>|<span data-ttu-id="18cd5-223">要卸载此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="18cd5-223">The command line to uninstall this app</span></span>|
|<span data-ttu-id="18cd5-224">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="18cd5-224">applicableArchitectures</span></span>|[<span data-ttu-id="18cd5-225">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="18cd5-225">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="18cd5-226">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="18cd5-226">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="18cd5-227">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="18cd5-227">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="18cd5-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="18cd5-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="18cd5-229">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="18cd5-229">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="18cd5-230">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="18cd5-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="18cd5-231">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="18cd5-231">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="18cd5-232">Int32</span><span class="sxs-lookup"><span data-stu-id="18cd5-232">Int32</span></span>|<span data-ttu-id="18cd5-233">安装此应用程序所需的最小可用磁盘空间的值。</span><span class="sxs-lookup"><span data-stu-id="18cd5-233">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="18cd5-234">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="18cd5-234">minimumMemoryInMB</span></span>|<span data-ttu-id="18cd5-235">Int32</span><span class="sxs-lookup"><span data-stu-id="18cd5-235">Int32</span></span>|<span data-ttu-id="18cd5-236">安装此应用程序所需的最小物理内存的值。</span><span class="sxs-lookup"><span data-stu-id="18cd5-236">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="18cd5-237">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="18cd5-237">minimumNumberOfProcessors</span></span>|<span data-ttu-id="18cd5-238">Int32</span><span class="sxs-lookup"><span data-stu-id="18cd5-238">Int32</span></span>|<span data-ttu-id="18cd5-239">安装此应用程序所需的最小处理器数的值。</span><span class="sxs-lookup"><span data-stu-id="18cd5-239">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="18cd5-240">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="18cd5-240">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="18cd5-241">Int32</span><span class="sxs-lookup"><span data-stu-id="18cd5-241">Int32</span></span>|<span data-ttu-id="18cd5-242">安装此应用程序所需的最低 CPU 速度的值。</span><span class="sxs-lookup"><span data-stu-id="18cd5-242">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="18cd5-243">detectionRules</span><span class="sxs-lookup"><span data-stu-id="18cd5-243">detectionRules</span></span>|<span data-ttu-id="18cd5-244">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)集合</span><span class="sxs-lookup"><span data-stu-id="18cd5-244">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="18cd5-245">检测到 Win32 业务线（LoB）应用程序的检测规则。</span><span class="sxs-lookup"><span data-stu-id="18cd5-245">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="18cd5-246">requirementRules</span><span class="sxs-lookup"><span data-stu-id="18cd5-246">requirementRules</span></span>|<span data-ttu-id="18cd5-247">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)集合</span><span class="sxs-lookup"><span data-stu-id="18cd5-247">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="18cd5-248">用于检测 Win32 业务线（LoB）应用程序的要求规则。</span><span class="sxs-lookup"><span data-stu-id="18cd5-248">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="18cd5-249">installExperience</span><span class="sxs-lookup"><span data-stu-id="18cd5-249">installExperience</span></span>|[<span data-ttu-id="18cd5-250">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="18cd5-250">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="18cd5-251">此应用的安装体验。</span><span class="sxs-lookup"><span data-stu-id="18cd5-251">The install experience for this app.</span></span>|
|<span data-ttu-id="18cd5-252">returnCodes</span><span class="sxs-lookup"><span data-stu-id="18cd5-252">returnCodes</span></span>|<span data-ttu-id="18cd5-253">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)集合</span><span class="sxs-lookup"><span data-stu-id="18cd5-253">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="18cd5-254">用于安装后行为的返回代码。</span><span class="sxs-lookup"><span data-stu-id="18cd5-254">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="18cd5-255">msiInformation</span><span class="sxs-lookup"><span data-stu-id="18cd5-255">msiInformation</span></span>|[<span data-ttu-id="18cd5-256">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="18cd5-256">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="18cd5-257">如果此 Win32 应用是 MSI 应用程序，则为 MSI 详细信息。</span><span class="sxs-lookup"><span data-stu-id="18cd5-257">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="18cd5-258">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="18cd5-258">setupFilePath</span></span>|<span data-ttu-id="18cd5-259">字符串</span><span class="sxs-lookup"><span data-stu-id="18cd5-259">String</span></span>|<span data-ttu-id="18cd5-260">加密的 Win32LobApp 包中的安装程序文件的相对路径。</span><span class="sxs-lookup"><span data-stu-id="18cd5-260">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="18cd5-261">installLanguage</span><span class="sxs-lookup"><span data-stu-id="18cd5-261">installLanguage</span></span>|<span data-ttu-id="18cd5-262">String</span><span class="sxs-lookup"><span data-stu-id="18cd5-262">String</span></span>|<span data-ttu-id="18cd5-263">尚未记录</span><span class="sxs-lookup"><span data-stu-id="18cd5-263">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="18cd5-264">响应</span><span class="sxs-lookup"><span data-stu-id="18cd5-264">Response</span></span>
<span data-ttu-id="18cd5-265">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[win32LobApp](../resources/intune-apps-win32lobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="18cd5-265">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18cd5-266">示例</span><span class="sxs-lookup"><span data-stu-id="18cd5-266">Example</span></span>

### <a name="request"></a><span data-ttu-id="18cd5-267">请求</span><span class="sxs-lookup"><span data-stu-id="18cd5-267">Request</span></span>
<span data-ttu-id="18cd5-268">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18cd5-268">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2865

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "installLanguage": "Install Language value"
}
```

### <a name="response"></a><span data-ttu-id="18cd5-269">响应</span><span class="sxs-lookup"><span data-stu-id="18cd5-269">Response</span></span>
<span data-ttu-id="18cd5-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="18cd5-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3037

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "installLanguage": "Install Language value"
}
```



