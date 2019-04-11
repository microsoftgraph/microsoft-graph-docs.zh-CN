---
title: 更新 iosLobApp
description: 更新 iosLobApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88e80c1aa29434d8cc7fad1319dca2f8da4d9f79
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780166"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="acfee-103">更新 iosLobApp</span><span class="sxs-lookup"><span data-stu-id="acfee-103">Update iosLobApp</span></span>

> <span data-ttu-id="acfee-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="acfee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="acfee-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="acfee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acfee-106">更新 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="acfee-106">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="acfee-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="acfee-107">Prerequisites</span></span>
<span data-ttu-id="acfee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="acfee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acfee-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="acfee-110">Permission type</span></span>|<span data-ttu-id="acfee-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="acfee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="acfee-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="acfee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="acfee-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acfee-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="acfee-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="acfee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="acfee-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="acfee-115">Not supported.</span></span>|
|<span data-ttu-id="acfee-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="acfee-116">Application</span></span>|<span data-ttu-id="acfee-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="acfee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="acfee-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="acfee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="acfee-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="acfee-119">Request headers</span></span>
|<span data-ttu-id="acfee-120">标头</span><span class="sxs-lookup"><span data-stu-id="acfee-120">Header</span></span>|<span data-ttu-id="acfee-121">值</span><span class="sxs-lookup"><span data-stu-id="acfee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="acfee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="acfee-122">Authorization</span></span>|<span data-ttu-id="acfee-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="acfee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="acfee-124">接受</span><span class="sxs-lookup"><span data-stu-id="acfee-124">Accept</span></span>|<span data-ttu-id="acfee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="acfee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="acfee-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="acfee-126">Request body</span></span>
<span data-ttu-id="acfee-127">在请求正文中，提供 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="acfee-127">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="acfee-128">下表显示了创建 [iosLobApp](../resources/intune-apps-ioslobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="acfee-128">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="acfee-129">属性</span><span class="sxs-lookup"><span data-stu-id="acfee-129">Property</span></span>|<span data-ttu-id="acfee-130">类型</span><span class="sxs-lookup"><span data-stu-id="acfee-130">Type</span></span>|<span data-ttu-id="acfee-131">说明</span><span class="sxs-lookup"><span data-stu-id="acfee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acfee-132">id</span><span class="sxs-lookup"><span data-stu-id="acfee-132">id</span></span>|<span data-ttu-id="acfee-133">String</span><span class="sxs-lookup"><span data-stu-id="acfee-133">String</span></span>|<span data-ttu-id="acfee-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="acfee-134">Key of the entity.</span></span> <span data-ttu-id="acfee-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-136">displayName</span><span class="sxs-lookup"><span data-stu-id="acfee-136">displayName</span></span>|<span data-ttu-id="acfee-137">String</span><span class="sxs-lookup"><span data-stu-id="acfee-137">String</span></span>|<span data-ttu-id="acfee-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="acfee-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="acfee-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-140">description</span><span class="sxs-lookup"><span data-stu-id="acfee-140">description</span></span>|<span data-ttu-id="acfee-141">String</span><span class="sxs-lookup"><span data-stu-id="acfee-141">String</span></span>|<span data-ttu-id="acfee-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="acfee-142">The description of the app.</span></span> <span data-ttu-id="acfee-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-144">publisher</span><span class="sxs-lookup"><span data-stu-id="acfee-144">publisher</span></span>|<span data-ttu-id="acfee-145">String</span><span class="sxs-lookup"><span data-stu-id="acfee-145">String</span></span>|<span data-ttu-id="acfee-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="acfee-146">The publisher of the app.</span></span> <span data-ttu-id="acfee-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="acfee-148">largeIcon</span></span>|[<span data-ttu-id="acfee-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="acfee-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="acfee-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="acfee-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="acfee-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="acfee-152">createdDateTime</span></span>|<span data-ttu-id="acfee-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acfee-153">DateTimeOffset</span></span>|<span data-ttu-id="acfee-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="acfee-154">The date and time the app was created.</span></span> <span data-ttu-id="acfee-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="acfee-156">lastModifiedDateTime</span></span>|<span data-ttu-id="acfee-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acfee-157">DateTimeOffset</span></span>|<span data-ttu-id="acfee-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="acfee-158">The date and time the app was last modified.</span></span> <span data-ttu-id="acfee-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="acfee-160">isFeatured</span></span>|<span data-ttu-id="acfee-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="acfee-161">Boolean</span></span>|<span data-ttu-id="acfee-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="acfee-163">privacyInformationUrl</span></span>|<span data-ttu-id="acfee-164">String</span><span class="sxs-lookup"><span data-stu-id="acfee-164">String</span></span>|<span data-ttu-id="acfee-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="acfee-165">The privacy statement Url.</span></span> <span data-ttu-id="acfee-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="acfee-167">informationUrl</span></span>|<span data-ttu-id="acfee-168">String</span><span class="sxs-lookup"><span data-stu-id="acfee-168">String</span></span>|<span data-ttu-id="acfee-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="acfee-169">The more information Url.</span></span> <span data-ttu-id="acfee-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-171">owner</span><span class="sxs-lookup"><span data-stu-id="acfee-171">owner</span></span>|<span data-ttu-id="acfee-172">字符串</span><span class="sxs-lookup"><span data-stu-id="acfee-172">String</span></span>|<span data-ttu-id="acfee-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="acfee-173">The owner of the app.</span></span> <span data-ttu-id="acfee-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-175">developer</span><span class="sxs-lookup"><span data-stu-id="acfee-175">developer</span></span>|<span data-ttu-id="acfee-176">String</span><span class="sxs-lookup"><span data-stu-id="acfee-176">String</span></span>|<span data-ttu-id="acfee-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="acfee-177">The developer of the app.</span></span> <span data-ttu-id="acfee-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-179">notes</span><span class="sxs-lookup"><span data-stu-id="acfee-179">notes</span></span>|<span data-ttu-id="acfee-180">String</span><span class="sxs-lookup"><span data-stu-id="acfee-180">String</span></span>|<span data-ttu-id="acfee-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="acfee-181">Notes for the app.</span></span> <span data-ttu-id="acfee-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="acfee-183">uploadState</span></span>|<span data-ttu-id="acfee-184">Int32</span><span class="sxs-lookup"><span data-stu-id="acfee-184">Int32</span></span>|<span data-ttu-id="acfee-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="acfee-185">The upload state.</span></span> <span data-ttu-id="acfee-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="acfee-187">publishingState</span></span>|[<span data-ttu-id="acfee-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="acfee-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="acfee-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="acfee-189">The publishing state for the app.</span></span> <span data-ttu-id="acfee-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="acfee-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="acfee-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="acfee-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="acfee-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="acfee-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="acfee-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="acfee-193">isAssigned</span></span>|<span data-ttu-id="acfee-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="acfee-194">Boolean</span></span>|<span data-ttu-id="acfee-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="acfee-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="acfee-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="acfee-197">roleScopeTagIds</span></span>|<span data-ttu-id="acfee-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="acfee-198">String collection</span></span>|<span data-ttu-id="acfee-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="acfee-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="acfee-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="acfee-201">dependentAppCount</span></span>|<span data-ttu-id="acfee-202">Int32</span><span class="sxs-lookup"><span data-stu-id="acfee-202">Int32</span></span>|<span data-ttu-id="acfee-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="acfee-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="acfee-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="acfee-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="acfee-205">committedContentVersion</span></span>|<span data-ttu-id="acfee-206">String</span><span class="sxs-lookup"><span data-stu-id="acfee-206">String</span></span>|<span data-ttu-id="acfee-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="acfee-207">The internal committed content version.</span></span> <span data-ttu-id="acfee-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="acfee-209">fileName</span><span class="sxs-lookup"><span data-stu-id="acfee-209">fileName</span></span>|<span data-ttu-id="acfee-210">String</span><span class="sxs-lookup"><span data-stu-id="acfee-210">String</span></span>|<span data-ttu-id="acfee-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="acfee-211">The name of the main Lob application file.</span></span> <span data-ttu-id="acfee-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="acfee-213">size</span><span class="sxs-lookup"><span data-stu-id="acfee-213">size</span></span>|<span data-ttu-id="acfee-214">Int64</span><span class="sxs-lookup"><span data-stu-id="acfee-214">Int64</span></span>|<span data-ttu-id="acfee-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="acfee-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="acfee-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="acfee-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="acfee-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="acfee-217">bundleId</span></span>|<span data-ttu-id="acfee-218">String</span><span class="sxs-lookup"><span data-stu-id="acfee-218">String</span></span>|<span data-ttu-id="acfee-219">标识名称。</span><span class="sxs-lookup"><span data-stu-id="acfee-219">The Identity Name.</span></span>|
|<span data-ttu-id="acfee-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="acfee-220">applicableDeviceType</span></span>|[<span data-ttu-id="acfee-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="acfee-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="acfee-222">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="acfee-222">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="acfee-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="acfee-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="acfee-224">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="acfee-224">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="acfee-225">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="acfee-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="acfee-226">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="acfee-226">expirationDateTime</span></span>|<span data-ttu-id="acfee-227">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="acfee-227">DateTimeOffset</span></span>|<span data-ttu-id="acfee-228">过期时间。</span><span class="sxs-lookup"><span data-stu-id="acfee-228">The expiration time.</span></span>|
|<span data-ttu-id="acfee-229">versionNumber</span><span class="sxs-lookup"><span data-stu-id="acfee-229">versionNumber</span></span>|<span data-ttu-id="acfee-230">String</span><span class="sxs-lookup"><span data-stu-id="acfee-230">String</span></span>|<span data-ttu-id="acfee-231">iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="acfee-231">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="acfee-232">buildNumber</span><span class="sxs-lookup"><span data-stu-id="acfee-232">buildNumber</span></span>|<span data-ttu-id="acfee-233">String</span><span class="sxs-lookup"><span data-stu-id="acfee-233">String</span></span>|<span data-ttu-id="acfee-234">iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="acfee-234">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="acfee-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="acfee-235">identityVersion</span></span>|<span data-ttu-id="acfee-236">String</span><span class="sxs-lookup"><span data-stu-id="acfee-236">String</span></span>|<span data-ttu-id="acfee-237">标识版本。</span><span class="sxs-lookup"><span data-stu-id="acfee-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="acfee-238">响应</span><span class="sxs-lookup"><span data-stu-id="acfee-238">Response</span></span>
<span data-ttu-id="acfee-239">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="acfee-239">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acfee-240">示例</span><span class="sxs-lookup"><span data-stu-id="acfee-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="acfee-241">请求</span><span class="sxs-lookup"><span data-stu-id="acfee-241">Request</span></span>
<span data-ttu-id="acfee-242">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="acfee-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="acfee-243">响应</span><span class="sxs-lookup"><span data-stu-id="acfee-243">Response</span></span>
<span data-ttu-id="acfee-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="acfee-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





