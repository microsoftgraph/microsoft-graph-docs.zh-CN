---
title: 更新 windowsUniversalAppX
description: 更新 windowsUniversalAppX 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da8f94a3b2824db1ec20248f9d771c1c370d6e78
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976097"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="98581-103">更新 windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="98581-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="98581-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="98581-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98581-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="98581-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98581-106">更新 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="98581-106">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98581-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="98581-107">Prerequisites</span></span>
<span data-ttu-id="98581-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98581-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98581-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="98581-110">Permission type</span></span>|<span data-ttu-id="98581-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="98581-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98581-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98581-112">Delegated (work or school account)</span></span>|<span data-ttu-id="98581-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98581-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="98581-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98581-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98581-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="98581-115">Not supported.</span></span>|
|<span data-ttu-id="98581-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="98581-116">Application</span></span>|<span data-ttu-id="98581-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="98581-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98581-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98581-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="98581-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="98581-119">Request headers</span></span>
|<span data-ttu-id="98581-120">标头</span><span class="sxs-lookup"><span data-stu-id="98581-120">Header</span></span>|<span data-ttu-id="98581-121">值</span><span class="sxs-lookup"><span data-stu-id="98581-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98581-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="98581-122">Authorization</span></span>|<span data-ttu-id="98581-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="98581-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98581-124">接受</span><span class="sxs-lookup"><span data-stu-id="98581-124">Accept</span></span>|<span data-ttu-id="98581-125">application/json</span><span class="sxs-lookup"><span data-stu-id="98581-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98581-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="98581-126">Request body</span></span>
<span data-ttu-id="98581-127">在请求正文中，提供 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98581-127">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="98581-128">下表显示创建 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="98581-128">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="98581-129">属性</span><span class="sxs-lookup"><span data-stu-id="98581-129">Property</span></span>|<span data-ttu-id="98581-130">类型</span><span class="sxs-lookup"><span data-stu-id="98581-130">Type</span></span>|<span data-ttu-id="98581-131">说明</span><span class="sxs-lookup"><span data-stu-id="98581-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98581-132">id</span><span class="sxs-lookup"><span data-stu-id="98581-132">id</span></span>|<span data-ttu-id="98581-133">String</span><span class="sxs-lookup"><span data-stu-id="98581-133">String</span></span>|<span data-ttu-id="98581-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="98581-134">Key of the entity.</span></span> <span data-ttu-id="98581-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-136">displayName</span><span class="sxs-lookup"><span data-stu-id="98581-136">displayName</span></span>|<span data-ttu-id="98581-137">String</span><span class="sxs-lookup"><span data-stu-id="98581-137">String</span></span>|<span data-ttu-id="98581-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="98581-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="98581-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-140">description</span><span class="sxs-lookup"><span data-stu-id="98581-140">description</span></span>|<span data-ttu-id="98581-141">String</span><span class="sxs-lookup"><span data-stu-id="98581-141">String</span></span>|<span data-ttu-id="98581-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="98581-142">The description of the app.</span></span> <span data-ttu-id="98581-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-144">publisher</span><span class="sxs-lookup"><span data-stu-id="98581-144">publisher</span></span>|<span data-ttu-id="98581-145">String</span><span class="sxs-lookup"><span data-stu-id="98581-145">String</span></span>|<span data-ttu-id="98581-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="98581-146">The publisher of the app.</span></span> <span data-ttu-id="98581-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="98581-148">largeIcon</span></span>|[<span data-ttu-id="98581-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="98581-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="98581-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="98581-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="98581-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="98581-152">createdDateTime</span></span>|<span data-ttu-id="98581-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98581-153">DateTimeOffset</span></span>|<span data-ttu-id="98581-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="98581-154">The date and time the app was created.</span></span> <span data-ttu-id="98581-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="98581-156">lastModifiedDateTime</span></span>|<span data-ttu-id="98581-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98581-157">DateTimeOffset</span></span>|<span data-ttu-id="98581-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="98581-158">The date and time the app was last modified.</span></span> <span data-ttu-id="98581-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="98581-160">isFeatured</span></span>|<span data-ttu-id="98581-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="98581-161">Boolean</span></span>|<span data-ttu-id="98581-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="98581-163">privacyInformationUrl</span></span>|<span data-ttu-id="98581-164">String</span><span class="sxs-lookup"><span data-stu-id="98581-164">String</span></span>|<span data-ttu-id="98581-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="98581-165">The privacy statement Url.</span></span> <span data-ttu-id="98581-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="98581-167">informationUrl</span></span>|<span data-ttu-id="98581-168">String</span><span class="sxs-lookup"><span data-stu-id="98581-168">String</span></span>|<span data-ttu-id="98581-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="98581-169">The more information Url.</span></span> <span data-ttu-id="98581-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-171">owner</span><span class="sxs-lookup"><span data-stu-id="98581-171">owner</span></span>|<span data-ttu-id="98581-172">字符串</span><span class="sxs-lookup"><span data-stu-id="98581-172">String</span></span>|<span data-ttu-id="98581-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="98581-173">The owner of the app.</span></span> <span data-ttu-id="98581-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-175">developer</span><span class="sxs-lookup"><span data-stu-id="98581-175">developer</span></span>|<span data-ttu-id="98581-176">String</span><span class="sxs-lookup"><span data-stu-id="98581-176">String</span></span>|<span data-ttu-id="98581-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="98581-177">The developer of the app.</span></span> <span data-ttu-id="98581-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-179">notes</span><span class="sxs-lookup"><span data-stu-id="98581-179">notes</span></span>|<span data-ttu-id="98581-180">String</span><span class="sxs-lookup"><span data-stu-id="98581-180">String</span></span>|<span data-ttu-id="98581-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="98581-181">Notes for the app.</span></span> <span data-ttu-id="98581-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="98581-183">uploadState</span></span>|<span data-ttu-id="98581-184">Int32</span><span class="sxs-lookup"><span data-stu-id="98581-184">Int32</span></span>|<span data-ttu-id="98581-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="98581-185">The upload state.</span></span> <span data-ttu-id="98581-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="98581-187">publishingState</span></span>|[<span data-ttu-id="98581-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="98581-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="98581-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="98581-189">The publishing state for the app.</span></span> <span data-ttu-id="98581-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="98581-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="98581-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="98581-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="98581-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="98581-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="98581-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="98581-193">isAssigned</span></span>|<span data-ttu-id="98581-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="98581-194">Boolean</span></span>|<span data-ttu-id="98581-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="98581-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="98581-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="98581-197">roleScopeTagIds</span></span>|<span data-ttu-id="98581-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="98581-198">String collection</span></span>|<span data-ttu-id="98581-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="98581-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="98581-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98581-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="98581-201">committedContentVersion</span></span>|<span data-ttu-id="98581-202">String</span><span class="sxs-lookup"><span data-stu-id="98581-202">String</span></span>|<span data-ttu-id="98581-203">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="98581-203">The internal committed content version.</span></span> <span data-ttu-id="98581-204">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="98581-205">fileName</span><span class="sxs-lookup"><span data-stu-id="98581-205">fileName</span></span>|<span data-ttu-id="98581-206">String</span><span class="sxs-lookup"><span data-stu-id="98581-206">String</span></span>|<span data-ttu-id="98581-207">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="98581-207">The name of the main Lob application file.</span></span> <span data-ttu-id="98581-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="98581-209">size</span><span class="sxs-lookup"><span data-stu-id="98581-209">size</span></span>|<span data-ttu-id="98581-210">Int64</span><span class="sxs-lookup"><span data-stu-id="98581-210">Int64</span></span>|<span data-ttu-id="98581-211">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="98581-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="98581-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="98581-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="98581-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="98581-213">applicableArchitectures</span></span>|[<span data-ttu-id="98581-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="98581-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="98581-215">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="98581-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="98581-216">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="98581-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="98581-217">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="98581-217">applicableDeviceTypes</span></span>|[<span data-ttu-id="98581-218">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="98581-218">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="98581-219">可运行此应用的 Windows 设备类型。</span><span class="sxs-lookup"><span data-stu-id="98581-219">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="98581-220">可取值为：`none`、`desktop`、`mobile`、`holographic`、`team`。</span><span class="sxs-lookup"><span data-stu-id="98581-220">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="98581-221">identityName</span><span class="sxs-lookup"><span data-stu-id="98581-221">identityName</span></span>|<span data-ttu-id="98581-222">String</span><span class="sxs-lookup"><span data-stu-id="98581-222">String</span></span>|<span data-ttu-id="98581-223">标识名称。</span><span class="sxs-lookup"><span data-stu-id="98581-223">The Identity Name.</span></span>|
|<span data-ttu-id="98581-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="98581-224">identityPublisherHash</span></span>|<span data-ttu-id="98581-225">String</span><span class="sxs-lookup"><span data-stu-id="98581-225">String</span></span>|<span data-ttu-id="98581-226">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="98581-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="98581-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="98581-227">identityResourceIdentifier</span></span>|<span data-ttu-id="98581-228">String</span><span class="sxs-lookup"><span data-stu-id="98581-228">String</span></span>|<span data-ttu-id="98581-229">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="98581-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="98581-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="98581-230">isBundle</span></span>|<span data-ttu-id="98581-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="98581-231">Boolean</span></span>|<span data-ttu-id="98581-232">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="98581-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="98581-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="98581-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="98581-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="98581-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="98581-235">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="98581-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="98581-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="98581-236">identityVersion</span></span>|<span data-ttu-id="98581-237">String</span><span class="sxs-lookup"><span data-stu-id="98581-237">String</span></span>|<span data-ttu-id="98581-238">标识版本。</span><span class="sxs-lookup"><span data-stu-id="98581-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="98581-239">响应</span><span class="sxs-lookup"><span data-stu-id="98581-239">Response</span></span>
<span data-ttu-id="98581-240">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="98581-240">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98581-241">示例</span><span class="sxs-lookup"><span data-stu-id="98581-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="98581-242">请求</span><span class="sxs-lookup"><span data-stu-id="98581-242">Request</span></span>
<span data-ttu-id="98581-243">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="98581-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1388

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableDeviceTypes": "desktop",
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

### <a name="response"></a><span data-ttu-id="98581-244">响应</span><span class="sxs-lookup"><span data-stu-id="98581-244">Response</span></span>
<span data-ttu-id="98581-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="98581-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1560

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "applicableDeviceTypes": "desktop",
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




