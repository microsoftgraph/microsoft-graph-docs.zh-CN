---
title: 创建 officeSuiteApp
description: 创建新的 officeSuiteApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ba737eb1348010951484e077f85d99842aaceed
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139457"
---
# <a name="create-officesuiteapp"></a><span data-ttu-id="bca69-103">创建 officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="bca69-103">Create officeSuiteApp</span></span>

<span data-ttu-id="bca69-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bca69-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bca69-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bca69-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bca69-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bca69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bca69-107">创建新的 [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bca69-107">Create a new [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bca69-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bca69-108">Prerequisites</span></span>
<span data-ttu-id="bca69-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bca69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bca69-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bca69-111">Permission type</span></span>|<span data-ttu-id="bca69-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bca69-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bca69-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bca69-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bca69-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bca69-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bca69-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bca69-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bca69-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bca69-116">Not supported.</span></span>|
|<span data-ttu-id="bca69-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bca69-117">Application</span></span>|<span data-ttu-id="bca69-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bca69-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bca69-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bca69-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bca69-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bca69-120">Request headers</span></span>
|<span data-ttu-id="bca69-121">标头</span><span class="sxs-lookup"><span data-stu-id="bca69-121">Header</span></span>|<span data-ttu-id="bca69-122">值</span><span class="sxs-lookup"><span data-stu-id="bca69-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bca69-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bca69-123">Authorization</span></span>|<span data-ttu-id="bca69-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bca69-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bca69-125">接受</span><span class="sxs-lookup"><span data-stu-id="bca69-125">Accept</span></span>|<span data-ttu-id="bca69-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bca69-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bca69-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bca69-127">Request body</span></span>
<span data-ttu-id="bca69-128">在请求正文中，提供 officeSuiteApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bca69-128">In the request body, supply a JSON representation for the officeSuiteApp object.</span></span>

<span data-ttu-id="bca69-129">下表显示创建 officeSuiteApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bca69-129">The following table shows the properties that are required when you create the officeSuiteApp.</span></span>

|<span data-ttu-id="bca69-130">属性</span><span class="sxs-lookup"><span data-stu-id="bca69-130">Property</span></span>|<span data-ttu-id="bca69-131">类型</span><span class="sxs-lookup"><span data-stu-id="bca69-131">Type</span></span>|<span data-ttu-id="bca69-132">说明</span><span class="sxs-lookup"><span data-stu-id="bca69-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bca69-133">id</span><span class="sxs-lookup"><span data-stu-id="bca69-133">id</span></span>|<span data-ttu-id="bca69-134">String</span><span class="sxs-lookup"><span data-stu-id="bca69-134">String</span></span>|<span data-ttu-id="bca69-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bca69-135">Key of the entity.</span></span> <span data-ttu-id="bca69-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-137">displayName</span><span class="sxs-lookup"><span data-stu-id="bca69-137">displayName</span></span>|<span data-ttu-id="bca69-138">String</span><span class="sxs-lookup"><span data-stu-id="bca69-138">String</span></span>|<span data-ttu-id="bca69-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="bca69-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bca69-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-141">说明</span><span class="sxs-lookup"><span data-stu-id="bca69-141">description</span></span>|<span data-ttu-id="bca69-142">String</span><span class="sxs-lookup"><span data-stu-id="bca69-142">String</span></span>|<span data-ttu-id="bca69-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="bca69-143">The description of the app.</span></span> <span data-ttu-id="bca69-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-145">publisher</span><span class="sxs-lookup"><span data-stu-id="bca69-145">publisher</span></span>|<span data-ttu-id="bca69-146">String</span><span class="sxs-lookup"><span data-stu-id="bca69-146">String</span></span>|<span data-ttu-id="bca69-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="bca69-147">The publisher of the app.</span></span> <span data-ttu-id="bca69-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bca69-149">largeIcon</span></span>|[<span data-ttu-id="bca69-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bca69-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bca69-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="bca69-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bca69-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bca69-153">createdDateTime</span></span>|<span data-ttu-id="bca69-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bca69-154">DateTimeOffset</span></span>|<span data-ttu-id="bca69-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bca69-155">The date and time the app was created.</span></span> <span data-ttu-id="bca69-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bca69-157">lastModifiedDateTime</span></span>|<span data-ttu-id="bca69-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bca69-158">DateTimeOffset</span></span>|<span data-ttu-id="bca69-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bca69-159">The date and time the app was last modified.</span></span> <span data-ttu-id="bca69-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bca69-161">isFeatured</span></span>|<span data-ttu-id="bca69-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="bca69-162">Boolean</span></span>|<span data-ttu-id="bca69-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bca69-164">privacyInformationUrl</span></span>|<span data-ttu-id="bca69-165">String</span><span class="sxs-lookup"><span data-stu-id="bca69-165">String</span></span>|<span data-ttu-id="bca69-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="bca69-166">The privacy statement Url.</span></span> <span data-ttu-id="bca69-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bca69-168">informationUrl</span></span>|<span data-ttu-id="bca69-169">String</span><span class="sxs-lookup"><span data-stu-id="bca69-169">String</span></span>|<span data-ttu-id="bca69-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="bca69-170">The more information Url.</span></span> <span data-ttu-id="bca69-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-172">owner</span><span class="sxs-lookup"><span data-stu-id="bca69-172">owner</span></span>|<span data-ttu-id="bca69-173">String</span><span class="sxs-lookup"><span data-stu-id="bca69-173">String</span></span>|<span data-ttu-id="bca69-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="bca69-174">The owner of the app.</span></span> <span data-ttu-id="bca69-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-176">developer</span><span class="sxs-lookup"><span data-stu-id="bca69-176">developer</span></span>|<span data-ttu-id="bca69-177">String</span><span class="sxs-lookup"><span data-stu-id="bca69-177">String</span></span>|<span data-ttu-id="bca69-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="bca69-178">The developer of the app.</span></span> <span data-ttu-id="bca69-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-180">notes</span><span class="sxs-lookup"><span data-stu-id="bca69-180">notes</span></span>|<span data-ttu-id="bca69-181">String</span><span class="sxs-lookup"><span data-stu-id="bca69-181">String</span></span>|<span data-ttu-id="bca69-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="bca69-182">Notes for the app.</span></span> <span data-ttu-id="bca69-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="bca69-184">uploadState</span></span>|<span data-ttu-id="bca69-185">Int32</span><span class="sxs-lookup"><span data-stu-id="bca69-185">Int32</span></span>|<span data-ttu-id="bca69-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="bca69-186">The upload state.</span></span> <span data-ttu-id="bca69-187">可能的值是：0 - `Not Ready` 、1 - `Ready` 、2 - `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="bca69-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="bca69-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="bca69-189">publishingState</span></span>|[<span data-ttu-id="bca69-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bca69-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bca69-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="bca69-191">The publishing state for the app.</span></span> <span data-ttu-id="bca69-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="bca69-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bca69-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="bca69-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="bca69-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="bca69-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bca69-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bca69-195">isAssigned</span></span>|<span data-ttu-id="bca69-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="bca69-196">Boolean</span></span>|<span data-ttu-id="bca69-197">指示是否将应用分配给至少一个组的值。</span><span class="sxs-lookup"><span data-stu-id="bca69-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="bca69-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bca69-199">roleScopeTagIds</span></span>|<span data-ttu-id="bca69-200">String collection</span><span class="sxs-lookup"><span data-stu-id="bca69-200">String collection</span></span>|<span data-ttu-id="bca69-201">此移动应用的范围标记 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="bca69-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="bca69-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="bca69-203">dependentAppCount</span></span>|<span data-ttu-id="bca69-204">Int32</span><span class="sxs-lookup"><span data-stu-id="bca69-204">Int32</span></span>|<span data-ttu-id="bca69-205">子应用具有的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="bca69-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="bca69-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="bca69-207">supersedingAppCount</span></span>|<span data-ttu-id="bca69-208">Int32</span><span class="sxs-lookup"><span data-stu-id="bca69-208">Int32</span></span>|<span data-ttu-id="bca69-209">此应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="bca69-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="bca69-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="bca69-211">supersededAppCount</span></span>|<span data-ttu-id="bca69-212">Int32</span><span class="sxs-lookup"><span data-stu-id="bca69-212">Int32</span></span>|<span data-ttu-id="bca69-213">此应用直接或间接被取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="bca69-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="bca69-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bca69-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="bca69-215">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="bca69-215">autoAcceptEula</span></span>|<span data-ttu-id="bca69-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="bca69-216">Boolean</span></span>|<span data-ttu-id="bca69-217">在最终用户的设备上自动接受 EULA 的值。</span><span class="sxs-lookup"><span data-stu-id="bca69-217">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="bca69-218">productIds</span><span class="sxs-lookup"><span data-stu-id="bca69-218">productIds</span></span>|<span data-ttu-id="bca69-219">[officeProductId](../resources/intune-apps-officeproductid.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bca69-219">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="bca69-220">表示 Office365 套件 SKU 的产品 ID。</span><span class="sxs-lookup"><span data-stu-id="bca69-220">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="bca69-221">可取值为：`o365ProPlusRetail`、`o365BusinessRetail`、`visioProRetail`、`projectProRetail`。</span><span class="sxs-lookup"><span data-stu-id="bca69-221">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="bca69-222">excludedApps</span><span class="sxs-lookup"><span data-stu-id="bca69-222">excludedApps</span></span>|[<span data-ttu-id="bca69-223">excludedApps</span><span class="sxs-lookup"><span data-stu-id="bca69-223">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="bca69-224">表示从所选 Office365 产品 ID 中排除的应用的属性。</span><span class="sxs-lookup"><span data-stu-id="bca69-224">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="bca69-225">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="bca69-225">useSharedComputerActivation</span></span>|<span data-ttu-id="bca69-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="bca69-226">Boolean</span></span>|<span data-ttu-id="bca69-227">表示共享计算机激活是否不用于 Office365 应用套件的属性。</span><span class="sxs-lookup"><span data-stu-id="bca69-227">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="bca69-228">updateChannel</span><span class="sxs-lookup"><span data-stu-id="bca69-228">updateChannel</span></span>|[<span data-ttu-id="bca69-229">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="bca69-229">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="bca69-230">表示 Office365 更新频道的属性。</span><span class="sxs-lookup"><span data-stu-id="bca69-230">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="bca69-231">可取值为：`none`、`current`、`deferred`、`firstReleaseCurrent`、`firstReleaseDeferred`、`monthlyEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="bca69-231">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`, `monthlyEnterprise`.</span></span>|
|<span data-ttu-id="bca69-232">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="bca69-232">officePlatformArchitecture</span></span>|[<span data-ttu-id="bca69-233">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="bca69-233">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="bca69-234">表示 Office365 应用套件版本的 属性。</span><span class="sxs-lookup"><span data-stu-id="bca69-234">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="bca69-235">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="bca69-235">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="bca69-236">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="bca69-236">localesToInstall</span></span>|<span data-ttu-id="bca69-237">String collection</span><span class="sxs-lookup"><span data-stu-id="bca69-237">String collection</span></span>|<span data-ttu-id="bca69-238">表示安装 Office365 应用时安装区域设置的属性。</span><span class="sxs-lookup"><span data-stu-id="bca69-238">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="bca69-239">它使用标准 RFC 6033。</span><span class="sxs-lookup"><span data-stu-id="bca69-239">It uses standard RFC 6033.</span></span> <span data-ttu-id="bca69-240">参考： https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="bca69-240">Ref: https://technet.microsoft.com/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="bca69-241">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="bca69-241">installProgressDisplayLevel</span></span>|[<span data-ttu-id="bca69-242">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="bca69-242">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="bca69-243">指定设备上安装进度安装程序 UI 的显示级别。</span><span class="sxs-lookup"><span data-stu-id="bca69-243">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="bca69-244">可取值为：`none`、`full`。</span><span class="sxs-lookup"><span data-stu-id="bca69-244">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="bca69-245">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="bca69-245">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="bca69-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="bca69-246">Boolean</span></span>|<span data-ttu-id="bca69-247">确定是否将 Office365 应用套件部署到设备时卸载现有 Office MSI 的属性。</span><span class="sxs-lookup"><span data-stu-id="bca69-247">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="bca69-248">targetVersion</span><span class="sxs-lookup"><span data-stu-id="bca69-248">targetVersion</span></span>|<span data-ttu-id="bca69-249">String</span><span class="sxs-lookup"><span data-stu-id="bca69-249">String</span></span>|<span data-ttu-id="bca69-250">表示 Office365 应用套件的特定目标版本的 属性，该版本应一直部署在设备上。</span><span class="sxs-lookup"><span data-stu-id="bca69-250">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="bca69-251">updateVersion</span><span class="sxs-lookup"><span data-stu-id="bca69-251">updateVersion</span></span>|<span data-ttu-id="bca69-252">String</span><span class="sxs-lookup"><span data-stu-id="bca69-252">String</span></span>|<span data-ttu-id="bca69-253">表示特定目标版本可用于 Office365 应用套件的更新版本的 属性。</span><span class="sxs-lookup"><span data-stu-id="bca69-253">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="bca69-254">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="bca69-254">officeConfigurationXml</span></span>|<span data-ttu-id="bca69-255">Binary</span><span class="sxs-lookup"><span data-stu-id="bca69-255">Binary</span></span>|<span data-ttu-id="bca69-256">表示可指定 Office ProPlus Apps 的 XML 配置文件的属性。</span><span class="sxs-lookup"><span data-stu-id="bca69-256">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="bca69-257">优先于所有其他属性。</span><span class="sxs-lookup"><span data-stu-id="bca69-257">Takes precedence over all other properties.</span></span> <span data-ttu-id="bca69-258">存在此参数时，XML 配置文件将用于创建应用。</span><span class="sxs-lookup"><span data-stu-id="bca69-258">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="bca69-259">响应</span><span class="sxs-lookup"><span data-stu-id="bca69-259">Response</span></span>
<span data-ttu-id="bca69-260">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bca69-260">If successful, this method returns a `201 Created` response code and a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bca69-261">示例</span><span class="sxs-lookup"><span data-stu-id="bca69-261">Example</span></span>

### <a name="request"></a><span data-ttu-id="bca69-262">请求</span><span class="sxs-lookup"><span data-stu-id="bca69-262">Request</span></span>
<span data-ttu-id="bca69-263">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bca69-263">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1675

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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

### <a name="response"></a><span data-ttu-id="bca69-264">响应</span><span class="sxs-lookup"><span data-stu-id="bca69-264">Response</span></span>
<span data-ttu-id="bca69-p127">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bca69-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1847

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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
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




