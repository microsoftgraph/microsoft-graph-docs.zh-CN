---
title: 创建 managedIOSLobApp
description: 创建新的 managedIOSLobApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a58dcbdabcd879d6a5164bbf830df9de6fc24c7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578076"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="d5443-103">创建 managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="d5443-103">Create managedIOSLobApp</span></span>

> <span data-ttu-id="d5443-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5443-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5443-105">创建新的 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d5443-105">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5443-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d5443-106">Prerequisites</span></span>
<span data-ttu-id="d5443-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5443-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5443-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5443-109">Permission type</span></span>|<span data-ttu-id="d5443-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d5443-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5443-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5443-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d5443-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5443-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d5443-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5443-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5443-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5443-114">Not supported.</span></span>|
|<span data-ttu-id="d5443-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5443-115">Application</span></span>|<span data-ttu-id="d5443-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5443-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5443-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5443-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d5443-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5443-118">Request headers</span></span>
|<span data-ttu-id="d5443-119">标头</span><span class="sxs-lookup"><span data-stu-id="d5443-119">Header</span></span>|<span data-ttu-id="d5443-120">值</span><span class="sxs-lookup"><span data-stu-id="d5443-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5443-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5443-121">Authorization</span></span>|<span data-ttu-id="d5443-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d5443-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5443-123">接受</span><span class="sxs-lookup"><span data-stu-id="d5443-123">Accept</span></span>|<span data-ttu-id="d5443-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d5443-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5443-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5443-125">Request body</span></span>
<span data-ttu-id="d5443-126">在请求正文中，提供 managedIOSLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5443-126">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="d5443-127">下表显示创建 managedIOSLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d5443-127">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="d5443-128">属性</span><span class="sxs-lookup"><span data-stu-id="d5443-128">Property</span></span>|<span data-ttu-id="d5443-129">类型</span><span class="sxs-lookup"><span data-stu-id="d5443-129">Type</span></span>|<span data-ttu-id="d5443-130">说明</span><span class="sxs-lookup"><span data-stu-id="d5443-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5443-131">id</span><span class="sxs-lookup"><span data-stu-id="d5443-131">id</span></span>|<span data-ttu-id="d5443-132">字符串</span><span class="sxs-lookup"><span data-stu-id="d5443-132">String</span></span>|<span data-ttu-id="d5443-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d5443-133">Key of the entity.</span></span> <span data-ttu-id="d5443-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5443-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d5443-135">displayName</span></span>|<span data-ttu-id="d5443-136">String</span><span class="sxs-lookup"><span data-stu-id="d5443-136">String</span></span>|<span data-ttu-id="d5443-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="d5443-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d5443-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5443-139">说明</span><span class="sxs-lookup"><span data-stu-id="d5443-139">description</span></span>|<span data-ttu-id="d5443-140">String</span><span class="sxs-lookup"><span data-stu-id="d5443-140">String</span></span>|<span data-ttu-id="d5443-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="d5443-141">The description of the app.</span></span> <span data-ttu-id="d5443-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5443-143">publisher</span><span class="sxs-lookup"><span data-stu-id="d5443-143">publisher</span></span>|<span data-ttu-id="d5443-144">String</span><span class="sxs-lookup"><span data-stu-id="d5443-144">String</span></span>|<span data-ttu-id="d5443-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="d5443-145">The publisher of the app.</span></span> <span data-ttu-id="d5443-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5443-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d5443-147">largeIcon</span></span>|[<span data-ttu-id="d5443-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d5443-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d5443-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="d5443-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d5443-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5443-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5443-151">createdDateTime</span></span>|<span data-ttu-id="d5443-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5443-152">DateTimeOffset</span></span>|<span data-ttu-id="d5443-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d5443-153">The date and time the app was created.</span></span> <span data-ttu-id="d5443-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5443-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5443-155">lastModifiedDateTime</span></span>|<span data-ttu-id="d5443-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5443-156">DateTimeOffset</span></span>|<span data-ttu-id="d5443-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d5443-157">The date and time the app was last modified.</span></span> <span data-ttu-id="d5443-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5443-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d5443-159">isFeatured</span></span>|<span data-ttu-id="d5443-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5443-160">Boolean</span></span>|<span data-ttu-id="d5443-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5443-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d5443-162">privacyInformationUrl</span></span>|<span data-ttu-id="d5443-163">String</span><span class="sxs-lookup"><span data-stu-id="d5443-163">String</span></span>|<span data-ttu-id="d5443-164">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="d5443-164">The privacy statement Url.</span></span> <span data-ttu-id="d5443-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5443-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d5443-166">informationUrl</span></span>|<span data-ttu-id="d5443-167">String</span><span class="sxs-lookup"><span data-stu-id="d5443-167">String</span></span>|<span data-ttu-id="d5443-168">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="d5443-168">The more information Url.</span></span> <span data-ttu-id="d5443-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5443-170">owner</span><span class="sxs-lookup"><span data-stu-id="d5443-170">owner</span></span>|<span data-ttu-id="d5443-171">字符串</span><span class="sxs-lookup"><span data-stu-id="d5443-171">String</span></span>|<span data-ttu-id="d5443-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="d5443-172">The owner of the app.</span></span> <span data-ttu-id="d5443-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5443-174">developer</span><span class="sxs-lookup"><span data-stu-id="d5443-174">developer</span></span>|<span data-ttu-id="d5443-175">String</span><span class="sxs-lookup"><span data-stu-id="d5443-175">String</span></span>|<span data-ttu-id="d5443-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="d5443-176">The developer of the app.</span></span> <span data-ttu-id="d5443-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5443-178">notes</span><span class="sxs-lookup"><span data-stu-id="d5443-178">notes</span></span>|<span data-ttu-id="d5443-179">String</span><span class="sxs-lookup"><span data-stu-id="d5443-179">String</span></span>|<span data-ttu-id="d5443-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="d5443-180">Notes for the app.</span></span> <span data-ttu-id="d5443-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d5443-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="d5443-182">publishingState</span></span>|[<span data-ttu-id="d5443-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d5443-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d5443-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="d5443-184">The publishing state for the app.</span></span> <span data-ttu-id="d5443-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="d5443-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d5443-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="d5443-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d5443-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="d5443-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d5443-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="d5443-188">appAvailability</span></span>|[<span data-ttu-id="d5443-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="d5443-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="d5443-190">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="d5443-190">The Application's availability.</span></span> <span data-ttu-id="d5443-191">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="d5443-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="d5443-192">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="d5443-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="d5443-193">version</span><span class="sxs-lookup"><span data-stu-id="d5443-193">version</span></span>|<span data-ttu-id="d5443-194">String</span><span class="sxs-lookup"><span data-stu-id="d5443-194">String</span></span>|<span data-ttu-id="d5443-195">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="d5443-195">The Application's version.</span></span> <span data-ttu-id="d5443-196">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="d5443-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d5443-197">committedContentVersion</span></span>|<span data-ttu-id="d5443-198">String</span><span class="sxs-lookup"><span data-stu-id="d5443-198">String</span></span>|<span data-ttu-id="d5443-199">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="d5443-199">The internal committed content version.</span></span> <span data-ttu-id="d5443-200">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d5443-201">fileName</span><span class="sxs-lookup"><span data-stu-id="d5443-201">fileName</span></span>|<span data-ttu-id="d5443-202">String</span><span class="sxs-lookup"><span data-stu-id="d5443-202">String</span></span>|<span data-ttu-id="d5443-203">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="d5443-203">The name of the main Lob application file.</span></span> <span data-ttu-id="d5443-204">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d5443-205">size</span><span class="sxs-lookup"><span data-stu-id="d5443-205">size</span></span>|<span data-ttu-id="d5443-206">Int64</span><span class="sxs-lookup"><span data-stu-id="d5443-206">Int64</span></span>|<span data-ttu-id="d5443-207">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="d5443-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="d5443-208">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d5443-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="d5443-209">bundleId</span><span class="sxs-lookup"><span data-stu-id="d5443-209">bundleId</span></span>|<span data-ttu-id="d5443-210">String</span><span class="sxs-lookup"><span data-stu-id="d5443-210">String</span></span>|<span data-ttu-id="d5443-211">标识名称。</span><span class="sxs-lookup"><span data-stu-id="d5443-211">The Identity Name.</span></span>|
|<span data-ttu-id="d5443-212">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="d5443-212">applicableDeviceType</span></span>|[<span data-ttu-id="d5443-213">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="d5443-213">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="d5443-214">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="d5443-214">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="d5443-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d5443-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d5443-216">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d5443-216">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="d5443-217">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="d5443-217">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d5443-218">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d5443-218">expirationDateTime</span></span>|<span data-ttu-id="d5443-219">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5443-219">DateTimeOffset</span></span>|<span data-ttu-id="d5443-220">过期时间。</span><span class="sxs-lookup"><span data-stu-id="d5443-220">The expiration time.</span></span>|
|<span data-ttu-id="d5443-221">versionNumber</span><span class="sxs-lookup"><span data-stu-id="d5443-221">versionNumber</span></span>|<span data-ttu-id="d5443-222">String</span><span class="sxs-lookup"><span data-stu-id="d5443-222">String</span></span>|<span data-ttu-id="d5443-223">托管 iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="d5443-223">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d5443-224">buildNumber</span><span class="sxs-lookup"><span data-stu-id="d5443-224">buildNumber</span></span>|<span data-ttu-id="d5443-225">String</span><span class="sxs-lookup"><span data-stu-id="d5443-225">String</span></span>|<span data-ttu-id="d5443-226">托管 iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="d5443-226">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="d5443-227">响应</span><span class="sxs-lookup"><span data-stu-id="d5443-227">Response</span></span>
<span data-ttu-id="d5443-228">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d5443-228">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5443-229">示例</span><span class="sxs-lookup"><span data-stu-id="d5443-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5443-230">请求</span><span class="sxs-lookup"><span data-stu-id="d5443-230">Request</span></span>
<span data-ttu-id="d5443-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5443-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1287

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
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="d5443-232">响应</span><span class="sxs-lookup"><span data-stu-id="d5443-232">Response</span></span>
<span data-ttu-id="d5443-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5443-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1459

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
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



