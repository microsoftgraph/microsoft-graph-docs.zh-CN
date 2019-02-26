---
title: 更新 managedAndroidLobApp
description: 更新 managedAndroidLobApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24d985046fa7fad39e121466e27c99c16909cd5b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261416"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="1f498-103">更新 managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="1f498-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="1f498-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1f498-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f498-105">更新 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1f498-105">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f498-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="1f498-106">Prerequisites</span></span>
<span data-ttu-id="1f498-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1f498-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1f498-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f498-109">Permission type</span></span>|<span data-ttu-id="1f498-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1f498-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f498-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f498-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1f498-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f498-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1f498-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f498-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f498-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f498-114">Not supported.</span></span>|
|<span data-ttu-id="1f498-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f498-115">Application</span></span>|<span data-ttu-id="1f498-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f498-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f498-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f498-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="1f498-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f498-118">Request headers</span></span>
|<span data-ttu-id="1f498-119">标头</span><span class="sxs-lookup"><span data-stu-id="1f498-119">Header</span></span>|<span data-ttu-id="1f498-120">值</span><span class="sxs-lookup"><span data-stu-id="1f498-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f498-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f498-121">Authorization</span></span>|<span data-ttu-id="1f498-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1f498-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f498-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1f498-123">Accept</span></span>|<span data-ttu-id="1f498-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1f498-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f498-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f498-125">Request body</span></span>
<span data-ttu-id="1f498-126">在请求正文中，提供 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f498-126">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="1f498-127">下表显示了创建 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1f498-127">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="1f498-128">属性</span><span class="sxs-lookup"><span data-stu-id="1f498-128">Property</span></span>|<span data-ttu-id="1f498-129">类型</span><span class="sxs-lookup"><span data-stu-id="1f498-129">Type</span></span>|<span data-ttu-id="1f498-130">说明</span><span class="sxs-lookup"><span data-stu-id="1f498-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f498-131">id</span><span class="sxs-lookup"><span data-stu-id="1f498-131">id</span></span>|<span data-ttu-id="1f498-132">字符串</span><span class="sxs-lookup"><span data-stu-id="1f498-132">String</span></span>|<span data-ttu-id="1f498-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1f498-133">Key of the entity.</span></span> <span data-ttu-id="1f498-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f498-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1f498-135">displayName</span></span>|<span data-ttu-id="1f498-136">String</span><span class="sxs-lookup"><span data-stu-id="1f498-136">String</span></span>|<span data-ttu-id="1f498-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="1f498-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1f498-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f498-139">description</span><span class="sxs-lookup"><span data-stu-id="1f498-139">description</span></span>|<span data-ttu-id="1f498-140">字符串</span><span class="sxs-lookup"><span data-stu-id="1f498-140">String</span></span>|<span data-ttu-id="1f498-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="1f498-141">The description of the app.</span></span> <span data-ttu-id="1f498-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f498-143">publisher</span><span class="sxs-lookup"><span data-stu-id="1f498-143">publisher</span></span>|<span data-ttu-id="1f498-144">String</span><span class="sxs-lookup"><span data-stu-id="1f498-144">String</span></span>|<span data-ttu-id="1f498-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="1f498-145">The publisher of the app.</span></span> <span data-ttu-id="1f498-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f498-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1f498-147">largeIcon</span></span>|[<span data-ttu-id="1f498-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1f498-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1f498-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="1f498-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1f498-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f498-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f498-151">createdDateTime</span></span>|<span data-ttu-id="1f498-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f498-152">DateTimeOffset</span></span>|<span data-ttu-id="1f498-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1f498-153">The date and time the app was created.</span></span> <span data-ttu-id="1f498-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f498-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f498-155">lastModifiedDateTime</span></span>|<span data-ttu-id="1f498-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f498-156">DateTimeOffset</span></span>|<span data-ttu-id="1f498-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1f498-157">The date and time the app was last modified.</span></span> <span data-ttu-id="1f498-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f498-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1f498-159">isFeatured</span></span>|<span data-ttu-id="1f498-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f498-160">Boolean</span></span>|<span data-ttu-id="1f498-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f498-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1f498-162">privacyInformationUrl</span></span>|<span data-ttu-id="1f498-163">String</span><span class="sxs-lookup"><span data-stu-id="1f498-163">String</span></span>|<span data-ttu-id="1f498-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="1f498-164">The privacy statement Url.</span></span> <span data-ttu-id="1f498-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f498-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1f498-166">informationUrl</span></span>|<span data-ttu-id="1f498-167">String</span><span class="sxs-lookup"><span data-stu-id="1f498-167">String</span></span>|<span data-ttu-id="1f498-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="1f498-168">The more information Url.</span></span> <span data-ttu-id="1f498-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f498-170">owner</span><span class="sxs-lookup"><span data-stu-id="1f498-170">owner</span></span>|<span data-ttu-id="1f498-171">String</span><span class="sxs-lookup"><span data-stu-id="1f498-171">String</span></span>|<span data-ttu-id="1f498-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="1f498-172">The owner of the app.</span></span> <span data-ttu-id="1f498-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f498-174">developer</span><span class="sxs-lookup"><span data-stu-id="1f498-174">developer</span></span>|<span data-ttu-id="1f498-175">String</span><span class="sxs-lookup"><span data-stu-id="1f498-175">String</span></span>|<span data-ttu-id="1f498-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="1f498-176">The developer of the app.</span></span> <span data-ttu-id="1f498-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f498-178">notes</span><span class="sxs-lookup"><span data-stu-id="1f498-178">notes</span></span>|<span data-ttu-id="1f498-179">String</span><span class="sxs-lookup"><span data-stu-id="1f498-179">String</span></span>|<span data-ttu-id="1f498-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="1f498-180">Notes for the app.</span></span> <span data-ttu-id="1f498-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f498-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="1f498-182">publishingState</span></span>|[<span data-ttu-id="1f498-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1f498-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1f498-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="1f498-184">The publishing state for the app.</span></span> <span data-ttu-id="1f498-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="1f498-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1f498-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="1f498-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1f498-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="1f498-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1f498-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="1f498-188">appAvailability</span></span>|[<span data-ttu-id="1f498-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="1f498-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="1f498-190">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="1f498-190">The Application's availability.</span></span> <span data-ttu-id="1f498-191">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="1f498-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="1f498-192">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="1f498-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="1f498-193">version</span><span class="sxs-lookup"><span data-stu-id="1f498-193">version</span></span>|<span data-ttu-id="1f498-194">String</span><span class="sxs-lookup"><span data-stu-id="1f498-194">String</span></span>|<span data-ttu-id="1f498-195">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="1f498-195">The Application's version.</span></span> <span data-ttu-id="1f498-196">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="1f498-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1f498-197">committedContentVersion</span></span>|<span data-ttu-id="1f498-198">String</span><span class="sxs-lookup"><span data-stu-id="1f498-198">String</span></span>|<span data-ttu-id="1f498-199">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="1f498-199">The internal committed content version.</span></span> <span data-ttu-id="1f498-200">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="1f498-201">fileName</span><span class="sxs-lookup"><span data-stu-id="1f498-201">fileName</span></span>|<span data-ttu-id="1f498-202">String</span><span class="sxs-lookup"><span data-stu-id="1f498-202">String</span></span>|<span data-ttu-id="1f498-203">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="1f498-203">The name of the main Lob application file.</span></span> <span data-ttu-id="1f498-204">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="1f498-205">size</span><span class="sxs-lookup"><span data-stu-id="1f498-205">size</span></span>|<span data-ttu-id="1f498-206">Int64</span><span class="sxs-lookup"><span data-stu-id="1f498-206">Int64</span></span>|<span data-ttu-id="1f498-207">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="1f498-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="1f498-208">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f498-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="1f498-209">packageId</span><span class="sxs-lookup"><span data-stu-id="1f498-209">packageId</span></span>|<span data-ttu-id="1f498-210">String</span><span class="sxs-lookup"><span data-stu-id="1f498-210">String</span></span>|<span data-ttu-id="1f498-211">包标识符。</span><span class="sxs-lookup"><span data-stu-id="1f498-211">The package identifier.</span></span>|
|<span data-ttu-id="1f498-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1f498-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1f498-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1f498-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="1f498-214">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="1f498-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="1f498-215">versionName</span><span class="sxs-lookup"><span data-stu-id="1f498-215">versionName</span></span>|<span data-ttu-id="1f498-216">String</span><span class="sxs-lookup"><span data-stu-id="1f498-216">String</span></span>|<span data-ttu-id="1f498-217">托管 Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="1f498-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1f498-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="1f498-218">versionCode</span></span>|<span data-ttu-id="1f498-219">String</span><span class="sxs-lookup"><span data-stu-id="1f498-219">String</span></span>|<span data-ttu-id="1f498-220">托管 Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="1f498-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="1f498-221">响应</span><span class="sxs-lookup"><span data-stu-id="1f498-221">Response</span></span>
<span data-ttu-id="1f498-222">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1f498-222">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f498-223">示例</span><span class="sxs-lookup"><span data-stu-id="1f498-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f498-224">请求</span><span class="sxs-lookup"><span data-stu-id="1f498-224">Request</span></span>
<span data-ttu-id="1f498-225">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1f498-225">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1f498-226">响应</span><span class="sxs-lookup"><span data-stu-id="1f498-226">Response</span></span>
<span data-ttu-id="1f498-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1f498-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



