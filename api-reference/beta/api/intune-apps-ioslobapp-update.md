---
title: 更新 iosLobApp
description: 更新 iosLobApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46d6aa0294375f0e2074b50dee45f2a5be267d75
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986500"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="75a47-103">更新 iosLobApp</span><span class="sxs-lookup"><span data-stu-id="75a47-103">Update iosLobApp</span></span>

> <span data-ttu-id="75a47-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="75a47-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75a47-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="75a47-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75a47-106">更新 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="75a47-106">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75a47-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="75a47-107">Prerequisites</span></span>
<span data-ttu-id="75a47-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="75a47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75a47-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="75a47-110">Permission type</span></span>|<span data-ttu-id="75a47-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="75a47-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75a47-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="75a47-112">Delegated (work or school account)</span></span>|<span data-ttu-id="75a47-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="75a47-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="75a47-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="75a47-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75a47-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="75a47-115">Not supported.</span></span>|
|<span data-ttu-id="75a47-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="75a47-116">Application</span></span>|<span data-ttu-id="75a47-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="75a47-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75a47-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="75a47-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="75a47-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="75a47-119">Request headers</span></span>
|<span data-ttu-id="75a47-120">标头</span><span class="sxs-lookup"><span data-stu-id="75a47-120">Header</span></span>|<span data-ttu-id="75a47-121">值</span><span class="sxs-lookup"><span data-stu-id="75a47-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75a47-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="75a47-122">Authorization</span></span>|<span data-ttu-id="75a47-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="75a47-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75a47-124">接受</span><span class="sxs-lookup"><span data-stu-id="75a47-124">Accept</span></span>|<span data-ttu-id="75a47-125">application/json</span><span class="sxs-lookup"><span data-stu-id="75a47-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75a47-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="75a47-126">Request body</span></span>
<span data-ttu-id="75a47-127">在请求正文中，提供 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75a47-127">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="75a47-128">下表显示了创建 [iosLobApp](../resources/intune-apps-ioslobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="75a47-128">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="75a47-129">属性</span><span class="sxs-lookup"><span data-stu-id="75a47-129">Property</span></span>|<span data-ttu-id="75a47-130">类型</span><span class="sxs-lookup"><span data-stu-id="75a47-130">Type</span></span>|<span data-ttu-id="75a47-131">说明</span><span class="sxs-lookup"><span data-stu-id="75a47-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75a47-132">id</span><span class="sxs-lookup"><span data-stu-id="75a47-132">id</span></span>|<span data-ttu-id="75a47-133">String</span><span class="sxs-lookup"><span data-stu-id="75a47-133">String</span></span>|<span data-ttu-id="75a47-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="75a47-134">Key of the entity.</span></span> <span data-ttu-id="75a47-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-136">displayName</span><span class="sxs-lookup"><span data-stu-id="75a47-136">displayName</span></span>|<span data-ttu-id="75a47-137">String</span><span class="sxs-lookup"><span data-stu-id="75a47-137">String</span></span>|<span data-ttu-id="75a47-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="75a47-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="75a47-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-140">description</span><span class="sxs-lookup"><span data-stu-id="75a47-140">description</span></span>|<span data-ttu-id="75a47-141">String</span><span class="sxs-lookup"><span data-stu-id="75a47-141">String</span></span>|<span data-ttu-id="75a47-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="75a47-142">The description of the app.</span></span> <span data-ttu-id="75a47-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-144">publisher</span><span class="sxs-lookup"><span data-stu-id="75a47-144">publisher</span></span>|<span data-ttu-id="75a47-145">String</span><span class="sxs-lookup"><span data-stu-id="75a47-145">String</span></span>|<span data-ttu-id="75a47-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="75a47-146">The publisher of the app.</span></span> <span data-ttu-id="75a47-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="75a47-148">largeIcon</span></span>|[<span data-ttu-id="75a47-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="75a47-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="75a47-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="75a47-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="75a47-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75a47-152">createdDateTime</span></span>|<span data-ttu-id="75a47-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75a47-153">DateTimeOffset</span></span>|<span data-ttu-id="75a47-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="75a47-154">The date and time the app was created.</span></span> <span data-ttu-id="75a47-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75a47-156">lastModifiedDateTime</span></span>|<span data-ttu-id="75a47-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75a47-157">DateTimeOffset</span></span>|<span data-ttu-id="75a47-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="75a47-158">The date and time the app was last modified.</span></span> <span data-ttu-id="75a47-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="75a47-160">isFeatured</span></span>|<span data-ttu-id="75a47-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="75a47-161">Boolean</span></span>|<span data-ttu-id="75a47-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="75a47-163">privacyInformationUrl</span></span>|<span data-ttu-id="75a47-164">String</span><span class="sxs-lookup"><span data-stu-id="75a47-164">String</span></span>|<span data-ttu-id="75a47-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="75a47-165">The privacy statement Url.</span></span> <span data-ttu-id="75a47-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="75a47-167">informationUrl</span></span>|<span data-ttu-id="75a47-168">String</span><span class="sxs-lookup"><span data-stu-id="75a47-168">String</span></span>|<span data-ttu-id="75a47-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="75a47-169">The more information Url.</span></span> <span data-ttu-id="75a47-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-171">owner</span><span class="sxs-lookup"><span data-stu-id="75a47-171">owner</span></span>|<span data-ttu-id="75a47-172">字符串</span><span class="sxs-lookup"><span data-stu-id="75a47-172">String</span></span>|<span data-ttu-id="75a47-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="75a47-173">The owner of the app.</span></span> <span data-ttu-id="75a47-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-175">developer</span><span class="sxs-lookup"><span data-stu-id="75a47-175">developer</span></span>|<span data-ttu-id="75a47-176">String</span><span class="sxs-lookup"><span data-stu-id="75a47-176">String</span></span>|<span data-ttu-id="75a47-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="75a47-177">The developer of the app.</span></span> <span data-ttu-id="75a47-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-179">notes</span><span class="sxs-lookup"><span data-stu-id="75a47-179">notes</span></span>|<span data-ttu-id="75a47-180">String</span><span class="sxs-lookup"><span data-stu-id="75a47-180">String</span></span>|<span data-ttu-id="75a47-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="75a47-181">Notes for the app.</span></span> <span data-ttu-id="75a47-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="75a47-183">uploadState</span></span>|<span data-ttu-id="75a47-184">Int32</span><span class="sxs-lookup"><span data-stu-id="75a47-184">Int32</span></span>|<span data-ttu-id="75a47-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="75a47-185">The upload state.</span></span> <span data-ttu-id="75a47-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="75a47-187">publishingState</span></span>|[<span data-ttu-id="75a47-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="75a47-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="75a47-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="75a47-189">The publishing state for the app.</span></span> <span data-ttu-id="75a47-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="75a47-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="75a47-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="75a47-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="75a47-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="75a47-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="75a47-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="75a47-193">isAssigned</span></span>|<span data-ttu-id="75a47-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="75a47-194">Boolean</span></span>|<span data-ttu-id="75a47-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="75a47-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="75a47-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="75a47-197">roleScopeTagIds</span></span>|<span data-ttu-id="75a47-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="75a47-198">String collection</span></span>|<span data-ttu-id="75a47-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="75a47-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="75a47-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="75a47-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="75a47-201">committedContentVersion</span></span>|<span data-ttu-id="75a47-202">String</span><span class="sxs-lookup"><span data-stu-id="75a47-202">String</span></span>|<span data-ttu-id="75a47-203">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="75a47-203">The internal committed content version.</span></span> <span data-ttu-id="75a47-204">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="75a47-205">fileName</span><span class="sxs-lookup"><span data-stu-id="75a47-205">fileName</span></span>|<span data-ttu-id="75a47-206">String</span><span class="sxs-lookup"><span data-stu-id="75a47-206">String</span></span>|<span data-ttu-id="75a47-207">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="75a47-207">The name of the main Lob application file.</span></span> <span data-ttu-id="75a47-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="75a47-209">size</span><span class="sxs-lookup"><span data-stu-id="75a47-209">size</span></span>|<span data-ttu-id="75a47-210">Int64</span><span class="sxs-lookup"><span data-stu-id="75a47-210">Int64</span></span>|<span data-ttu-id="75a47-211">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="75a47-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="75a47-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="75a47-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="75a47-213">bundleId</span><span class="sxs-lookup"><span data-stu-id="75a47-213">bundleId</span></span>|<span data-ttu-id="75a47-214">String</span><span class="sxs-lookup"><span data-stu-id="75a47-214">String</span></span>|<span data-ttu-id="75a47-215">标识名称。</span><span class="sxs-lookup"><span data-stu-id="75a47-215">The Identity Name.</span></span>|
|<span data-ttu-id="75a47-216">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="75a47-216">applicableDeviceType</span></span>|[<span data-ttu-id="75a47-217">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="75a47-217">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="75a47-218">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="75a47-218">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="75a47-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="75a47-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="75a47-220">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="75a47-220">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="75a47-221">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="75a47-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="75a47-222">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="75a47-222">expirationDateTime</span></span>|<span data-ttu-id="75a47-223">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75a47-223">DateTimeOffset</span></span>|<span data-ttu-id="75a47-224">过期时间。</span><span class="sxs-lookup"><span data-stu-id="75a47-224">The expiration time.</span></span>|
|<span data-ttu-id="75a47-225">versionNumber</span><span class="sxs-lookup"><span data-stu-id="75a47-225">versionNumber</span></span>|<span data-ttu-id="75a47-226">String</span><span class="sxs-lookup"><span data-stu-id="75a47-226">String</span></span>|<span data-ttu-id="75a47-227">iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="75a47-227">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="75a47-228">buildNumber</span><span class="sxs-lookup"><span data-stu-id="75a47-228">buildNumber</span></span>|<span data-ttu-id="75a47-229">String</span><span class="sxs-lookup"><span data-stu-id="75a47-229">String</span></span>|<span data-ttu-id="75a47-230">iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="75a47-230">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="75a47-231">identityVersion</span><span class="sxs-lookup"><span data-stu-id="75a47-231">identityVersion</span></span>|<span data-ttu-id="75a47-232">String</span><span class="sxs-lookup"><span data-stu-id="75a47-232">String</span></span>|<span data-ttu-id="75a47-233">标识版本。</span><span class="sxs-lookup"><span data-stu-id="75a47-233">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="75a47-234">响应</span><span class="sxs-lookup"><span data-stu-id="75a47-234">Response</span></span>
<span data-ttu-id="75a47-235">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="75a47-235">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75a47-236">示例</span><span class="sxs-lookup"><span data-stu-id="75a47-236">Example</span></span>

### <a name="request"></a><span data-ttu-id="75a47-237">请求</span><span class="sxs-lookup"><span data-stu-id="75a47-237">Request</span></span>
<span data-ttu-id="75a47-238">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="75a47-238">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1364

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

### <a name="response"></a><span data-ttu-id="75a47-239">响应</span><span class="sxs-lookup"><span data-stu-id="75a47-239">Response</span></span>
<span data-ttu-id="75a47-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="75a47-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1536

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




