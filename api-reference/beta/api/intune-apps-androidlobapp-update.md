---
title: 更新 androidLobApp
description: 更新 androidLobApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f2cc9177d374e7720821b9195a8b4d40bf2cf55
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784598"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="490e7-103">更新 androidLobApp</span><span class="sxs-lookup"><span data-stu-id="490e7-103">Update androidLobApp</span></span>

> <span data-ttu-id="490e7-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="490e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="490e7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="490e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="490e7-106">更新 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="490e7-106">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="490e7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="490e7-107">Prerequisites</span></span>
<span data-ttu-id="490e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="490e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="490e7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="490e7-110">Permission type</span></span>|<span data-ttu-id="490e7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="490e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="490e7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="490e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="490e7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="490e7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="490e7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="490e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="490e7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="490e7-115">Not supported.</span></span>|
|<span data-ttu-id="490e7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="490e7-116">Application</span></span>|<span data-ttu-id="490e7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="490e7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="490e7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="490e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="490e7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="490e7-119">Request headers</span></span>
|<span data-ttu-id="490e7-120">标头</span><span class="sxs-lookup"><span data-stu-id="490e7-120">Header</span></span>|<span data-ttu-id="490e7-121">值</span><span class="sxs-lookup"><span data-stu-id="490e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="490e7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="490e7-122">Authorization</span></span>|<span data-ttu-id="490e7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="490e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="490e7-124">接受</span><span class="sxs-lookup"><span data-stu-id="490e7-124">Accept</span></span>|<span data-ttu-id="490e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="490e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="490e7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="490e7-126">Request body</span></span>
<span data-ttu-id="490e7-127">在请求正文中，提供 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="490e7-127">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="490e7-128">下表显示了创建 [androidLobApp](../resources/intune-apps-androidlobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="490e7-128">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="490e7-129">属性</span><span class="sxs-lookup"><span data-stu-id="490e7-129">Property</span></span>|<span data-ttu-id="490e7-130">类型</span><span class="sxs-lookup"><span data-stu-id="490e7-130">Type</span></span>|<span data-ttu-id="490e7-131">说明</span><span class="sxs-lookup"><span data-stu-id="490e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="490e7-132">id</span><span class="sxs-lookup"><span data-stu-id="490e7-132">id</span></span>|<span data-ttu-id="490e7-133">String</span><span class="sxs-lookup"><span data-stu-id="490e7-133">String</span></span>|<span data-ttu-id="490e7-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="490e7-134">Key of the entity.</span></span> <span data-ttu-id="490e7-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="490e7-136">displayName</span></span>|<span data-ttu-id="490e7-137">String</span><span class="sxs-lookup"><span data-stu-id="490e7-137">String</span></span>|<span data-ttu-id="490e7-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="490e7-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="490e7-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-140">description</span><span class="sxs-lookup"><span data-stu-id="490e7-140">description</span></span>|<span data-ttu-id="490e7-141">String</span><span class="sxs-lookup"><span data-stu-id="490e7-141">String</span></span>|<span data-ttu-id="490e7-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="490e7-142">The description of the app.</span></span> <span data-ttu-id="490e7-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-144">publisher</span><span class="sxs-lookup"><span data-stu-id="490e7-144">publisher</span></span>|<span data-ttu-id="490e7-145">String</span><span class="sxs-lookup"><span data-stu-id="490e7-145">String</span></span>|<span data-ttu-id="490e7-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="490e7-146">The publisher of the app.</span></span> <span data-ttu-id="490e7-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="490e7-148">largeIcon</span></span>|[<span data-ttu-id="490e7-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="490e7-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="490e7-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="490e7-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="490e7-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="490e7-152">createdDateTime</span></span>|<span data-ttu-id="490e7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="490e7-153">DateTimeOffset</span></span>|<span data-ttu-id="490e7-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="490e7-154">The date and time the app was created.</span></span> <span data-ttu-id="490e7-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="490e7-156">lastModifiedDateTime</span></span>|<span data-ttu-id="490e7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="490e7-157">DateTimeOffset</span></span>|<span data-ttu-id="490e7-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="490e7-158">The date and time the app was last modified.</span></span> <span data-ttu-id="490e7-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="490e7-160">isFeatured</span></span>|<span data-ttu-id="490e7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="490e7-161">Boolean</span></span>|<span data-ttu-id="490e7-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="490e7-163">privacyInformationUrl</span></span>|<span data-ttu-id="490e7-164">String</span><span class="sxs-lookup"><span data-stu-id="490e7-164">String</span></span>|<span data-ttu-id="490e7-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="490e7-165">The privacy statement Url.</span></span> <span data-ttu-id="490e7-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="490e7-167">informationUrl</span></span>|<span data-ttu-id="490e7-168">String</span><span class="sxs-lookup"><span data-stu-id="490e7-168">String</span></span>|<span data-ttu-id="490e7-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="490e7-169">The more information Url.</span></span> <span data-ttu-id="490e7-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-171">owner</span><span class="sxs-lookup"><span data-stu-id="490e7-171">owner</span></span>|<span data-ttu-id="490e7-172">字符串</span><span class="sxs-lookup"><span data-stu-id="490e7-172">String</span></span>|<span data-ttu-id="490e7-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="490e7-173">The owner of the app.</span></span> <span data-ttu-id="490e7-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-175">developer</span><span class="sxs-lookup"><span data-stu-id="490e7-175">developer</span></span>|<span data-ttu-id="490e7-176">String</span><span class="sxs-lookup"><span data-stu-id="490e7-176">String</span></span>|<span data-ttu-id="490e7-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="490e7-177">The developer of the app.</span></span> <span data-ttu-id="490e7-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-179">notes</span><span class="sxs-lookup"><span data-stu-id="490e7-179">notes</span></span>|<span data-ttu-id="490e7-180">String</span><span class="sxs-lookup"><span data-stu-id="490e7-180">String</span></span>|<span data-ttu-id="490e7-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="490e7-181">Notes for the app.</span></span> <span data-ttu-id="490e7-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="490e7-183">uploadState</span></span>|<span data-ttu-id="490e7-184">Int32</span><span class="sxs-lookup"><span data-stu-id="490e7-184">Int32</span></span>|<span data-ttu-id="490e7-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="490e7-185">The upload state.</span></span> <span data-ttu-id="490e7-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="490e7-187">publishingState</span></span>|[<span data-ttu-id="490e7-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="490e7-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="490e7-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="490e7-189">The publishing state for the app.</span></span> <span data-ttu-id="490e7-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="490e7-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="490e7-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="490e7-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="490e7-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="490e7-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="490e7-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="490e7-193">isAssigned</span></span>|<span data-ttu-id="490e7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="490e7-194">Boolean</span></span>|<span data-ttu-id="490e7-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="490e7-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="490e7-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="490e7-197">roleScopeTagIds</span></span>|<span data-ttu-id="490e7-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="490e7-198">String collection</span></span>|<span data-ttu-id="490e7-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="490e7-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="490e7-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="490e7-201">dependentAppCount</span></span>|<span data-ttu-id="490e7-202">Int32</span><span class="sxs-lookup"><span data-stu-id="490e7-202">Int32</span></span>|<span data-ttu-id="490e7-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="490e7-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="490e7-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="490e7-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="490e7-205">committedContentVersion</span></span>|<span data-ttu-id="490e7-206">String</span><span class="sxs-lookup"><span data-stu-id="490e7-206">String</span></span>|<span data-ttu-id="490e7-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="490e7-207">The internal committed content version.</span></span> <span data-ttu-id="490e7-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="490e7-209">fileName</span><span class="sxs-lookup"><span data-stu-id="490e7-209">fileName</span></span>|<span data-ttu-id="490e7-210">String</span><span class="sxs-lookup"><span data-stu-id="490e7-210">String</span></span>|<span data-ttu-id="490e7-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="490e7-211">The name of the main Lob application file.</span></span> <span data-ttu-id="490e7-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="490e7-213">size</span><span class="sxs-lookup"><span data-stu-id="490e7-213">size</span></span>|<span data-ttu-id="490e7-214">Int64</span><span class="sxs-lookup"><span data-stu-id="490e7-214">Int64</span></span>|<span data-ttu-id="490e7-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="490e7-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="490e7-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="490e7-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="490e7-217">packageId</span><span class="sxs-lookup"><span data-stu-id="490e7-217">packageId</span></span>|<span data-ttu-id="490e7-218">String</span><span class="sxs-lookup"><span data-stu-id="490e7-218">String</span></span>|<span data-ttu-id="490e7-219">包标识符。</span><span class="sxs-lookup"><span data-stu-id="490e7-219">The package identifier.</span></span>|
|<span data-ttu-id="490e7-220">identityName</span><span class="sxs-lookup"><span data-stu-id="490e7-220">identityName</span></span>|<span data-ttu-id="490e7-221">String</span><span class="sxs-lookup"><span data-stu-id="490e7-221">String</span></span>|<span data-ttu-id="490e7-222">标识名称。</span><span class="sxs-lookup"><span data-stu-id="490e7-222">The Identity Name.</span></span>|
|<span data-ttu-id="490e7-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="490e7-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="490e7-224">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="490e7-224">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="490e7-225">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="490e7-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="490e7-226">versionName</span><span class="sxs-lookup"><span data-stu-id="490e7-226">versionName</span></span>|<span data-ttu-id="490e7-227">String</span><span class="sxs-lookup"><span data-stu-id="490e7-227">String</span></span>|<span data-ttu-id="490e7-228">Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="490e7-228">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="490e7-229">versionCode</span><span class="sxs-lookup"><span data-stu-id="490e7-229">versionCode</span></span>|<span data-ttu-id="490e7-230">String</span><span class="sxs-lookup"><span data-stu-id="490e7-230">String</span></span>|<span data-ttu-id="490e7-231">Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="490e7-231">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="490e7-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="490e7-232">identityVersion</span></span>|<span data-ttu-id="490e7-233">String</span><span class="sxs-lookup"><span data-stu-id="490e7-233">String</span></span>|<span data-ttu-id="490e7-234">标识版本。</span><span class="sxs-lookup"><span data-stu-id="490e7-234">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="490e7-235">响应</span><span class="sxs-lookup"><span data-stu-id="490e7-235">Response</span></span>
<span data-ttu-id="490e7-236">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidLobApp](../resources/intune-apps-androidlobapp.md)  对象。</span><span class="sxs-lookup"><span data-stu-id="490e7-236">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="490e7-237">示例</span><span class="sxs-lookup"><span data-stu-id="490e7-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="490e7-238">请求</span><span class="sxs-lookup"><span data-stu-id="490e7-238">Request</span></span>
<span data-ttu-id="490e7-239">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="490e7-239">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="490e7-240">响应</span><span class="sxs-lookup"><span data-stu-id="490e7-240">Response</span></span>
<span data-ttu-id="490e7-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="490e7-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





