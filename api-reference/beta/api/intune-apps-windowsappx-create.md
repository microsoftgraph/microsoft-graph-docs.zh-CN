---
title: 创建 windowsAppX
description: 创建新的 windowsAppX 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1d046e3fa04a7e1cd89979ffe00502cca0eb3d4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780866"
---
# <a name="create-windowsappx"></a><span data-ttu-id="79873-103">创建 windowsAppX</span><span class="sxs-lookup"><span data-stu-id="79873-103">Create windowsAppX</span></span>

> <span data-ttu-id="79873-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="79873-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79873-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79873-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79873-106">创建新的[windowsAppX](../resources/intune-apps-windowsappx.md)对象。</span><span class="sxs-lookup"><span data-stu-id="79873-106">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79873-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="79873-107">Prerequisites</span></span>
<span data-ttu-id="79873-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79873-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79873-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="79873-110">Permission type</span></span>|<span data-ttu-id="79873-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="79873-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79873-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79873-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79873-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79873-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="79873-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79873-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79873-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="79873-115">Not supported.</span></span>|
|<span data-ttu-id="79873-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="79873-116">Application</span></span>|<span data-ttu-id="79873-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="79873-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79873-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79873-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="79873-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="79873-119">Request headers</span></span>
|<span data-ttu-id="79873-120">标头</span><span class="sxs-lookup"><span data-stu-id="79873-120">Header</span></span>|<span data-ttu-id="79873-121">值</span><span class="sxs-lookup"><span data-stu-id="79873-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79873-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="79873-122">Authorization</span></span>|<span data-ttu-id="79873-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="79873-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79873-124">接受</span><span class="sxs-lookup"><span data-stu-id="79873-124">Accept</span></span>|<span data-ttu-id="79873-125">application/json</span><span class="sxs-lookup"><span data-stu-id="79873-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79873-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="79873-126">Request body</span></span>
<span data-ttu-id="79873-127">在请求正文中, 提供 windowsAppX 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79873-127">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="79873-128">下表显示创建 windowsAppX 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="79873-128">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="79873-129">属性</span><span class="sxs-lookup"><span data-stu-id="79873-129">Property</span></span>|<span data-ttu-id="79873-130">类型</span><span class="sxs-lookup"><span data-stu-id="79873-130">Type</span></span>|<span data-ttu-id="79873-131">说明</span><span class="sxs-lookup"><span data-stu-id="79873-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79873-132">id</span><span class="sxs-lookup"><span data-stu-id="79873-132">id</span></span>|<span data-ttu-id="79873-133">String</span><span class="sxs-lookup"><span data-stu-id="79873-133">String</span></span>|<span data-ttu-id="79873-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="79873-134">Key of the entity.</span></span> <span data-ttu-id="79873-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-136">displayName</span><span class="sxs-lookup"><span data-stu-id="79873-136">displayName</span></span>|<span data-ttu-id="79873-137">String</span><span class="sxs-lookup"><span data-stu-id="79873-137">String</span></span>|<span data-ttu-id="79873-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="79873-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="79873-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-140">description</span><span class="sxs-lookup"><span data-stu-id="79873-140">description</span></span>|<span data-ttu-id="79873-141">String</span><span class="sxs-lookup"><span data-stu-id="79873-141">String</span></span>|<span data-ttu-id="79873-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="79873-142">The description of the app.</span></span> <span data-ttu-id="79873-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-144">publisher</span><span class="sxs-lookup"><span data-stu-id="79873-144">publisher</span></span>|<span data-ttu-id="79873-145">String</span><span class="sxs-lookup"><span data-stu-id="79873-145">String</span></span>|<span data-ttu-id="79873-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="79873-146">The publisher of the app.</span></span> <span data-ttu-id="79873-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="79873-148">largeIcon</span></span>|[<span data-ttu-id="79873-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="79873-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="79873-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="79873-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="79873-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79873-152">createdDateTime</span></span>|<span data-ttu-id="79873-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79873-153">DateTimeOffset</span></span>|<span data-ttu-id="79873-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="79873-154">The date and time the app was created.</span></span> <span data-ttu-id="79873-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79873-156">lastModifiedDateTime</span></span>|<span data-ttu-id="79873-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79873-157">DateTimeOffset</span></span>|<span data-ttu-id="79873-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="79873-158">The date and time the app was last modified.</span></span> <span data-ttu-id="79873-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="79873-160">isFeatured</span></span>|<span data-ttu-id="79873-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="79873-161">Boolean</span></span>|<span data-ttu-id="79873-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="79873-163">privacyInformationUrl</span></span>|<span data-ttu-id="79873-164">String</span><span class="sxs-lookup"><span data-stu-id="79873-164">String</span></span>|<span data-ttu-id="79873-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="79873-165">The privacy statement Url.</span></span> <span data-ttu-id="79873-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="79873-167">informationUrl</span></span>|<span data-ttu-id="79873-168">String</span><span class="sxs-lookup"><span data-stu-id="79873-168">String</span></span>|<span data-ttu-id="79873-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="79873-169">The more information Url.</span></span> <span data-ttu-id="79873-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-171">owner</span><span class="sxs-lookup"><span data-stu-id="79873-171">owner</span></span>|<span data-ttu-id="79873-172">字符串</span><span class="sxs-lookup"><span data-stu-id="79873-172">String</span></span>|<span data-ttu-id="79873-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="79873-173">The owner of the app.</span></span> <span data-ttu-id="79873-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-175">developer</span><span class="sxs-lookup"><span data-stu-id="79873-175">developer</span></span>|<span data-ttu-id="79873-176">String</span><span class="sxs-lookup"><span data-stu-id="79873-176">String</span></span>|<span data-ttu-id="79873-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="79873-177">The developer of the app.</span></span> <span data-ttu-id="79873-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-179">notes</span><span class="sxs-lookup"><span data-stu-id="79873-179">notes</span></span>|<span data-ttu-id="79873-180">String</span><span class="sxs-lookup"><span data-stu-id="79873-180">String</span></span>|<span data-ttu-id="79873-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="79873-181">Notes for the app.</span></span> <span data-ttu-id="79873-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="79873-183">uploadState</span></span>|<span data-ttu-id="79873-184">Int32</span><span class="sxs-lookup"><span data-stu-id="79873-184">Int32</span></span>|<span data-ttu-id="79873-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="79873-185">The upload state.</span></span> <span data-ttu-id="79873-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="79873-187">publishingState</span></span>|[<span data-ttu-id="79873-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="79873-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="79873-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="79873-189">The publishing state for the app.</span></span> <span data-ttu-id="79873-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="79873-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="79873-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="79873-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="79873-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="79873-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="79873-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="79873-193">isAssigned</span></span>|<span data-ttu-id="79873-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="79873-194">Boolean</span></span>|<span data-ttu-id="79873-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="79873-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="79873-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="79873-197">roleScopeTagIds</span></span>|<span data-ttu-id="79873-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="79873-198">String collection</span></span>|<span data-ttu-id="79873-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="79873-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="79873-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="79873-201">dependentAppCount</span></span>|<span data-ttu-id="79873-202">Int32</span><span class="sxs-lookup"><span data-stu-id="79873-202">Int32</span></span>|<span data-ttu-id="79873-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="79873-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="79873-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="79873-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="79873-205">committedContentVersion</span></span>|<span data-ttu-id="79873-206">String</span><span class="sxs-lookup"><span data-stu-id="79873-206">String</span></span>|<span data-ttu-id="79873-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="79873-207">The internal committed content version.</span></span> <span data-ttu-id="79873-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="79873-209">fileName</span><span class="sxs-lookup"><span data-stu-id="79873-209">fileName</span></span>|<span data-ttu-id="79873-210">String</span><span class="sxs-lookup"><span data-stu-id="79873-210">String</span></span>|<span data-ttu-id="79873-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="79873-211">The name of the main Lob application file.</span></span> <span data-ttu-id="79873-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="79873-213">size</span><span class="sxs-lookup"><span data-stu-id="79873-213">size</span></span>|<span data-ttu-id="79873-214">Int64</span><span class="sxs-lookup"><span data-stu-id="79873-214">Int64</span></span>|<span data-ttu-id="79873-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="79873-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="79873-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="79873-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="79873-217">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="79873-217">applicableArchitectures</span></span>|[<span data-ttu-id="79873-218">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="79873-218">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="79873-219">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="79873-219">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="79873-220">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="79873-220">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="79873-221">identityName</span><span class="sxs-lookup"><span data-stu-id="79873-221">identityName</span></span>|<span data-ttu-id="79873-222">String</span><span class="sxs-lookup"><span data-stu-id="79873-222">String</span></span>|<span data-ttu-id="79873-223">标识名称。</span><span class="sxs-lookup"><span data-stu-id="79873-223">The Identity Name.</span></span>|
|<span data-ttu-id="79873-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="79873-224">identityPublisherHash</span></span>|<span data-ttu-id="79873-225">String</span><span class="sxs-lookup"><span data-stu-id="79873-225">String</span></span>|<span data-ttu-id="79873-226">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="79873-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="79873-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="79873-227">identityResourceIdentifier</span></span>|<span data-ttu-id="79873-228">String</span><span class="sxs-lookup"><span data-stu-id="79873-228">String</span></span>|<span data-ttu-id="79873-229">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="79873-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="79873-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="79873-230">isBundle</span></span>|<span data-ttu-id="79873-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="79873-231">Boolean</span></span>|<span data-ttu-id="79873-232">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="79873-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="79873-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="79873-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="79873-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="79873-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="79873-235">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="79873-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="79873-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="79873-236">identityVersion</span></span>|<span data-ttu-id="79873-237">String</span><span class="sxs-lookup"><span data-stu-id="79873-237">String</span></span>|<span data-ttu-id="79873-238">标识版本。</span><span class="sxs-lookup"><span data-stu-id="79873-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="79873-239">响应</span><span class="sxs-lookup"><span data-stu-id="79873-239">Response</span></span>
<span data-ttu-id="79873-240">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsAppX](../resources/intune-apps-windowsappx.md)对象。</span><span class="sxs-lookup"><span data-stu-id="79873-240">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79873-241">示例</span><span class="sxs-lookup"><span data-stu-id="79873-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="79873-242">请求</span><span class="sxs-lookup"><span data-stu-id="79873-242">Request</span></span>
<span data-ttu-id="79873-243">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79873-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1367

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
  "dependentAppCount": 1,
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

### <a name="response"></a><span data-ttu-id="79873-244">响应</span><span class="sxs-lookup"><span data-stu-id="79873-244">Response</span></span>
<span data-ttu-id="79873-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="79873-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1539

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
  "dependentAppCount": 1,
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





