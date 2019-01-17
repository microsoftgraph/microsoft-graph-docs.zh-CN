---
title: 创建 managedIOSLobApp
description: 创建新的 managedIOSLobApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b2bbd4ff7721f4d89dc3b201a2c58277d9f0baca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936149"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="d496f-103">创建 managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="d496f-103">Create managedIOSLobApp</span></span>

> <span data-ttu-id="d496f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d496f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d496f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d496f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d496f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d496f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d496f-107">创建新的 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d496f-107">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d496f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d496f-108">Prerequisites</span></span>
<span data-ttu-id="d496f-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d496f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d496f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d496f-111">Permission type</span></span>|<span data-ttu-id="d496f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d496f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d496f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d496f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d496f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d496f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d496f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d496f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d496f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d496f-116">Not supported.</span></span>|
|<span data-ttu-id="d496f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d496f-117">Application</span></span>|<span data-ttu-id="d496f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d496f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d496f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d496f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d496f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d496f-120">Request headers</span></span>
|<span data-ttu-id="d496f-121">标头</span><span class="sxs-lookup"><span data-stu-id="d496f-121">Header</span></span>|<span data-ttu-id="d496f-122">值</span><span class="sxs-lookup"><span data-stu-id="d496f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d496f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d496f-123">Authorization</span></span>|<span data-ttu-id="d496f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d496f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d496f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d496f-125">Accept</span></span>|<span data-ttu-id="d496f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d496f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d496f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d496f-127">Request body</span></span>
<span data-ttu-id="d496f-128">在请求正文中，提供 managedIOSLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d496f-128">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="d496f-129">下表显示创建 managedIOSLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d496f-129">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="d496f-130">属性</span><span class="sxs-lookup"><span data-stu-id="d496f-130">Property</span></span>|<span data-ttu-id="d496f-131">类型</span><span class="sxs-lookup"><span data-stu-id="d496f-131">Type</span></span>|<span data-ttu-id="d496f-132">说明</span><span class="sxs-lookup"><span data-stu-id="d496f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d496f-133">id</span><span class="sxs-lookup"><span data-stu-id="d496f-133">id</span></span>|<span data-ttu-id="d496f-134">String</span><span class="sxs-lookup"><span data-stu-id="d496f-134">String</span></span>|<span data-ttu-id="d496f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d496f-135">Key of the entity.</span></span> <span data-ttu-id="d496f-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d496f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d496f-137">displayName</span></span>|<span data-ttu-id="d496f-138">String</span><span class="sxs-lookup"><span data-stu-id="d496f-138">String</span></span>|<span data-ttu-id="d496f-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="d496f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d496f-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d496f-141">description</span><span class="sxs-lookup"><span data-stu-id="d496f-141">description</span></span>|<span data-ttu-id="d496f-142">String</span><span class="sxs-lookup"><span data-stu-id="d496f-142">String</span></span>|<span data-ttu-id="d496f-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="d496f-143">The description of the app.</span></span> <span data-ttu-id="d496f-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d496f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="d496f-145">publisher</span></span>|<span data-ttu-id="d496f-146">String</span><span class="sxs-lookup"><span data-stu-id="d496f-146">String</span></span>|<span data-ttu-id="d496f-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="d496f-147">The publisher of the app.</span></span> <span data-ttu-id="d496f-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d496f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d496f-149">largeIcon</span></span>|[<span data-ttu-id="d496f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d496f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d496f-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="d496f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d496f-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d496f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d496f-153">createdDateTime</span></span>|<span data-ttu-id="d496f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d496f-154">DateTimeOffset</span></span>|<span data-ttu-id="d496f-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d496f-155">The date and time the app was created.</span></span> <span data-ttu-id="d496f-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d496f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d496f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d496f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d496f-158">DateTimeOffset</span></span>|<span data-ttu-id="d496f-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d496f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d496f-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d496f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d496f-161">isFeatured</span></span>|<span data-ttu-id="d496f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d496f-162">Boolean</span></span>|<span data-ttu-id="d496f-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d496f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d496f-164">privacyInformationUrl</span></span>|<span data-ttu-id="d496f-165">String</span><span class="sxs-lookup"><span data-stu-id="d496f-165">String</span></span>|<span data-ttu-id="d496f-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="d496f-166">The privacy statement Url.</span></span> <span data-ttu-id="d496f-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d496f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d496f-168">informationUrl</span></span>|<span data-ttu-id="d496f-169">String</span><span class="sxs-lookup"><span data-stu-id="d496f-169">String</span></span>|<span data-ttu-id="d496f-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="d496f-170">The more information Url.</span></span> <span data-ttu-id="d496f-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d496f-172">owner</span><span class="sxs-lookup"><span data-stu-id="d496f-172">owner</span></span>|<span data-ttu-id="d496f-173">String</span><span class="sxs-lookup"><span data-stu-id="d496f-173">String</span></span>|<span data-ttu-id="d496f-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="d496f-174">The owner of the app.</span></span> <span data-ttu-id="d496f-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d496f-176">developer</span><span class="sxs-lookup"><span data-stu-id="d496f-176">developer</span></span>|<span data-ttu-id="d496f-177">String</span><span class="sxs-lookup"><span data-stu-id="d496f-177">String</span></span>|<span data-ttu-id="d496f-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="d496f-178">The developer of the app.</span></span> <span data-ttu-id="d496f-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d496f-180">notes</span><span class="sxs-lookup"><span data-stu-id="d496f-180">notes</span></span>|<span data-ttu-id="d496f-181">String</span><span class="sxs-lookup"><span data-stu-id="d496f-181">String</span></span>|<span data-ttu-id="d496f-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="d496f-182">Notes for the app.</span></span> <span data-ttu-id="d496f-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d496f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d496f-184">uploadState</span></span>|<span data-ttu-id="d496f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d496f-185">Int32</span></span>|<span data-ttu-id="d496f-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="d496f-186">The upload state.</span></span> <span data-ttu-id="d496f-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d496f-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="d496f-188">publishingState</span></span>|[<span data-ttu-id="d496f-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d496f-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d496f-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="d496f-190">The publishing state for the app.</span></span> <span data-ttu-id="d496f-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="d496f-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d496f-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="d496f-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d496f-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="d496f-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d496f-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="d496f-194">appAvailability</span></span>|[<span data-ttu-id="d496f-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="d496f-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="d496f-196">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="d496f-196">The Application's availability.</span></span> <span data-ttu-id="d496f-197">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="d496f-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="d496f-198">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="d496f-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="d496f-199">version</span><span class="sxs-lookup"><span data-stu-id="d496f-199">version</span></span>|<span data-ttu-id="d496f-200">String</span><span class="sxs-lookup"><span data-stu-id="d496f-200">String</span></span>|<span data-ttu-id="d496f-201">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="d496f-201">The Application's version.</span></span> <span data-ttu-id="d496f-202">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="d496f-203">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d496f-203">committedContentVersion</span></span>|<span data-ttu-id="d496f-204">String</span><span class="sxs-lookup"><span data-stu-id="d496f-204">String</span></span>|<span data-ttu-id="d496f-205">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="d496f-205">The internal committed content version.</span></span> <span data-ttu-id="d496f-206">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-206">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d496f-207">fileName</span><span class="sxs-lookup"><span data-stu-id="d496f-207">fileName</span></span>|<span data-ttu-id="d496f-208">String</span><span class="sxs-lookup"><span data-stu-id="d496f-208">String</span></span>|<span data-ttu-id="d496f-209">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="d496f-209">The name of the main Lob application file.</span></span> <span data-ttu-id="d496f-210">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-210">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d496f-211">size</span><span class="sxs-lookup"><span data-stu-id="d496f-211">size</span></span>|<span data-ttu-id="d496f-212">Int64</span><span class="sxs-lookup"><span data-stu-id="d496f-212">Int64</span></span>|<span data-ttu-id="d496f-213">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="d496f-213">The total size, including all uploaded files.</span></span> <span data-ttu-id="d496f-214">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d496f-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d496f-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="d496f-215">bundleId</span></span>|<span data-ttu-id="d496f-216">String</span><span class="sxs-lookup"><span data-stu-id="d496f-216">String</span></span>|<span data-ttu-id="d496f-217">标识名称。</span><span class="sxs-lookup"><span data-stu-id="d496f-217">The Identity Name.</span></span>|
|<span data-ttu-id="d496f-218">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="d496f-218">applicableDeviceType</span></span>|[<span data-ttu-id="d496f-219">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="d496f-219">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="d496f-220">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="d496f-220">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="d496f-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d496f-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d496f-222">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d496f-222">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="d496f-223">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="d496f-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d496f-224">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d496f-224">expirationDateTime</span></span>|<span data-ttu-id="d496f-225">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d496f-225">DateTimeOffset</span></span>|<span data-ttu-id="d496f-226">过期时间。</span><span class="sxs-lookup"><span data-stu-id="d496f-226">The expiration time.</span></span>|
|<span data-ttu-id="d496f-227">versionNumber</span><span class="sxs-lookup"><span data-stu-id="d496f-227">versionNumber</span></span>|<span data-ttu-id="d496f-228">String</span><span class="sxs-lookup"><span data-stu-id="d496f-228">String</span></span>|<span data-ttu-id="d496f-229">托管 iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="d496f-229">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d496f-230">buildNumber</span><span class="sxs-lookup"><span data-stu-id="d496f-230">buildNumber</span></span>|<span data-ttu-id="d496f-231">String</span><span class="sxs-lookup"><span data-stu-id="d496f-231">String</span></span>|<span data-ttu-id="d496f-232">托管 iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="d496f-232">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d496f-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="d496f-233">identityVersion</span></span>|<span data-ttu-id="d496f-234">String</span><span class="sxs-lookup"><span data-stu-id="d496f-234">String</span></span>|<span data-ttu-id="d496f-235">标识版本。</span><span class="sxs-lookup"><span data-stu-id="d496f-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="d496f-236">响应</span><span class="sxs-lookup"><span data-stu-id="d496f-236">Response</span></span>
<span data-ttu-id="d496f-237">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d496f-237">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d496f-238">示例</span><span class="sxs-lookup"><span data-stu-id="d496f-238">Example</span></span>
### <a name="request"></a><span data-ttu-id="d496f-239">请求</span><span class="sxs-lookup"><span data-stu-id="d496f-239">Request</span></span>
<span data-ttu-id="d496f-240">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d496f-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1421

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="d496f-241">响应</span><span class="sxs-lookup"><span data-stu-id="d496f-241">Response</span></span>
<span data-ttu-id="d496f-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d496f-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1529

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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





