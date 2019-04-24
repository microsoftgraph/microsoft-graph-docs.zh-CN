---
title: 创建 androidManagedStoreApp
description: 创建新的 androidManagedStoreApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eeb677be50132c8da0d48ad564eba8284fd69fef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32496889"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="81392-103">创建 androidManagedStoreApp</span><span class="sxs-lookup"><span data-stu-id="81392-103">Create androidManagedStoreApp</span></span>

> <span data-ttu-id="81392-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="81392-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81392-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81392-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81392-106">创建新的[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="81392-106">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81392-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="81392-107">Prerequisites</span></span>
<span data-ttu-id="81392-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81392-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81392-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="81392-110">Permission type</span></span>|<span data-ttu-id="81392-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="81392-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81392-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81392-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81392-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81392-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="81392-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81392-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81392-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="81392-115">Not supported.</span></span>|
|<span data-ttu-id="81392-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="81392-116">Application</span></span>|<span data-ttu-id="81392-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="81392-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81392-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81392-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="81392-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="81392-119">Request headers</span></span>
|<span data-ttu-id="81392-120">标头</span><span class="sxs-lookup"><span data-stu-id="81392-120">Header</span></span>|<span data-ttu-id="81392-121">值</span><span class="sxs-lookup"><span data-stu-id="81392-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81392-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="81392-122">Authorization</span></span>|<span data-ttu-id="81392-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="81392-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81392-124">接受</span><span class="sxs-lookup"><span data-stu-id="81392-124">Accept</span></span>|<span data-ttu-id="81392-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81392-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81392-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="81392-126">Request body</span></span>
<span data-ttu-id="81392-127">在请求正文中, 提供 androidManagedStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81392-127">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="81392-128">下表显示创建 androidManagedStoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="81392-128">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="81392-129">属性</span><span class="sxs-lookup"><span data-stu-id="81392-129">Property</span></span>|<span data-ttu-id="81392-130">类型</span><span class="sxs-lookup"><span data-stu-id="81392-130">Type</span></span>|<span data-ttu-id="81392-131">说明</span><span class="sxs-lookup"><span data-stu-id="81392-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81392-132">id</span><span class="sxs-lookup"><span data-stu-id="81392-132">id</span></span>|<span data-ttu-id="81392-133">String</span><span class="sxs-lookup"><span data-stu-id="81392-133">String</span></span>|<span data-ttu-id="81392-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="81392-134">Key of the entity.</span></span> <span data-ttu-id="81392-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-136">displayName</span><span class="sxs-lookup"><span data-stu-id="81392-136">displayName</span></span>|<span data-ttu-id="81392-137">字符串</span><span class="sxs-lookup"><span data-stu-id="81392-137">String</span></span>|<span data-ttu-id="81392-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="81392-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="81392-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-140">description</span><span class="sxs-lookup"><span data-stu-id="81392-140">description</span></span>|<span data-ttu-id="81392-141">字符串</span><span class="sxs-lookup"><span data-stu-id="81392-141">String</span></span>|<span data-ttu-id="81392-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="81392-142">The description of the app.</span></span> <span data-ttu-id="81392-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-144">publisher</span><span class="sxs-lookup"><span data-stu-id="81392-144">publisher</span></span>|<span data-ttu-id="81392-145">字符串</span><span class="sxs-lookup"><span data-stu-id="81392-145">String</span></span>|<span data-ttu-id="81392-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="81392-146">The publisher of the app.</span></span> <span data-ttu-id="81392-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="81392-148">largeIcon</span></span>|[<span data-ttu-id="81392-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="81392-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="81392-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="81392-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="81392-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81392-152">createdDateTime</span></span>|<span data-ttu-id="81392-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81392-153">DateTimeOffset</span></span>|<span data-ttu-id="81392-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="81392-154">The date and time the app was created.</span></span> <span data-ttu-id="81392-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="81392-156">lastModifiedDateTime</span></span>|<span data-ttu-id="81392-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81392-157">DateTimeOffset</span></span>|<span data-ttu-id="81392-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="81392-158">The date and time the app was last modified.</span></span> <span data-ttu-id="81392-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="81392-160">isFeatured</span></span>|<span data-ttu-id="81392-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="81392-161">Boolean</span></span>|<span data-ttu-id="81392-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="81392-163">privacyInformationUrl</span></span>|<span data-ttu-id="81392-164">字符串</span><span class="sxs-lookup"><span data-stu-id="81392-164">String</span></span>|<span data-ttu-id="81392-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="81392-165">The privacy statement Url.</span></span> <span data-ttu-id="81392-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="81392-167">informationUrl</span></span>|<span data-ttu-id="81392-168">字符串</span><span class="sxs-lookup"><span data-stu-id="81392-168">String</span></span>|<span data-ttu-id="81392-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="81392-169">The more information Url.</span></span> <span data-ttu-id="81392-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-171">owner</span><span class="sxs-lookup"><span data-stu-id="81392-171">owner</span></span>|<span data-ttu-id="81392-172">字符串</span><span class="sxs-lookup"><span data-stu-id="81392-172">String</span></span>|<span data-ttu-id="81392-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="81392-173">The owner of the app.</span></span> <span data-ttu-id="81392-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-175">developer</span><span class="sxs-lookup"><span data-stu-id="81392-175">developer</span></span>|<span data-ttu-id="81392-176">字符串</span><span class="sxs-lookup"><span data-stu-id="81392-176">String</span></span>|<span data-ttu-id="81392-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="81392-177">The developer of the app.</span></span> <span data-ttu-id="81392-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-179">notes</span><span class="sxs-lookup"><span data-stu-id="81392-179">notes</span></span>|<span data-ttu-id="81392-180">字符串</span><span class="sxs-lookup"><span data-stu-id="81392-180">String</span></span>|<span data-ttu-id="81392-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="81392-181">Notes for the app.</span></span> <span data-ttu-id="81392-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="81392-183">uploadState</span></span>|<span data-ttu-id="81392-184">Int32</span><span class="sxs-lookup"><span data-stu-id="81392-184">Int32</span></span>|<span data-ttu-id="81392-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="81392-185">The upload state.</span></span> <span data-ttu-id="81392-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="81392-187">publishingState</span></span>|[<span data-ttu-id="81392-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="81392-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="81392-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="81392-189">The publishing state for the app.</span></span> <span data-ttu-id="81392-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="81392-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="81392-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="81392-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="81392-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="81392-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="81392-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="81392-193">isAssigned</span></span>|<span data-ttu-id="81392-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="81392-194">Boolean</span></span>|<span data-ttu-id="81392-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="81392-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="81392-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="81392-197">roleScopeTagIds</span></span>|<span data-ttu-id="81392-198">String collection</span><span class="sxs-lookup"><span data-stu-id="81392-198">String collection</span></span>|<span data-ttu-id="81392-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="81392-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="81392-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="81392-201">dependentAppCount</span></span>|<span data-ttu-id="81392-202">Int32</span><span class="sxs-lookup"><span data-stu-id="81392-202">Int32</span></span>|<span data-ttu-id="81392-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="81392-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="81392-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="81392-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="81392-205">packageId</span><span class="sxs-lookup"><span data-stu-id="81392-205">packageId</span></span>|<span data-ttu-id="81392-206">字符串</span><span class="sxs-lookup"><span data-stu-id="81392-206">String</span></span>|<span data-ttu-id="81392-207">包标识符。</span><span class="sxs-lookup"><span data-stu-id="81392-207">The package identifier.</span></span>|
|<span data-ttu-id="81392-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="81392-208">appIdentifier</span></span>|<span data-ttu-id="81392-209">String</span><span class="sxs-lookup"><span data-stu-id="81392-209">String</span></span>|<span data-ttu-id="81392-210">标识名称。</span><span class="sxs-lookup"><span data-stu-id="81392-210">The Identity Name.</span></span>|
|<span data-ttu-id="81392-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="81392-211">usedLicenseCount</span></span>|<span data-ttu-id="81392-212">Int32</span><span class="sxs-lookup"><span data-stu-id="81392-212">Int32</span></span>|<span data-ttu-id="81392-213">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="81392-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="81392-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="81392-214">totalLicenseCount</span></span>|<span data-ttu-id="81392-215">Int32</span><span class="sxs-lookup"><span data-stu-id="81392-215">Int32</span></span>|<span data-ttu-id="81392-216">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="81392-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="81392-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="81392-217">appStoreUrl</span></span>|<span data-ttu-id="81392-218">String</span><span class="sxs-lookup"><span data-stu-id="81392-218">String</span></span>|<span data-ttu-id="81392-219">"播放工作商店" 应用程序 URL。</span><span class="sxs-lookup"><span data-stu-id="81392-219">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="81392-220">supportsOemConfig</span><span class="sxs-lookup"><span data-stu-id="81392-220">supportsOemConfig</span></span>|<span data-ttu-id="81392-221">布尔</span><span class="sxs-lookup"><span data-stu-id="81392-221">Boolean</span></span>|<span data-ttu-id="81392-222">此应用是否支持 OEMConfig 策略。</span><span class="sxs-lookup"><span data-stu-id="81392-222">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="81392-223">响应</span><span class="sxs-lookup"><span data-stu-id="81392-223">Response</span></span>
<span data-ttu-id="81392-224">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="81392-224">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81392-225">示例</span><span class="sxs-lookup"><span data-stu-id="81392-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="81392-226">请求</span><span class="sxs-lookup"><span data-stu-id="81392-226">Request</span></span>
<span data-ttu-id="81392-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="81392-227">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 938

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
  "dependentAppCount": 1,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="81392-228">响应</span><span class="sxs-lookup"><span data-stu-id="81392-228">Response</span></span>
<span data-ttu-id="81392-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="81392-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1110

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
  "dependentAppCount": 1,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```





