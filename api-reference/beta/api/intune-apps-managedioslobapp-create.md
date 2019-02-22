---
title: 创建 managedIOSLobApp
description: 创建新的 managedIOSLobApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9178692b0918a099fbb5aae9271ddc244c1a60ab
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147297"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="da157-103">创建 managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="da157-103">Create managedIOSLobApp</span></span>

> <span data-ttu-id="da157-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da157-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da157-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da157-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da157-106">创建新的 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da157-106">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da157-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="da157-107">Prerequisites</span></span>
<span data-ttu-id="da157-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="da157-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="da157-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="da157-110">Permission type</span></span>|<span data-ttu-id="da157-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="da157-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da157-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da157-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da157-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da157-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="da157-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da157-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da157-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="da157-115">Not supported.</span></span>|
|<span data-ttu-id="da157-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="da157-116">Application</span></span>|<span data-ttu-id="da157-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="da157-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da157-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da157-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="da157-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="da157-119">Request headers</span></span>
|<span data-ttu-id="da157-120">标头</span><span class="sxs-lookup"><span data-stu-id="da157-120">Header</span></span>|<span data-ttu-id="da157-121">值</span><span class="sxs-lookup"><span data-stu-id="da157-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da157-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="da157-122">Authorization</span></span>|<span data-ttu-id="da157-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da157-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da157-124">Accept</span><span class="sxs-lookup"><span data-stu-id="da157-124">Accept</span></span>|<span data-ttu-id="da157-125">application/json</span><span class="sxs-lookup"><span data-stu-id="da157-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da157-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="da157-126">Request body</span></span>
<span data-ttu-id="da157-127">在请求正文中，提供 managedIOSLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da157-127">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="da157-128">下表显示创建 managedIOSLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="da157-128">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="da157-129">属性</span><span class="sxs-lookup"><span data-stu-id="da157-129">Property</span></span>|<span data-ttu-id="da157-130">类型</span><span class="sxs-lookup"><span data-stu-id="da157-130">Type</span></span>|<span data-ttu-id="da157-131">说明</span><span class="sxs-lookup"><span data-stu-id="da157-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da157-132">id</span><span class="sxs-lookup"><span data-stu-id="da157-132">id</span></span>|<span data-ttu-id="da157-133">字串符号</span><span class="sxs-lookup"><span data-stu-id="da157-133">String</span></span>|<span data-ttu-id="da157-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="da157-134">Key of the entity.</span></span> <span data-ttu-id="da157-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-136">displayName</span><span class="sxs-lookup"><span data-stu-id="da157-136">displayName</span></span>|<span data-ttu-id="da157-137">字符串</span><span class="sxs-lookup"><span data-stu-id="da157-137">String</span></span>|<span data-ttu-id="da157-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="da157-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="da157-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-140">description</span><span class="sxs-lookup"><span data-stu-id="da157-140">description</span></span>|<span data-ttu-id="da157-141">字符串</span><span class="sxs-lookup"><span data-stu-id="da157-141">String</span></span>|<span data-ttu-id="da157-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="da157-142">The description of the app.</span></span> <span data-ttu-id="da157-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-144">publisher</span><span class="sxs-lookup"><span data-stu-id="da157-144">publisher</span></span>|<span data-ttu-id="da157-145">字符串</span><span class="sxs-lookup"><span data-stu-id="da157-145">String</span></span>|<span data-ttu-id="da157-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="da157-146">The publisher of the app.</span></span> <span data-ttu-id="da157-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="da157-148">largeIcon</span></span>|[<span data-ttu-id="da157-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="da157-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="da157-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="da157-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="da157-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da157-152">createdDateTime</span></span>|<span data-ttu-id="da157-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da157-153">DateTimeOffset</span></span>|<span data-ttu-id="da157-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="da157-154">The date and time the app was created.</span></span> <span data-ttu-id="da157-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da157-156">lastModifiedDateTime</span></span>|<span data-ttu-id="da157-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da157-157">DateTimeOffset</span></span>|<span data-ttu-id="da157-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="da157-158">The date and time the app was last modified.</span></span> <span data-ttu-id="da157-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="da157-160">isFeatured</span></span>|<span data-ttu-id="da157-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="da157-161">Boolean</span></span>|<span data-ttu-id="da157-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="da157-163">privacyInformationUrl</span></span>|<span data-ttu-id="da157-164">字符串</span><span class="sxs-lookup"><span data-stu-id="da157-164">String</span></span>|<span data-ttu-id="da157-165">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="da157-165">The privacy statement Url.</span></span> <span data-ttu-id="da157-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="da157-167">informationUrl</span></span>|<span data-ttu-id="da157-168">字符串</span><span class="sxs-lookup"><span data-stu-id="da157-168">String</span></span>|<span data-ttu-id="da157-169">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="da157-169">The more information Url.</span></span> <span data-ttu-id="da157-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-171">owner</span><span class="sxs-lookup"><span data-stu-id="da157-171">owner</span></span>|<span data-ttu-id="da157-172">String</span><span class="sxs-lookup"><span data-stu-id="da157-172">String</span></span>|<span data-ttu-id="da157-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="da157-173">The owner of the app.</span></span> <span data-ttu-id="da157-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-175">developer</span><span class="sxs-lookup"><span data-stu-id="da157-175">developer</span></span>|<span data-ttu-id="da157-176">String</span><span class="sxs-lookup"><span data-stu-id="da157-176">String</span></span>|<span data-ttu-id="da157-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="da157-177">The developer of the app.</span></span> <span data-ttu-id="da157-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-179">notes</span><span class="sxs-lookup"><span data-stu-id="da157-179">notes</span></span>|<span data-ttu-id="da157-180">String</span><span class="sxs-lookup"><span data-stu-id="da157-180">String</span></span>|<span data-ttu-id="da157-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="da157-181">Notes for the app.</span></span> <span data-ttu-id="da157-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="da157-183">uploadState</span></span>|<span data-ttu-id="da157-184">Int32</span><span class="sxs-lookup"><span data-stu-id="da157-184">Int32</span></span>|<span data-ttu-id="da157-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="da157-185">The upload state.</span></span> <span data-ttu-id="da157-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="da157-187">publishingState</span></span>|[<span data-ttu-id="da157-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="da157-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="da157-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="da157-189">The publishing state for the app.</span></span> <span data-ttu-id="da157-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="da157-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="da157-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="da157-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="da157-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="da157-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="da157-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="da157-193">isAssigned</span></span>|<span data-ttu-id="da157-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="da157-194">Boolean</span></span>|<span data-ttu-id="da157-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="da157-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="da157-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="da157-197">roleScopeTagIds</span></span>|<span data-ttu-id="da157-198">String collection</span><span class="sxs-lookup"><span data-stu-id="da157-198">String collection</span></span>|<span data-ttu-id="da157-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="da157-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="da157-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da157-201">appAvailability</span><span class="sxs-lookup"><span data-stu-id="da157-201">appAvailability</span></span>|[<span data-ttu-id="da157-202">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="da157-202">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="da157-203">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="da157-203">The Application's availability.</span></span> <span data-ttu-id="da157-204">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="da157-204">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="da157-205">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="da157-205">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="da157-206">version</span><span class="sxs-lookup"><span data-stu-id="da157-206">version</span></span>|<span data-ttu-id="da157-207">字符串</span><span class="sxs-lookup"><span data-stu-id="da157-207">String</span></span>|<span data-ttu-id="da157-208">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="da157-208">The Application's version.</span></span> <span data-ttu-id="da157-209">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-209">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="da157-210">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="da157-210">committedContentVersion</span></span>|<span data-ttu-id="da157-211">字符串</span><span class="sxs-lookup"><span data-stu-id="da157-211">String</span></span>|<span data-ttu-id="da157-212">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="da157-212">The internal committed content version.</span></span> <span data-ttu-id="da157-213">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-213">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="da157-214">fileName</span><span class="sxs-lookup"><span data-stu-id="da157-214">fileName</span></span>|<span data-ttu-id="da157-215">字符串</span><span class="sxs-lookup"><span data-stu-id="da157-215">String</span></span>|<span data-ttu-id="da157-216">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="da157-216">The name of the main Lob application file.</span></span> <span data-ttu-id="da157-217">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="da157-218">size</span><span class="sxs-lookup"><span data-stu-id="da157-218">size</span></span>|<span data-ttu-id="da157-219">Int64</span><span class="sxs-lookup"><span data-stu-id="da157-219">Int64</span></span>|<span data-ttu-id="da157-220">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="da157-220">The total size, including all uploaded files.</span></span> <span data-ttu-id="da157-221">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="da157-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="da157-222">bundleId</span><span class="sxs-lookup"><span data-stu-id="da157-222">bundleId</span></span>|<span data-ttu-id="da157-223">字符串</span><span class="sxs-lookup"><span data-stu-id="da157-223">String</span></span>|<span data-ttu-id="da157-224">标识名称。</span><span class="sxs-lookup"><span data-stu-id="da157-224">The Identity Name.</span></span>|
|<span data-ttu-id="da157-225">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="da157-225">applicableDeviceType</span></span>|[<span data-ttu-id="da157-226">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="da157-226">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="da157-227">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="da157-227">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="da157-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="da157-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="da157-229">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="da157-229">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="da157-230">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="da157-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="da157-231">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="da157-231">expirationDateTime</span></span>|<span data-ttu-id="da157-232">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da157-232">DateTimeOffset</span></span>|<span data-ttu-id="da157-233">过期时间。</span><span class="sxs-lookup"><span data-stu-id="da157-233">The expiration time.</span></span>|
|<span data-ttu-id="da157-234">versionNumber</span><span class="sxs-lookup"><span data-stu-id="da157-234">versionNumber</span></span>|<span data-ttu-id="da157-235">String</span><span class="sxs-lookup"><span data-stu-id="da157-235">String</span></span>|<span data-ttu-id="da157-236">托管 iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="da157-236">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="da157-237">buildNumber</span><span class="sxs-lookup"><span data-stu-id="da157-237">buildNumber</span></span>|<span data-ttu-id="da157-238">字符串</span><span class="sxs-lookup"><span data-stu-id="da157-238">String</span></span>|<span data-ttu-id="da157-239">托管 iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="da157-239">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="da157-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="da157-240">identityVersion</span></span>|<span data-ttu-id="da157-241">String</span><span class="sxs-lookup"><span data-stu-id="da157-241">String</span></span>|<span data-ttu-id="da157-242">标识版本。</span><span class="sxs-lookup"><span data-stu-id="da157-242">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="da157-243">响应</span><span class="sxs-lookup"><span data-stu-id="da157-243">Response</span></span>
<span data-ttu-id="da157-244">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da157-244">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da157-245">示例</span><span class="sxs-lookup"><span data-stu-id="da157-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="da157-246">请求</span><span class="sxs-lookup"><span data-stu-id="da157-246">Request</span></span>
<span data-ttu-id="da157-247">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da157-247">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1442

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="da157-248">响应</span><span class="sxs-lookup"><span data-stu-id="da157-248">Response</span></span>
<span data-ttu-id="da157-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da157-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1614

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




