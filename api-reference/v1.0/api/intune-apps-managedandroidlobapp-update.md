---
title: 更新 managedAndroidLobApp
description: 更新 managedAndroidLobApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 66d94d9bca1d83ba8d99afb218451667848f90e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813235"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="a4776-103">更新 managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="a4776-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="a4776-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a4776-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4776-105">更新 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a4776-105">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a4776-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4776-106">Prerequisites</span></span>
<span data-ttu-id="a4776-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a4776-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4776-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4776-109">Permission type</span></span>|<span data-ttu-id="a4776-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a4776-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4776-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4776-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4776-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4776-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a4776-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4776-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4776-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4776-114">Not supported.</span></span>|
|<span data-ttu-id="a4776-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4776-115">Application</span></span>|<span data-ttu-id="a4776-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4776-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4776-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4776-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="a4776-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4776-118">Request headers</span></span>
|<span data-ttu-id="a4776-119">标头</span><span class="sxs-lookup"><span data-stu-id="a4776-119">Header</span></span>|<span data-ttu-id="a4776-120">值</span><span class="sxs-lookup"><span data-stu-id="a4776-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4776-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4776-121">Authorization</span></span>|<span data-ttu-id="a4776-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4776-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4776-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a4776-123">Accept</span></span>|<span data-ttu-id="a4776-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a4776-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4776-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4776-125">Request body</span></span>
<span data-ttu-id="a4776-126">在请求正文中，提供 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4776-126">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="a4776-127">下表显示了创建 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a4776-127">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="a4776-128">属性</span><span class="sxs-lookup"><span data-stu-id="a4776-128">Property</span></span>|<span data-ttu-id="a4776-129">类型</span><span class="sxs-lookup"><span data-stu-id="a4776-129">Type</span></span>|<span data-ttu-id="a4776-130">说明</span><span class="sxs-lookup"><span data-stu-id="a4776-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4776-131">id</span><span class="sxs-lookup"><span data-stu-id="a4776-131">id</span></span>|<span data-ttu-id="a4776-132">String</span><span class="sxs-lookup"><span data-stu-id="a4776-132">String</span></span>|<span data-ttu-id="a4776-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a4776-133">Key of the entity.</span></span> <span data-ttu-id="a4776-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4776-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a4776-135">displayName</span></span>|<span data-ttu-id="a4776-136">String</span><span class="sxs-lookup"><span data-stu-id="a4776-136">String</span></span>|<span data-ttu-id="a4776-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="a4776-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a4776-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4776-139">description</span><span class="sxs-lookup"><span data-stu-id="a4776-139">description</span></span>|<span data-ttu-id="a4776-140">String</span><span class="sxs-lookup"><span data-stu-id="a4776-140">String</span></span>|<span data-ttu-id="a4776-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="a4776-141">The description of the app.</span></span> <span data-ttu-id="a4776-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4776-143">publisher</span><span class="sxs-lookup"><span data-stu-id="a4776-143">publisher</span></span>|<span data-ttu-id="a4776-144">String</span><span class="sxs-lookup"><span data-stu-id="a4776-144">String</span></span>|<span data-ttu-id="a4776-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="a4776-145">The publisher of the app.</span></span> <span data-ttu-id="a4776-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4776-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a4776-147">largeIcon</span></span>|[<span data-ttu-id="a4776-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a4776-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a4776-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="a4776-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a4776-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4776-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4776-151">createdDateTime</span></span>|<span data-ttu-id="a4776-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4776-152">DateTimeOffset</span></span>|<span data-ttu-id="a4776-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a4776-153">The date and time the app was created.</span></span> <span data-ttu-id="a4776-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4776-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4776-155">lastModifiedDateTime</span></span>|<span data-ttu-id="a4776-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4776-156">DateTimeOffset</span></span>|<span data-ttu-id="a4776-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a4776-157">The date and time the app was last modified.</span></span> <span data-ttu-id="a4776-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4776-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a4776-159">isFeatured</span></span>|<span data-ttu-id="a4776-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4776-160">Boolean</span></span>|<span data-ttu-id="a4776-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4776-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a4776-162">privacyInformationUrl</span></span>|<span data-ttu-id="a4776-163">String</span><span class="sxs-lookup"><span data-stu-id="a4776-163">String</span></span>|<span data-ttu-id="a4776-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="a4776-164">The privacy statement Url.</span></span> <span data-ttu-id="a4776-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4776-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a4776-166">informationUrl</span></span>|<span data-ttu-id="a4776-167">String</span><span class="sxs-lookup"><span data-stu-id="a4776-167">String</span></span>|<span data-ttu-id="a4776-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="a4776-168">The more information Url.</span></span> <span data-ttu-id="a4776-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4776-170">owner</span><span class="sxs-lookup"><span data-stu-id="a4776-170">owner</span></span>|<span data-ttu-id="a4776-171">String</span><span class="sxs-lookup"><span data-stu-id="a4776-171">String</span></span>|<span data-ttu-id="a4776-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="a4776-172">The owner of the app.</span></span> <span data-ttu-id="a4776-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4776-174">developer</span><span class="sxs-lookup"><span data-stu-id="a4776-174">developer</span></span>|<span data-ttu-id="a4776-175">String</span><span class="sxs-lookup"><span data-stu-id="a4776-175">String</span></span>|<span data-ttu-id="a4776-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="a4776-176">The developer of the app.</span></span> <span data-ttu-id="a4776-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4776-178">notes</span><span class="sxs-lookup"><span data-stu-id="a4776-178">notes</span></span>|<span data-ttu-id="a4776-179">String</span><span class="sxs-lookup"><span data-stu-id="a4776-179">String</span></span>|<span data-ttu-id="a4776-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="a4776-180">Notes for the app.</span></span> <span data-ttu-id="a4776-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4776-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="a4776-182">publishingState</span></span>|[<span data-ttu-id="a4776-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a4776-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a4776-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="a4776-184">The publishing state for the app.</span></span> <span data-ttu-id="a4776-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="a4776-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a4776-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="a4776-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a4776-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="a4776-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a4776-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="a4776-188">appAvailability</span></span>|[<span data-ttu-id="a4776-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="a4776-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="a4776-190">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="a4776-190">The Application's availability.</span></span> <span data-ttu-id="a4776-191">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="a4776-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="a4776-192">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="a4776-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="a4776-193">version</span><span class="sxs-lookup"><span data-stu-id="a4776-193">version</span></span>|<span data-ttu-id="a4776-194">String</span><span class="sxs-lookup"><span data-stu-id="a4776-194">String</span></span>|<span data-ttu-id="a4776-195">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="a4776-195">The Application's version.</span></span> <span data-ttu-id="a4776-196">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="a4776-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a4776-197">committedContentVersion</span></span>|<span data-ttu-id="a4776-198">String</span><span class="sxs-lookup"><span data-stu-id="a4776-198">String</span></span>|<span data-ttu-id="a4776-199">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="a4776-199">The internal committed content version.</span></span> <span data-ttu-id="a4776-200">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a4776-201">fileName</span><span class="sxs-lookup"><span data-stu-id="a4776-201">fileName</span></span>|<span data-ttu-id="a4776-202">String</span><span class="sxs-lookup"><span data-stu-id="a4776-202">String</span></span>|<span data-ttu-id="a4776-203">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="a4776-203">The name of the main Lob application file.</span></span> <span data-ttu-id="a4776-204">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a4776-205">size</span><span class="sxs-lookup"><span data-stu-id="a4776-205">size</span></span>|<span data-ttu-id="a4776-206">Int64</span><span class="sxs-lookup"><span data-stu-id="a4776-206">Int64</span></span>|<span data-ttu-id="a4776-207">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="a4776-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="a4776-208">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4776-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a4776-209">packageId</span><span class="sxs-lookup"><span data-stu-id="a4776-209">packageId</span></span>|<span data-ttu-id="a4776-210">String</span><span class="sxs-lookup"><span data-stu-id="a4776-210">String</span></span>|<span data-ttu-id="a4776-211">包标识符。</span><span class="sxs-lookup"><span data-stu-id="a4776-211">The package identifier.</span></span>|
|<span data-ttu-id="a4776-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a4776-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a4776-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a4776-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="a4776-214">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="a4776-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="a4776-215">versionName</span><span class="sxs-lookup"><span data-stu-id="a4776-215">versionName</span></span>|<span data-ttu-id="a4776-216">String</span><span class="sxs-lookup"><span data-stu-id="a4776-216">String</span></span>|<span data-ttu-id="a4776-217">托管 Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="a4776-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="a4776-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="a4776-218">versionCode</span></span>|<span data-ttu-id="a4776-219">String</span><span class="sxs-lookup"><span data-stu-id="a4776-219">String</span></span>|<span data-ttu-id="a4776-220">托管 Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="a4776-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="a4776-221">响应</span><span class="sxs-lookup"><span data-stu-id="a4776-221">Response</span></span>
<span data-ttu-id="a4776-222">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a4776-222">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4776-223">示例</span><span class="sxs-lookup"><span data-stu-id="a4776-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="a4776-224">请求</span><span class="sxs-lookup"><span data-stu-id="a4776-224">Request</span></span>
<span data-ttu-id="a4776-225">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4776-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a4776-226">响应</span><span class="sxs-lookup"><span data-stu-id="a4776-226">Response</span></span>
<span data-ttu-id="a4776-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4776-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



