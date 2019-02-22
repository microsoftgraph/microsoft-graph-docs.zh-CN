---
title: 更新 windowsAppX
description: 更新 windowsAppX 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c5abc2a461019ad7970d6b4c500e2c593b9c4aa7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141228"
---
# <a name="update-windowsappx"></a><span data-ttu-id="e7719-103">更新 windowsAppX</span><span class="sxs-lookup"><span data-stu-id="e7719-103">Update windowsAppX</span></span>

> <span data-ttu-id="e7719-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e7719-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7719-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e7719-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7719-106">更新[windowsAppX](../resources/intune-apps-windowsappx.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e7719-106">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7719-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e7719-107">Prerequisites</span></span>
<span data-ttu-id="e7719-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e7719-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e7719-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7719-110">Permission type</span></span>|<span data-ttu-id="e7719-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e7719-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7719-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7719-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7719-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7719-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e7719-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7719-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7719-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7719-115">Not supported.</span></span>|
|<span data-ttu-id="e7719-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7719-116">Application</span></span>|<span data-ttu-id="e7719-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7719-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7719-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7719-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e7719-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7719-119">Request headers</span></span>
|<span data-ttu-id="e7719-120">标头</span><span class="sxs-lookup"><span data-stu-id="e7719-120">Header</span></span>|<span data-ttu-id="e7719-121">值</span><span class="sxs-lookup"><span data-stu-id="e7719-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7719-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7719-122">Authorization</span></span>|<span data-ttu-id="e7719-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e7719-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7719-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e7719-124">Accept</span></span>|<span data-ttu-id="e7719-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7719-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7719-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7719-126">Request body</span></span>
<span data-ttu-id="e7719-127">在请求正文中, 提供[windowsAppX](../resources/intune-apps-windowsappx.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7719-127">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="e7719-128">下表显示创建[windowsAppX](../resources/intune-apps-windowsappx.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e7719-128">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="e7719-129">属性</span><span class="sxs-lookup"><span data-stu-id="e7719-129">Property</span></span>|<span data-ttu-id="e7719-130">类型</span><span class="sxs-lookup"><span data-stu-id="e7719-130">Type</span></span>|<span data-ttu-id="e7719-131">说明</span><span class="sxs-lookup"><span data-stu-id="e7719-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7719-132">id</span><span class="sxs-lookup"><span data-stu-id="e7719-132">id</span></span>|<span data-ttu-id="e7719-133">字串符号</span><span class="sxs-lookup"><span data-stu-id="e7719-133">String</span></span>|<span data-ttu-id="e7719-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e7719-134">Key of the entity.</span></span> <span data-ttu-id="e7719-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e7719-136">displayName</span></span>|<span data-ttu-id="e7719-137">字符串</span><span class="sxs-lookup"><span data-stu-id="e7719-137">String</span></span>|<span data-ttu-id="e7719-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="e7719-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e7719-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-140">description</span><span class="sxs-lookup"><span data-stu-id="e7719-140">description</span></span>|<span data-ttu-id="e7719-141">字符串</span><span class="sxs-lookup"><span data-stu-id="e7719-141">String</span></span>|<span data-ttu-id="e7719-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="e7719-142">The description of the app.</span></span> <span data-ttu-id="e7719-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-144">publisher</span><span class="sxs-lookup"><span data-stu-id="e7719-144">publisher</span></span>|<span data-ttu-id="e7719-145">字符串</span><span class="sxs-lookup"><span data-stu-id="e7719-145">String</span></span>|<span data-ttu-id="e7719-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="e7719-146">The publisher of the app.</span></span> <span data-ttu-id="e7719-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e7719-148">largeIcon</span></span>|[<span data-ttu-id="e7719-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e7719-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e7719-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="e7719-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e7719-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7719-152">createdDateTime</span></span>|<span data-ttu-id="e7719-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7719-153">DateTimeOffset</span></span>|<span data-ttu-id="e7719-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e7719-154">The date and time the app was created.</span></span> <span data-ttu-id="e7719-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7719-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e7719-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7719-157">DateTimeOffset</span></span>|<span data-ttu-id="e7719-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e7719-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e7719-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e7719-160">isFeatured</span></span>|<span data-ttu-id="e7719-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7719-161">Boolean</span></span>|<span data-ttu-id="e7719-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e7719-163">privacyInformationUrl</span></span>|<span data-ttu-id="e7719-164">字符串</span><span class="sxs-lookup"><span data-stu-id="e7719-164">String</span></span>|<span data-ttu-id="e7719-165">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="e7719-165">The privacy statement Url.</span></span> <span data-ttu-id="e7719-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e7719-167">informationUrl</span></span>|<span data-ttu-id="e7719-168">字符串</span><span class="sxs-lookup"><span data-stu-id="e7719-168">String</span></span>|<span data-ttu-id="e7719-169">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="e7719-169">The more information Url.</span></span> <span data-ttu-id="e7719-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-171">owner</span><span class="sxs-lookup"><span data-stu-id="e7719-171">owner</span></span>|<span data-ttu-id="e7719-172">字符串</span><span class="sxs-lookup"><span data-stu-id="e7719-172">String</span></span>|<span data-ttu-id="e7719-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="e7719-173">The owner of the app.</span></span> <span data-ttu-id="e7719-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-175">developer</span><span class="sxs-lookup"><span data-stu-id="e7719-175">developer</span></span>|<span data-ttu-id="e7719-176">字符串</span><span class="sxs-lookup"><span data-stu-id="e7719-176">String</span></span>|<span data-ttu-id="e7719-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="e7719-177">The developer of the app.</span></span> <span data-ttu-id="e7719-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-179">notes</span><span class="sxs-lookup"><span data-stu-id="e7719-179">notes</span></span>|<span data-ttu-id="e7719-180">字符串</span><span class="sxs-lookup"><span data-stu-id="e7719-180">String</span></span>|<span data-ttu-id="e7719-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="e7719-181">Notes for the app.</span></span> <span data-ttu-id="e7719-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="e7719-183">uploadState</span></span>|<span data-ttu-id="e7719-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e7719-184">Int32</span></span>|<span data-ttu-id="e7719-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="e7719-185">The upload state.</span></span> <span data-ttu-id="e7719-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="e7719-187">publishingState</span></span>|[<span data-ttu-id="e7719-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e7719-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e7719-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="e7719-189">The publishing state for the app.</span></span> <span data-ttu-id="e7719-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="e7719-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e7719-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="e7719-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e7719-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="e7719-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e7719-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e7719-193">isAssigned</span></span>|<span data-ttu-id="e7719-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7719-194">Boolean</span></span>|<span data-ttu-id="e7719-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="e7719-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e7719-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e7719-197">roleScopeTagIds</span></span>|<span data-ttu-id="e7719-198">String collection</span><span class="sxs-lookup"><span data-stu-id="e7719-198">String collection</span></span>|<span data-ttu-id="e7719-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="e7719-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e7719-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7719-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e7719-201">committedContentVersion</span></span>|<span data-ttu-id="e7719-202">String</span><span class="sxs-lookup"><span data-stu-id="e7719-202">String</span></span>|<span data-ttu-id="e7719-203">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="e7719-203">The internal committed content version.</span></span> <span data-ttu-id="e7719-204">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e7719-205">fileName</span><span class="sxs-lookup"><span data-stu-id="e7719-205">fileName</span></span>|<span data-ttu-id="e7719-206">字符串</span><span class="sxs-lookup"><span data-stu-id="e7719-206">String</span></span>|<span data-ttu-id="e7719-207">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="e7719-207">The name of the main Lob application file.</span></span> <span data-ttu-id="e7719-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e7719-209">size</span><span class="sxs-lookup"><span data-stu-id="e7719-209">size</span></span>|<span data-ttu-id="e7719-210">Int64</span><span class="sxs-lookup"><span data-stu-id="e7719-210">Int64</span></span>|<span data-ttu-id="e7719-211">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="e7719-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="e7719-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e7719-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e7719-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="e7719-213">applicableArchitectures</span></span>|[<span data-ttu-id="e7719-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="e7719-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="e7719-215">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="e7719-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="e7719-216">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="e7719-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="e7719-217">identityName</span><span class="sxs-lookup"><span data-stu-id="e7719-217">identityName</span></span>|<span data-ttu-id="e7719-218">字符串</span><span class="sxs-lookup"><span data-stu-id="e7719-218">String</span></span>|<span data-ttu-id="e7719-219">标识名称。</span><span class="sxs-lookup"><span data-stu-id="e7719-219">The Identity Name.</span></span>|
|<span data-ttu-id="e7719-220">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="e7719-220">identityPublisherHash</span></span>|<span data-ttu-id="e7719-221">字符串</span><span class="sxs-lookup"><span data-stu-id="e7719-221">String</span></span>|<span data-ttu-id="e7719-222">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="e7719-222">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="e7719-223">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e7719-223">identityResourceIdentifier</span></span>|<span data-ttu-id="e7719-224">String</span><span class="sxs-lookup"><span data-stu-id="e7719-224">String</span></span>|<span data-ttu-id="e7719-225">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="e7719-225">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="e7719-226">isBundle</span><span class="sxs-lookup"><span data-stu-id="e7719-226">isBundle</span></span>|<span data-ttu-id="e7719-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7719-227">Boolean</span></span>|<span data-ttu-id="e7719-228">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="e7719-228">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="e7719-229">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e7719-229">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e7719-230">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e7719-230">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="e7719-231">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="e7719-231">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e7719-232">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e7719-232">identityVersion</span></span>|<span data-ttu-id="e7719-233">String</span><span class="sxs-lookup"><span data-stu-id="e7719-233">String</span></span>|<span data-ttu-id="e7719-234">标识版本。</span><span class="sxs-lookup"><span data-stu-id="e7719-234">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="e7719-235">响应</span><span class="sxs-lookup"><span data-stu-id="e7719-235">Response</span></span>
<span data-ttu-id="e7719-236">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsAppX](../resources/intune-apps-windowsappx.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e7719-236">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7719-237">示例</span><span class="sxs-lookup"><span data-stu-id="e7719-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7719-238">请求</span><span class="sxs-lookup"><span data-stu-id="e7719-238">Request</span></span>
<span data-ttu-id="e7719-239">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7719-239">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1340

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="e7719-240">响应</span><span class="sxs-lookup"><span data-stu-id="e7719-240">Response</span></span>
<span data-ttu-id="e7719-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e7719-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1512

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```




