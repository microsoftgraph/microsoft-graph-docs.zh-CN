---
title: 创建 androidForWorkApp
description: 创建新的 androidForWorkApp 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 77b3dbffec6e870d9ebd3ed786d93460df55954d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324894"
---
# <a name="create-androidforworkapp"></a><span data-ttu-id="80dbc-103">创建 androidForWorkApp</span><span class="sxs-lookup"><span data-stu-id="80dbc-103">Create androidForWorkApp</span></span>

> <span data-ttu-id="80dbc-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="80dbc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80dbc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="80dbc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80dbc-106">创建新的[androidForWorkApp](../resources/intune-apps-androidforworkapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="80dbc-106">Create a new [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80dbc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="80dbc-107">Prerequisites</span></span>
<span data-ttu-id="80dbc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80dbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80dbc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="80dbc-110">Permission type</span></span>|<span data-ttu-id="80dbc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="80dbc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80dbc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80dbc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80dbc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80dbc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="80dbc-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80dbc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80dbc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="80dbc-115">Not supported.</span></span>|
|<span data-ttu-id="80dbc-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="80dbc-116">Application</span></span>|<span data-ttu-id="80dbc-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80dbc-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80dbc-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80dbc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="80dbc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="80dbc-119">Request headers</span></span>
|<span data-ttu-id="80dbc-120">标头</span><span class="sxs-lookup"><span data-stu-id="80dbc-120">Header</span></span>|<span data-ttu-id="80dbc-121">值</span><span class="sxs-lookup"><span data-stu-id="80dbc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80dbc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="80dbc-122">Authorization</span></span>|<span data-ttu-id="80dbc-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="80dbc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80dbc-124">接受</span><span class="sxs-lookup"><span data-stu-id="80dbc-124">Accept</span></span>|<span data-ttu-id="80dbc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80dbc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80dbc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="80dbc-126">Request body</span></span>
<span data-ttu-id="80dbc-127">在请求正文中, 提供 androidForWorkApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80dbc-127">In the request body, supply a JSON representation for the androidForWorkApp object.</span></span>

<span data-ttu-id="80dbc-128">下表显示创建 androidForWorkApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="80dbc-128">The following table shows the properties that are required when you create the androidForWorkApp.</span></span>

|<span data-ttu-id="80dbc-129">属性</span><span class="sxs-lookup"><span data-stu-id="80dbc-129">Property</span></span>|<span data-ttu-id="80dbc-130">类型</span><span class="sxs-lookup"><span data-stu-id="80dbc-130">Type</span></span>|<span data-ttu-id="80dbc-131">说明</span><span class="sxs-lookup"><span data-stu-id="80dbc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80dbc-132">id</span><span class="sxs-lookup"><span data-stu-id="80dbc-132">id</span></span>|<span data-ttu-id="80dbc-133">字符串</span><span class="sxs-lookup"><span data-stu-id="80dbc-133">String</span></span>|<span data-ttu-id="80dbc-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="80dbc-134">Key of the entity.</span></span> <span data-ttu-id="80dbc-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="80dbc-136">displayName</span></span>|<span data-ttu-id="80dbc-137">String</span><span class="sxs-lookup"><span data-stu-id="80dbc-137">String</span></span>|<span data-ttu-id="80dbc-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="80dbc-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="80dbc-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-140">说明</span><span class="sxs-lookup"><span data-stu-id="80dbc-140">description</span></span>|<span data-ttu-id="80dbc-141">字符串</span><span class="sxs-lookup"><span data-stu-id="80dbc-141">String</span></span>|<span data-ttu-id="80dbc-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="80dbc-142">The description of the app.</span></span> <span data-ttu-id="80dbc-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-144">publisher</span><span class="sxs-lookup"><span data-stu-id="80dbc-144">publisher</span></span>|<span data-ttu-id="80dbc-145">String</span><span class="sxs-lookup"><span data-stu-id="80dbc-145">String</span></span>|<span data-ttu-id="80dbc-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="80dbc-146">The publisher of the app.</span></span> <span data-ttu-id="80dbc-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="80dbc-148">largeIcon</span></span>|[<span data-ttu-id="80dbc-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="80dbc-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="80dbc-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="80dbc-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="80dbc-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80dbc-152">createdDateTime</span></span>|<span data-ttu-id="80dbc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80dbc-153">DateTimeOffset</span></span>|<span data-ttu-id="80dbc-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="80dbc-154">The date and time the app was created.</span></span> <span data-ttu-id="80dbc-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80dbc-156">lastModifiedDateTime</span></span>|<span data-ttu-id="80dbc-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80dbc-157">DateTimeOffset</span></span>|<span data-ttu-id="80dbc-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="80dbc-158">The date and time the app was last modified.</span></span> <span data-ttu-id="80dbc-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="80dbc-160">isFeatured</span></span>|<span data-ttu-id="80dbc-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="80dbc-161">Boolean</span></span>|<span data-ttu-id="80dbc-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="80dbc-163">privacyInformationUrl</span></span>|<span data-ttu-id="80dbc-164">String</span><span class="sxs-lookup"><span data-stu-id="80dbc-164">String</span></span>|<span data-ttu-id="80dbc-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="80dbc-165">The privacy statement Url.</span></span> <span data-ttu-id="80dbc-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="80dbc-167">informationUrl</span></span>|<span data-ttu-id="80dbc-168">String</span><span class="sxs-lookup"><span data-stu-id="80dbc-168">String</span></span>|<span data-ttu-id="80dbc-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="80dbc-169">The more information Url.</span></span> <span data-ttu-id="80dbc-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-171">owner</span><span class="sxs-lookup"><span data-stu-id="80dbc-171">owner</span></span>|<span data-ttu-id="80dbc-172">String</span><span class="sxs-lookup"><span data-stu-id="80dbc-172">String</span></span>|<span data-ttu-id="80dbc-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="80dbc-173">The owner of the app.</span></span> <span data-ttu-id="80dbc-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-175">developer</span><span class="sxs-lookup"><span data-stu-id="80dbc-175">developer</span></span>|<span data-ttu-id="80dbc-176">String</span><span class="sxs-lookup"><span data-stu-id="80dbc-176">String</span></span>|<span data-ttu-id="80dbc-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="80dbc-177">The developer of the app.</span></span> <span data-ttu-id="80dbc-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-179">notes</span><span class="sxs-lookup"><span data-stu-id="80dbc-179">notes</span></span>|<span data-ttu-id="80dbc-180">String</span><span class="sxs-lookup"><span data-stu-id="80dbc-180">String</span></span>|<span data-ttu-id="80dbc-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="80dbc-181">Notes for the app.</span></span> <span data-ttu-id="80dbc-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="80dbc-183">uploadState</span></span>|<span data-ttu-id="80dbc-184">Int32</span><span class="sxs-lookup"><span data-stu-id="80dbc-184">Int32</span></span>|<span data-ttu-id="80dbc-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="80dbc-185">The upload state.</span></span> <span data-ttu-id="80dbc-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="80dbc-187">publishingState</span></span>|[<span data-ttu-id="80dbc-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="80dbc-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="80dbc-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="80dbc-189">The publishing state for the app.</span></span> <span data-ttu-id="80dbc-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="80dbc-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="80dbc-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="80dbc-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="80dbc-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="80dbc-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="80dbc-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="80dbc-193">isAssigned</span></span>|<span data-ttu-id="80dbc-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="80dbc-194">Boolean</span></span>|<span data-ttu-id="80dbc-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="80dbc-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="80dbc-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="80dbc-197">roleScopeTagIds</span></span>|<span data-ttu-id="80dbc-198">String collection</span><span class="sxs-lookup"><span data-stu-id="80dbc-198">String collection</span></span>|<span data-ttu-id="80dbc-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="80dbc-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="80dbc-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="80dbc-201">dependentAppCount</span></span>|<span data-ttu-id="80dbc-202">Int32</span><span class="sxs-lookup"><span data-stu-id="80dbc-202">Int32</span></span>|<span data-ttu-id="80dbc-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="80dbc-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="80dbc-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="80dbc-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80dbc-205">packageId</span><span class="sxs-lookup"><span data-stu-id="80dbc-205">packageId</span></span>|<span data-ttu-id="80dbc-206">String</span><span class="sxs-lookup"><span data-stu-id="80dbc-206">String</span></span>|<span data-ttu-id="80dbc-207">包标识符。</span><span class="sxs-lookup"><span data-stu-id="80dbc-207">The package identifier.</span></span>|
|<span data-ttu-id="80dbc-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="80dbc-208">appIdentifier</span></span>|<span data-ttu-id="80dbc-209">String</span><span class="sxs-lookup"><span data-stu-id="80dbc-209">String</span></span>|<span data-ttu-id="80dbc-210">标识名称。</span><span class="sxs-lookup"><span data-stu-id="80dbc-210">The Identity Name.</span></span>|
|<span data-ttu-id="80dbc-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="80dbc-211">usedLicenseCount</span></span>|<span data-ttu-id="80dbc-212">Int32</span><span class="sxs-lookup"><span data-stu-id="80dbc-212">Int32</span></span>|<span data-ttu-id="80dbc-213">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="80dbc-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="80dbc-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="80dbc-214">totalLicenseCount</span></span>|<span data-ttu-id="80dbc-215">Int32</span><span class="sxs-lookup"><span data-stu-id="80dbc-215">Int32</span></span>|<span data-ttu-id="80dbc-216">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="80dbc-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="80dbc-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="80dbc-217">appStoreUrl</span></span>|<span data-ttu-id="80dbc-218">String</span><span class="sxs-lookup"><span data-stu-id="80dbc-218">String</span></span>|<span data-ttu-id="80dbc-219">"播放工作商店" 应用程序 URL。</span><span class="sxs-lookup"><span data-stu-id="80dbc-219">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="80dbc-220">响应</span><span class="sxs-lookup"><span data-stu-id="80dbc-220">Response</span></span>
<span data-ttu-id="80dbc-221">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidForWorkApp](../resources/intune-apps-androidforworkapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="80dbc-221">If successful, this method returns a `201 Created` response code and a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80dbc-222">示例</span><span class="sxs-lookup"><span data-stu-id="80dbc-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="80dbc-223">请求</span><span class="sxs-lookup"><span data-stu-id="80dbc-223">Request</span></span>
<span data-ttu-id="80dbc-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80dbc-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 903

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="80dbc-225">响应</span><span class="sxs-lookup"><span data-stu-id="80dbc-225">Response</span></span>
<span data-ttu-id="80dbc-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80dbc-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1075

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```






