---
title: 更新 androidManagedStoreApp
description: 更新 androidManagedStoreApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1558994f71fbf62f7d401b64a61d687e39c8215a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964827"
---
# <a name="update-androidmanagedstoreapp"></a><span data-ttu-id="2600d-103">更新 androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="2600d-103">Update androidManagedStoreApp</span></span>

> <span data-ttu-id="2600d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2600d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2600d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2600d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2600d-106">更新[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2600d-106">Update the properties of a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2600d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2600d-107">Prerequisites</span></span>
<span data-ttu-id="2600d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2600d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2600d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2600d-110">Permission type</span></span>|<span data-ttu-id="2600d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2600d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2600d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2600d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2600d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2600d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2600d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2600d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2600d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2600d-115">Not supported.</span></span>|
|<span data-ttu-id="2600d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2600d-116">Application</span></span>|<span data-ttu-id="2600d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2600d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2600d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2600d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="2600d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2600d-119">Request headers</span></span>
|<span data-ttu-id="2600d-120">标头</span><span class="sxs-lookup"><span data-stu-id="2600d-120">Header</span></span>|<span data-ttu-id="2600d-121">值</span><span class="sxs-lookup"><span data-stu-id="2600d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2600d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2600d-122">Authorization</span></span>|<span data-ttu-id="2600d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2600d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2600d-124">接受</span><span class="sxs-lookup"><span data-stu-id="2600d-124">Accept</span></span>|<span data-ttu-id="2600d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2600d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2600d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2600d-126">Request body</span></span>
<span data-ttu-id="2600d-127">在请求正文中, 提供[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2600d-127">In the request body, supply a JSON representation for the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

<span data-ttu-id="2600d-128">下表显示创建[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2600d-128">The following table shows the properties that are required when you create the [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md).</span></span>

|<span data-ttu-id="2600d-129">属性</span><span class="sxs-lookup"><span data-stu-id="2600d-129">Property</span></span>|<span data-ttu-id="2600d-130">类型</span><span class="sxs-lookup"><span data-stu-id="2600d-130">Type</span></span>|<span data-ttu-id="2600d-131">说明</span><span class="sxs-lookup"><span data-stu-id="2600d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2600d-132">id</span><span class="sxs-lookup"><span data-stu-id="2600d-132">id</span></span>|<span data-ttu-id="2600d-133">String</span><span class="sxs-lookup"><span data-stu-id="2600d-133">String</span></span>|<span data-ttu-id="2600d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2600d-134">Key of the entity.</span></span> <span data-ttu-id="2600d-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2600d-136">displayName</span></span>|<span data-ttu-id="2600d-137">String</span><span class="sxs-lookup"><span data-stu-id="2600d-137">String</span></span>|<span data-ttu-id="2600d-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="2600d-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2600d-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-140">description</span><span class="sxs-lookup"><span data-stu-id="2600d-140">description</span></span>|<span data-ttu-id="2600d-141">String</span><span class="sxs-lookup"><span data-stu-id="2600d-141">String</span></span>|<span data-ttu-id="2600d-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="2600d-142">The description of the app.</span></span> <span data-ttu-id="2600d-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-144">publisher</span><span class="sxs-lookup"><span data-stu-id="2600d-144">publisher</span></span>|<span data-ttu-id="2600d-145">String</span><span class="sxs-lookup"><span data-stu-id="2600d-145">String</span></span>|<span data-ttu-id="2600d-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="2600d-146">The publisher of the app.</span></span> <span data-ttu-id="2600d-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2600d-148">largeIcon</span></span>|[<span data-ttu-id="2600d-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2600d-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2600d-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="2600d-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2600d-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2600d-152">createdDateTime</span></span>|<span data-ttu-id="2600d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2600d-153">DateTimeOffset</span></span>|<span data-ttu-id="2600d-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2600d-154">The date and time the app was created.</span></span> <span data-ttu-id="2600d-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2600d-156">lastModifiedDateTime</span></span>|<span data-ttu-id="2600d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2600d-157">DateTimeOffset</span></span>|<span data-ttu-id="2600d-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2600d-158">The date and time the app was last modified.</span></span> <span data-ttu-id="2600d-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2600d-160">isFeatured</span></span>|<span data-ttu-id="2600d-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2600d-161">Boolean</span></span>|<span data-ttu-id="2600d-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2600d-163">privacyInformationUrl</span></span>|<span data-ttu-id="2600d-164">String</span><span class="sxs-lookup"><span data-stu-id="2600d-164">String</span></span>|<span data-ttu-id="2600d-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="2600d-165">The privacy statement Url.</span></span> <span data-ttu-id="2600d-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2600d-167">informationUrl</span></span>|<span data-ttu-id="2600d-168">String</span><span class="sxs-lookup"><span data-stu-id="2600d-168">String</span></span>|<span data-ttu-id="2600d-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="2600d-169">The more information Url.</span></span> <span data-ttu-id="2600d-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-171">owner</span><span class="sxs-lookup"><span data-stu-id="2600d-171">owner</span></span>|<span data-ttu-id="2600d-172">字符串</span><span class="sxs-lookup"><span data-stu-id="2600d-172">String</span></span>|<span data-ttu-id="2600d-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="2600d-173">The owner of the app.</span></span> <span data-ttu-id="2600d-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-175">developer</span><span class="sxs-lookup"><span data-stu-id="2600d-175">developer</span></span>|<span data-ttu-id="2600d-176">String</span><span class="sxs-lookup"><span data-stu-id="2600d-176">String</span></span>|<span data-ttu-id="2600d-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="2600d-177">The developer of the app.</span></span> <span data-ttu-id="2600d-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-179">notes</span><span class="sxs-lookup"><span data-stu-id="2600d-179">notes</span></span>|<span data-ttu-id="2600d-180">String</span><span class="sxs-lookup"><span data-stu-id="2600d-180">String</span></span>|<span data-ttu-id="2600d-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="2600d-181">Notes for the app.</span></span> <span data-ttu-id="2600d-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="2600d-183">uploadState</span></span>|<span data-ttu-id="2600d-184">Int32</span><span class="sxs-lookup"><span data-stu-id="2600d-184">Int32</span></span>|<span data-ttu-id="2600d-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="2600d-185">The upload state.</span></span> <span data-ttu-id="2600d-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="2600d-187">publishingState</span></span>|[<span data-ttu-id="2600d-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2600d-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2600d-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="2600d-189">The publishing state for the app.</span></span> <span data-ttu-id="2600d-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="2600d-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2600d-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="2600d-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2600d-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="2600d-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2600d-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2600d-193">isAssigned</span></span>|<span data-ttu-id="2600d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="2600d-194">Boolean</span></span>|<span data-ttu-id="2600d-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="2600d-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="2600d-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2600d-197">roleScopeTagIds</span></span>|<span data-ttu-id="2600d-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="2600d-198">String collection</span></span>|<span data-ttu-id="2600d-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="2600d-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="2600d-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2600d-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2600d-201">packageId</span><span class="sxs-lookup"><span data-stu-id="2600d-201">packageId</span></span>|<span data-ttu-id="2600d-202">String</span><span class="sxs-lookup"><span data-stu-id="2600d-202">String</span></span>|<span data-ttu-id="2600d-203">包标识符。</span><span class="sxs-lookup"><span data-stu-id="2600d-203">The package identifier.</span></span>|
|<span data-ttu-id="2600d-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="2600d-204">appIdentifier</span></span>|<span data-ttu-id="2600d-205">String</span><span class="sxs-lookup"><span data-stu-id="2600d-205">String</span></span>|<span data-ttu-id="2600d-206">标识名称。</span><span class="sxs-lookup"><span data-stu-id="2600d-206">The Identity Name.</span></span>|
|<span data-ttu-id="2600d-207">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2600d-207">usedLicenseCount</span></span>|<span data-ttu-id="2600d-208">Int32</span><span class="sxs-lookup"><span data-stu-id="2600d-208">Int32</span></span>|<span data-ttu-id="2600d-209">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="2600d-209">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="2600d-210">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2600d-210">totalLicenseCount</span></span>|<span data-ttu-id="2600d-211">Int32</span><span class="sxs-lookup"><span data-stu-id="2600d-211">Int32</span></span>|<span data-ttu-id="2600d-212">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="2600d-212">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="2600d-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2600d-213">appStoreUrl</span></span>|<span data-ttu-id="2600d-214">String</span><span class="sxs-lookup"><span data-stu-id="2600d-214">String</span></span>|<span data-ttu-id="2600d-215">"播放工作商店" 应用程序 URL。</span><span class="sxs-lookup"><span data-stu-id="2600d-215">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="2600d-216">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="2600d-216">supportsOemConfig</span></span>|<span data-ttu-id="2600d-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="2600d-217">Boolean</span></span>|<span data-ttu-id="2600d-218">此应用是否支持 OEMConfig 策略。</span><span class="sxs-lookup"><span data-stu-id="2600d-218">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="2600d-219">响应</span><span class="sxs-lookup"><span data-stu-id="2600d-219">Response</span></span>
<span data-ttu-id="2600d-220">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2600d-220">If successful, this method returns a `200 OK` response code and an updated [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2600d-221">示例</span><span class="sxs-lookup"><span data-stu-id="2600d-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="2600d-222">请求</span><span class="sxs-lookup"><span data-stu-id="2600d-222">Request</span></span>
<span data-ttu-id="2600d-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2600d-223">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 911

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="2600d-224">响应</span><span class="sxs-lookup"><span data-stu-id="2600d-224">Response</span></span>
<span data-ttu-id="2600d-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2600d-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1083

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```




