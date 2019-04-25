---
title: 创建 managedAndroidLobApp
description: 创建新的 managedAndroidLobApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d2f7932a9ea627769432b9c686420c892cc04eb2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577096"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="86a5f-103">创建 managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="86a5f-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="86a5f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86a5f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86a5f-105">创建新的 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86a5f-105">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86a5f-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="86a5f-106">Prerequisites</span></span>
<span data-ttu-id="86a5f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86a5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86a5f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="86a5f-109">Permission type</span></span>|<span data-ttu-id="86a5f-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="86a5f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86a5f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86a5f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="86a5f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86a5f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="86a5f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86a5f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86a5f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="86a5f-114">Not supported.</span></span>|
|<span data-ttu-id="86a5f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="86a5f-115">Application</span></span>|<span data-ttu-id="86a5f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="86a5f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86a5f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86a5f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="86a5f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="86a5f-118">Request headers</span></span>
|<span data-ttu-id="86a5f-119">标头</span><span class="sxs-lookup"><span data-stu-id="86a5f-119">Header</span></span>|<span data-ttu-id="86a5f-120">值</span><span class="sxs-lookup"><span data-stu-id="86a5f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86a5f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="86a5f-121">Authorization</span></span>|<span data-ttu-id="86a5f-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="86a5f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86a5f-123">接受</span><span class="sxs-lookup"><span data-stu-id="86a5f-123">Accept</span></span>|<span data-ttu-id="86a5f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="86a5f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86a5f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="86a5f-125">Request body</span></span>
<span data-ttu-id="86a5f-126">在请求正文中，提供 managedAndroidLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86a5f-126">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="86a5f-127">下表显示了创建 managedAndroidLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="86a5f-127">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="86a5f-128">属性</span><span class="sxs-lookup"><span data-stu-id="86a5f-128">Property</span></span>|<span data-ttu-id="86a5f-129">类型</span><span class="sxs-lookup"><span data-stu-id="86a5f-129">Type</span></span>|<span data-ttu-id="86a5f-130">说明</span><span class="sxs-lookup"><span data-stu-id="86a5f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86a5f-131">id</span><span class="sxs-lookup"><span data-stu-id="86a5f-131">id</span></span>|<span data-ttu-id="86a5f-132">字符串</span><span class="sxs-lookup"><span data-stu-id="86a5f-132">String</span></span>|<span data-ttu-id="86a5f-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="86a5f-133">Key of the entity.</span></span> <span data-ttu-id="86a5f-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86a5f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="86a5f-135">displayName</span></span>|<span data-ttu-id="86a5f-136">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-136">String</span></span>|<span data-ttu-id="86a5f-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="86a5f-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="86a5f-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86a5f-139">说明</span><span class="sxs-lookup"><span data-stu-id="86a5f-139">description</span></span>|<span data-ttu-id="86a5f-140">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-140">String</span></span>|<span data-ttu-id="86a5f-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="86a5f-141">The description of the app.</span></span> <span data-ttu-id="86a5f-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86a5f-143">publisher</span><span class="sxs-lookup"><span data-stu-id="86a5f-143">publisher</span></span>|<span data-ttu-id="86a5f-144">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-144">String</span></span>|<span data-ttu-id="86a5f-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="86a5f-145">The publisher of the app.</span></span> <span data-ttu-id="86a5f-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86a5f-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="86a5f-147">largeIcon</span></span>|[<span data-ttu-id="86a5f-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="86a5f-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="86a5f-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="86a5f-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="86a5f-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86a5f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86a5f-151">createdDateTime</span></span>|<span data-ttu-id="86a5f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86a5f-152">DateTimeOffset</span></span>|<span data-ttu-id="86a5f-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="86a5f-153">The date and time the app was created.</span></span> <span data-ttu-id="86a5f-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86a5f-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86a5f-155">lastModifiedDateTime</span></span>|<span data-ttu-id="86a5f-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86a5f-156">DateTimeOffset</span></span>|<span data-ttu-id="86a5f-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="86a5f-157">The date and time the app was last modified.</span></span> <span data-ttu-id="86a5f-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86a5f-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="86a5f-159">isFeatured</span></span>|<span data-ttu-id="86a5f-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a5f-160">Boolean</span></span>|<span data-ttu-id="86a5f-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86a5f-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="86a5f-162">privacyInformationUrl</span></span>|<span data-ttu-id="86a5f-163">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-163">String</span></span>|<span data-ttu-id="86a5f-164">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="86a5f-164">The privacy statement Url.</span></span> <span data-ttu-id="86a5f-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86a5f-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="86a5f-166">informationUrl</span></span>|<span data-ttu-id="86a5f-167">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-167">String</span></span>|<span data-ttu-id="86a5f-168">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="86a5f-168">The more information Url.</span></span> <span data-ttu-id="86a5f-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86a5f-170">owner</span><span class="sxs-lookup"><span data-stu-id="86a5f-170">owner</span></span>|<span data-ttu-id="86a5f-171">字符串</span><span class="sxs-lookup"><span data-stu-id="86a5f-171">String</span></span>|<span data-ttu-id="86a5f-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="86a5f-172">The owner of the app.</span></span> <span data-ttu-id="86a5f-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86a5f-174">developer</span><span class="sxs-lookup"><span data-stu-id="86a5f-174">developer</span></span>|<span data-ttu-id="86a5f-175">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-175">String</span></span>|<span data-ttu-id="86a5f-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="86a5f-176">The developer of the app.</span></span> <span data-ttu-id="86a5f-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86a5f-178">notes</span><span class="sxs-lookup"><span data-stu-id="86a5f-178">notes</span></span>|<span data-ttu-id="86a5f-179">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-179">String</span></span>|<span data-ttu-id="86a5f-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="86a5f-180">Notes for the app.</span></span> <span data-ttu-id="86a5f-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86a5f-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="86a5f-182">publishingState</span></span>|[<span data-ttu-id="86a5f-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="86a5f-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="86a5f-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="86a5f-184">The publishing state for the app.</span></span> <span data-ttu-id="86a5f-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="86a5f-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="86a5f-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="86a5f-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="86a5f-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="86a5f-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="86a5f-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="86a5f-188">appAvailability</span></span>|[<span data-ttu-id="86a5f-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="86a5f-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="86a5f-190">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="86a5f-190">The Application's availability.</span></span> <span data-ttu-id="86a5f-191">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="86a5f-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="86a5f-192">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="86a5f-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="86a5f-193">version</span><span class="sxs-lookup"><span data-stu-id="86a5f-193">version</span></span>|<span data-ttu-id="86a5f-194">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-194">String</span></span>|<span data-ttu-id="86a5f-195">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="86a5f-195">The Application's version.</span></span> <span data-ttu-id="86a5f-196">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="86a5f-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="86a5f-197">committedContentVersion</span></span>|<span data-ttu-id="86a5f-198">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-198">String</span></span>|<span data-ttu-id="86a5f-199">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="86a5f-199">The internal committed content version.</span></span> <span data-ttu-id="86a5f-200">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="86a5f-201">fileName</span><span class="sxs-lookup"><span data-stu-id="86a5f-201">fileName</span></span>|<span data-ttu-id="86a5f-202">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-202">String</span></span>|<span data-ttu-id="86a5f-203">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="86a5f-203">The name of the main Lob application file.</span></span> <span data-ttu-id="86a5f-204">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="86a5f-205">size</span><span class="sxs-lookup"><span data-stu-id="86a5f-205">size</span></span>|<span data-ttu-id="86a5f-206">Int64</span><span class="sxs-lookup"><span data-stu-id="86a5f-206">Int64</span></span>|<span data-ttu-id="86a5f-207">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="86a5f-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="86a5f-208">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="86a5f-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="86a5f-209">packageId</span><span class="sxs-lookup"><span data-stu-id="86a5f-209">packageId</span></span>|<span data-ttu-id="86a5f-210">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-210">String</span></span>|<span data-ttu-id="86a5f-211">包标识符。</span><span class="sxs-lookup"><span data-stu-id="86a5f-211">The package identifier.</span></span>|
|<span data-ttu-id="86a5f-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="86a5f-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="86a5f-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="86a5f-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="86a5f-214">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="86a5f-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="86a5f-215">versionName</span><span class="sxs-lookup"><span data-stu-id="86a5f-215">versionName</span></span>|<span data-ttu-id="86a5f-216">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-216">String</span></span>|<span data-ttu-id="86a5f-217">托管 Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="86a5f-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="86a5f-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="86a5f-218">versionCode</span></span>|<span data-ttu-id="86a5f-219">String</span><span class="sxs-lookup"><span data-stu-id="86a5f-219">String</span></span>|<span data-ttu-id="86a5f-220">托管 Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="86a5f-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="86a5f-221">响应</span><span class="sxs-lookup"><span data-stu-id="86a5f-221">Response</span></span>
<span data-ttu-id="86a5f-222">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86a5f-222">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86a5f-223">示例</span><span class="sxs-lookup"><span data-stu-id="86a5f-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="86a5f-224">请求</span><span class="sxs-lookup"><span data-stu-id="86a5f-224">Request</span></span>
<span data-ttu-id="86a5f-225">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86a5f-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="86a5f-226">响应</span><span class="sxs-lookup"><span data-stu-id="86a5f-226">Response</span></span>
<span data-ttu-id="86a5f-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86a5f-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



