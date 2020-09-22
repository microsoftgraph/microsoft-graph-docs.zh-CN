---
title: 更新 managedIOSLobApp
description: 更新 managedIOSLobApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5532d5e68dfa2adb085cad2dc5924edb61e020c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992284"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="8c185-103">更新 managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="8c185-103">Update managedIOSLobApp</span></span>

<span data-ttu-id="8c185-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c185-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c185-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c185-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c185-106">更新 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8c185-106">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8c185-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8c185-107">Prerequisites</span></span>
<span data-ttu-id="8c185-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8c185-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8c185-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c185-110">Permission type</span></span>|<span data-ttu-id="8c185-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8c185-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c185-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c185-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8c185-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c185-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c185-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c185-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c185-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c185-115">Not supported.</span></span>|
|<span data-ttu-id="8c185-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c185-116">Application</span></span>|<span data-ttu-id="8c185-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c185-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c185-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c185-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="8c185-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c185-119">Request headers</span></span>
|<span data-ttu-id="8c185-120">标头</span><span class="sxs-lookup"><span data-stu-id="8c185-120">Header</span></span>|<span data-ttu-id="8c185-121">值</span><span class="sxs-lookup"><span data-stu-id="8c185-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c185-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c185-122">Authorization</span></span>|<span data-ttu-id="8c185-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8c185-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c185-124">接受</span><span class="sxs-lookup"><span data-stu-id="8c185-124">Accept</span></span>|<span data-ttu-id="8c185-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8c185-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c185-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c185-126">Request body</span></span>
<span data-ttu-id="8c185-127">在请求正文中，提供 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c185-127">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="8c185-128">下表显示创建 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8c185-128">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="8c185-129">属性</span><span class="sxs-lookup"><span data-stu-id="8c185-129">Property</span></span>|<span data-ttu-id="8c185-130">类型</span><span class="sxs-lookup"><span data-stu-id="8c185-130">Type</span></span>|<span data-ttu-id="8c185-131">说明</span><span class="sxs-lookup"><span data-stu-id="8c185-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c185-132">id</span><span class="sxs-lookup"><span data-stu-id="8c185-132">id</span></span>|<span data-ttu-id="8c185-133">String</span><span class="sxs-lookup"><span data-stu-id="8c185-133">String</span></span>|<span data-ttu-id="8c185-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8c185-134">Key of the entity.</span></span> <span data-ttu-id="8c185-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c185-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8c185-136">displayName</span></span>|<span data-ttu-id="8c185-137">String</span><span class="sxs-lookup"><span data-stu-id="8c185-137">String</span></span>|<span data-ttu-id="8c185-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="8c185-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8c185-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c185-140">description</span><span class="sxs-lookup"><span data-stu-id="8c185-140">description</span></span>|<span data-ttu-id="8c185-141">String</span><span class="sxs-lookup"><span data-stu-id="8c185-141">String</span></span>|<span data-ttu-id="8c185-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="8c185-142">The description of the app.</span></span> <span data-ttu-id="8c185-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c185-144">publisher</span><span class="sxs-lookup"><span data-stu-id="8c185-144">publisher</span></span>|<span data-ttu-id="8c185-145">String</span><span class="sxs-lookup"><span data-stu-id="8c185-145">String</span></span>|<span data-ttu-id="8c185-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="8c185-146">The publisher of the app.</span></span> <span data-ttu-id="8c185-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c185-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8c185-148">largeIcon</span></span>|[<span data-ttu-id="8c185-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8c185-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8c185-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="8c185-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8c185-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c185-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c185-152">createdDateTime</span></span>|<span data-ttu-id="8c185-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c185-153">DateTimeOffset</span></span>|<span data-ttu-id="8c185-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8c185-154">The date and time the app was created.</span></span> <span data-ttu-id="8c185-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c185-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c185-156">lastModifiedDateTime</span></span>|<span data-ttu-id="8c185-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c185-157">DateTimeOffset</span></span>|<span data-ttu-id="8c185-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8c185-158">The date and time the app was last modified.</span></span> <span data-ttu-id="8c185-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c185-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8c185-160">isFeatured</span></span>|<span data-ttu-id="8c185-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c185-161">Boolean</span></span>|<span data-ttu-id="8c185-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c185-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8c185-163">privacyInformationUrl</span></span>|<span data-ttu-id="8c185-164">String</span><span class="sxs-lookup"><span data-stu-id="8c185-164">String</span></span>|<span data-ttu-id="8c185-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="8c185-165">The privacy statement Url.</span></span> <span data-ttu-id="8c185-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c185-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8c185-167">informationUrl</span></span>|<span data-ttu-id="8c185-168">String</span><span class="sxs-lookup"><span data-stu-id="8c185-168">String</span></span>|<span data-ttu-id="8c185-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="8c185-169">The more information Url.</span></span> <span data-ttu-id="8c185-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c185-171">所有者</span><span class="sxs-lookup"><span data-stu-id="8c185-171">owner</span></span>|<span data-ttu-id="8c185-172">String</span><span class="sxs-lookup"><span data-stu-id="8c185-172">String</span></span>|<span data-ttu-id="8c185-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="8c185-173">The owner of the app.</span></span> <span data-ttu-id="8c185-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c185-175">developer</span><span class="sxs-lookup"><span data-stu-id="8c185-175">developer</span></span>|<span data-ttu-id="8c185-176">String</span><span class="sxs-lookup"><span data-stu-id="8c185-176">String</span></span>|<span data-ttu-id="8c185-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="8c185-177">The developer of the app.</span></span> <span data-ttu-id="8c185-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c185-179">notes</span><span class="sxs-lookup"><span data-stu-id="8c185-179">notes</span></span>|<span data-ttu-id="8c185-180">String</span><span class="sxs-lookup"><span data-stu-id="8c185-180">String</span></span>|<span data-ttu-id="8c185-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="8c185-181">Notes for the app.</span></span> <span data-ttu-id="8c185-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8c185-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="8c185-183">publishingState</span></span>|[<span data-ttu-id="8c185-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8c185-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8c185-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="8c185-185">The publishing state for the app.</span></span> <span data-ttu-id="8c185-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="8c185-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8c185-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="8c185-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8c185-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="8c185-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8c185-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="8c185-189">appAvailability</span></span>|[<span data-ttu-id="8c185-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="8c185-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="8c185-191">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="8c185-191">The Application's availability.</span></span> <span data-ttu-id="8c185-192">继承自 [managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="8c185-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="8c185-193">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="8c185-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="8c185-194">version</span><span class="sxs-lookup"><span data-stu-id="8c185-194">version</span></span>|<span data-ttu-id="8c185-195">String</span><span class="sxs-lookup"><span data-stu-id="8c185-195">String</span></span>|<span data-ttu-id="8c185-196">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="8c185-196">The Application's version.</span></span> <span data-ttu-id="8c185-197">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="8c185-198">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8c185-198">committedContentVersion</span></span>|<span data-ttu-id="8c185-199">String</span><span class="sxs-lookup"><span data-stu-id="8c185-199">String</span></span>|<span data-ttu-id="8c185-200">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="8c185-200">The internal committed content version.</span></span> <span data-ttu-id="8c185-201">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-201">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="8c185-202">fileName</span><span class="sxs-lookup"><span data-stu-id="8c185-202">fileName</span></span>|<span data-ttu-id="8c185-203">String</span><span class="sxs-lookup"><span data-stu-id="8c185-203">String</span></span>|<span data-ttu-id="8c185-204">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="8c185-204">The name of the main Lob application file.</span></span> <span data-ttu-id="8c185-205">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-205">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="8c185-206">size</span><span class="sxs-lookup"><span data-stu-id="8c185-206">size</span></span>|<span data-ttu-id="8c185-207">Int64</span><span class="sxs-lookup"><span data-stu-id="8c185-207">Int64</span></span>|<span data-ttu-id="8c185-208">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="8c185-208">The total size, including all uploaded files.</span></span> <span data-ttu-id="8c185-209">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8c185-209">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="8c185-210">bundleId</span><span class="sxs-lookup"><span data-stu-id="8c185-210">bundleId</span></span>|<span data-ttu-id="8c185-211">String</span><span class="sxs-lookup"><span data-stu-id="8c185-211">String</span></span>|<span data-ttu-id="8c185-212">标识名称。</span><span class="sxs-lookup"><span data-stu-id="8c185-212">The Identity Name.</span></span>|
|<span data-ttu-id="8c185-213">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="8c185-213">applicableDeviceType</span></span>|[<span data-ttu-id="8c185-214">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="8c185-214">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="8c185-215">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="8c185-215">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="8c185-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8c185-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8c185-217">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8c185-217">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="8c185-218">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="8c185-218">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="8c185-219">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8c185-219">expirationDateTime</span></span>|<span data-ttu-id="8c185-220">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c185-220">DateTimeOffset</span></span>|<span data-ttu-id="8c185-221">过期时间。</span><span class="sxs-lookup"><span data-stu-id="8c185-221">The expiration time.</span></span>|
|<span data-ttu-id="8c185-222">versionNumber</span><span class="sxs-lookup"><span data-stu-id="8c185-222">versionNumber</span></span>|<span data-ttu-id="8c185-223">String</span><span class="sxs-lookup"><span data-stu-id="8c185-223">String</span></span>|<span data-ttu-id="8c185-224">托管 iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="8c185-224">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8c185-225">buildNumber</span><span class="sxs-lookup"><span data-stu-id="8c185-225">buildNumber</span></span>|<span data-ttu-id="8c185-226">String</span><span class="sxs-lookup"><span data-stu-id="8c185-226">String</span></span>|<span data-ttu-id="8c185-227">托管 iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="8c185-227">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="8c185-228">响应</span><span class="sxs-lookup"><span data-stu-id="8c185-228">Response</span></span>
<span data-ttu-id="8c185-229">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8c185-229">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c185-230">示例</span><span class="sxs-lookup"><span data-stu-id="8c185-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c185-231">请求</span><span class="sxs-lookup"><span data-stu-id="8c185-231">Request</span></span>
<span data-ttu-id="8c185-232">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8c185-232">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1307

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
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="8c185-233">响应</span><span class="sxs-lookup"><span data-stu-id="8c185-233">Response</span></span>
<span data-ttu-id="8c185-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8c185-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1479

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
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```









