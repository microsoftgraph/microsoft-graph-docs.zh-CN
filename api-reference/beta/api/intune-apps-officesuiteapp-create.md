---
title: 创建 officeSuiteApp
description: 创建新的 officeSuiteApp 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 664fc19eb20079c10352571e9d9d1cdb754bb7d8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960508"
---
# <a name="create-officesuiteapp"></a><span data-ttu-id="f741a-103">创建 officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="f741a-103">Create officeSuiteApp</span></span>

> <span data-ttu-id="f741a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f741a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f741a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f741a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f741a-106">创建新的[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f741a-106">Create a new [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f741a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f741a-107">Prerequisites</span></span>
<span data-ttu-id="f741a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f741a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f741a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f741a-110">Permission type</span></span>|<span data-ttu-id="f741a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f741a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f741a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f741a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f741a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f741a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f741a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f741a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f741a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f741a-115">Not supported.</span></span>|
|<span data-ttu-id="f741a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f741a-116">Application</span></span>|<span data-ttu-id="f741a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f741a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f741a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f741a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f741a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f741a-119">Request headers</span></span>
|<span data-ttu-id="f741a-120">标头</span><span class="sxs-lookup"><span data-stu-id="f741a-120">Header</span></span>|<span data-ttu-id="f741a-121">值</span><span class="sxs-lookup"><span data-stu-id="f741a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f741a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f741a-122">Authorization</span></span>|<span data-ttu-id="f741a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f741a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f741a-124">接受</span><span class="sxs-lookup"><span data-stu-id="f741a-124">Accept</span></span>|<span data-ttu-id="f741a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f741a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f741a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f741a-126">Request body</span></span>
<span data-ttu-id="f741a-127">在请求正文中, 提供 officeSuiteApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f741a-127">In the request body, supply a JSON representation for the officeSuiteApp object.</span></span>

<span data-ttu-id="f741a-128">下表显示创建 officeSuiteApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f741a-128">The following table shows the properties that are required when you create the officeSuiteApp.</span></span>

|<span data-ttu-id="f741a-129">属性</span><span class="sxs-lookup"><span data-stu-id="f741a-129">Property</span></span>|<span data-ttu-id="f741a-130">类型</span><span class="sxs-lookup"><span data-stu-id="f741a-130">Type</span></span>|<span data-ttu-id="f741a-131">说明</span><span class="sxs-lookup"><span data-stu-id="f741a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f741a-132">id</span><span class="sxs-lookup"><span data-stu-id="f741a-132">id</span></span>|<span data-ttu-id="f741a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f741a-133">String</span></span>|<span data-ttu-id="f741a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f741a-134">Key of the entity.</span></span> <span data-ttu-id="f741a-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f741a-136">displayName</span></span>|<span data-ttu-id="f741a-137">String</span><span class="sxs-lookup"><span data-stu-id="f741a-137">String</span></span>|<span data-ttu-id="f741a-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="f741a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f741a-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-140">说明</span><span class="sxs-lookup"><span data-stu-id="f741a-140">description</span></span>|<span data-ttu-id="f741a-141">字符串</span><span class="sxs-lookup"><span data-stu-id="f741a-141">String</span></span>|<span data-ttu-id="f741a-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="f741a-142">The description of the app.</span></span> <span data-ttu-id="f741a-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-144">publisher</span><span class="sxs-lookup"><span data-stu-id="f741a-144">publisher</span></span>|<span data-ttu-id="f741a-145">String</span><span class="sxs-lookup"><span data-stu-id="f741a-145">String</span></span>|<span data-ttu-id="f741a-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="f741a-146">The publisher of the app.</span></span> <span data-ttu-id="f741a-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f741a-148">largeIcon</span></span>|[<span data-ttu-id="f741a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f741a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f741a-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="f741a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f741a-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f741a-152">createdDateTime</span></span>|<span data-ttu-id="f741a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f741a-153">DateTimeOffset</span></span>|<span data-ttu-id="f741a-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f741a-154">The date and time the app was created.</span></span> <span data-ttu-id="f741a-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f741a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f741a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f741a-157">DateTimeOffset</span></span>|<span data-ttu-id="f741a-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f741a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f741a-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f741a-160">isFeatured</span></span>|<span data-ttu-id="f741a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f741a-161">Boolean</span></span>|<span data-ttu-id="f741a-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f741a-163">privacyInformationUrl</span></span>|<span data-ttu-id="f741a-164">String</span><span class="sxs-lookup"><span data-stu-id="f741a-164">String</span></span>|<span data-ttu-id="f741a-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="f741a-165">The privacy statement Url.</span></span> <span data-ttu-id="f741a-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f741a-167">informationUrl</span></span>|<span data-ttu-id="f741a-168">String</span><span class="sxs-lookup"><span data-stu-id="f741a-168">String</span></span>|<span data-ttu-id="f741a-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="f741a-169">The more information Url.</span></span> <span data-ttu-id="f741a-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-171">owner</span><span class="sxs-lookup"><span data-stu-id="f741a-171">owner</span></span>|<span data-ttu-id="f741a-172">String</span><span class="sxs-lookup"><span data-stu-id="f741a-172">String</span></span>|<span data-ttu-id="f741a-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="f741a-173">The owner of the app.</span></span> <span data-ttu-id="f741a-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-175">developer</span><span class="sxs-lookup"><span data-stu-id="f741a-175">developer</span></span>|<span data-ttu-id="f741a-176">String</span><span class="sxs-lookup"><span data-stu-id="f741a-176">String</span></span>|<span data-ttu-id="f741a-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="f741a-177">The developer of the app.</span></span> <span data-ttu-id="f741a-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-179">notes</span><span class="sxs-lookup"><span data-stu-id="f741a-179">notes</span></span>|<span data-ttu-id="f741a-180">String</span><span class="sxs-lookup"><span data-stu-id="f741a-180">String</span></span>|<span data-ttu-id="f741a-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="f741a-181">Notes for the app.</span></span> <span data-ttu-id="f741a-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="f741a-183">uploadState</span></span>|<span data-ttu-id="f741a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f741a-184">Int32</span></span>|<span data-ttu-id="f741a-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="f741a-185">The upload state.</span></span> <span data-ttu-id="f741a-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="f741a-187">publishingState</span></span>|[<span data-ttu-id="f741a-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f741a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f741a-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="f741a-189">The publishing state for the app.</span></span> <span data-ttu-id="f741a-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="f741a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f741a-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="f741a-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f741a-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="f741a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f741a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f741a-193">isAssigned</span></span>|<span data-ttu-id="f741a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f741a-194">Boolean</span></span>|<span data-ttu-id="f741a-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="f741a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f741a-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f741a-197">roleScopeTagIds</span></span>|<span data-ttu-id="f741a-198">String collection</span><span class="sxs-lookup"><span data-stu-id="f741a-198">String collection</span></span>|<span data-ttu-id="f741a-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="f741a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f741a-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="f741a-201">dependentAppCount</span></span>|<span data-ttu-id="f741a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="f741a-202">Int32</span></span>|<span data-ttu-id="f741a-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="f741a-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f741a-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f741a-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f741a-205">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="f741a-205">autoAcceptEula</span></span>|<span data-ttu-id="f741a-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="f741a-206">Boolean</span></span>|<span data-ttu-id="f741a-207">要在 enduser 的设备上自动接受 EULA 的值。</span><span class="sxs-lookup"><span data-stu-id="f741a-207">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="f741a-208">productIds</span><span class="sxs-lookup"><span data-stu-id="f741a-208">productIds</span></span>|<span data-ttu-id="f741a-209">[officeProductId](../resources/intune-apps-officeproductid.md)集合</span><span class="sxs-lookup"><span data-stu-id="f741a-209">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="f741a-210">表示 Office365 套件 SKU 的产品 Id。</span><span class="sxs-lookup"><span data-stu-id="f741a-210">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="f741a-211">可取值为：`o365ProPlusRetail`、`o365BusinessRetail`、`visioProRetail`、`projectProRetail`。</span><span class="sxs-lookup"><span data-stu-id="f741a-211">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="f741a-212">excludedApps</span><span class="sxs-lookup"><span data-stu-id="f741a-212">excludedApps</span></span>|[<span data-ttu-id="f741a-213">excludedApps</span><span class="sxs-lookup"><span data-stu-id="f741a-213">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="f741a-214">表示从所选 Office365 产品 Id 中排除的应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="f741a-214">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="f741a-215">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="f741a-215">useSharedComputerActivation</span></span>|<span data-ttu-id="f741a-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="f741a-216">Boolean</span></span>|<span data-ttu-id="f741a-217">表示共享计算机激活是否不适用于 Office365 应用程序套件的属性。</span><span class="sxs-lookup"><span data-stu-id="f741a-217">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="f741a-218">updateChannel</span><span class="sxs-lookup"><span data-stu-id="f741a-218">updateChannel</span></span>|[<span data-ttu-id="f741a-219">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="f741a-219">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="f741a-220">用于表示 Office365 更新通道的属性。</span><span class="sxs-lookup"><span data-stu-id="f741a-220">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="f741a-221">可取值为：`none`、`current`、`deferred`、`firstReleaseCurrent`、`firstReleaseDeferred`。</span><span class="sxs-lookup"><span data-stu-id="f741a-221">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="f741a-222">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="f741a-222">officePlatformArchitecture</span></span>|[<span data-ttu-id="f741a-223">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="f741a-223">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="f741a-224">表示 Office365 应用程序套件版本的属性。</span><span class="sxs-lookup"><span data-stu-id="f741a-224">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="f741a-225">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="f741a-225">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="f741a-226">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="f741a-226">localesToInstall</span></span>|<span data-ttu-id="f741a-227">String collection</span><span class="sxs-lookup"><span data-stu-id="f741a-227">String collection</span></span>|<span data-ttu-id="f741a-228">用于表示安装 Office365 中的应用程序时所安装的区域设置的属性。</span><span class="sxs-lookup"><span data-stu-id="f741a-228">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="f741a-229">它使用标准 RFC 6033。</span><span class="sxs-lookup"><span data-stu-id="f741a-229">It uses standard RFC 6033.</span></span> <span data-ttu-id="f741a-230">Refhttps://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="f741a-230">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="f741a-231">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="f741a-231">installProgressDisplayLevel</span></span>|[<span data-ttu-id="f741a-232">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="f741a-232">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="f741a-233">指定设备上安装进度设置 UI 的显示级别。</span><span class="sxs-lookup"><span data-stu-id="f741a-233">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="f741a-234">可取值为：`none`、`full`。</span><span class="sxs-lookup"><span data-stu-id="f741a-234">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="f741a-235">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="f741a-235">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="f741a-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="f741a-236">Boolean</span></span>|<span data-ttu-id="f741a-237">用于确定是否在将 Office365 应用套件部署到设备时是否卸载现有 Office MSI 的属性。</span><span class="sxs-lookup"><span data-stu-id="f741a-237">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="f741a-238">targetVersion</span><span class="sxs-lookup"><span data-stu-id="f741a-238">targetVersion</span></span>|<span data-ttu-id="f741a-239">String</span><span class="sxs-lookup"><span data-stu-id="f741a-239">String</span></span>|<span data-ttu-id="f741a-240">表示应在设备上保持部署的 Office365 应用程序套件的特定目标版本的属性。</span><span class="sxs-lookup"><span data-stu-id="f741a-240">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="f741a-241">updateVersion</span><span class="sxs-lookup"><span data-stu-id="f741a-241">updateVersion</span></span>|<span data-ttu-id="f741a-242">String</span><span class="sxs-lookup"><span data-stu-id="f741a-242">String</span></span>|<span data-ttu-id="f741a-243">表示可用于 Office365 应用程序套件的特定目标版本的更新版本的属性。</span><span class="sxs-lookup"><span data-stu-id="f741a-243">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="f741a-244">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="f741a-244">officeConfigurationXml</span></span>|<span data-ttu-id="f741a-245">Binary</span><span class="sxs-lookup"><span data-stu-id="f741a-245">Binary</span></span>|<span data-ttu-id="f741a-246">表示可为 Office 专业增强版应用程序指定的 XML 配置文件的属性。</span><span class="sxs-lookup"><span data-stu-id="f741a-246">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="f741a-247">优先于所有其他属性。</span><span class="sxs-lookup"><span data-stu-id="f741a-247">Takes precedence over all other properties.</span></span> <span data-ttu-id="f741a-248">如果存在, 将使用 XML 配置文件来创建应用程序。</span><span class="sxs-lookup"><span data-stu-id="f741a-248">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="f741a-249">响应</span><span class="sxs-lookup"><span data-stu-id="f741a-249">Response</span></span>
<span data-ttu-id="f741a-250">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f741a-250">If successful, this method returns a `201 Created` response code and a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f741a-251">示例</span><span class="sxs-lookup"><span data-stu-id="f741a-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="f741a-252">请求</span><span class="sxs-lookup"><span data-stu-id="f741a-252">Request</span></span>
<span data-ttu-id="f741a-253">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f741a-253">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="f741a-254">响应</span><span class="sxs-lookup"><span data-stu-id="f741a-254">Response</span></span>
<span data-ttu-id="f741a-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f741a-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





