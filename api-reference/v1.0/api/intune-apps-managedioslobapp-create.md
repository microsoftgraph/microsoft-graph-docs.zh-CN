---
title: 创建 managedIOSLobApp
description: 创建新的 managedIOSLobApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8407b6d11c237ab44efa908f7a613b7be2aad45
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759810"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="d44be-103">创建 managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="d44be-103">Create managedIOSLobApp</span></span>

<span data-ttu-id="d44be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d44be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d44be-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d44be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d44be-106">创建新的 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d44be-106">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d44be-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d44be-107">Prerequisites</span></span>
<span data-ttu-id="d44be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d44be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d44be-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d44be-110">Permission type</span></span>|<span data-ttu-id="d44be-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d44be-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d44be-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d44be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d44be-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d44be-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d44be-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d44be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d44be-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d44be-115">Not supported.</span></span>|
|<span data-ttu-id="d44be-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d44be-116">Application</span></span>|<span data-ttu-id="d44be-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d44be-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d44be-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d44be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d44be-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d44be-119">Request headers</span></span>
|<span data-ttu-id="d44be-120">标头</span><span class="sxs-lookup"><span data-stu-id="d44be-120">Header</span></span>|<span data-ttu-id="d44be-121">值</span><span class="sxs-lookup"><span data-stu-id="d44be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d44be-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d44be-122">Authorization</span></span>|<span data-ttu-id="d44be-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d44be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d44be-124">接受</span><span class="sxs-lookup"><span data-stu-id="d44be-124">Accept</span></span>|<span data-ttu-id="d44be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d44be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d44be-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d44be-126">Request body</span></span>
<span data-ttu-id="d44be-127">在请求正文中，提供 managedIOSLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d44be-127">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="d44be-128">下表显示创建 managedIOSLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d44be-128">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="d44be-129">属性</span><span class="sxs-lookup"><span data-stu-id="d44be-129">Property</span></span>|<span data-ttu-id="d44be-130">类型</span><span class="sxs-lookup"><span data-stu-id="d44be-130">Type</span></span>|<span data-ttu-id="d44be-131">说明</span><span class="sxs-lookup"><span data-stu-id="d44be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d44be-132">id</span><span class="sxs-lookup"><span data-stu-id="d44be-132">id</span></span>|<span data-ttu-id="d44be-133">String</span><span class="sxs-lookup"><span data-stu-id="d44be-133">String</span></span>|<span data-ttu-id="d44be-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d44be-134">Key of the entity.</span></span> <span data-ttu-id="d44be-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d44be-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d44be-136">displayName</span></span>|<span data-ttu-id="d44be-137">String</span><span class="sxs-lookup"><span data-stu-id="d44be-137">String</span></span>|<span data-ttu-id="d44be-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="d44be-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d44be-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d44be-140">description</span><span class="sxs-lookup"><span data-stu-id="d44be-140">description</span></span>|<span data-ttu-id="d44be-141">String</span><span class="sxs-lookup"><span data-stu-id="d44be-141">String</span></span>|<span data-ttu-id="d44be-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="d44be-142">The description of the app.</span></span> <span data-ttu-id="d44be-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d44be-144">publisher</span><span class="sxs-lookup"><span data-stu-id="d44be-144">publisher</span></span>|<span data-ttu-id="d44be-145">String</span><span class="sxs-lookup"><span data-stu-id="d44be-145">String</span></span>|<span data-ttu-id="d44be-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="d44be-146">The publisher of the app.</span></span> <span data-ttu-id="d44be-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d44be-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d44be-148">largeIcon</span></span>|[<span data-ttu-id="d44be-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d44be-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d44be-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="d44be-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d44be-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d44be-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d44be-152">createdDateTime</span></span>|<span data-ttu-id="d44be-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d44be-153">DateTimeOffset</span></span>|<span data-ttu-id="d44be-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d44be-154">The date and time the app was created.</span></span> <span data-ttu-id="d44be-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d44be-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d44be-156">lastModifiedDateTime</span></span>|<span data-ttu-id="d44be-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d44be-157">DateTimeOffset</span></span>|<span data-ttu-id="d44be-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d44be-158">The date and time the app was last modified.</span></span> <span data-ttu-id="d44be-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d44be-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d44be-160">isFeatured</span></span>|<span data-ttu-id="d44be-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d44be-161">Boolean</span></span>|<span data-ttu-id="d44be-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d44be-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d44be-163">privacyInformationUrl</span></span>|<span data-ttu-id="d44be-164">String</span><span class="sxs-lookup"><span data-stu-id="d44be-164">String</span></span>|<span data-ttu-id="d44be-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="d44be-165">The privacy statement Url.</span></span> <span data-ttu-id="d44be-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d44be-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d44be-167">informationUrl</span></span>|<span data-ttu-id="d44be-168">String</span><span class="sxs-lookup"><span data-stu-id="d44be-168">String</span></span>|<span data-ttu-id="d44be-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="d44be-169">The more information Url.</span></span> <span data-ttu-id="d44be-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d44be-171">所有者</span><span class="sxs-lookup"><span data-stu-id="d44be-171">owner</span></span>|<span data-ttu-id="d44be-172">String</span><span class="sxs-lookup"><span data-stu-id="d44be-172">String</span></span>|<span data-ttu-id="d44be-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="d44be-173">The owner of the app.</span></span> <span data-ttu-id="d44be-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d44be-175">developer</span><span class="sxs-lookup"><span data-stu-id="d44be-175">developer</span></span>|<span data-ttu-id="d44be-176">String</span><span class="sxs-lookup"><span data-stu-id="d44be-176">String</span></span>|<span data-ttu-id="d44be-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="d44be-177">The developer of the app.</span></span> <span data-ttu-id="d44be-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d44be-179">notes</span><span class="sxs-lookup"><span data-stu-id="d44be-179">notes</span></span>|<span data-ttu-id="d44be-180">String</span><span class="sxs-lookup"><span data-stu-id="d44be-180">String</span></span>|<span data-ttu-id="d44be-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="d44be-181">Notes for the app.</span></span> <span data-ttu-id="d44be-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d44be-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="d44be-183">publishingState</span></span>|[<span data-ttu-id="d44be-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d44be-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d44be-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="d44be-185">The publishing state for the app.</span></span> <span data-ttu-id="d44be-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="d44be-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d44be-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="d44be-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d44be-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="d44be-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d44be-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="d44be-189">appAvailability</span></span>|[<span data-ttu-id="d44be-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="d44be-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="d44be-191">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="d44be-191">The Application's availability.</span></span> <span data-ttu-id="d44be-192">继承自 [managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="d44be-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="d44be-193">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="d44be-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="d44be-194">version</span><span class="sxs-lookup"><span data-stu-id="d44be-194">version</span></span>|<span data-ttu-id="d44be-195">String</span><span class="sxs-lookup"><span data-stu-id="d44be-195">String</span></span>|<span data-ttu-id="d44be-196">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="d44be-196">The Application's version.</span></span> <span data-ttu-id="d44be-197">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="d44be-198">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d44be-198">committedContentVersion</span></span>|<span data-ttu-id="d44be-199">String</span><span class="sxs-lookup"><span data-stu-id="d44be-199">String</span></span>|<span data-ttu-id="d44be-200">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="d44be-200">The internal committed content version.</span></span> <span data-ttu-id="d44be-201">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-201">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d44be-202">fileName</span><span class="sxs-lookup"><span data-stu-id="d44be-202">fileName</span></span>|<span data-ttu-id="d44be-203">String</span><span class="sxs-lookup"><span data-stu-id="d44be-203">String</span></span>|<span data-ttu-id="d44be-204">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="d44be-204">The name of the main Lob application file.</span></span> <span data-ttu-id="d44be-205">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-205">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d44be-206">size</span><span class="sxs-lookup"><span data-stu-id="d44be-206">size</span></span>|<span data-ttu-id="d44be-207">Int64</span><span class="sxs-lookup"><span data-stu-id="d44be-207">Int64</span></span>|<span data-ttu-id="d44be-208">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="d44be-208">The total size, including all uploaded files.</span></span> <span data-ttu-id="d44be-209">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d44be-209">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d44be-210">bundleId</span><span class="sxs-lookup"><span data-stu-id="d44be-210">bundleId</span></span>|<span data-ttu-id="d44be-211">String</span><span class="sxs-lookup"><span data-stu-id="d44be-211">String</span></span>|<span data-ttu-id="d44be-212">标识名称。</span><span class="sxs-lookup"><span data-stu-id="d44be-212">The Identity Name.</span></span>|
|<span data-ttu-id="d44be-213">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="d44be-213">applicableDeviceType</span></span>|[<span data-ttu-id="d44be-214">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="d44be-214">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="d44be-215">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="d44be-215">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="d44be-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d44be-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d44be-217">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d44be-217">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="d44be-218">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="d44be-218">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d44be-219">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d44be-219">expirationDateTime</span></span>|<span data-ttu-id="d44be-220">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d44be-220">DateTimeOffset</span></span>|<span data-ttu-id="d44be-221">过期时间。</span><span class="sxs-lookup"><span data-stu-id="d44be-221">The expiration time.</span></span>|
|<span data-ttu-id="d44be-222">versionNumber</span><span class="sxs-lookup"><span data-stu-id="d44be-222">versionNumber</span></span>|<span data-ttu-id="d44be-223">String</span><span class="sxs-lookup"><span data-stu-id="d44be-223">String</span></span>|<span data-ttu-id="d44be-224">托管 iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="d44be-224">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d44be-225">buildNumber</span><span class="sxs-lookup"><span data-stu-id="d44be-225">buildNumber</span></span>|<span data-ttu-id="d44be-226">String</span><span class="sxs-lookup"><span data-stu-id="d44be-226">String</span></span>|<span data-ttu-id="d44be-227">托管 iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="d44be-227">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="d44be-228">响应</span><span class="sxs-lookup"><span data-stu-id="d44be-228">Response</span></span>
<span data-ttu-id="d44be-229">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d44be-229">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d44be-230">示例</span><span class="sxs-lookup"><span data-stu-id="d44be-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="d44be-231">请求</span><span class="sxs-lookup"><span data-stu-id="d44be-231">Request</span></span>
<span data-ttu-id="d44be-232">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d44be-232">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1327

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
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
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
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="d44be-233">响应</span><span class="sxs-lookup"><span data-stu-id="d44be-233">Response</span></span>
<span data-ttu-id="d44be-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d44be-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1499

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
    "v12_0": true,
    "v13_0": true,
    "v14_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```




