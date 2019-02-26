---
title: 更新 windowsPhoneXAP
description: 更新 windowsPhoneXAP 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 096e7430d0f1e544b5fbd4a9475b70e45ecb0719
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150034"
---
# <a name="update-windowsphonexap"></a><span data-ttu-id="bb77c-103">更新 windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="bb77c-103">Update windowsPhoneXAP</span></span>

> <span data-ttu-id="bb77c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb77c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb77c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb77c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb77c-106">更新[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bb77c-106">Update the properties of a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb77c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bb77c-107">Prerequisites</span></span>
<span data-ttu-id="bb77c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bb77c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bb77c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb77c-110">Permission type</span></span>|<span data-ttu-id="bb77c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bb77c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb77c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb77c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bb77c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb77c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bb77c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb77c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb77c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb77c-115">Not supported.</span></span>|
|<span data-ttu-id="bb77c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb77c-116">Application</span></span>|<span data-ttu-id="bb77c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb77c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb77c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb77c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="bb77c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb77c-119">Request headers</span></span>
|<span data-ttu-id="bb77c-120">标头</span><span class="sxs-lookup"><span data-stu-id="bb77c-120">Header</span></span>|<span data-ttu-id="bb77c-121">值</span><span class="sxs-lookup"><span data-stu-id="bb77c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb77c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb77c-122">Authorization</span></span>|<span data-ttu-id="bb77c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bb77c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb77c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bb77c-124">Accept</span></span>|<span data-ttu-id="bb77c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bb77c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb77c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb77c-126">Request body</span></span>
<span data-ttu-id="bb77c-127">在请求正文中, 提供[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb77c-127">In the request body, supply a JSON representation for the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

<span data-ttu-id="bb77c-128">下表显示创建[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bb77c-128">The following table shows the properties that are required when you create the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span></span>

|<span data-ttu-id="bb77c-129">属性</span><span class="sxs-lookup"><span data-stu-id="bb77c-129">Property</span></span>|<span data-ttu-id="bb77c-130">类型</span><span class="sxs-lookup"><span data-stu-id="bb77c-130">Type</span></span>|<span data-ttu-id="bb77c-131">说明</span><span class="sxs-lookup"><span data-stu-id="bb77c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb77c-132">id</span><span class="sxs-lookup"><span data-stu-id="bb77c-132">id</span></span>|<span data-ttu-id="bb77c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="bb77c-133">String</span></span>|<span data-ttu-id="bb77c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bb77c-134">Key of the entity.</span></span> <span data-ttu-id="bb77c-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bb77c-136">displayName</span></span>|<span data-ttu-id="bb77c-137">String</span><span class="sxs-lookup"><span data-stu-id="bb77c-137">String</span></span>|<span data-ttu-id="bb77c-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="bb77c-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="bb77c-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-140">description</span><span class="sxs-lookup"><span data-stu-id="bb77c-140">description</span></span>|<span data-ttu-id="bb77c-141">字符串</span><span class="sxs-lookup"><span data-stu-id="bb77c-141">String</span></span>|<span data-ttu-id="bb77c-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="bb77c-142">The description of the app.</span></span> <span data-ttu-id="bb77c-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-144">publisher</span><span class="sxs-lookup"><span data-stu-id="bb77c-144">publisher</span></span>|<span data-ttu-id="bb77c-145">String</span><span class="sxs-lookup"><span data-stu-id="bb77c-145">String</span></span>|<span data-ttu-id="bb77c-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="bb77c-146">The publisher of the app.</span></span> <span data-ttu-id="bb77c-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="bb77c-148">largeIcon</span></span>|[<span data-ttu-id="bb77c-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bb77c-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bb77c-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="bb77c-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="bb77c-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb77c-152">createdDateTime</span></span>|<span data-ttu-id="bb77c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb77c-153">DateTimeOffset</span></span>|<span data-ttu-id="bb77c-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bb77c-154">The date and time the app was created.</span></span> <span data-ttu-id="bb77c-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb77c-156">lastModifiedDateTime</span></span>|<span data-ttu-id="bb77c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb77c-157">DateTimeOffset</span></span>|<span data-ttu-id="bb77c-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bb77c-158">The date and time the app was last modified.</span></span> <span data-ttu-id="bb77c-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="bb77c-160">isFeatured</span></span>|<span data-ttu-id="bb77c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb77c-161">Boolean</span></span>|<span data-ttu-id="bb77c-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bb77c-163">privacyInformationUrl</span></span>|<span data-ttu-id="bb77c-164">String</span><span class="sxs-lookup"><span data-stu-id="bb77c-164">String</span></span>|<span data-ttu-id="bb77c-165">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="bb77c-165">The privacy statement Url.</span></span> <span data-ttu-id="bb77c-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bb77c-167">informationUrl</span></span>|<span data-ttu-id="bb77c-168">String</span><span class="sxs-lookup"><span data-stu-id="bb77c-168">String</span></span>|<span data-ttu-id="bb77c-169">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="bb77c-169">The more information Url.</span></span> <span data-ttu-id="bb77c-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-171">owner</span><span class="sxs-lookup"><span data-stu-id="bb77c-171">owner</span></span>|<span data-ttu-id="bb77c-172">String</span><span class="sxs-lookup"><span data-stu-id="bb77c-172">String</span></span>|<span data-ttu-id="bb77c-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="bb77c-173">The owner of the app.</span></span> <span data-ttu-id="bb77c-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-175">developer</span><span class="sxs-lookup"><span data-stu-id="bb77c-175">developer</span></span>|<span data-ttu-id="bb77c-176">String</span><span class="sxs-lookup"><span data-stu-id="bb77c-176">String</span></span>|<span data-ttu-id="bb77c-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="bb77c-177">The developer of the app.</span></span> <span data-ttu-id="bb77c-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-179">notes</span><span class="sxs-lookup"><span data-stu-id="bb77c-179">notes</span></span>|<span data-ttu-id="bb77c-180">String</span><span class="sxs-lookup"><span data-stu-id="bb77c-180">String</span></span>|<span data-ttu-id="bb77c-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="bb77c-181">Notes for the app.</span></span> <span data-ttu-id="bb77c-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="bb77c-183">uploadState</span></span>|<span data-ttu-id="bb77c-184">Int32</span><span class="sxs-lookup"><span data-stu-id="bb77c-184">Int32</span></span>|<span data-ttu-id="bb77c-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="bb77c-185">The upload state.</span></span> <span data-ttu-id="bb77c-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="bb77c-187">publishingState</span></span>|[<span data-ttu-id="bb77c-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="bb77c-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="bb77c-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="bb77c-189">The publishing state for the app.</span></span> <span data-ttu-id="bb77c-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="bb77c-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="bb77c-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="bb77c-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="bb77c-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="bb77c-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="bb77c-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="bb77c-193">isAssigned</span></span>|<span data-ttu-id="bb77c-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb77c-194">Boolean</span></span>|<span data-ttu-id="bb77c-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="bb77c-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="bb77c-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bb77c-197">roleScopeTagIds</span></span>|<span data-ttu-id="bb77c-198">String collection</span><span class="sxs-lookup"><span data-stu-id="bb77c-198">String collection</span></span>|<span data-ttu-id="bb77c-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="bb77c-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="bb77c-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="bb77c-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="bb77c-201">committedContentVersion</span></span>|<span data-ttu-id="bb77c-202">String</span><span class="sxs-lookup"><span data-stu-id="bb77c-202">String</span></span>|<span data-ttu-id="bb77c-203">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="bb77c-203">The internal committed content version.</span></span> <span data-ttu-id="bb77c-204">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bb77c-205">fileName</span><span class="sxs-lookup"><span data-stu-id="bb77c-205">fileName</span></span>|<span data-ttu-id="bb77c-206">String</span><span class="sxs-lookup"><span data-stu-id="bb77c-206">String</span></span>|<span data-ttu-id="bb77c-207">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="bb77c-207">The name of the main Lob application file.</span></span> <span data-ttu-id="bb77c-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bb77c-209">size</span><span class="sxs-lookup"><span data-stu-id="bb77c-209">size</span></span>|<span data-ttu-id="bb77c-210">Int64</span><span class="sxs-lookup"><span data-stu-id="bb77c-210">Int64</span></span>|<span data-ttu-id="bb77c-211">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="bb77c-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="bb77c-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="bb77c-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="bb77c-213">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bb77c-213">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="bb77c-214">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="bb77c-214">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="bb77c-215">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="bb77c-215">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="bb77c-216">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="bb77c-216">productIdentifier</span></span>|<span data-ttu-id="bb77c-217">String</span><span class="sxs-lookup"><span data-stu-id="bb77c-217">String</span></span>|<span data-ttu-id="bb77c-218">产品标识符。</span><span class="sxs-lookup"><span data-stu-id="bb77c-218">The Product Identifier.</span></span>|
|<span data-ttu-id="bb77c-219">identityVersion</span><span class="sxs-lookup"><span data-stu-id="bb77c-219">identityVersion</span></span>|<span data-ttu-id="bb77c-220">String</span><span class="sxs-lookup"><span data-stu-id="bb77c-220">String</span></span>|<span data-ttu-id="bb77c-221">标识版本。</span><span class="sxs-lookup"><span data-stu-id="bb77c-221">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="bb77c-222">响应</span><span class="sxs-lookup"><span data-stu-id="bb77c-222">Response</span></span>
<span data-ttu-id="bb77c-223">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bb77c-223">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb77c-224">示例</span><span class="sxs-lookup"><span data-stu-id="bb77c-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb77c-225">请求</span><span class="sxs-lookup"><span data-stu-id="bb77c-225">Request</span></span>
<span data-ttu-id="bb77c-226">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb77c-226">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1164

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="bb77c-227">响应</span><span class="sxs-lookup"><span data-stu-id="bb77c-227">Response</span></span>
<span data-ttu-id="bb77c-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb77c-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1336

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```




