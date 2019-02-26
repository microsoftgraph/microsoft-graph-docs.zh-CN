---
title: 更新 managedIOSLobApp
description: 更新 managedIOSLobApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d50c79e7a6dfcd0f4863571ff9e04da3ccc5bb7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264272"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="f984b-103">更新 managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="f984b-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="f984b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f984b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f984b-105">更新 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f984b-105">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f984b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f984b-106">Prerequisites</span></span>
<span data-ttu-id="f984b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f984b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f984b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f984b-109">Permission type</span></span>|<span data-ttu-id="f984b-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f984b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f984b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f984b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f984b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f984b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f984b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f984b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f984b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f984b-114">Not supported.</span></span>|
|<span data-ttu-id="f984b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f984b-115">Application</span></span>|<span data-ttu-id="f984b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f984b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f984b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f984b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="f984b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f984b-118">Request headers</span></span>
|<span data-ttu-id="f984b-119">标头</span><span class="sxs-lookup"><span data-stu-id="f984b-119">Header</span></span>|<span data-ttu-id="f984b-120">值</span><span class="sxs-lookup"><span data-stu-id="f984b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f984b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f984b-121">Authorization</span></span>|<span data-ttu-id="f984b-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f984b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f984b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f984b-123">Accept</span></span>|<span data-ttu-id="f984b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f984b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f984b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f984b-125">Request body</span></span>
<span data-ttu-id="f984b-126">在请求正文中，提供 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f984b-126">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="f984b-127">下表显示创建 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f984b-127">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="f984b-128">属性</span><span class="sxs-lookup"><span data-stu-id="f984b-128">Property</span></span>|<span data-ttu-id="f984b-129">类型</span><span class="sxs-lookup"><span data-stu-id="f984b-129">Type</span></span>|<span data-ttu-id="f984b-130">说明</span><span class="sxs-lookup"><span data-stu-id="f984b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f984b-131">id</span><span class="sxs-lookup"><span data-stu-id="f984b-131">id</span></span>|<span data-ttu-id="f984b-132">字符串</span><span class="sxs-lookup"><span data-stu-id="f984b-132">String</span></span>|<span data-ttu-id="f984b-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f984b-133">Key of the entity.</span></span> <span data-ttu-id="f984b-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f984b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f984b-135">displayName</span></span>|<span data-ttu-id="f984b-136">String</span><span class="sxs-lookup"><span data-stu-id="f984b-136">String</span></span>|<span data-ttu-id="f984b-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="f984b-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f984b-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f984b-139">description</span><span class="sxs-lookup"><span data-stu-id="f984b-139">description</span></span>|<span data-ttu-id="f984b-140">字符串</span><span class="sxs-lookup"><span data-stu-id="f984b-140">String</span></span>|<span data-ttu-id="f984b-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="f984b-141">The description of the app.</span></span> <span data-ttu-id="f984b-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f984b-143">publisher</span><span class="sxs-lookup"><span data-stu-id="f984b-143">publisher</span></span>|<span data-ttu-id="f984b-144">String</span><span class="sxs-lookup"><span data-stu-id="f984b-144">String</span></span>|<span data-ttu-id="f984b-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="f984b-145">The publisher of the app.</span></span> <span data-ttu-id="f984b-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f984b-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f984b-147">largeIcon</span></span>|[<span data-ttu-id="f984b-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f984b-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f984b-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="f984b-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f984b-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f984b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f984b-151">createdDateTime</span></span>|<span data-ttu-id="f984b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f984b-152">DateTimeOffset</span></span>|<span data-ttu-id="f984b-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f984b-153">The date and time the app was created.</span></span> <span data-ttu-id="f984b-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f984b-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f984b-155">lastModifiedDateTime</span></span>|<span data-ttu-id="f984b-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f984b-156">DateTimeOffset</span></span>|<span data-ttu-id="f984b-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f984b-157">The date and time the app was last modified.</span></span> <span data-ttu-id="f984b-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f984b-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f984b-159">isFeatured</span></span>|<span data-ttu-id="f984b-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="f984b-160">Boolean</span></span>|<span data-ttu-id="f984b-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f984b-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f984b-162">privacyInformationUrl</span></span>|<span data-ttu-id="f984b-163">String</span><span class="sxs-lookup"><span data-stu-id="f984b-163">String</span></span>|<span data-ttu-id="f984b-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="f984b-164">The privacy statement Url.</span></span> <span data-ttu-id="f984b-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f984b-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f984b-166">informationUrl</span></span>|<span data-ttu-id="f984b-167">String</span><span class="sxs-lookup"><span data-stu-id="f984b-167">String</span></span>|<span data-ttu-id="f984b-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="f984b-168">The more information Url.</span></span> <span data-ttu-id="f984b-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f984b-170">owner</span><span class="sxs-lookup"><span data-stu-id="f984b-170">owner</span></span>|<span data-ttu-id="f984b-171">String</span><span class="sxs-lookup"><span data-stu-id="f984b-171">String</span></span>|<span data-ttu-id="f984b-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="f984b-172">The owner of the app.</span></span> <span data-ttu-id="f984b-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f984b-174">developer</span><span class="sxs-lookup"><span data-stu-id="f984b-174">developer</span></span>|<span data-ttu-id="f984b-175">String</span><span class="sxs-lookup"><span data-stu-id="f984b-175">String</span></span>|<span data-ttu-id="f984b-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="f984b-176">The developer of the app.</span></span> <span data-ttu-id="f984b-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f984b-178">notes</span><span class="sxs-lookup"><span data-stu-id="f984b-178">notes</span></span>|<span data-ttu-id="f984b-179">String</span><span class="sxs-lookup"><span data-stu-id="f984b-179">String</span></span>|<span data-ttu-id="f984b-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="f984b-180">Notes for the app.</span></span> <span data-ttu-id="f984b-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f984b-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="f984b-182">publishingState</span></span>|[<span data-ttu-id="f984b-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f984b-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f984b-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="f984b-184">The publishing state for the app.</span></span> <span data-ttu-id="f984b-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="f984b-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f984b-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="f984b-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f984b-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="f984b-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f984b-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="f984b-188">appAvailability</span></span>|[<span data-ttu-id="f984b-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="f984b-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="f984b-190">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="f984b-190">The Application's availability.</span></span> <span data-ttu-id="f984b-191">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="f984b-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="f984b-192">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="f984b-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="f984b-193">version</span><span class="sxs-lookup"><span data-stu-id="f984b-193">version</span></span>|<span data-ttu-id="f984b-194">String</span><span class="sxs-lookup"><span data-stu-id="f984b-194">String</span></span>|<span data-ttu-id="f984b-195">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="f984b-195">The Application's version.</span></span> <span data-ttu-id="f984b-196">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="f984b-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f984b-197">committedContentVersion</span></span>|<span data-ttu-id="f984b-198">String</span><span class="sxs-lookup"><span data-stu-id="f984b-198">String</span></span>|<span data-ttu-id="f984b-199">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="f984b-199">The internal committed content version.</span></span> <span data-ttu-id="f984b-200">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f984b-201">fileName</span><span class="sxs-lookup"><span data-stu-id="f984b-201">fileName</span></span>|<span data-ttu-id="f984b-202">String</span><span class="sxs-lookup"><span data-stu-id="f984b-202">String</span></span>|<span data-ttu-id="f984b-203">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="f984b-203">The name of the main Lob application file.</span></span> <span data-ttu-id="f984b-204">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f984b-205">size</span><span class="sxs-lookup"><span data-stu-id="f984b-205">size</span></span>|<span data-ttu-id="f984b-206">Int64</span><span class="sxs-lookup"><span data-stu-id="f984b-206">Int64</span></span>|<span data-ttu-id="f984b-207">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="f984b-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="f984b-208">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f984b-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f984b-209">bundleId</span><span class="sxs-lookup"><span data-stu-id="f984b-209">bundleId</span></span>|<span data-ttu-id="f984b-210">String</span><span class="sxs-lookup"><span data-stu-id="f984b-210">String</span></span>|<span data-ttu-id="f984b-211">标识名称。</span><span class="sxs-lookup"><span data-stu-id="f984b-211">The Identity Name.</span></span>|
|<span data-ttu-id="f984b-212">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="f984b-212">applicableDeviceType</span></span>|[<span data-ttu-id="f984b-213">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="f984b-213">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="f984b-214">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="f984b-214">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="f984b-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f984b-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f984b-216">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f984b-216">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="f984b-217">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="f984b-217">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f984b-218">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f984b-218">expirationDateTime</span></span>|<span data-ttu-id="f984b-219">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f984b-219">DateTimeOffset</span></span>|<span data-ttu-id="f984b-220">过期时间。</span><span class="sxs-lookup"><span data-stu-id="f984b-220">The expiration time.</span></span>|
|<span data-ttu-id="f984b-221">versionNumber</span><span class="sxs-lookup"><span data-stu-id="f984b-221">versionNumber</span></span>|<span data-ttu-id="f984b-222">String</span><span class="sxs-lookup"><span data-stu-id="f984b-222">String</span></span>|<span data-ttu-id="f984b-223">托管 iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="f984b-223">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f984b-224">buildNumber</span><span class="sxs-lookup"><span data-stu-id="f984b-224">buildNumber</span></span>|<span data-ttu-id="f984b-225">String</span><span class="sxs-lookup"><span data-stu-id="f984b-225">String</span></span>|<span data-ttu-id="f984b-226">托管 iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="f984b-226">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="f984b-227">响应</span><span class="sxs-lookup"><span data-stu-id="f984b-227">Response</span></span>
<span data-ttu-id="f984b-228">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f984b-228">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f984b-229">示例</span><span class="sxs-lookup"><span data-stu-id="f984b-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="f984b-230">请求</span><span class="sxs-lookup"><span data-stu-id="f984b-230">Request</span></span>
<span data-ttu-id="f984b-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f984b-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="f984b-232">响应</span><span class="sxs-lookup"><span data-stu-id="f984b-232">Response</span></span>
<span data-ttu-id="f984b-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f984b-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



