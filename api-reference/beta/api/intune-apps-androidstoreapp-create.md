---
title: 创建 androidStoreApp
description: 创建新的 androidStoreApp 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4e2fc78d02ac0afc367cd9d5d8b43331cd2744b9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34965212"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="7cfcb-103">创建 androidStoreApp</span><span class="sxs-lookup"><span data-stu-id="7cfcb-103">Create androidStoreApp</span></span>

> <span data-ttu-id="7cfcb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7cfcb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cfcb-106">创建新的 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-106">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7cfcb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7cfcb-107">Prerequisites</span></span>
<span data-ttu-id="7cfcb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cfcb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7cfcb-110">Permission type</span></span>|<span data-ttu-id="7cfcb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7cfcb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cfcb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7cfcb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7cfcb-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cfcb-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7cfcb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7cfcb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cfcb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-115">Not supported.</span></span>|
|<span data-ttu-id="7cfcb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7cfcb-116">Application</span></span>|<span data-ttu-id="7cfcb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cfcb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7cfcb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7cfcb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7cfcb-119">Request headers</span></span>
|<span data-ttu-id="7cfcb-120">标头</span><span class="sxs-lookup"><span data-stu-id="7cfcb-120">Header</span></span>|<span data-ttu-id="7cfcb-121">值</span><span class="sxs-lookup"><span data-stu-id="7cfcb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cfcb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cfcb-122">Authorization</span></span>|<span data-ttu-id="7cfcb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cfcb-124">接受</span><span class="sxs-lookup"><span data-stu-id="7cfcb-124">Accept</span></span>|<span data-ttu-id="7cfcb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7cfcb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cfcb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7cfcb-126">Request body</span></span>
<span data-ttu-id="7cfcb-127">在请求正文中，提供 androidStoreApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-127">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="7cfcb-128">下表显示创建 androidStoreApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-128">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="7cfcb-129">属性</span><span class="sxs-lookup"><span data-stu-id="7cfcb-129">Property</span></span>|<span data-ttu-id="7cfcb-130">类型</span><span class="sxs-lookup"><span data-stu-id="7cfcb-130">Type</span></span>|<span data-ttu-id="7cfcb-131">说明</span><span class="sxs-lookup"><span data-stu-id="7cfcb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cfcb-132">id</span><span class="sxs-lookup"><span data-stu-id="7cfcb-132">id</span></span>|<span data-ttu-id="7cfcb-133">字符串</span><span class="sxs-lookup"><span data-stu-id="7cfcb-133">String</span></span>|<span data-ttu-id="7cfcb-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-134">Key of the entity.</span></span> <span data-ttu-id="7cfcb-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="7cfcb-136">displayName</span></span>|<span data-ttu-id="7cfcb-137">String</span><span class="sxs-lookup"><span data-stu-id="7cfcb-137">String</span></span>|<span data-ttu-id="7cfcb-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7cfcb-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-140">说明</span><span class="sxs-lookup"><span data-stu-id="7cfcb-140">description</span></span>|<span data-ttu-id="7cfcb-141">字符串</span><span class="sxs-lookup"><span data-stu-id="7cfcb-141">String</span></span>|<span data-ttu-id="7cfcb-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-142">The description of the app.</span></span> <span data-ttu-id="7cfcb-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-144">publisher</span><span class="sxs-lookup"><span data-stu-id="7cfcb-144">publisher</span></span>|<span data-ttu-id="7cfcb-145">String</span><span class="sxs-lookup"><span data-stu-id="7cfcb-145">String</span></span>|<span data-ttu-id="7cfcb-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-146">The publisher of the app.</span></span> <span data-ttu-id="7cfcb-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7cfcb-148">largeIcon</span></span>|[<span data-ttu-id="7cfcb-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7cfcb-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7cfcb-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7cfcb-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7cfcb-152">createdDateTime</span></span>|<span data-ttu-id="7cfcb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cfcb-153">DateTimeOffset</span></span>|<span data-ttu-id="7cfcb-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-154">The date and time the app was created.</span></span> <span data-ttu-id="7cfcb-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7cfcb-156">lastModifiedDateTime</span></span>|<span data-ttu-id="7cfcb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7cfcb-157">DateTimeOffset</span></span>|<span data-ttu-id="7cfcb-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-158">The date and time the app was last modified.</span></span> <span data-ttu-id="7cfcb-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7cfcb-160">isFeatured</span></span>|<span data-ttu-id="7cfcb-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cfcb-161">Boolean</span></span>|<span data-ttu-id="7cfcb-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7cfcb-163">privacyInformationUrl</span></span>|<span data-ttu-id="7cfcb-164">String</span><span class="sxs-lookup"><span data-stu-id="7cfcb-164">String</span></span>|<span data-ttu-id="7cfcb-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-165">The privacy statement Url.</span></span> <span data-ttu-id="7cfcb-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7cfcb-167">informationUrl</span></span>|<span data-ttu-id="7cfcb-168">String</span><span class="sxs-lookup"><span data-stu-id="7cfcb-168">String</span></span>|<span data-ttu-id="7cfcb-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-169">The more information Url.</span></span> <span data-ttu-id="7cfcb-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-171">owner</span><span class="sxs-lookup"><span data-stu-id="7cfcb-171">owner</span></span>|<span data-ttu-id="7cfcb-172">String</span><span class="sxs-lookup"><span data-stu-id="7cfcb-172">String</span></span>|<span data-ttu-id="7cfcb-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-173">The owner of the app.</span></span> <span data-ttu-id="7cfcb-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-175">developer</span><span class="sxs-lookup"><span data-stu-id="7cfcb-175">developer</span></span>|<span data-ttu-id="7cfcb-176">String</span><span class="sxs-lookup"><span data-stu-id="7cfcb-176">String</span></span>|<span data-ttu-id="7cfcb-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-177">The developer of the app.</span></span> <span data-ttu-id="7cfcb-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-179">notes</span><span class="sxs-lookup"><span data-stu-id="7cfcb-179">notes</span></span>|<span data-ttu-id="7cfcb-180">String</span><span class="sxs-lookup"><span data-stu-id="7cfcb-180">String</span></span>|<span data-ttu-id="7cfcb-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-181">Notes for the app.</span></span> <span data-ttu-id="7cfcb-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="7cfcb-183">uploadState</span></span>|<span data-ttu-id="7cfcb-184">Int32</span><span class="sxs-lookup"><span data-stu-id="7cfcb-184">Int32</span></span>|<span data-ttu-id="7cfcb-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-185">The upload state.</span></span> <span data-ttu-id="7cfcb-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="7cfcb-187">publishingState</span></span>|[<span data-ttu-id="7cfcb-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7cfcb-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7cfcb-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-189">The publishing state for the app.</span></span> <span data-ttu-id="7cfcb-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7cfcb-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7cfcb-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7cfcb-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7cfcb-193">isAssigned</span></span>|<span data-ttu-id="7cfcb-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cfcb-194">Boolean</span></span>|<span data-ttu-id="7cfcb-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="7cfcb-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7cfcb-197">roleScopeTagIds</span></span>|<span data-ttu-id="7cfcb-198">String collection</span><span class="sxs-lookup"><span data-stu-id="7cfcb-198">String collection</span></span>|<span data-ttu-id="7cfcb-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="7cfcb-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="7cfcb-201">dependentAppCount</span></span>|<span data-ttu-id="7cfcb-202">Int32</span><span class="sxs-lookup"><span data-stu-id="7cfcb-202">Int32</span></span>|<span data-ttu-id="7cfcb-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="7cfcb-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7cfcb-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7cfcb-205">packageId</span><span class="sxs-lookup"><span data-stu-id="7cfcb-205">packageId</span></span>|<span data-ttu-id="7cfcb-206">String</span><span class="sxs-lookup"><span data-stu-id="7cfcb-206">String</span></span>|<span data-ttu-id="7cfcb-207">包标识符。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-207">The package identifier.</span></span>|
|<span data-ttu-id="7cfcb-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="7cfcb-208">appIdentifier</span></span>|<span data-ttu-id="7cfcb-209">String</span><span class="sxs-lookup"><span data-stu-id="7cfcb-209">String</span></span>|<span data-ttu-id="7cfcb-210">标识名称。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-210">The Identity Name.</span></span>|
|<span data-ttu-id="7cfcb-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7cfcb-211">appStoreUrl</span></span>|<span data-ttu-id="7cfcb-212">String</span><span class="sxs-lookup"><span data-stu-id="7cfcb-212">String</span></span>|<span data-ttu-id="7cfcb-213">Android 应用商店 URL。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-213">The Android app store URL.</span></span>|
|<span data-ttu-id="7cfcb-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7cfcb-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7cfcb-215">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7cfcb-215">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="7cfcb-216">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-216">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="7cfcb-217">响应</span><span class="sxs-lookup"><span data-stu-id="7cfcb-217">Response</span></span>
<span data-ttu-id="7cfcb-218">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [androidStoreApp](../resources/intune-apps-androidstoreapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-218">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cfcb-219">示例</span><span class="sxs-lookup"><span data-stu-id="7cfcb-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cfcb-220">请求</span><span class="sxs-lookup"><span data-stu-id="7cfcb-220">Request</span></span>
<span data-ttu-id="7cfcb-221">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1230

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="7cfcb-222">响应</span><span class="sxs-lookup"><span data-stu-id="7cfcb-222">Response</span></span>
<span data-ttu-id="7cfcb-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7cfcb-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1402

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```





