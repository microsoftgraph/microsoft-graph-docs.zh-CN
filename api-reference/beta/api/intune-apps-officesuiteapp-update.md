---
title: 更新 officeSuiteApp
description: 更新 officeSuiteApp 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8badffb9a84411a00eaa9a52d194c3b431ef7812
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450634"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="50406-103">更新 officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="50406-103">Update officeSuiteApp</span></span>

<span data-ttu-id="50406-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="50406-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50406-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="50406-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50406-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="50406-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50406-107">更新[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="50406-107">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50406-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="50406-108">Prerequisites</span></span>
<span data-ttu-id="50406-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50406-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50406-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="50406-111">Permission type</span></span>|<span data-ttu-id="50406-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="50406-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50406-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50406-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50406-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50406-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="50406-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50406-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50406-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="50406-116">Not supported.</span></span>|
|<span data-ttu-id="50406-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="50406-117">Application</span></span>|<span data-ttu-id="50406-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50406-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50406-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50406-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="50406-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="50406-120">Request headers</span></span>
|<span data-ttu-id="50406-121">标头</span><span class="sxs-lookup"><span data-stu-id="50406-121">Header</span></span>|<span data-ttu-id="50406-122">值</span><span class="sxs-lookup"><span data-stu-id="50406-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50406-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50406-123">Authorization</span></span>|<span data-ttu-id="50406-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="50406-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50406-125">接受</span><span class="sxs-lookup"><span data-stu-id="50406-125">Accept</span></span>|<span data-ttu-id="50406-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50406-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50406-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="50406-127">Request body</span></span>
<span data-ttu-id="50406-128">在请求正文中，提供[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50406-128">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="50406-129">下表显示创建[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="50406-129">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="50406-130">属性</span><span class="sxs-lookup"><span data-stu-id="50406-130">Property</span></span>|<span data-ttu-id="50406-131">类型</span><span class="sxs-lookup"><span data-stu-id="50406-131">Type</span></span>|<span data-ttu-id="50406-132">说明</span><span class="sxs-lookup"><span data-stu-id="50406-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50406-133">id</span><span class="sxs-lookup"><span data-stu-id="50406-133">id</span></span>|<span data-ttu-id="50406-134">字符串</span><span class="sxs-lookup"><span data-stu-id="50406-134">String</span></span>|<span data-ttu-id="50406-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="50406-135">Key of the entity.</span></span> <span data-ttu-id="50406-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-137">displayName</span><span class="sxs-lookup"><span data-stu-id="50406-137">displayName</span></span>|<span data-ttu-id="50406-138">String</span><span class="sxs-lookup"><span data-stu-id="50406-138">String</span></span>|<span data-ttu-id="50406-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="50406-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="50406-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-141">说明</span><span class="sxs-lookup"><span data-stu-id="50406-141">description</span></span>|<span data-ttu-id="50406-142">字符串</span><span class="sxs-lookup"><span data-stu-id="50406-142">String</span></span>|<span data-ttu-id="50406-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="50406-143">The description of the app.</span></span> <span data-ttu-id="50406-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-145">publisher</span><span class="sxs-lookup"><span data-stu-id="50406-145">publisher</span></span>|<span data-ttu-id="50406-146">String</span><span class="sxs-lookup"><span data-stu-id="50406-146">String</span></span>|<span data-ttu-id="50406-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="50406-147">The publisher of the app.</span></span> <span data-ttu-id="50406-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="50406-149">largeIcon</span></span>|[<span data-ttu-id="50406-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="50406-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="50406-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="50406-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="50406-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50406-153">createdDateTime</span></span>|<span data-ttu-id="50406-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50406-154">DateTimeOffset</span></span>|<span data-ttu-id="50406-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="50406-155">The date and time the app was created.</span></span> <span data-ttu-id="50406-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50406-157">lastModifiedDateTime</span></span>|<span data-ttu-id="50406-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50406-158">DateTimeOffset</span></span>|<span data-ttu-id="50406-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="50406-159">The date and time the app was last modified.</span></span> <span data-ttu-id="50406-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="50406-161">isFeatured</span></span>|<span data-ttu-id="50406-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="50406-162">Boolean</span></span>|<span data-ttu-id="50406-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="50406-164">privacyInformationUrl</span></span>|<span data-ttu-id="50406-165">String</span><span class="sxs-lookup"><span data-stu-id="50406-165">String</span></span>|<span data-ttu-id="50406-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="50406-166">The privacy statement Url.</span></span> <span data-ttu-id="50406-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="50406-168">informationUrl</span></span>|<span data-ttu-id="50406-169">String</span><span class="sxs-lookup"><span data-stu-id="50406-169">String</span></span>|<span data-ttu-id="50406-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="50406-170">The more information Url.</span></span> <span data-ttu-id="50406-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-172">owner</span><span class="sxs-lookup"><span data-stu-id="50406-172">owner</span></span>|<span data-ttu-id="50406-173">String</span><span class="sxs-lookup"><span data-stu-id="50406-173">String</span></span>|<span data-ttu-id="50406-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="50406-174">The owner of the app.</span></span> <span data-ttu-id="50406-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-176">developer</span><span class="sxs-lookup"><span data-stu-id="50406-176">developer</span></span>|<span data-ttu-id="50406-177">String</span><span class="sxs-lookup"><span data-stu-id="50406-177">String</span></span>|<span data-ttu-id="50406-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="50406-178">The developer of the app.</span></span> <span data-ttu-id="50406-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-180">notes</span><span class="sxs-lookup"><span data-stu-id="50406-180">notes</span></span>|<span data-ttu-id="50406-181">String</span><span class="sxs-lookup"><span data-stu-id="50406-181">String</span></span>|<span data-ttu-id="50406-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="50406-182">Notes for the app.</span></span> <span data-ttu-id="50406-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="50406-184">uploadState</span></span>|<span data-ttu-id="50406-185">Int32</span><span class="sxs-lookup"><span data-stu-id="50406-185">Int32</span></span>|<span data-ttu-id="50406-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="50406-186">The upload state.</span></span> <span data-ttu-id="50406-187">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="50406-188">publishingState</span></span>|[<span data-ttu-id="50406-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="50406-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="50406-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="50406-190">The publishing state for the app.</span></span> <span data-ttu-id="50406-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="50406-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="50406-192">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="50406-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="50406-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="50406-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="50406-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="50406-194">isAssigned</span></span>|<span data-ttu-id="50406-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="50406-195">Boolean</span></span>|<span data-ttu-id="50406-196">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="50406-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="50406-197">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="50406-198">roleScopeTagIds</span></span>|<span data-ttu-id="50406-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="50406-199">String collection</span></span>|<span data-ttu-id="50406-200">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="50406-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="50406-201">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="50406-202">dependentAppCount</span></span>|<span data-ttu-id="50406-203">Int32</span><span class="sxs-lookup"><span data-stu-id="50406-203">Int32</span></span>|<span data-ttu-id="50406-204">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="50406-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="50406-205">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="50406-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="50406-206">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="50406-206">autoAcceptEula</span></span>|<span data-ttu-id="50406-207">布尔</span><span class="sxs-lookup"><span data-stu-id="50406-207">Boolean</span></span>|<span data-ttu-id="50406-208">要在 enduser 的设备上自动接受 EULA 的值。</span><span class="sxs-lookup"><span data-stu-id="50406-208">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="50406-209">productIds</span><span class="sxs-lookup"><span data-stu-id="50406-209">productIds</span></span>|<span data-ttu-id="50406-210">[officeProductId](../resources/intune-apps-officeproductid.md)集合</span><span class="sxs-lookup"><span data-stu-id="50406-210">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="50406-211">表示 Office365 套件 SKU 的产品 Id。</span><span class="sxs-lookup"><span data-stu-id="50406-211">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="50406-212">可取值为：`o365ProPlusRetail`、`o365BusinessRetail`、`visioProRetail`、`projectProRetail`。</span><span class="sxs-lookup"><span data-stu-id="50406-212">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="50406-213">excludedApps</span><span class="sxs-lookup"><span data-stu-id="50406-213">excludedApps</span></span>|[<span data-ttu-id="50406-214">excludedApps</span><span class="sxs-lookup"><span data-stu-id="50406-214">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="50406-215">表示从所选 Office365 产品 Id 中排除的应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="50406-215">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="50406-216">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="50406-216">useSharedComputerActivation</span></span>|<span data-ttu-id="50406-217">布尔</span><span class="sxs-lookup"><span data-stu-id="50406-217">Boolean</span></span>|<span data-ttu-id="50406-218">表示共享计算机激活是否不适用于 Office365 应用程序套件的属性。</span><span class="sxs-lookup"><span data-stu-id="50406-218">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="50406-219">updateChannel</span><span class="sxs-lookup"><span data-stu-id="50406-219">updateChannel</span></span>|[<span data-ttu-id="50406-220">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="50406-220">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="50406-221">用于表示 Office365 更新通道的属性。</span><span class="sxs-lookup"><span data-stu-id="50406-221">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="50406-222">可取值为：`none`、`current`、`deferred`、`firstReleaseCurrent`、`firstReleaseDeferred`。</span><span class="sxs-lookup"><span data-stu-id="50406-222">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="50406-223">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="50406-223">officePlatformArchitecture</span></span>|[<span data-ttu-id="50406-224">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="50406-224">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="50406-225">表示 Office365 应用程序套件版本的属性。</span><span class="sxs-lookup"><span data-stu-id="50406-225">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="50406-226">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="50406-226">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="50406-227">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="50406-227">localesToInstall</span></span>|<span data-ttu-id="50406-228">String 集合</span><span class="sxs-lookup"><span data-stu-id="50406-228">String collection</span></span>|<span data-ttu-id="50406-229">用于表示安装 Office365 中的应用程序时所安装的区域设置的属性。</span><span class="sxs-lookup"><span data-stu-id="50406-229">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="50406-230">它使用标准 RFC 6033。</span><span class="sxs-lookup"><span data-stu-id="50406-230">It uses standard RFC 6033.</span></span> <span data-ttu-id="50406-231">Refhttps://technet.microsoft.com/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="50406-231">Ref: https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="50406-232">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="50406-232">installProgressDisplayLevel</span></span>|[<span data-ttu-id="50406-233">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="50406-233">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="50406-234">指定设备上安装进度设置 UI 的显示级别。</span><span class="sxs-lookup"><span data-stu-id="50406-234">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="50406-235">可取值为：`none`、`full`。</span><span class="sxs-lookup"><span data-stu-id="50406-235">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="50406-236">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="50406-236">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="50406-237">布尔</span><span class="sxs-lookup"><span data-stu-id="50406-237">Boolean</span></span>|<span data-ttu-id="50406-238">用于确定是否在将 Office365 应用套件部署到设备时是否卸载现有 Office MSI 的属性。</span><span class="sxs-lookup"><span data-stu-id="50406-238">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="50406-239">targetVersion</span><span class="sxs-lookup"><span data-stu-id="50406-239">targetVersion</span></span>|<span data-ttu-id="50406-240">String</span><span class="sxs-lookup"><span data-stu-id="50406-240">String</span></span>|<span data-ttu-id="50406-241">表示应在设备上保持部署的 Office365 应用程序套件的特定目标版本的属性。</span><span class="sxs-lookup"><span data-stu-id="50406-241">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="50406-242">updateVersion</span><span class="sxs-lookup"><span data-stu-id="50406-242">updateVersion</span></span>|<span data-ttu-id="50406-243">String</span><span class="sxs-lookup"><span data-stu-id="50406-243">String</span></span>|<span data-ttu-id="50406-244">表示可用于 Office365 应用程序套件的特定目标版本的更新版本的属性。</span><span class="sxs-lookup"><span data-stu-id="50406-244">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="50406-245">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="50406-245">officeConfigurationXml</span></span>|<span data-ttu-id="50406-246">Binary</span><span class="sxs-lookup"><span data-stu-id="50406-246">Binary</span></span>|<span data-ttu-id="50406-247">表示可为 Office 专业增强版应用程序指定的 XML 配置文件的属性。</span><span class="sxs-lookup"><span data-stu-id="50406-247">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="50406-248">优先于所有其他属性。</span><span class="sxs-lookup"><span data-stu-id="50406-248">Takes precedence over all other properties.</span></span> <span data-ttu-id="50406-249">如果存在，将使用 XML 配置文件来创建应用程序。</span><span class="sxs-lookup"><span data-stu-id="50406-249">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="50406-250">响应</span><span class="sxs-lookup"><span data-stu-id="50406-250">Response</span></span>
<span data-ttu-id="50406-251">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="50406-251">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50406-252">示例</span><span class="sxs-lookup"><span data-stu-id="50406-252">Example</span></span>

### <a name="request"></a><span data-ttu-id="50406-253">请求</span><span class="sxs-lookup"><span data-stu-id="50406-253">Request</span></span>
<span data-ttu-id="50406-254">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50406-254">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1599

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="50406-255">响应</span><span class="sxs-lookup"><span data-stu-id="50406-255">Response</span></span>
<span data-ttu-id="50406-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50406-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1771

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "id": "9b263b46-3b46-9b26-463b-269b463b269b",
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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```





