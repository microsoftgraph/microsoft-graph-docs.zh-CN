---
title: 更新 windowsUniversalAppX
description: 更新 windowsUniversalAppX 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 003b4450c17025cf44f4d7bde88c7cbd02277412
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32485906"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="f4199-103">更新 windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="f4199-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="f4199-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4199-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4199-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4199-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4199-106">更新 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f4199-106">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4199-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f4199-107">Prerequisites</span></span>
<span data-ttu-id="f4199-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4199-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4199-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4199-110">Permission type</span></span>|<span data-ttu-id="f4199-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f4199-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4199-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4199-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f4199-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4199-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f4199-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4199-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4199-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4199-115">Not supported.</span></span>|
|<span data-ttu-id="f4199-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4199-116">Application</span></span>|<span data-ttu-id="f4199-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4199-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4199-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4199-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f4199-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4199-119">Request headers</span></span>
|<span data-ttu-id="f4199-120">标头</span><span class="sxs-lookup"><span data-stu-id="f4199-120">Header</span></span>|<span data-ttu-id="f4199-121">值</span><span class="sxs-lookup"><span data-stu-id="f4199-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4199-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4199-122">Authorization</span></span>|<span data-ttu-id="f4199-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f4199-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4199-124">接受</span><span class="sxs-lookup"><span data-stu-id="f4199-124">Accept</span></span>|<span data-ttu-id="f4199-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f4199-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4199-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4199-126">Request body</span></span>
<span data-ttu-id="f4199-127">在请求正文中，提供 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4199-127">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="f4199-128">下表显示创建 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f4199-128">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="f4199-129">属性</span><span class="sxs-lookup"><span data-stu-id="f4199-129">Property</span></span>|<span data-ttu-id="f4199-130">类型</span><span class="sxs-lookup"><span data-stu-id="f4199-130">Type</span></span>|<span data-ttu-id="f4199-131">说明</span><span class="sxs-lookup"><span data-stu-id="f4199-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4199-132">id</span><span class="sxs-lookup"><span data-stu-id="f4199-132">id</span></span>|<span data-ttu-id="f4199-133">String</span><span class="sxs-lookup"><span data-stu-id="f4199-133">String</span></span>|<span data-ttu-id="f4199-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f4199-134">Key of the entity.</span></span> <span data-ttu-id="f4199-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f4199-136">displayName</span></span>|<span data-ttu-id="f4199-137">字符串</span><span class="sxs-lookup"><span data-stu-id="f4199-137">String</span></span>|<span data-ttu-id="f4199-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="f4199-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f4199-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-140">description</span><span class="sxs-lookup"><span data-stu-id="f4199-140">description</span></span>|<span data-ttu-id="f4199-141">字符串</span><span class="sxs-lookup"><span data-stu-id="f4199-141">String</span></span>|<span data-ttu-id="f4199-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="f4199-142">The description of the app.</span></span> <span data-ttu-id="f4199-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-144">publisher</span><span class="sxs-lookup"><span data-stu-id="f4199-144">publisher</span></span>|<span data-ttu-id="f4199-145">字符串</span><span class="sxs-lookup"><span data-stu-id="f4199-145">String</span></span>|<span data-ttu-id="f4199-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="f4199-146">The publisher of the app.</span></span> <span data-ttu-id="f4199-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f4199-148">largeIcon</span></span>|[<span data-ttu-id="f4199-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f4199-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f4199-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="f4199-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f4199-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4199-152">createdDateTime</span></span>|<span data-ttu-id="f4199-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4199-153">DateTimeOffset</span></span>|<span data-ttu-id="f4199-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f4199-154">The date and time the app was created.</span></span> <span data-ttu-id="f4199-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4199-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f4199-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4199-157">DateTimeOffset</span></span>|<span data-ttu-id="f4199-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f4199-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f4199-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f4199-160">isFeatured</span></span>|<span data-ttu-id="f4199-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4199-161">Boolean</span></span>|<span data-ttu-id="f4199-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f4199-163">privacyInformationUrl</span></span>|<span data-ttu-id="f4199-164">字符串</span><span class="sxs-lookup"><span data-stu-id="f4199-164">String</span></span>|<span data-ttu-id="f4199-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="f4199-165">The privacy statement Url.</span></span> <span data-ttu-id="f4199-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f4199-167">informationUrl</span></span>|<span data-ttu-id="f4199-168">字符串</span><span class="sxs-lookup"><span data-stu-id="f4199-168">String</span></span>|<span data-ttu-id="f4199-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="f4199-169">The more information Url.</span></span> <span data-ttu-id="f4199-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-171">owner</span><span class="sxs-lookup"><span data-stu-id="f4199-171">owner</span></span>|<span data-ttu-id="f4199-172">字符串</span><span class="sxs-lookup"><span data-stu-id="f4199-172">String</span></span>|<span data-ttu-id="f4199-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="f4199-173">The owner of the app.</span></span> <span data-ttu-id="f4199-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-175">developer</span><span class="sxs-lookup"><span data-stu-id="f4199-175">developer</span></span>|<span data-ttu-id="f4199-176">字符串</span><span class="sxs-lookup"><span data-stu-id="f4199-176">String</span></span>|<span data-ttu-id="f4199-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="f4199-177">The developer of the app.</span></span> <span data-ttu-id="f4199-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-179">notes</span><span class="sxs-lookup"><span data-stu-id="f4199-179">notes</span></span>|<span data-ttu-id="f4199-180">字符串</span><span class="sxs-lookup"><span data-stu-id="f4199-180">String</span></span>|<span data-ttu-id="f4199-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="f4199-181">Notes for the app.</span></span> <span data-ttu-id="f4199-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="f4199-183">uploadState</span></span>|<span data-ttu-id="f4199-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f4199-184">Int32</span></span>|<span data-ttu-id="f4199-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="f4199-185">The upload state.</span></span> <span data-ttu-id="f4199-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="f4199-187">publishingState</span></span>|[<span data-ttu-id="f4199-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f4199-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f4199-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="f4199-189">The publishing state for the app.</span></span> <span data-ttu-id="f4199-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="f4199-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f4199-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="f4199-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f4199-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="f4199-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f4199-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f4199-193">isAssigned</span></span>|<span data-ttu-id="f4199-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4199-194">Boolean</span></span>|<span data-ttu-id="f4199-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="f4199-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f4199-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f4199-197">roleScopeTagIds</span></span>|<span data-ttu-id="f4199-198">String collection</span><span class="sxs-lookup"><span data-stu-id="f4199-198">String collection</span></span>|<span data-ttu-id="f4199-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="f4199-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f4199-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="f4199-201">dependentAppCount</span></span>|<span data-ttu-id="f4199-202">Int32</span><span class="sxs-lookup"><span data-stu-id="f4199-202">Int32</span></span>|<span data-ttu-id="f4199-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="f4199-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f4199-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4199-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f4199-205">committedContentVersion</span></span>|<span data-ttu-id="f4199-206">字符串</span><span class="sxs-lookup"><span data-stu-id="f4199-206">String</span></span>|<span data-ttu-id="f4199-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="f4199-207">The internal committed content version.</span></span> <span data-ttu-id="f4199-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f4199-209">fileName</span><span class="sxs-lookup"><span data-stu-id="f4199-209">fileName</span></span>|<span data-ttu-id="f4199-210">字符串</span><span class="sxs-lookup"><span data-stu-id="f4199-210">String</span></span>|<span data-ttu-id="f4199-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="f4199-211">The name of the main Lob application file.</span></span> <span data-ttu-id="f4199-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f4199-213">size</span><span class="sxs-lookup"><span data-stu-id="f4199-213">size</span></span>|<span data-ttu-id="f4199-214">Int64</span><span class="sxs-lookup"><span data-stu-id="f4199-214">Int64</span></span>|<span data-ttu-id="f4199-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="f4199-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="f4199-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4199-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f4199-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="f4199-217">applicableArchitectures</span></span>|[<span data-ttu-id="f4199-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="f4199-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="f4199-219">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="f4199-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="f4199-220">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="f4199-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="f4199-221">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="f4199-221">applicableDeviceTypes</span></span>|[<span data-ttu-id="f4199-222">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="f4199-222">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="f4199-223">可运行此应用的 Windows 设备类型。</span><span class="sxs-lookup"><span data-stu-id="f4199-223">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="f4199-224">可取值为：`none`、`desktop`、`mobile`、`holographic`、`team`。</span><span class="sxs-lookup"><span data-stu-id="f4199-224">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="f4199-225">identityName</span><span class="sxs-lookup"><span data-stu-id="f4199-225">identityName</span></span>|<span data-ttu-id="f4199-226">String</span><span class="sxs-lookup"><span data-stu-id="f4199-226">String</span></span>|<span data-ttu-id="f4199-227">标识名称。</span><span class="sxs-lookup"><span data-stu-id="f4199-227">The Identity Name.</span></span>|
|<span data-ttu-id="f4199-228">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="f4199-228">identityPublisherHash</span></span>|<span data-ttu-id="f4199-229">字符串</span><span class="sxs-lookup"><span data-stu-id="f4199-229">String</span></span>|<span data-ttu-id="f4199-230">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="f4199-230">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="f4199-231">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f4199-231">identityResourceIdentifier</span></span>|<span data-ttu-id="f4199-232">字符串</span><span class="sxs-lookup"><span data-stu-id="f4199-232">String</span></span>|<span data-ttu-id="f4199-233">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="f4199-233">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="f4199-234">isBundle</span><span class="sxs-lookup"><span data-stu-id="f4199-234">isBundle</span></span>|<span data-ttu-id="f4199-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4199-235">Boolean</span></span>|<span data-ttu-id="f4199-236">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="f4199-236">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="f4199-237">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f4199-237">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f4199-238">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f4199-238">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="f4199-239">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="f4199-239">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f4199-240">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f4199-240">identityVersion</span></span>|<span data-ttu-id="f4199-241">String</span><span class="sxs-lookup"><span data-stu-id="f4199-241">String</span></span>|<span data-ttu-id="f4199-242">标识版本。</span><span class="sxs-lookup"><span data-stu-id="f4199-242">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="f4199-243">响应</span><span class="sxs-lookup"><span data-stu-id="f4199-243">Response</span></span>
<span data-ttu-id="f4199-244">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4199-244">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4199-245">示例</span><span class="sxs-lookup"><span data-stu-id="f4199-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4199-246">请求</span><span class="sxs-lookup"><span data-stu-id="f4199-246">Request</span></span>
<span data-ttu-id="f4199-247">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f4199-247">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1415

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
  "dependentAppCount": 1,
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

### <a name="response"></a><span data-ttu-id="f4199-248">响应</span><span class="sxs-lookup"><span data-stu-id="f4199-248">Response</span></span>
<span data-ttu-id="f4199-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f4199-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1587

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
  "dependentAppCount": 1,
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





