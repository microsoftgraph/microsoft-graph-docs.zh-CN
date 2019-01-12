---
title: 更新 managedIOSLobApp
description: 更新 managedIOSLobApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 82a3a3b1b9e767e0fe8cb93b6c2380896ae22851
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939964"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="c47a5-103">更新 managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="c47a5-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="c47a5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c47a5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c47a5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c47a5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c47a5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c47a5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c47a5-107">更新 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c47a5-107">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c47a5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c47a5-108">Prerequisites</span></span>
<span data-ttu-id="c47a5-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c47a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c47a5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c47a5-111">Permission type</span></span>|<span data-ttu-id="c47a5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c47a5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c47a5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c47a5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c47a5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c47a5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c47a5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c47a5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c47a5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c47a5-116">Not supported.</span></span>|
|<span data-ttu-id="c47a5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c47a5-117">Application</span></span>|<span data-ttu-id="c47a5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c47a5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c47a5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c47a5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="c47a5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c47a5-120">Request headers</span></span>
|<span data-ttu-id="c47a5-121">标头</span><span class="sxs-lookup"><span data-stu-id="c47a5-121">Header</span></span>|<span data-ttu-id="c47a5-122">值</span><span class="sxs-lookup"><span data-stu-id="c47a5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c47a5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c47a5-123">Authorization</span></span>|<span data-ttu-id="c47a5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c47a5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c47a5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c47a5-125">Accept</span></span>|<span data-ttu-id="c47a5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c47a5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c47a5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c47a5-127">Request body</span></span>
<span data-ttu-id="c47a5-128">在请求正文中，提供 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c47a5-128">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="c47a5-129">下表显示创建 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c47a5-129">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="c47a5-130">属性</span><span class="sxs-lookup"><span data-stu-id="c47a5-130">Property</span></span>|<span data-ttu-id="c47a5-131">类型</span><span class="sxs-lookup"><span data-stu-id="c47a5-131">Type</span></span>|<span data-ttu-id="c47a5-132">说明</span><span class="sxs-lookup"><span data-stu-id="c47a5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c47a5-133">id</span><span class="sxs-lookup"><span data-stu-id="c47a5-133">id</span></span>|<span data-ttu-id="c47a5-134">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-134">String</span></span>|<span data-ttu-id="c47a5-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c47a5-135">Key of the entity.</span></span> <span data-ttu-id="c47a5-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c47a5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c47a5-137">displayName</span></span>|<span data-ttu-id="c47a5-138">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-138">String</span></span>|<span data-ttu-id="c47a5-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="c47a5-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c47a5-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c47a5-141">description</span><span class="sxs-lookup"><span data-stu-id="c47a5-141">description</span></span>|<span data-ttu-id="c47a5-142">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-142">String</span></span>|<span data-ttu-id="c47a5-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="c47a5-143">The description of the app.</span></span> <span data-ttu-id="c47a5-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c47a5-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c47a5-145">publisher</span></span>|<span data-ttu-id="c47a5-146">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-146">String</span></span>|<span data-ttu-id="c47a5-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="c47a5-147">The publisher of the app.</span></span> <span data-ttu-id="c47a5-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c47a5-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c47a5-149">largeIcon</span></span>|[<span data-ttu-id="c47a5-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c47a5-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c47a5-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="c47a5-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c47a5-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c47a5-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c47a5-153">createdDateTime</span></span>|<span data-ttu-id="c47a5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c47a5-154">DateTimeOffset</span></span>|<span data-ttu-id="c47a5-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c47a5-155">The date and time the app was created.</span></span> <span data-ttu-id="c47a5-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c47a5-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c47a5-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c47a5-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c47a5-158">DateTimeOffset</span></span>|<span data-ttu-id="c47a5-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c47a5-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c47a5-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c47a5-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c47a5-161">isFeatured</span></span>|<span data-ttu-id="c47a5-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c47a5-162">Boolean</span></span>|<span data-ttu-id="c47a5-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c47a5-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c47a5-164">privacyInformationUrl</span></span>|<span data-ttu-id="c47a5-165">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-165">String</span></span>|<span data-ttu-id="c47a5-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="c47a5-166">The privacy statement Url.</span></span> <span data-ttu-id="c47a5-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c47a5-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c47a5-168">informationUrl</span></span>|<span data-ttu-id="c47a5-169">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-169">String</span></span>|<span data-ttu-id="c47a5-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="c47a5-170">The more information Url.</span></span> <span data-ttu-id="c47a5-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c47a5-172">owner</span><span class="sxs-lookup"><span data-stu-id="c47a5-172">owner</span></span>|<span data-ttu-id="c47a5-173">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-173">String</span></span>|<span data-ttu-id="c47a5-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="c47a5-174">The owner of the app.</span></span> <span data-ttu-id="c47a5-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c47a5-176">developer</span><span class="sxs-lookup"><span data-stu-id="c47a5-176">developer</span></span>|<span data-ttu-id="c47a5-177">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-177">String</span></span>|<span data-ttu-id="c47a5-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="c47a5-178">The developer of the app.</span></span> <span data-ttu-id="c47a5-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c47a5-180">notes</span><span class="sxs-lookup"><span data-stu-id="c47a5-180">notes</span></span>|<span data-ttu-id="c47a5-181">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-181">String</span></span>|<span data-ttu-id="c47a5-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="c47a5-182">Notes for the app.</span></span> <span data-ttu-id="c47a5-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c47a5-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c47a5-184">uploadState</span></span>|<span data-ttu-id="c47a5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c47a5-185">Int32</span></span>|<span data-ttu-id="c47a5-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="c47a5-186">The upload state.</span></span> <span data-ttu-id="c47a5-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c47a5-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="c47a5-188">publishingState</span></span>|[<span data-ttu-id="c47a5-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c47a5-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c47a5-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="c47a5-190">The publishing state for the app.</span></span> <span data-ttu-id="c47a5-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="c47a5-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c47a5-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="c47a5-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c47a5-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="c47a5-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c47a5-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="c47a5-194">appAvailability</span></span>|[<span data-ttu-id="c47a5-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="c47a5-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="c47a5-196">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="c47a5-196">The Application's availability.</span></span> <span data-ttu-id="c47a5-197">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="c47a5-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="c47a5-198">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="c47a5-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="c47a5-199">version</span><span class="sxs-lookup"><span data-stu-id="c47a5-199">version</span></span>|<span data-ttu-id="c47a5-200">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-200">String</span></span>|<span data-ttu-id="c47a5-201">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="c47a5-201">The Application's version.</span></span> <span data-ttu-id="c47a5-202">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="c47a5-203">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="c47a5-203">committedContentVersion</span></span>|<span data-ttu-id="c47a5-204">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-204">String</span></span>|<span data-ttu-id="c47a5-205">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="c47a5-205">The internal committed content version.</span></span> <span data-ttu-id="c47a5-206">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-206">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="c47a5-207">fileName</span><span class="sxs-lookup"><span data-stu-id="c47a5-207">fileName</span></span>|<span data-ttu-id="c47a5-208">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-208">String</span></span>|<span data-ttu-id="c47a5-209">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="c47a5-209">The name of the main Lob application file.</span></span> <span data-ttu-id="c47a5-210">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-210">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="c47a5-211">size</span><span class="sxs-lookup"><span data-stu-id="c47a5-211">size</span></span>|<span data-ttu-id="c47a5-212">Int64</span><span class="sxs-lookup"><span data-stu-id="c47a5-212">Int64</span></span>|<span data-ttu-id="c47a5-213">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="c47a5-213">The total size, including all uploaded files.</span></span> <span data-ttu-id="c47a5-214">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c47a5-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="c47a5-215">bundleId</span><span class="sxs-lookup"><span data-stu-id="c47a5-215">bundleId</span></span>|<span data-ttu-id="c47a5-216">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-216">String</span></span>|<span data-ttu-id="c47a5-217">标识名称。</span><span class="sxs-lookup"><span data-stu-id="c47a5-217">The Identity Name.</span></span>|
|<span data-ttu-id="c47a5-218">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="c47a5-218">applicableDeviceType</span></span>|[<span data-ttu-id="c47a5-219">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="c47a5-219">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="c47a5-220">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="c47a5-220">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="c47a5-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c47a5-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c47a5-222">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c47a5-222">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="c47a5-223">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="c47a5-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="c47a5-224">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c47a5-224">expirationDateTime</span></span>|<span data-ttu-id="c47a5-225">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c47a5-225">DateTimeOffset</span></span>|<span data-ttu-id="c47a5-226">过期时间。</span><span class="sxs-lookup"><span data-stu-id="c47a5-226">The expiration time.</span></span>|
|<span data-ttu-id="c47a5-227">versionNumber</span><span class="sxs-lookup"><span data-stu-id="c47a5-227">versionNumber</span></span>|<span data-ttu-id="c47a5-228">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-228">String</span></span>|<span data-ttu-id="c47a5-229">托管 iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="c47a5-229">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c47a5-230">buildNumber</span><span class="sxs-lookup"><span data-stu-id="c47a5-230">buildNumber</span></span>|<span data-ttu-id="c47a5-231">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-231">String</span></span>|<span data-ttu-id="c47a5-232">托管 iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="c47a5-232">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c47a5-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="c47a5-233">identityVersion</span></span>|<span data-ttu-id="c47a5-234">String</span><span class="sxs-lookup"><span data-stu-id="c47a5-234">String</span></span>|<span data-ttu-id="c47a5-235">标识版本。</span><span class="sxs-lookup"><span data-stu-id="c47a5-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="c47a5-236">响应</span><span class="sxs-lookup"><span data-stu-id="c47a5-236">Response</span></span>
<span data-ttu-id="c47a5-237">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c47a5-237">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c47a5-238">示例</span><span class="sxs-lookup"><span data-stu-id="c47a5-238">Example</span></span>
### <a name="request"></a><span data-ttu-id="c47a5-239">请求</span><span class="sxs-lookup"><span data-stu-id="c47a5-239">Request</span></span>
<span data-ttu-id="c47a5-240">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c47a5-240">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1366

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

### <a name="response"></a><span data-ttu-id="c47a5-241">响应</span><span class="sxs-lookup"><span data-stu-id="c47a5-241">Response</span></span>
<span data-ttu-id="c47a5-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c47a5-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





