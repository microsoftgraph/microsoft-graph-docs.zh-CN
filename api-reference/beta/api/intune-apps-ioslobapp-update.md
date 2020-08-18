---
title: 更新 iosLobApp
description: 更新 iosLobApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 39b00e5393784266ac3e9c61e59e338480011f44
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791132"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="35f7e-103">更新 iosLobApp</span><span class="sxs-lookup"><span data-stu-id="35f7e-103">Update iosLobApp</span></span>

<span data-ttu-id="35f7e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35f7e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35f7e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35f7e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35f7e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35f7e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35f7e-107">更新 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="35f7e-107">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35f7e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="35f7e-108">Prerequisites</span></span>
<span data-ttu-id="35f7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35f7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35f7e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="35f7e-111">Permission type</span></span>|<span data-ttu-id="35f7e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="35f7e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35f7e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35f7e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="35f7e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35f7e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="35f7e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35f7e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35f7e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="35f7e-116">Not supported.</span></span>|
|<span data-ttu-id="35f7e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="35f7e-117">Application</span></span>|<span data-ttu-id="35f7e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35f7e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="35f7e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35f7e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="35f7e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="35f7e-120">Request headers</span></span>
|<span data-ttu-id="35f7e-121">标头</span><span class="sxs-lookup"><span data-stu-id="35f7e-121">Header</span></span>|<span data-ttu-id="35f7e-122">值</span><span class="sxs-lookup"><span data-stu-id="35f7e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35f7e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="35f7e-123">Authorization</span></span>|<span data-ttu-id="35f7e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="35f7e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35f7e-125">接受</span><span class="sxs-lookup"><span data-stu-id="35f7e-125">Accept</span></span>|<span data-ttu-id="35f7e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="35f7e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35f7e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="35f7e-127">Request body</span></span>
<span data-ttu-id="35f7e-128">在请求正文中，提供 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35f7e-128">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="35f7e-129">下表显示了创建 [iosLobApp](../resources/intune-apps-ioslobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="35f7e-129">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="35f7e-130">属性</span><span class="sxs-lookup"><span data-stu-id="35f7e-130">Property</span></span>|<span data-ttu-id="35f7e-131">类型</span><span class="sxs-lookup"><span data-stu-id="35f7e-131">Type</span></span>|<span data-ttu-id="35f7e-132">说明</span><span class="sxs-lookup"><span data-stu-id="35f7e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35f7e-133">id</span><span class="sxs-lookup"><span data-stu-id="35f7e-133">id</span></span>|<span data-ttu-id="35f7e-134">String</span><span class="sxs-lookup"><span data-stu-id="35f7e-134">String</span></span>|<span data-ttu-id="35f7e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="35f7e-135">Key of the entity.</span></span> <span data-ttu-id="35f7e-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="35f7e-137">displayName</span></span>|<span data-ttu-id="35f7e-138">String</span><span class="sxs-lookup"><span data-stu-id="35f7e-138">String</span></span>|<span data-ttu-id="35f7e-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="35f7e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="35f7e-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-141">description</span><span class="sxs-lookup"><span data-stu-id="35f7e-141">description</span></span>|<span data-ttu-id="35f7e-142">String</span><span class="sxs-lookup"><span data-stu-id="35f7e-142">String</span></span>|<span data-ttu-id="35f7e-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="35f7e-143">The description of the app.</span></span> <span data-ttu-id="35f7e-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="35f7e-145">publisher</span></span>|<span data-ttu-id="35f7e-146">String</span><span class="sxs-lookup"><span data-stu-id="35f7e-146">String</span></span>|<span data-ttu-id="35f7e-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="35f7e-147">The publisher of the app.</span></span> <span data-ttu-id="35f7e-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="35f7e-149">largeIcon</span></span>|[<span data-ttu-id="35f7e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="35f7e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="35f7e-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="35f7e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="35f7e-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35f7e-153">createdDateTime</span></span>|<span data-ttu-id="35f7e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35f7e-154">DateTimeOffset</span></span>|<span data-ttu-id="35f7e-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="35f7e-155">The date and time the app was created.</span></span> <span data-ttu-id="35f7e-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35f7e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="35f7e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35f7e-158">DateTimeOffset</span></span>|<span data-ttu-id="35f7e-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="35f7e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="35f7e-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="35f7e-161">isFeatured</span></span>|<span data-ttu-id="35f7e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f7e-162">Boolean</span></span>|<span data-ttu-id="35f7e-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="35f7e-164">privacyInformationUrl</span></span>|<span data-ttu-id="35f7e-165">String</span><span class="sxs-lookup"><span data-stu-id="35f7e-165">String</span></span>|<span data-ttu-id="35f7e-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="35f7e-166">The privacy statement Url.</span></span> <span data-ttu-id="35f7e-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="35f7e-168">informationUrl</span></span>|<span data-ttu-id="35f7e-169">String</span><span class="sxs-lookup"><span data-stu-id="35f7e-169">String</span></span>|<span data-ttu-id="35f7e-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="35f7e-170">The more information Url.</span></span> <span data-ttu-id="35f7e-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-172">所有者</span><span class="sxs-lookup"><span data-stu-id="35f7e-172">owner</span></span>|<span data-ttu-id="35f7e-173">String</span><span class="sxs-lookup"><span data-stu-id="35f7e-173">String</span></span>|<span data-ttu-id="35f7e-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="35f7e-174">The owner of the app.</span></span> <span data-ttu-id="35f7e-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-176">developer</span><span class="sxs-lookup"><span data-stu-id="35f7e-176">developer</span></span>|<span data-ttu-id="35f7e-177">String</span><span class="sxs-lookup"><span data-stu-id="35f7e-177">String</span></span>|<span data-ttu-id="35f7e-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="35f7e-178">The developer of the app.</span></span> <span data-ttu-id="35f7e-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-180">notes</span><span class="sxs-lookup"><span data-stu-id="35f7e-180">notes</span></span>|<span data-ttu-id="35f7e-181">String</span><span class="sxs-lookup"><span data-stu-id="35f7e-181">String</span></span>|<span data-ttu-id="35f7e-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="35f7e-182">Notes for the app.</span></span> <span data-ttu-id="35f7e-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="35f7e-184">uploadState</span></span>|<span data-ttu-id="35f7e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="35f7e-185">Int32</span></span>|<span data-ttu-id="35f7e-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="35f7e-186">The upload state.</span></span> <span data-ttu-id="35f7e-187">可能的值包括： 0- `Not Ready` 、1- `Ready` 、2- `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="35f7e-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="35f7e-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="35f7e-189">publishingState</span></span>|[<span data-ttu-id="35f7e-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="35f7e-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="35f7e-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="35f7e-191">The publishing state for the app.</span></span> <span data-ttu-id="35f7e-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="35f7e-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="35f7e-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="35f7e-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="35f7e-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="35f7e-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="35f7e-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="35f7e-195">isAssigned</span></span>|<span data-ttu-id="35f7e-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f7e-196">Boolean</span></span>|<span data-ttu-id="35f7e-197">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="35f7e-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="35f7e-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="35f7e-199">roleScopeTagIds</span></span>|<span data-ttu-id="35f7e-200">字符串集合</span><span class="sxs-lookup"><span data-stu-id="35f7e-200">String collection</span></span>|<span data-ttu-id="35f7e-201">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="35f7e-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="35f7e-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="35f7e-203">dependentAppCount</span></span>|<span data-ttu-id="35f7e-204">Int32</span><span class="sxs-lookup"><span data-stu-id="35f7e-204">Int32</span></span>|<span data-ttu-id="35f7e-205">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="35f7e-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="35f7e-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="35f7e-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="35f7e-207">committedContentVersion</span></span>|<span data-ttu-id="35f7e-208">String</span><span class="sxs-lookup"><span data-stu-id="35f7e-208">String</span></span>|<span data-ttu-id="35f7e-209">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="35f7e-209">The internal committed content version.</span></span> <span data-ttu-id="35f7e-210">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="35f7e-211">fileName</span><span class="sxs-lookup"><span data-stu-id="35f7e-211">fileName</span></span>|<span data-ttu-id="35f7e-212">String</span><span class="sxs-lookup"><span data-stu-id="35f7e-212">String</span></span>|<span data-ttu-id="35f7e-213">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="35f7e-213">The name of the main Lob application file.</span></span> <span data-ttu-id="35f7e-214">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="35f7e-215">size</span><span class="sxs-lookup"><span data-stu-id="35f7e-215">size</span></span>|<span data-ttu-id="35f7e-216">Int64</span><span class="sxs-lookup"><span data-stu-id="35f7e-216">Int64</span></span>|<span data-ttu-id="35f7e-217">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="35f7e-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="35f7e-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="35f7e-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="35f7e-219">bundleId</span><span class="sxs-lookup"><span data-stu-id="35f7e-219">bundleId</span></span>|<span data-ttu-id="35f7e-220">String</span><span class="sxs-lookup"><span data-stu-id="35f7e-220">String</span></span>|<span data-ttu-id="35f7e-221">标识名称。</span><span class="sxs-lookup"><span data-stu-id="35f7e-221">The Identity Name.</span></span>|
|<span data-ttu-id="35f7e-222">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="35f7e-222">applicableDeviceType</span></span>|[<span data-ttu-id="35f7e-223">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="35f7e-223">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="35f7e-224">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="35f7e-224">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="35f7e-225">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="35f7e-225">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="35f7e-226">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="35f7e-226">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="35f7e-227">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="35f7e-227">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="35f7e-228">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="35f7e-228">expirationDateTime</span></span>|<span data-ttu-id="35f7e-229">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35f7e-229">DateTimeOffset</span></span>|<span data-ttu-id="35f7e-230">过期时间。</span><span class="sxs-lookup"><span data-stu-id="35f7e-230">The expiration time.</span></span>|
|<span data-ttu-id="35f7e-231">versionNumber</span><span class="sxs-lookup"><span data-stu-id="35f7e-231">versionNumber</span></span>|<span data-ttu-id="35f7e-232">String</span><span class="sxs-lookup"><span data-stu-id="35f7e-232">String</span></span>|<span data-ttu-id="35f7e-233">iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="35f7e-233">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="35f7e-234">buildNumber</span><span class="sxs-lookup"><span data-stu-id="35f7e-234">buildNumber</span></span>|<span data-ttu-id="35f7e-235">String</span><span class="sxs-lookup"><span data-stu-id="35f7e-235">String</span></span>|<span data-ttu-id="35f7e-236">iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="35f7e-236">The build number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="35f7e-237">identityVersion</span><span class="sxs-lookup"><span data-stu-id="35f7e-237">identityVersion</span></span>|<span data-ttu-id="35f7e-238">String</span><span class="sxs-lookup"><span data-stu-id="35f7e-238">String</span></span>|<span data-ttu-id="35f7e-239">标识版本。</span><span class="sxs-lookup"><span data-stu-id="35f7e-239">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="35f7e-240">响应</span><span class="sxs-lookup"><span data-stu-id="35f7e-240">Response</span></span>
<span data-ttu-id="35f7e-241">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="35f7e-241">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35f7e-242">示例</span><span class="sxs-lookup"><span data-stu-id="35f7e-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="35f7e-243">请求</span><span class="sxs-lookup"><span data-stu-id="35f7e-243">Request</span></span>
<span data-ttu-id="35f7e-244">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="35f7e-244">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1411

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "dependentAppCount": 1,
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
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="35f7e-245">响应</span><span class="sxs-lookup"><span data-stu-id="35f7e-245">Response</span></span>
<span data-ttu-id="35f7e-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="35f7e-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1583

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "dependentAppCount": 1,
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
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```



