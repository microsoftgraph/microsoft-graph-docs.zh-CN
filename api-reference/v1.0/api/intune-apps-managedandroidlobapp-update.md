---
title: 更新 managedAndroidLobApp
description: 更新 managedAndroidLobApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b00e4bbe0b4dff1a45e9ffe89c59edc4379b1b89
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578608"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="e39db-103">更新 managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="e39db-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="e39db-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e39db-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e39db-105">更新 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e39db-105">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e39db-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="e39db-106">Prerequisites</span></span>
<span data-ttu-id="e39db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e39db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e39db-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e39db-109">Permission type</span></span>|<span data-ttu-id="e39db-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e39db-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e39db-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e39db-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e39db-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e39db-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e39db-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e39db-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e39db-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e39db-114">Not supported.</span></span>|
|<span data-ttu-id="e39db-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e39db-115">Application</span></span>|<span data-ttu-id="e39db-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e39db-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e39db-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e39db-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="e39db-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e39db-118">Request headers</span></span>
|<span data-ttu-id="e39db-119">标头</span><span class="sxs-lookup"><span data-stu-id="e39db-119">Header</span></span>|<span data-ttu-id="e39db-120">值</span><span class="sxs-lookup"><span data-stu-id="e39db-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e39db-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e39db-121">Authorization</span></span>|<span data-ttu-id="e39db-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e39db-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e39db-123">接受</span><span class="sxs-lookup"><span data-stu-id="e39db-123">Accept</span></span>|<span data-ttu-id="e39db-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e39db-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e39db-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e39db-125">Request body</span></span>
<span data-ttu-id="e39db-126">在请求正文中，提供 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e39db-126">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="e39db-127">下表显示了创建 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e39db-127">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="e39db-128">属性</span><span class="sxs-lookup"><span data-stu-id="e39db-128">Property</span></span>|<span data-ttu-id="e39db-129">类型</span><span class="sxs-lookup"><span data-stu-id="e39db-129">Type</span></span>|<span data-ttu-id="e39db-130">说明</span><span class="sxs-lookup"><span data-stu-id="e39db-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e39db-131">id</span><span class="sxs-lookup"><span data-stu-id="e39db-131">id</span></span>|<span data-ttu-id="e39db-132">字符串</span><span class="sxs-lookup"><span data-stu-id="e39db-132">String</span></span>|<span data-ttu-id="e39db-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e39db-133">Key of the entity.</span></span> <span data-ttu-id="e39db-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39db-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e39db-135">displayName</span></span>|<span data-ttu-id="e39db-136">String</span><span class="sxs-lookup"><span data-stu-id="e39db-136">String</span></span>|<span data-ttu-id="e39db-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="e39db-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e39db-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39db-139">说明</span><span class="sxs-lookup"><span data-stu-id="e39db-139">description</span></span>|<span data-ttu-id="e39db-140">String</span><span class="sxs-lookup"><span data-stu-id="e39db-140">String</span></span>|<span data-ttu-id="e39db-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="e39db-141">The description of the app.</span></span> <span data-ttu-id="e39db-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39db-143">publisher</span><span class="sxs-lookup"><span data-stu-id="e39db-143">publisher</span></span>|<span data-ttu-id="e39db-144">String</span><span class="sxs-lookup"><span data-stu-id="e39db-144">String</span></span>|<span data-ttu-id="e39db-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="e39db-145">The publisher of the app.</span></span> <span data-ttu-id="e39db-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39db-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e39db-147">largeIcon</span></span>|[<span data-ttu-id="e39db-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e39db-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e39db-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="e39db-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e39db-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39db-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e39db-151">createdDateTime</span></span>|<span data-ttu-id="e39db-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e39db-152">DateTimeOffset</span></span>|<span data-ttu-id="e39db-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e39db-153">The date and time the app was created.</span></span> <span data-ttu-id="e39db-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39db-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e39db-155">lastModifiedDateTime</span></span>|<span data-ttu-id="e39db-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e39db-156">DateTimeOffset</span></span>|<span data-ttu-id="e39db-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e39db-157">The date and time the app was last modified.</span></span> <span data-ttu-id="e39db-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39db-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e39db-159">isFeatured</span></span>|<span data-ttu-id="e39db-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="e39db-160">Boolean</span></span>|<span data-ttu-id="e39db-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39db-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e39db-162">privacyInformationUrl</span></span>|<span data-ttu-id="e39db-163">String</span><span class="sxs-lookup"><span data-stu-id="e39db-163">String</span></span>|<span data-ttu-id="e39db-164">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="e39db-164">The privacy statement Url.</span></span> <span data-ttu-id="e39db-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39db-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e39db-166">informationUrl</span></span>|<span data-ttu-id="e39db-167">String</span><span class="sxs-lookup"><span data-stu-id="e39db-167">String</span></span>|<span data-ttu-id="e39db-168">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="e39db-168">The more information Url.</span></span> <span data-ttu-id="e39db-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39db-170">owner</span><span class="sxs-lookup"><span data-stu-id="e39db-170">owner</span></span>|<span data-ttu-id="e39db-171">字符串</span><span class="sxs-lookup"><span data-stu-id="e39db-171">String</span></span>|<span data-ttu-id="e39db-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="e39db-172">The owner of the app.</span></span> <span data-ttu-id="e39db-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39db-174">developer</span><span class="sxs-lookup"><span data-stu-id="e39db-174">developer</span></span>|<span data-ttu-id="e39db-175">String</span><span class="sxs-lookup"><span data-stu-id="e39db-175">String</span></span>|<span data-ttu-id="e39db-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="e39db-176">The developer of the app.</span></span> <span data-ttu-id="e39db-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39db-178">notes</span><span class="sxs-lookup"><span data-stu-id="e39db-178">notes</span></span>|<span data-ttu-id="e39db-179">String</span><span class="sxs-lookup"><span data-stu-id="e39db-179">String</span></span>|<span data-ttu-id="e39db-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="e39db-180">Notes for the app.</span></span> <span data-ttu-id="e39db-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e39db-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="e39db-182">publishingState</span></span>|[<span data-ttu-id="e39db-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e39db-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e39db-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="e39db-184">The publishing state for the app.</span></span> <span data-ttu-id="e39db-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="e39db-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e39db-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="e39db-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e39db-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="e39db-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e39db-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="e39db-188">appAvailability</span></span>|[<span data-ttu-id="e39db-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="e39db-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="e39db-190">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="e39db-190">The Application's availability.</span></span> <span data-ttu-id="e39db-191">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="e39db-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="e39db-192">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="e39db-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="e39db-193">version</span><span class="sxs-lookup"><span data-stu-id="e39db-193">version</span></span>|<span data-ttu-id="e39db-194">String</span><span class="sxs-lookup"><span data-stu-id="e39db-194">String</span></span>|<span data-ttu-id="e39db-195">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="e39db-195">The Application's version.</span></span> <span data-ttu-id="e39db-196">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="e39db-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e39db-197">committedContentVersion</span></span>|<span data-ttu-id="e39db-198">String</span><span class="sxs-lookup"><span data-stu-id="e39db-198">String</span></span>|<span data-ttu-id="e39db-199">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="e39db-199">The internal committed content version.</span></span> <span data-ttu-id="e39db-200">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e39db-201">fileName</span><span class="sxs-lookup"><span data-stu-id="e39db-201">fileName</span></span>|<span data-ttu-id="e39db-202">String</span><span class="sxs-lookup"><span data-stu-id="e39db-202">String</span></span>|<span data-ttu-id="e39db-203">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="e39db-203">The name of the main Lob application file.</span></span> <span data-ttu-id="e39db-204">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e39db-205">size</span><span class="sxs-lookup"><span data-stu-id="e39db-205">size</span></span>|<span data-ttu-id="e39db-206">Int64</span><span class="sxs-lookup"><span data-stu-id="e39db-206">Int64</span></span>|<span data-ttu-id="e39db-207">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="e39db-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="e39db-208">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e39db-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="e39db-209">packageId</span><span class="sxs-lookup"><span data-stu-id="e39db-209">packageId</span></span>|<span data-ttu-id="e39db-210">String</span><span class="sxs-lookup"><span data-stu-id="e39db-210">String</span></span>|<span data-ttu-id="e39db-211">包标识符。</span><span class="sxs-lookup"><span data-stu-id="e39db-211">The package identifier.</span></span>|
|<span data-ttu-id="e39db-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e39db-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e39db-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e39db-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="e39db-214">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="e39db-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e39db-215">versionName</span><span class="sxs-lookup"><span data-stu-id="e39db-215">versionName</span></span>|<span data-ttu-id="e39db-216">String</span><span class="sxs-lookup"><span data-stu-id="e39db-216">String</span></span>|<span data-ttu-id="e39db-217">托管 Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="e39db-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e39db-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="e39db-218">versionCode</span></span>|<span data-ttu-id="e39db-219">String</span><span class="sxs-lookup"><span data-stu-id="e39db-219">String</span></span>|<span data-ttu-id="e39db-220">托管 Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="e39db-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="e39db-221">响应</span><span class="sxs-lookup"><span data-stu-id="e39db-221">Response</span></span>
<span data-ttu-id="e39db-222">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e39db-222">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e39db-223">示例</span><span class="sxs-lookup"><span data-stu-id="e39db-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="e39db-224">请求</span><span class="sxs-lookup"><span data-stu-id="e39db-224">Request</span></span>
<span data-ttu-id="e39db-225">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e39db-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1153

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="e39db-226">响应</span><span class="sxs-lookup"><span data-stu-id="e39db-226">Response</span></span>
<span data-ttu-id="e39db-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e39db-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1325

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```



