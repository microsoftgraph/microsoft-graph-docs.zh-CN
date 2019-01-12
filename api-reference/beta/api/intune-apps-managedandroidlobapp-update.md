---
title: 更新 managedAndroidLobApp
description: 更新 managedAndroidLobApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7baaccbb28702cbf71226a95ff7523763a007e87
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985716"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="a4721-103">更新 managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="a4721-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="a4721-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a4721-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4721-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a4721-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4721-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a4721-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4721-107">更新 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a4721-107">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a4721-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4721-108">Prerequisites</span></span>
<span data-ttu-id="a4721-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a4721-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4721-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4721-111">Permission type</span></span>|<span data-ttu-id="a4721-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a4721-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4721-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4721-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4721-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4721-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a4721-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4721-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4721-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4721-116">Not supported.</span></span>|
|<span data-ttu-id="a4721-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4721-117">Application</span></span>|<span data-ttu-id="a4721-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4721-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4721-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4721-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="a4721-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4721-120">Request headers</span></span>
|<span data-ttu-id="a4721-121">标头</span><span class="sxs-lookup"><span data-stu-id="a4721-121">Header</span></span>|<span data-ttu-id="a4721-122">值</span><span class="sxs-lookup"><span data-stu-id="a4721-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4721-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4721-123">Authorization</span></span>|<span data-ttu-id="a4721-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4721-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4721-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a4721-125">Accept</span></span>|<span data-ttu-id="a4721-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4721-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4721-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4721-127">Request body</span></span>
<span data-ttu-id="a4721-128">在请求正文中，提供 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4721-128">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="a4721-129">下表显示了创建 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a4721-129">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="a4721-130">属性</span><span class="sxs-lookup"><span data-stu-id="a4721-130">Property</span></span>|<span data-ttu-id="a4721-131">类型</span><span class="sxs-lookup"><span data-stu-id="a4721-131">Type</span></span>|<span data-ttu-id="a4721-132">说明</span><span class="sxs-lookup"><span data-stu-id="a4721-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4721-133">id</span><span class="sxs-lookup"><span data-stu-id="a4721-133">id</span></span>|<span data-ttu-id="a4721-134">String</span><span class="sxs-lookup"><span data-stu-id="a4721-134">String</span></span>|<span data-ttu-id="a4721-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a4721-135">Key of the entity.</span></span> <span data-ttu-id="a4721-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4721-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a4721-137">displayName</span></span>|<span data-ttu-id="a4721-138">String</span><span class="sxs-lookup"><span data-stu-id="a4721-138">String</span></span>|<span data-ttu-id="a4721-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="a4721-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a4721-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4721-141">description</span><span class="sxs-lookup"><span data-stu-id="a4721-141">description</span></span>|<span data-ttu-id="a4721-142">String</span><span class="sxs-lookup"><span data-stu-id="a4721-142">String</span></span>|<span data-ttu-id="a4721-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="a4721-143">The description of the app.</span></span> <span data-ttu-id="a4721-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4721-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a4721-145">publisher</span></span>|<span data-ttu-id="a4721-146">String</span><span class="sxs-lookup"><span data-stu-id="a4721-146">String</span></span>|<span data-ttu-id="a4721-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="a4721-147">The publisher of the app.</span></span> <span data-ttu-id="a4721-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4721-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a4721-149">largeIcon</span></span>|[<span data-ttu-id="a4721-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a4721-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a4721-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="a4721-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a4721-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4721-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4721-153">createdDateTime</span></span>|<span data-ttu-id="a4721-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4721-154">DateTimeOffset</span></span>|<span data-ttu-id="a4721-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a4721-155">The date and time the app was created.</span></span> <span data-ttu-id="a4721-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4721-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4721-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a4721-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4721-158">DateTimeOffset</span></span>|<span data-ttu-id="a4721-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a4721-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a4721-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4721-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a4721-161">isFeatured</span></span>|<span data-ttu-id="a4721-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4721-162">Boolean</span></span>|<span data-ttu-id="a4721-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4721-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a4721-164">privacyInformationUrl</span></span>|<span data-ttu-id="a4721-165">String</span><span class="sxs-lookup"><span data-stu-id="a4721-165">String</span></span>|<span data-ttu-id="a4721-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="a4721-166">The privacy statement Url.</span></span> <span data-ttu-id="a4721-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4721-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a4721-168">informationUrl</span></span>|<span data-ttu-id="a4721-169">String</span><span class="sxs-lookup"><span data-stu-id="a4721-169">String</span></span>|<span data-ttu-id="a4721-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="a4721-170">The more information Url.</span></span> <span data-ttu-id="a4721-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4721-172">owner</span><span class="sxs-lookup"><span data-stu-id="a4721-172">owner</span></span>|<span data-ttu-id="a4721-173">String</span><span class="sxs-lookup"><span data-stu-id="a4721-173">String</span></span>|<span data-ttu-id="a4721-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="a4721-174">The owner of the app.</span></span> <span data-ttu-id="a4721-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4721-176">developer</span><span class="sxs-lookup"><span data-stu-id="a4721-176">developer</span></span>|<span data-ttu-id="a4721-177">String</span><span class="sxs-lookup"><span data-stu-id="a4721-177">String</span></span>|<span data-ttu-id="a4721-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="a4721-178">The developer of the app.</span></span> <span data-ttu-id="a4721-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4721-180">notes</span><span class="sxs-lookup"><span data-stu-id="a4721-180">notes</span></span>|<span data-ttu-id="a4721-181">String</span><span class="sxs-lookup"><span data-stu-id="a4721-181">String</span></span>|<span data-ttu-id="a4721-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="a4721-182">Notes for the app.</span></span> <span data-ttu-id="a4721-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4721-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a4721-184">uploadState</span></span>|<span data-ttu-id="a4721-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a4721-185">Int32</span></span>|<span data-ttu-id="a4721-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="a4721-186">The upload state.</span></span> <span data-ttu-id="a4721-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4721-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="a4721-188">publishingState</span></span>|[<span data-ttu-id="a4721-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a4721-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a4721-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="a4721-190">The publishing state for the app.</span></span> <span data-ttu-id="a4721-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="a4721-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a4721-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="a4721-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a4721-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="a4721-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a4721-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="a4721-194">appAvailability</span></span>|[<span data-ttu-id="a4721-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="a4721-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="a4721-196">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="a4721-196">The Application's availability.</span></span> <span data-ttu-id="a4721-197">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="a4721-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="a4721-198">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="a4721-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="a4721-199">version</span><span class="sxs-lookup"><span data-stu-id="a4721-199">version</span></span>|<span data-ttu-id="a4721-200">String</span><span class="sxs-lookup"><span data-stu-id="a4721-200">String</span></span>|<span data-ttu-id="a4721-201">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="a4721-201">The Application's version.</span></span> <span data-ttu-id="a4721-202">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="a4721-203">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a4721-203">committedContentVersion</span></span>|<span data-ttu-id="a4721-204">String</span><span class="sxs-lookup"><span data-stu-id="a4721-204">String</span></span>|<span data-ttu-id="a4721-205">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="a4721-205">The internal committed content version.</span></span> <span data-ttu-id="a4721-206">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-206">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a4721-207">fileName</span><span class="sxs-lookup"><span data-stu-id="a4721-207">fileName</span></span>|<span data-ttu-id="a4721-208">String</span><span class="sxs-lookup"><span data-stu-id="a4721-208">String</span></span>|<span data-ttu-id="a4721-209">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="a4721-209">The name of the main Lob application file.</span></span> <span data-ttu-id="a4721-210">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-210">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a4721-211">size</span><span class="sxs-lookup"><span data-stu-id="a4721-211">size</span></span>|<span data-ttu-id="a4721-212">Int64</span><span class="sxs-lookup"><span data-stu-id="a4721-212">Int64</span></span>|<span data-ttu-id="a4721-213">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="a4721-213">The total size, including all uploaded files.</span></span> <span data-ttu-id="a4721-214">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4721-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="a4721-215">packageId</span><span class="sxs-lookup"><span data-stu-id="a4721-215">packageId</span></span>|<span data-ttu-id="a4721-216">String</span><span class="sxs-lookup"><span data-stu-id="a4721-216">String</span></span>|<span data-ttu-id="a4721-217">包标识符。</span><span class="sxs-lookup"><span data-stu-id="a4721-217">The package identifier.</span></span>|
|<span data-ttu-id="a4721-218">identityName</span><span class="sxs-lookup"><span data-stu-id="a4721-218">identityName</span></span>|<span data-ttu-id="a4721-219">String</span><span class="sxs-lookup"><span data-stu-id="a4721-219">String</span></span>|<span data-ttu-id="a4721-220">标识名称。</span><span class="sxs-lookup"><span data-stu-id="a4721-220">The Identity Name.</span></span>|
|<span data-ttu-id="a4721-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a4721-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a4721-222">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a4721-222">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="a4721-223">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="a4721-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="a4721-224">versionName</span><span class="sxs-lookup"><span data-stu-id="a4721-224">versionName</span></span>|<span data-ttu-id="a4721-225">String</span><span class="sxs-lookup"><span data-stu-id="a4721-225">String</span></span>|<span data-ttu-id="a4721-226">托管 Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="a4721-226">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="a4721-227">versionCode</span><span class="sxs-lookup"><span data-stu-id="a4721-227">versionCode</span></span>|<span data-ttu-id="a4721-228">String</span><span class="sxs-lookup"><span data-stu-id="a4721-228">String</span></span>|<span data-ttu-id="a4721-229">托管 Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="a4721-229">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="a4721-230">identityVersion</span><span class="sxs-lookup"><span data-stu-id="a4721-230">identityVersion</span></span>|<span data-ttu-id="a4721-231">String</span><span class="sxs-lookup"><span data-stu-id="a4721-231">String</span></span>|<span data-ttu-id="a4721-232">标识版本。</span><span class="sxs-lookup"><span data-stu-id="a4721-232">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="a4721-233">响应</span><span class="sxs-lookup"><span data-stu-id="a4721-233">Response</span></span>
<span data-ttu-id="a4721-234">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a4721-234">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4721-235">示例</span><span class="sxs-lookup"><span data-stu-id="a4721-235">Example</span></span>
### <a name="request"></a><span data-ttu-id="a4721-236">请求</span><span class="sxs-lookup"><span data-stu-id="a4721-236">Request</span></span>
<span data-ttu-id="a4721-237">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4721-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1384

{
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
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="a4721-238">响应</span><span class="sxs-lookup"><span data-stu-id="a4721-238">Response</span></span>
<span data-ttu-id="a4721-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4721-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1551

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
  "uploadState": 11,
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```





