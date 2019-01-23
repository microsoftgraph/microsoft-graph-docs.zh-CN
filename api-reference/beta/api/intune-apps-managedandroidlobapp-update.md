---
title: 更新 managedAndroidLobApp
description: 更新 managedAndroidLobApp 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7fa0ace9f4e1235b5ca63ee9c7249d7f667c8b2e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394640"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="cb8f7-103">更新 managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="cb8f7-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="cb8f7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cb8f7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cb8f7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb8f7-107">更新 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-107">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb8f7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cb8f7-108">Prerequisites</span></span>
<span data-ttu-id="cb8f7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cb8f7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb8f7-111">Permission type</span></span>|<span data-ttu-id="cb8f7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cb8f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb8f7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb8f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb8f7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb8f7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cb8f7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb8f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb8f7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-116">Not supported.</span></span>|
|<span data-ttu-id="cb8f7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb8f7-117">Application</span></span>|<span data-ttu-id="cb8f7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb8f7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb8f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="cb8f7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb8f7-120">Request headers</span></span>
|<span data-ttu-id="cb8f7-121">标头</span><span class="sxs-lookup"><span data-stu-id="cb8f7-121">Header</span></span>|<span data-ttu-id="cb8f7-122">值</span><span class="sxs-lookup"><span data-stu-id="cb8f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb8f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb8f7-123">Authorization</span></span>|<span data-ttu-id="cb8f7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb8f7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cb8f7-125">Accept</span></span>|<span data-ttu-id="cb8f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb8f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb8f7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb8f7-127">Request body</span></span>
<span data-ttu-id="cb8f7-128">在请求正文中，提供 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-128">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="cb8f7-129">下表显示了创建 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-129">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="cb8f7-130">属性</span><span class="sxs-lookup"><span data-stu-id="cb8f7-130">Property</span></span>|<span data-ttu-id="cb8f7-131">类型</span><span class="sxs-lookup"><span data-stu-id="cb8f7-131">Type</span></span>|<span data-ttu-id="cb8f7-132">说明</span><span class="sxs-lookup"><span data-stu-id="cb8f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb8f7-133">id</span><span class="sxs-lookup"><span data-stu-id="cb8f7-133">id</span></span>|<span data-ttu-id="cb8f7-134">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-134">String</span></span>|<span data-ttu-id="cb8f7-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-135">Key of the entity.</span></span> <span data-ttu-id="cb8f7-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="cb8f7-137">displayName</span></span>|<span data-ttu-id="cb8f7-138">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-138">String</span></span>|<span data-ttu-id="cb8f7-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="cb8f7-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-141">description</span><span class="sxs-lookup"><span data-stu-id="cb8f7-141">description</span></span>|<span data-ttu-id="cb8f7-142">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-142">String</span></span>|<span data-ttu-id="cb8f7-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-143">The description of the app.</span></span> <span data-ttu-id="cb8f7-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-145">publisher</span><span class="sxs-lookup"><span data-stu-id="cb8f7-145">publisher</span></span>|<span data-ttu-id="cb8f7-146">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-146">String</span></span>|<span data-ttu-id="cb8f7-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-147">The publisher of the app.</span></span> <span data-ttu-id="cb8f7-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="cb8f7-149">largeIcon</span></span>|[<span data-ttu-id="cb8f7-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="cb8f7-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="cb8f7-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="cb8f7-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb8f7-153">createdDateTime</span></span>|<span data-ttu-id="cb8f7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb8f7-154">DateTimeOffset</span></span>|<span data-ttu-id="cb8f7-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-155">The date and time the app was created.</span></span> <span data-ttu-id="cb8f7-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb8f7-157">lastModifiedDateTime</span></span>|<span data-ttu-id="cb8f7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb8f7-158">DateTimeOffset</span></span>|<span data-ttu-id="cb8f7-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-159">The date and time the app was last modified.</span></span> <span data-ttu-id="cb8f7-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="cb8f7-161">isFeatured</span></span>|<span data-ttu-id="cb8f7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb8f7-162">Boolean</span></span>|<span data-ttu-id="cb8f7-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="cb8f7-164">privacyInformationUrl</span></span>|<span data-ttu-id="cb8f7-165">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-165">String</span></span>|<span data-ttu-id="cb8f7-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-166">The privacy statement Url.</span></span> <span data-ttu-id="cb8f7-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="cb8f7-168">informationUrl</span></span>|<span data-ttu-id="cb8f7-169">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-169">String</span></span>|<span data-ttu-id="cb8f7-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-170">The more information Url.</span></span> <span data-ttu-id="cb8f7-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-172">owner</span><span class="sxs-lookup"><span data-stu-id="cb8f7-172">owner</span></span>|<span data-ttu-id="cb8f7-173">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-173">String</span></span>|<span data-ttu-id="cb8f7-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-174">The owner of the app.</span></span> <span data-ttu-id="cb8f7-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-176">developer</span><span class="sxs-lookup"><span data-stu-id="cb8f7-176">developer</span></span>|<span data-ttu-id="cb8f7-177">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-177">String</span></span>|<span data-ttu-id="cb8f7-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-178">The developer of the app.</span></span> <span data-ttu-id="cb8f7-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-180">notes</span><span class="sxs-lookup"><span data-stu-id="cb8f7-180">notes</span></span>|<span data-ttu-id="cb8f7-181">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-181">String</span></span>|<span data-ttu-id="cb8f7-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-182">Notes for the app.</span></span> <span data-ttu-id="cb8f7-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="cb8f7-184">uploadState</span></span>|<span data-ttu-id="cb8f7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="cb8f7-185">Int32</span></span>|<span data-ttu-id="cb8f7-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-186">The upload state.</span></span> <span data-ttu-id="cb8f7-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="cb8f7-188">publishingState</span></span>|[<span data-ttu-id="cb8f7-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="cb8f7-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="cb8f7-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-190">The publishing state for the app.</span></span> <span data-ttu-id="cb8f7-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="cb8f7-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="cb8f7-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="cb8f7-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="cb8f7-194">isAssigned</span></span>|<span data-ttu-id="cb8f7-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb8f7-195">Boolean</span></span>|<span data-ttu-id="cb8f7-196">值，指示是否将应用程序分配给至少一个组。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="cb8f7-197">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cb8f7-198">roleScopeTagIds</span></span>|<span data-ttu-id="cb8f7-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="cb8f7-199">String collection</span></span>|<span data-ttu-id="cb8f7-200">此移动应用程序的作用域标记 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="cb8f7-201">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="cb8f7-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="cb8f7-202">appAvailability</span></span>|[<span data-ttu-id="cb8f7-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="cb8f7-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="cb8f7-204">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-204">The Application's availability.</span></span> <span data-ttu-id="cb8f7-205">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="cb8f7-206">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="cb8f7-207">version</span><span class="sxs-lookup"><span data-stu-id="cb8f7-207">version</span></span>|<span data-ttu-id="cb8f7-208">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-208">String</span></span>|<span data-ttu-id="cb8f7-209">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-209">The Application's version.</span></span> <span data-ttu-id="cb8f7-210">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="cb8f7-211">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="cb8f7-211">committedContentVersion</span></span>|<span data-ttu-id="cb8f7-212">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-212">String</span></span>|<span data-ttu-id="cb8f7-213">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-213">The internal committed content version.</span></span> <span data-ttu-id="cb8f7-214">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="cb8f7-215">fileName</span><span class="sxs-lookup"><span data-stu-id="cb8f7-215">fileName</span></span>|<span data-ttu-id="cb8f7-216">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-216">String</span></span>|<span data-ttu-id="cb8f7-217">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-217">The name of the main Lob application file.</span></span> <span data-ttu-id="cb8f7-218">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="cb8f7-219">size</span><span class="sxs-lookup"><span data-stu-id="cb8f7-219">size</span></span>|<span data-ttu-id="cb8f7-220">Int64</span><span class="sxs-lookup"><span data-stu-id="cb8f7-220">Int64</span></span>|<span data-ttu-id="cb8f7-221">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-221">The total size, including all uploaded files.</span></span> <span data-ttu-id="cb8f7-222">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="cb8f7-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="cb8f7-223">packageId</span><span class="sxs-lookup"><span data-stu-id="cb8f7-223">packageId</span></span>|<span data-ttu-id="cb8f7-224">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-224">String</span></span>|<span data-ttu-id="cb8f7-225">包标识符。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-225">The package identifier.</span></span>|
|<span data-ttu-id="cb8f7-226">identityName</span><span class="sxs-lookup"><span data-stu-id="cb8f7-226">identityName</span></span>|<span data-ttu-id="cb8f7-227">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-227">String</span></span>|<span data-ttu-id="cb8f7-228">标识名称。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-228">The Identity Name.</span></span>|
|<span data-ttu-id="cb8f7-229">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cb8f7-229">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="cb8f7-230">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="cb8f7-230">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="cb8f7-231">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-231">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="cb8f7-232">versionName</span><span class="sxs-lookup"><span data-stu-id="cb8f7-232">versionName</span></span>|<span data-ttu-id="cb8f7-233">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-233">String</span></span>|<span data-ttu-id="cb8f7-234">托管 Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-234">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="cb8f7-235">versionCode</span><span class="sxs-lookup"><span data-stu-id="cb8f7-235">versionCode</span></span>|<span data-ttu-id="cb8f7-236">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-236">String</span></span>|<span data-ttu-id="cb8f7-237">托管 Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-237">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="cb8f7-238">identityVersion</span><span class="sxs-lookup"><span data-stu-id="cb8f7-238">identityVersion</span></span>|<span data-ttu-id="cb8f7-239">String</span><span class="sxs-lookup"><span data-stu-id="cb8f7-239">String</span></span>|<span data-ttu-id="cb8f7-240">标识版本。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-240">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="cb8f7-241">响应</span><span class="sxs-lookup"><span data-stu-id="cb8f7-241">Response</span></span>
<span data-ttu-id="cb8f7-242">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-242">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb8f7-243">示例</span><span class="sxs-lookup"><span data-stu-id="cb8f7-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb8f7-244">请求</span><span class="sxs-lookup"><span data-stu-id="cb8f7-244">Request</span></span>
<span data-ttu-id="cb8f7-245">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-245">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1464

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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="cb8f7-246">响应</span><span class="sxs-lookup"><span data-stu-id="cb8f7-246">Response</span></span>
<span data-ttu-id="cb8f7-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cb8f7-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1636

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




