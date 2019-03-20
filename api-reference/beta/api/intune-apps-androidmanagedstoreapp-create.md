---
title: 创建 androidManagedStoreApp
description: 创建新的 androidManagedStoreApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aee8b173e7b0a1af7ef730efbb43b3347cdb0162
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572528"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="a4231-103">创建 androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="a4231-103">Create androidManagedStoreApp</span></span>

> <span data-ttu-id="a4231-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a4231-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4231-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4231-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4231-106">创建新的[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a4231-106">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4231-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4231-107">Prerequisites</span></span>
<span data-ttu-id="a4231-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a4231-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a4231-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4231-110">Permission type</span></span>|<span data-ttu-id="a4231-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a4231-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4231-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4231-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4231-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4231-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a4231-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4231-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4231-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4231-115">Not supported.</span></span>|
|<span data-ttu-id="a4231-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4231-116">Application</span></span>|<span data-ttu-id="a4231-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4231-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4231-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4231-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a4231-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4231-119">Request headers</span></span>
|<span data-ttu-id="a4231-120">标头</span><span class="sxs-lookup"><span data-stu-id="a4231-120">Header</span></span>|<span data-ttu-id="a4231-121">值</span><span class="sxs-lookup"><span data-stu-id="a4231-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4231-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4231-122">Authorization</span></span>|<span data-ttu-id="a4231-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4231-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4231-124">接受</span><span class="sxs-lookup"><span data-stu-id="a4231-124">Accept</span></span>|<span data-ttu-id="a4231-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4231-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4231-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4231-126">Request body</span></span>
<span data-ttu-id="a4231-127">在请求正文中, 提供 androidManagedStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4231-127">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="a4231-128">下表显示创建 androidManagedStoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a4231-128">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="a4231-129">属性</span><span class="sxs-lookup"><span data-stu-id="a4231-129">Property</span></span>|<span data-ttu-id="a4231-130">类型</span><span class="sxs-lookup"><span data-stu-id="a4231-130">Type</span></span>|<span data-ttu-id="a4231-131">说明</span><span class="sxs-lookup"><span data-stu-id="a4231-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4231-132">id</span><span class="sxs-lookup"><span data-stu-id="a4231-132">id</span></span>|<span data-ttu-id="a4231-133">String</span><span class="sxs-lookup"><span data-stu-id="a4231-133">String</span></span>|<span data-ttu-id="a4231-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a4231-134">Key of the entity.</span></span> <span data-ttu-id="a4231-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a4231-136">displayName</span></span>|<span data-ttu-id="a4231-137">字符串</span><span class="sxs-lookup"><span data-stu-id="a4231-137">String</span></span>|<span data-ttu-id="a4231-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="a4231-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a4231-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-140">说明</span><span class="sxs-lookup"><span data-stu-id="a4231-140">description</span></span>|<span data-ttu-id="a4231-141">字符串</span><span class="sxs-lookup"><span data-stu-id="a4231-141">String</span></span>|<span data-ttu-id="a4231-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="a4231-142">The description of the app.</span></span> <span data-ttu-id="a4231-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-144">publisher</span><span class="sxs-lookup"><span data-stu-id="a4231-144">publisher</span></span>|<span data-ttu-id="a4231-145">字符串</span><span class="sxs-lookup"><span data-stu-id="a4231-145">String</span></span>|<span data-ttu-id="a4231-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="a4231-146">The publisher of the app.</span></span> <span data-ttu-id="a4231-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a4231-148">largeIcon</span></span>|[<span data-ttu-id="a4231-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a4231-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a4231-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="a4231-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a4231-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4231-152">createdDateTime</span></span>|<span data-ttu-id="a4231-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4231-153">DateTimeOffset</span></span>|<span data-ttu-id="a4231-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a4231-154">The date and time the app was created.</span></span> <span data-ttu-id="a4231-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4231-156">lastModifiedDateTime</span></span>|<span data-ttu-id="a4231-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4231-157">DateTimeOffset</span></span>|<span data-ttu-id="a4231-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a4231-158">The date and time the app was last modified.</span></span> <span data-ttu-id="a4231-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a4231-160">isFeatured</span></span>|<span data-ttu-id="a4231-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4231-161">Boolean</span></span>|<span data-ttu-id="a4231-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a4231-163">privacyInformationUrl</span></span>|<span data-ttu-id="a4231-164">字符串</span><span class="sxs-lookup"><span data-stu-id="a4231-164">String</span></span>|<span data-ttu-id="a4231-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="a4231-165">The privacy statement Url.</span></span> <span data-ttu-id="a4231-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a4231-167">informationUrl</span></span>|<span data-ttu-id="a4231-168">字符串</span><span class="sxs-lookup"><span data-stu-id="a4231-168">String</span></span>|<span data-ttu-id="a4231-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="a4231-169">The more information Url.</span></span> <span data-ttu-id="a4231-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-171">owner</span><span class="sxs-lookup"><span data-stu-id="a4231-171">owner</span></span>|<span data-ttu-id="a4231-172">字符串</span><span class="sxs-lookup"><span data-stu-id="a4231-172">String</span></span>|<span data-ttu-id="a4231-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="a4231-173">The owner of the app.</span></span> <span data-ttu-id="a4231-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-175">developer</span><span class="sxs-lookup"><span data-stu-id="a4231-175">developer</span></span>|<span data-ttu-id="a4231-176">字符串</span><span class="sxs-lookup"><span data-stu-id="a4231-176">String</span></span>|<span data-ttu-id="a4231-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="a4231-177">The developer of the app.</span></span> <span data-ttu-id="a4231-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-179">notes</span><span class="sxs-lookup"><span data-stu-id="a4231-179">notes</span></span>|<span data-ttu-id="a4231-180">字符串</span><span class="sxs-lookup"><span data-stu-id="a4231-180">String</span></span>|<span data-ttu-id="a4231-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="a4231-181">Notes for the app.</span></span> <span data-ttu-id="a4231-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="a4231-183">uploadState</span></span>|<span data-ttu-id="a4231-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a4231-184">Int32</span></span>|<span data-ttu-id="a4231-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="a4231-185">The upload state.</span></span> <span data-ttu-id="a4231-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="a4231-187">publishingState</span></span>|[<span data-ttu-id="a4231-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a4231-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a4231-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="a4231-189">The publishing state for the app.</span></span> <span data-ttu-id="a4231-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="a4231-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a4231-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="a4231-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a4231-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="a4231-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a4231-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a4231-193">isAssigned</span></span>|<span data-ttu-id="a4231-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4231-194">Boolean</span></span>|<span data-ttu-id="a4231-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="a4231-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a4231-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a4231-197">roleScopeTagIds</span></span>|<span data-ttu-id="a4231-198">String collection</span><span class="sxs-lookup"><span data-stu-id="a4231-198">String collection</span></span>|<span data-ttu-id="a4231-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="a4231-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a4231-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a4231-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a4231-201">packageId</span><span class="sxs-lookup"><span data-stu-id="a4231-201">packageId</span></span>|<span data-ttu-id="a4231-202">字符串</span><span class="sxs-lookup"><span data-stu-id="a4231-202">String</span></span>|<span data-ttu-id="a4231-203">包标识符。</span><span class="sxs-lookup"><span data-stu-id="a4231-203">The package identifier.</span></span>|
|<span data-ttu-id="a4231-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="a4231-204">appIdentifier</span></span>|<span data-ttu-id="a4231-205">String</span><span class="sxs-lookup"><span data-stu-id="a4231-205">String</span></span>|<span data-ttu-id="a4231-206">标识名称。</span><span class="sxs-lookup"><span data-stu-id="a4231-206">The Identity Name.</span></span>|
|<span data-ttu-id="a4231-207">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a4231-207">usedLicenseCount</span></span>|<span data-ttu-id="a4231-208">Int32</span><span class="sxs-lookup"><span data-stu-id="a4231-208">Int32</span></span>|<span data-ttu-id="a4231-209">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="a4231-209">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="a4231-210">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a4231-210">totalLicenseCount</span></span>|<span data-ttu-id="a4231-211">Int32</span><span class="sxs-lookup"><span data-stu-id="a4231-211">Int32</span></span>|<span data-ttu-id="a4231-212">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="a4231-212">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="a4231-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a4231-213">appStoreUrl</span></span>|<span data-ttu-id="a4231-214">String</span><span class="sxs-lookup"><span data-stu-id="a4231-214">String</span></span>|<span data-ttu-id="a4231-215">"播放工作商店" 应用程序 URL。</span><span class="sxs-lookup"><span data-stu-id="a4231-215">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="a4231-216">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="a4231-216">supportsOemConfig</span></span>|<span data-ttu-id="a4231-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4231-217">Boolean</span></span>|<span data-ttu-id="a4231-218">此应用是否支持 OEMConfig 策略。</span><span class="sxs-lookup"><span data-stu-id="a4231-218">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="a4231-219">响应</span><span class="sxs-lookup"><span data-stu-id="a4231-219">Response</span></span>
<span data-ttu-id="a4231-220">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a4231-220">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4231-221">示例</span><span class="sxs-lookup"><span data-stu-id="a4231-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4231-222">请求</span><span class="sxs-lookup"><span data-stu-id="a4231-222">Request</span></span>
<span data-ttu-id="a4231-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4231-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="a4231-224">响应</span><span class="sxs-lookup"><span data-stu-id="a4231-224">Response</span></span>
<span data-ttu-id="a4231-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4231-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




