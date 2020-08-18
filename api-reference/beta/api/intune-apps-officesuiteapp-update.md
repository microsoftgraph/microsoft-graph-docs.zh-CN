---
title: 更新 officeSuiteApp
description: 更新 officeSuiteApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7570ac026779d0508a40991179fdbb5496c8c3b6
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791909"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="07f52-103">更新 officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="07f52-103">Update officeSuiteApp</span></span>

<span data-ttu-id="07f52-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07f52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07f52-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="07f52-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07f52-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07f52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07f52-107">更新 [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="07f52-107">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07f52-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="07f52-108">Prerequisites</span></span>
<span data-ttu-id="07f52-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07f52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07f52-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="07f52-111">Permission type</span></span>|<span data-ttu-id="07f52-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="07f52-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07f52-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07f52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07f52-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07f52-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="07f52-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07f52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07f52-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="07f52-116">Not supported.</span></span>|
|<span data-ttu-id="07f52-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="07f52-117">Application</span></span>|<span data-ttu-id="07f52-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07f52-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07f52-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07f52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="07f52-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="07f52-120">Request headers</span></span>
|<span data-ttu-id="07f52-121">标头</span><span class="sxs-lookup"><span data-stu-id="07f52-121">Header</span></span>|<span data-ttu-id="07f52-122">值</span><span class="sxs-lookup"><span data-stu-id="07f52-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07f52-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07f52-123">Authorization</span></span>|<span data-ttu-id="07f52-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="07f52-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07f52-125">接受</span><span class="sxs-lookup"><span data-stu-id="07f52-125">Accept</span></span>|<span data-ttu-id="07f52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07f52-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07f52-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="07f52-127">Request body</span></span>
<span data-ttu-id="07f52-128">在请求正文中，提供 [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07f52-128">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="07f52-129">下表显示创建 [officeSuiteApp](../resources/intune-apps-officesuiteapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="07f52-129">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="07f52-130">属性</span><span class="sxs-lookup"><span data-stu-id="07f52-130">Property</span></span>|<span data-ttu-id="07f52-131">类型</span><span class="sxs-lookup"><span data-stu-id="07f52-131">Type</span></span>|<span data-ttu-id="07f52-132">说明</span><span class="sxs-lookup"><span data-stu-id="07f52-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07f52-133">id</span><span class="sxs-lookup"><span data-stu-id="07f52-133">id</span></span>|<span data-ttu-id="07f52-134">String</span><span class="sxs-lookup"><span data-stu-id="07f52-134">String</span></span>|<span data-ttu-id="07f52-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="07f52-135">Key of the entity.</span></span> <span data-ttu-id="07f52-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-137">displayName</span><span class="sxs-lookup"><span data-stu-id="07f52-137">displayName</span></span>|<span data-ttu-id="07f52-138">String</span><span class="sxs-lookup"><span data-stu-id="07f52-138">String</span></span>|<span data-ttu-id="07f52-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="07f52-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="07f52-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-141">description</span><span class="sxs-lookup"><span data-stu-id="07f52-141">description</span></span>|<span data-ttu-id="07f52-142">String</span><span class="sxs-lookup"><span data-stu-id="07f52-142">String</span></span>|<span data-ttu-id="07f52-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="07f52-143">The description of the app.</span></span> <span data-ttu-id="07f52-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-145">publisher</span><span class="sxs-lookup"><span data-stu-id="07f52-145">publisher</span></span>|<span data-ttu-id="07f52-146">String</span><span class="sxs-lookup"><span data-stu-id="07f52-146">String</span></span>|<span data-ttu-id="07f52-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="07f52-147">The publisher of the app.</span></span> <span data-ttu-id="07f52-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="07f52-149">largeIcon</span></span>|[<span data-ttu-id="07f52-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="07f52-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="07f52-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="07f52-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="07f52-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07f52-153">createdDateTime</span></span>|<span data-ttu-id="07f52-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07f52-154">DateTimeOffset</span></span>|<span data-ttu-id="07f52-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="07f52-155">The date and time the app was created.</span></span> <span data-ttu-id="07f52-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07f52-157">lastModifiedDateTime</span></span>|<span data-ttu-id="07f52-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07f52-158">DateTimeOffset</span></span>|<span data-ttu-id="07f52-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="07f52-159">The date and time the app was last modified.</span></span> <span data-ttu-id="07f52-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="07f52-161">isFeatured</span></span>|<span data-ttu-id="07f52-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="07f52-162">Boolean</span></span>|<span data-ttu-id="07f52-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="07f52-164">privacyInformationUrl</span></span>|<span data-ttu-id="07f52-165">String</span><span class="sxs-lookup"><span data-stu-id="07f52-165">String</span></span>|<span data-ttu-id="07f52-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="07f52-166">The privacy statement Url.</span></span> <span data-ttu-id="07f52-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="07f52-168">informationUrl</span></span>|<span data-ttu-id="07f52-169">String</span><span class="sxs-lookup"><span data-stu-id="07f52-169">String</span></span>|<span data-ttu-id="07f52-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="07f52-170">The more information Url.</span></span> <span data-ttu-id="07f52-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-172">所有者</span><span class="sxs-lookup"><span data-stu-id="07f52-172">owner</span></span>|<span data-ttu-id="07f52-173">String</span><span class="sxs-lookup"><span data-stu-id="07f52-173">String</span></span>|<span data-ttu-id="07f52-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="07f52-174">The owner of the app.</span></span> <span data-ttu-id="07f52-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-176">developer</span><span class="sxs-lookup"><span data-stu-id="07f52-176">developer</span></span>|<span data-ttu-id="07f52-177">String</span><span class="sxs-lookup"><span data-stu-id="07f52-177">String</span></span>|<span data-ttu-id="07f52-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="07f52-178">The developer of the app.</span></span> <span data-ttu-id="07f52-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-180">notes</span><span class="sxs-lookup"><span data-stu-id="07f52-180">notes</span></span>|<span data-ttu-id="07f52-181">String</span><span class="sxs-lookup"><span data-stu-id="07f52-181">String</span></span>|<span data-ttu-id="07f52-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="07f52-182">Notes for the app.</span></span> <span data-ttu-id="07f52-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="07f52-184">uploadState</span></span>|<span data-ttu-id="07f52-185">Int32</span><span class="sxs-lookup"><span data-stu-id="07f52-185">Int32</span></span>|<span data-ttu-id="07f52-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="07f52-186">The upload state.</span></span> <span data-ttu-id="07f52-187">可能的值包括： 0- `Not Ready` 、1- `Ready` 、2- `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="07f52-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="07f52-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="07f52-189">publishingState</span></span>|[<span data-ttu-id="07f52-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="07f52-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="07f52-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="07f52-191">The publishing state for the app.</span></span> <span data-ttu-id="07f52-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="07f52-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="07f52-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="07f52-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="07f52-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="07f52-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="07f52-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="07f52-195">isAssigned</span></span>|<span data-ttu-id="07f52-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="07f52-196">Boolean</span></span>|<span data-ttu-id="07f52-197">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="07f52-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="07f52-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="07f52-199">roleScopeTagIds</span></span>|<span data-ttu-id="07f52-200">字符串集合</span><span class="sxs-lookup"><span data-stu-id="07f52-200">String collection</span></span>|<span data-ttu-id="07f52-201">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="07f52-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="07f52-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="07f52-203">dependentAppCount</span></span>|<span data-ttu-id="07f52-204">Int32</span><span class="sxs-lookup"><span data-stu-id="07f52-204">Int32</span></span>|<span data-ttu-id="07f52-205">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="07f52-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="07f52-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="07f52-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="07f52-207">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="07f52-207">autoAcceptEula</span></span>|<span data-ttu-id="07f52-208">布尔值</span><span class="sxs-lookup"><span data-stu-id="07f52-208">Boolean</span></span>|<span data-ttu-id="07f52-209">要在 enduser 的设备上自动接受 EULA 的值。</span><span class="sxs-lookup"><span data-stu-id="07f52-209">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="07f52-210">productIds</span><span class="sxs-lookup"><span data-stu-id="07f52-210">productIds</span></span>|<span data-ttu-id="07f52-211">[officeProductId](../resources/intune-apps-officeproductid.md) 集合</span><span class="sxs-lookup"><span data-stu-id="07f52-211">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="07f52-212">表示 Office365 套件 SKU 的产品 Id。</span><span class="sxs-lookup"><span data-stu-id="07f52-212">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="07f52-213">可取值为：`o365ProPlusRetail`、`o365BusinessRetail`、`visioProRetail`、`projectProRetail`。</span><span class="sxs-lookup"><span data-stu-id="07f52-213">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="07f52-214">excludedApps</span><span class="sxs-lookup"><span data-stu-id="07f52-214">excludedApps</span></span>|[<span data-ttu-id="07f52-215">excludedApps</span><span class="sxs-lookup"><span data-stu-id="07f52-215">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="07f52-216">表示从所选 Office365 产品 Id 中排除的应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="07f52-216">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="07f52-217">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="07f52-217">useSharedComputerActivation</span></span>|<span data-ttu-id="07f52-218">布尔值</span><span class="sxs-lookup"><span data-stu-id="07f52-218">Boolean</span></span>|<span data-ttu-id="07f52-219">表示共享计算机激活是否不适用于 Office365 应用程序套件的属性。</span><span class="sxs-lookup"><span data-stu-id="07f52-219">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="07f52-220">updateChannel</span><span class="sxs-lookup"><span data-stu-id="07f52-220">updateChannel</span></span>|[<span data-ttu-id="07f52-221">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="07f52-221">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="07f52-222">用于表示 Office365 更新通道的属性。</span><span class="sxs-lookup"><span data-stu-id="07f52-222">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="07f52-223">可取值为：`none`、`current`、`deferred`、`firstReleaseCurrent`、`firstReleaseDeferred`、`monthlyEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="07f52-223">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`, `monthlyEnterprise`.</span></span>|
|<span data-ttu-id="07f52-224">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="07f52-224">officePlatformArchitecture</span></span>|[<span data-ttu-id="07f52-225">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="07f52-225">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="07f52-226">表示 Office365 应用程序套件版本的属性。</span><span class="sxs-lookup"><span data-stu-id="07f52-226">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="07f52-227">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="07f52-227">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="07f52-228">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="07f52-228">localesToInstall</span></span>|<span data-ttu-id="07f52-229">字符串集合</span><span class="sxs-lookup"><span data-stu-id="07f52-229">String collection</span></span>|<span data-ttu-id="07f52-230">用于表示安装 Office365 中的应用程序时所安装的区域设置的属性。</span><span class="sxs-lookup"><span data-stu-id="07f52-230">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="07f52-231">它使用标准 RFC 6033。</span><span class="sxs-lookup"><span data-stu-id="07f52-231">It uses standard RFC 6033.</span></span> <span data-ttu-id="07f52-232">Ref https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="07f52-232">Ref: https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="07f52-233">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="07f52-233">installProgressDisplayLevel</span></span>|[<span data-ttu-id="07f52-234">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="07f52-234">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="07f52-235">指定设备上安装进度设置 UI 的显示级别。</span><span class="sxs-lookup"><span data-stu-id="07f52-235">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="07f52-236">可取值为：`none`、`full`。</span><span class="sxs-lookup"><span data-stu-id="07f52-236">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="07f52-237">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="07f52-237">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="07f52-238">布尔值</span><span class="sxs-lookup"><span data-stu-id="07f52-238">Boolean</span></span>|<span data-ttu-id="07f52-239">用于确定是否在将 Office365 应用套件部署到设备时是否卸载现有 Office MSI 的属性。</span><span class="sxs-lookup"><span data-stu-id="07f52-239">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="07f52-240">targetVersion</span><span class="sxs-lookup"><span data-stu-id="07f52-240">targetVersion</span></span>|<span data-ttu-id="07f52-241">String</span><span class="sxs-lookup"><span data-stu-id="07f52-241">String</span></span>|<span data-ttu-id="07f52-242">表示应在设备上保持部署的 Office365 应用程序套件的特定目标版本的属性。</span><span class="sxs-lookup"><span data-stu-id="07f52-242">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="07f52-243">updateVersion</span><span class="sxs-lookup"><span data-stu-id="07f52-243">updateVersion</span></span>|<span data-ttu-id="07f52-244">String</span><span class="sxs-lookup"><span data-stu-id="07f52-244">String</span></span>|<span data-ttu-id="07f52-245">表示可用于 Office365 应用程序套件的特定目标版本的更新版本的属性。</span><span class="sxs-lookup"><span data-stu-id="07f52-245">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="07f52-246">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="07f52-246">officeConfigurationXml</span></span>|<span data-ttu-id="07f52-247">Binary</span><span class="sxs-lookup"><span data-stu-id="07f52-247">Binary</span></span>|<span data-ttu-id="07f52-248">表示可为 Office 专业增强版应用程序指定的 XML 配置文件的属性。</span><span class="sxs-lookup"><span data-stu-id="07f52-248">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="07f52-249">优先于所有其他属性。</span><span class="sxs-lookup"><span data-stu-id="07f52-249">Takes precedence over all other properties.</span></span> <span data-ttu-id="07f52-250">如果存在，将使用 XML 配置文件来创建应用程序。</span><span class="sxs-lookup"><span data-stu-id="07f52-250">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="07f52-251">响应</span><span class="sxs-lookup"><span data-stu-id="07f52-251">Response</span></span>
<span data-ttu-id="07f52-252">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07f52-252">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07f52-253">示例</span><span class="sxs-lookup"><span data-stu-id="07f52-253">Example</span></span>

### <a name="request"></a><span data-ttu-id="07f52-254">请求</span><span class="sxs-lookup"><span data-stu-id="07f52-254">Request</span></span>
<span data-ttu-id="07f52-255">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="07f52-255">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1618

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
    "bing": true,
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

### <a name="response"></a><span data-ttu-id="07f52-256">响应</span><span class="sxs-lookup"><span data-stu-id="07f52-256">Response</span></span>
<span data-ttu-id="07f52-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="07f52-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1790

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
    "bing": true,
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



