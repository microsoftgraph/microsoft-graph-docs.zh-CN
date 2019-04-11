---
title: 创建 microsoftStoreForBusinessApp
description: 创建新的 microsoftStoreForBusinessApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dccf72a194af76ea082f0006bb3e69e7d00ced11
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802784"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="a9e36-103">创建 microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="a9e36-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="a9e36-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a9e36-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9e36-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9e36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9e36-106">创建新的 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a9e36-106">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9e36-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a9e36-107">Prerequisites</span></span>
<span data-ttu-id="a9e36-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9e36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9e36-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9e36-110">Permission type</span></span>|<span data-ttu-id="a9e36-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a9e36-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9e36-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9e36-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9e36-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9e36-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a9e36-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9e36-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9e36-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9e36-115">Not supported.</span></span>|
|<span data-ttu-id="a9e36-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9e36-116">Application</span></span>|<span data-ttu-id="a9e36-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9e36-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9e36-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9e36-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a9e36-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9e36-119">Request headers</span></span>
|<span data-ttu-id="a9e36-120">标头</span><span class="sxs-lookup"><span data-stu-id="a9e36-120">Header</span></span>|<span data-ttu-id="a9e36-121">值</span><span class="sxs-lookup"><span data-stu-id="a9e36-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9e36-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9e36-122">Authorization</span></span>|<span data-ttu-id="a9e36-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a9e36-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9e36-124">接受</span><span class="sxs-lookup"><span data-stu-id="a9e36-124">Accept</span></span>|<span data-ttu-id="a9e36-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9e36-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9e36-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9e36-126">Request body</span></span>
<span data-ttu-id="a9e36-127">在请求正文中，提供 microsoftStoreForBusinessApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9e36-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="a9e36-128">下表显示了创建 microsoftStoreForBusinessApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a9e36-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="a9e36-129">属性</span><span class="sxs-lookup"><span data-stu-id="a9e36-129">Property</span></span>|<span data-ttu-id="a9e36-130">类型</span><span class="sxs-lookup"><span data-stu-id="a9e36-130">Type</span></span>|<span data-ttu-id="a9e36-131">说明</span><span class="sxs-lookup"><span data-stu-id="a9e36-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9e36-132">id</span><span class="sxs-lookup"><span data-stu-id="a9e36-132">id</span></span>|<span data-ttu-id="a9e36-133">String</span><span class="sxs-lookup"><span data-stu-id="a9e36-133">String</span></span>|<span data-ttu-id="a9e36-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a9e36-134">Key of the entity.</span></span> <span data-ttu-id="a9e36-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a9e36-136">displayName</span></span>|<span data-ttu-id="a9e36-137">String</span><span class="sxs-lookup"><span data-stu-id="a9e36-137">String</span></span>|<span data-ttu-id="a9e36-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="a9e36-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a9e36-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-140">description</span><span class="sxs-lookup"><span data-stu-id="a9e36-140">description</span></span>|<span data-ttu-id="a9e36-141">String</span><span class="sxs-lookup"><span data-stu-id="a9e36-141">String</span></span>|<span data-ttu-id="a9e36-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="a9e36-142">The description of the app.</span></span> <span data-ttu-id="a9e36-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-144">publisher</span><span class="sxs-lookup"><span data-stu-id="a9e36-144">publisher</span></span>|<span data-ttu-id="a9e36-145">String</span><span class="sxs-lookup"><span data-stu-id="a9e36-145">String</span></span>|<span data-ttu-id="a9e36-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="a9e36-146">The publisher of the app.</span></span> <span data-ttu-id="a9e36-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a9e36-148">largeIcon</span></span>|[<span data-ttu-id="a9e36-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a9e36-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a9e36-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="a9e36-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a9e36-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9e36-152">createdDateTime</span></span>|<span data-ttu-id="a9e36-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9e36-153">DateTimeOffset</span></span>|<span data-ttu-id="a9e36-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a9e36-154">The date and time the app was created.</span></span> <span data-ttu-id="a9e36-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9e36-156">lastModifiedDateTime</span></span>|<span data-ttu-id="a9e36-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9e36-157">DateTimeOffset</span></span>|<span data-ttu-id="a9e36-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a9e36-158">The date and time the app was last modified.</span></span> <span data-ttu-id="a9e36-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a9e36-160">isFeatured</span></span>|<span data-ttu-id="a9e36-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9e36-161">Boolean</span></span>|<span data-ttu-id="a9e36-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a9e36-163">privacyInformationUrl</span></span>|<span data-ttu-id="a9e36-164">String</span><span class="sxs-lookup"><span data-stu-id="a9e36-164">String</span></span>|<span data-ttu-id="a9e36-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="a9e36-165">The privacy statement Url.</span></span> <span data-ttu-id="a9e36-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a9e36-167">informationUrl</span></span>|<span data-ttu-id="a9e36-168">String</span><span class="sxs-lookup"><span data-stu-id="a9e36-168">String</span></span>|<span data-ttu-id="a9e36-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="a9e36-169">The more information Url.</span></span> <span data-ttu-id="a9e36-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-171">owner</span><span class="sxs-lookup"><span data-stu-id="a9e36-171">owner</span></span>|<span data-ttu-id="a9e36-172">字符串</span><span class="sxs-lookup"><span data-stu-id="a9e36-172">String</span></span>|<span data-ttu-id="a9e36-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="a9e36-173">The owner of the app.</span></span> <span data-ttu-id="a9e36-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-175">developer</span><span class="sxs-lookup"><span data-stu-id="a9e36-175">developer</span></span>|<span data-ttu-id="a9e36-176">String</span><span class="sxs-lookup"><span data-stu-id="a9e36-176">String</span></span>|<span data-ttu-id="a9e36-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="a9e36-177">The developer of the app.</span></span> <span data-ttu-id="a9e36-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-179">notes</span><span class="sxs-lookup"><span data-stu-id="a9e36-179">notes</span></span>|<span data-ttu-id="a9e36-180">String</span><span class="sxs-lookup"><span data-stu-id="a9e36-180">String</span></span>|<span data-ttu-id="a9e36-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="a9e36-181">Notes for the app.</span></span> <span data-ttu-id="a9e36-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="a9e36-183">uploadState</span></span>|<span data-ttu-id="a9e36-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a9e36-184">Int32</span></span>|<span data-ttu-id="a9e36-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="a9e36-185">The upload state.</span></span> <span data-ttu-id="a9e36-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="a9e36-187">publishingState</span></span>|[<span data-ttu-id="a9e36-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a9e36-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a9e36-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="a9e36-189">The publishing state for the app.</span></span> <span data-ttu-id="a9e36-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="a9e36-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a9e36-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="a9e36-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a9e36-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="a9e36-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a9e36-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a9e36-193">isAssigned</span></span>|<span data-ttu-id="a9e36-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9e36-194">Boolean</span></span>|<span data-ttu-id="a9e36-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="a9e36-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a9e36-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a9e36-197">roleScopeTagIds</span></span>|<span data-ttu-id="a9e36-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="a9e36-198">String collection</span></span>|<span data-ttu-id="a9e36-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="a9e36-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a9e36-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="a9e36-201">dependentAppCount</span></span>|<span data-ttu-id="a9e36-202">Int32</span><span class="sxs-lookup"><span data-stu-id="a9e36-202">Int32</span></span>|<span data-ttu-id="a9e36-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="a9e36-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="a9e36-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a9e36-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a9e36-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a9e36-205">usedLicenseCount</span></span>|<span data-ttu-id="a9e36-206">Int32</span><span class="sxs-lookup"><span data-stu-id="a9e36-206">Int32</span></span>|<span data-ttu-id="a9e36-207">使用中的适用于企业的 Microsoft Store 许可证数。</span><span class="sxs-lookup"><span data-stu-id="a9e36-207">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="a9e36-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a9e36-208">totalLicenseCount</span></span>|<span data-ttu-id="a9e36-209">Int32</span><span class="sxs-lookup"><span data-stu-id="a9e36-209">Int32</span></span>|<span data-ttu-id="a9e36-210">适用于企业的 Microsoft Store 许可证总数。</span><span class="sxs-lookup"><span data-stu-id="a9e36-210">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="a9e36-211">productKey</span><span class="sxs-lookup"><span data-stu-id="a9e36-211">productKey</span></span>|<span data-ttu-id="a9e36-212">字串符号</span><span class="sxs-lookup"><span data-stu-id="a9e36-212">String</span></span>|<span data-ttu-id="a9e36-213">应用产品密钥</span><span class="sxs-lookup"><span data-stu-id="a9e36-213">The app product key</span></span>|
|<span data-ttu-id="a9e36-214">licenseType</span><span class="sxs-lookup"><span data-stu-id="a9e36-214">licenseType</span></span>|[<span data-ttu-id="a9e36-215">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="a9e36-215">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="a9e36-216">应用程序许可证类型。</span><span class="sxs-lookup"><span data-stu-id="a9e36-216">The app license type.</span></span> <span data-ttu-id="a9e36-217">可取值为：`offline`、`online`。</span><span class="sxs-lookup"><span data-stu-id="a9e36-217">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="a9e36-218">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="a9e36-218">packageIdentityName</span></span>|<span data-ttu-id="a9e36-219">String</span><span class="sxs-lookup"><span data-stu-id="a9e36-219">String</span></span>|<span data-ttu-id="a9e36-220">应用包标识符</span><span class="sxs-lookup"><span data-stu-id="a9e36-220">The app package identifier</span></span>|
|<span data-ttu-id="a9e36-221">licensingType</span><span class="sxs-lookup"><span data-stu-id="a9e36-221">licensingType</span></span>|[<span data-ttu-id="a9e36-222">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="a9e36-222">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="a9e36-223">受支持的许可证类型。</span><span class="sxs-lookup"><span data-stu-id="a9e36-223">The supported License Type.</span></span>|



## <a name="response"></a><span data-ttu-id="a9e36-224">响应</span><span class="sxs-lookup"><span data-stu-id="a9e36-224">Response</span></span>
<span data-ttu-id="a9e36-225">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a9e36-225">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9e36-226">示例</span><span class="sxs-lookup"><span data-stu-id="a9e36-226">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9e36-227">请求</span><span class="sxs-lookup"><span data-stu-id="a9e36-227">Request</span></span>
<span data-ttu-id="a9e36-228">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9e36-228">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1132

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```

### <a name="response"></a><span data-ttu-id="a9e36-229">响应</span><span class="sxs-lookup"><span data-stu-id="a9e36-229">Response</span></span>
<span data-ttu-id="a9e36-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a9e36-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1304

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  }
}
```





