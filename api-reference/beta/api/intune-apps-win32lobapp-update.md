---
title: 更新 win32LobApp
description: 更新 win32LobApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2f528f854195af119a4a3c7404d017943bd1701
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970917"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="86534-103">更新 win32LobApp</span><span class="sxs-lookup"><span data-stu-id="86534-103">Update win32LobApp</span></span>

> <span data-ttu-id="86534-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="86534-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86534-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="86534-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86534-106">更新[win32LobApp](../resources/intune-apps-win32lobapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="86534-106">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86534-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="86534-107">Prerequisites</span></span>
<span data-ttu-id="86534-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86534-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86534-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="86534-110">Permission type</span></span>|<span data-ttu-id="86534-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="86534-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86534-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86534-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86534-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86534-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="86534-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86534-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86534-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="86534-115">Not supported.</span></span>|
|<span data-ttu-id="86534-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="86534-116">Application</span></span>|<span data-ttu-id="86534-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="86534-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86534-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86534-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="86534-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="86534-119">Request headers</span></span>
|<span data-ttu-id="86534-120">标头</span><span class="sxs-lookup"><span data-stu-id="86534-120">Header</span></span>|<span data-ttu-id="86534-121">值</span><span class="sxs-lookup"><span data-stu-id="86534-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86534-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86534-122">Authorization</span></span>|<span data-ttu-id="86534-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="86534-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86534-124">接受</span><span class="sxs-lookup"><span data-stu-id="86534-124">Accept</span></span>|<span data-ttu-id="86534-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86534-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86534-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="86534-126">Request body</span></span>
<span data-ttu-id="86534-127">在请求正文中, 提供[win32LobApp](../resources/intune-apps-win32lobapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86534-127">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="86534-128">下表显示创建[win32LobApp](../resources/intune-apps-win32lobapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="86534-128">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="86534-129">属性</span><span class="sxs-lookup"><span data-stu-id="86534-129">Property</span></span>|<span data-ttu-id="86534-130">类型</span><span class="sxs-lookup"><span data-stu-id="86534-130">Type</span></span>|<span data-ttu-id="86534-131">说明</span><span class="sxs-lookup"><span data-stu-id="86534-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86534-132">id</span><span class="sxs-lookup"><span data-stu-id="86534-132">id</span></span>|<span data-ttu-id="86534-133">String</span><span class="sxs-lookup"><span data-stu-id="86534-133">String</span></span>|<span data-ttu-id="86534-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="86534-134">Key of the entity.</span></span> <span data-ttu-id="86534-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-136">displayName</span><span class="sxs-lookup"><span data-stu-id="86534-136">displayName</span></span>|<span data-ttu-id="86534-137">String</span><span class="sxs-lookup"><span data-stu-id="86534-137">String</span></span>|<span data-ttu-id="86534-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="86534-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="86534-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-140">description</span><span class="sxs-lookup"><span data-stu-id="86534-140">description</span></span>|<span data-ttu-id="86534-141">String</span><span class="sxs-lookup"><span data-stu-id="86534-141">String</span></span>|<span data-ttu-id="86534-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="86534-142">The description of the app.</span></span> <span data-ttu-id="86534-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-144">publisher</span><span class="sxs-lookup"><span data-stu-id="86534-144">publisher</span></span>|<span data-ttu-id="86534-145">String</span><span class="sxs-lookup"><span data-stu-id="86534-145">String</span></span>|<span data-ttu-id="86534-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="86534-146">The publisher of the app.</span></span> <span data-ttu-id="86534-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="86534-148">largeIcon</span></span>|[<span data-ttu-id="86534-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="86534-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="86534-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="86534-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="86534-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="86534-152">createdDateTime</span></span>|<span data-ttu-id="86534-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86534-153">DateTimeOffset</span></span>|<span data-ttu-id="86534-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="86534-154">The date and time the app was created.</span></span> <span data-ttu-id="86534-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="86534-156">lastModifiedDateTime</span></span>|<span data-ttu-id="86534-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86534-157">DateTimeOffset</span></span>|<span data-ttu-id="86534-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="86534-158">The date and time the app was last modified.</span></span> <span data-ttu-id="86534-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="86534-160">isFeatured</span></span>|<span data-ttu-id="86534-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="86534-161">Boolean</span></span>|<span data-ttu-id="86534-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="86534-163">privacyInformationUrl</span></span>|<span data-ttu-id="86534-164">String</span><span class="sxs-lookup"><span data-stu-id="86534-164">String</span></span>|<span data-ttu-id="86534-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="86534-165">The privacy statement Url.</span></span> <span data-ttu-id="86534-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="86534-167">informationUrl</span></span>|<span data-ttu-id="86534-168">String</span><span class="sxs-lookup"><span data-stu-id="86534-168">String</span></span>|<span data-ttu-id="86534-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="86534-169">The more information Url.</span></span> <span data-ttu-id="86534-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-171">owner</span><span class="sxs-lookup"><span data-stu-id="86534-171">owner</span></span>|<span data-ttu-id="86534-172">字符串</span><span class="sxs-lookup"><span data-stu-id="86534-172">String</span></span>|<span data-ttu-id="86534-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="86534-173">The owner of the app.</span></span> <span data-ttu-id="86534-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-175">developer</span><span class="sxs-lookup"><span data-stu-id="86534-175">developer</span></span>|<span data-ttu-id="86534-176">String</span><span class="sxs-lookup"><span data-stu-id="86534-176">String</span></span>|<span data-ttu-id="86534-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="86534-177">The developer of the app.</span></span> <span data-ttu-id="86534-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-179">notes</span><span class="sxs-lookup"><span data-stu-id="86534-179">notes</span></span>|<span data-ttu-id="86534-180">String</span><span class="sxs-lookup"><span data-stu-id="86534-180">String</span></span>|<span data-ttu-id="86534-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="86534-181">Notes for the app.</span></span> <span data-ttu-id="86534-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="86534-183">uploadState</span></span>|<span data-ttu-id="86534-184">Int32</span><span class="sxs-lookup"><span data-stu-id="86534-184">Int32</span></span>|<span data-ttu-id="86534-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="86534-185">The upload state.</span></span> <span data-ttu-id="86534-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="86534-187">publishingState</span></span>|[<span data-ttu-id="86534-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="86534-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="86534-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="86534-189">The publishing state for the app.</span></span> <span data-ttu-id="86534-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="86534-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="86534-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="86534-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="86534-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="86534-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="86534-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="86534-193">isAssigned</span></span>|<span data-ttu-id="86534-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="86534-194">Boolean</span></span>|<span data-ttu-id="86534-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="86534-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="86534-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="86534-197">roleScopeTagIds</span></span>|<span data-ttu-id="86534-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="86534-198">String collection</span></span>|<span data-ttu-id="86534-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="86534-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="86534-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="86534-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="86534-201">committedContentVersion</span></span>|<span data-ttu-id="86534-202">String</span><span class="sxs-lookup"><span data-stu-id="86534-202">String</span></span>|<span data-ttu-id="86534-203">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="86534-203">The internal committed content version.</span></span> <span data-ttu-id="86534-204">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="86534-205">fileName</span><span class="sxs-lookup"><span data-stu-id="86534-205">fileName</span></span>|<span data-ttu-id="86534-206">String</span><span class="sxs-lookup"><span data-stu-id="86534-206">String</span></span>|<span data-ttu-id="86534-207">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="86534-207">The name of the main Lob application file.</span></span> <span data-ttu-id="86534-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="86534-209">size</span><span class="sxs-lookup"><span data-stu-id="86534-209">size</span></span>|<span data-ttu-id="86534-210">Int64</span><span class="sxs-lookup"><span data-stu-id="86534-210">Int64</span></span>|<span data-ttu-id="86534-211">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="86534-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="86534-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="86534-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="86534-213">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="86534-213">installCommandLine</span></span>|<span data-ttu-id="86534-214">String</span><span class="sxs-lookup"><span data-stu-id="86534-214">String</span></span>|<span data-ttu-id="86534-215">要安装此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="86534-215">The command line to install this app</span></span>|
|<span data-ttu-id="86534-216">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="86534-216">uninstallCommandLine</span></span>|<span data-ttu-id="86534-217">String</span><span class="sxs-lookup"><span data-stu-id="86534-217">String</span></span>|<span data-ttu-id="86534-218">要卸载此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="86534-218">The command line to uninstall this app</span></span>|
|<span data-ttu-id="86534-219">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="86534-219">applicableArchitectures</span></span>|[<span data-ttu-id="86534-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="86534-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="86534-221">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="86534-221">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="86534-222">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="86534-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="86534-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="86534-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="86534-224">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="86534-224">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="86534-225">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="86534-225">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="86534-226">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="86534-226">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="86534-227">Int32</span><span class="sxs-lookup"><span data-stu-id="86534-227">Int32</span></span>|<span data-ttu-id="86534-228">安装此应用程序所需的最小可用磁盘空间的值。</span><span class="sxs-lookup"><span data-stu-id="86534-228">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="86534-229">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="86534-229">minimumMemoryInMB</span></span>|<span data-ttu-id="86534-230">Int32</span><span class="sxs-lookup"><span data-stu-id="86534-230">Int32</span></span>|<span data-ttu-id="86534-231">安装此应用程序所需的最小物理内存的值。</span><span class="sxs-lookup"><span data-stu-id="86534-231">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="86534-232">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="86534-232">minimumNumberOfProcessors</span></span>|<span data-ttu-id="86534-233">Int32</span><span class="sxs-lookup"><span data-stu-id="86534-233">Int32</span></span>|<span data-ttu-id="86534-234">安装此应用程序所需的最小处理器数的值。</span><span class="sxs-lookup"><span data-stu-id="86534-234">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="86534-235">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="86534-235">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="86534-236">Int32</span><span class="sxs-lookup"><span data-stu-id="86534-236">Int32</span></span>|<span data-ttu-id="86534-237">安装此应用程序所需的最低 CPU 速度的值。</span><span class="sxs-lookup"><span data-stu-id="86534-237">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="86534-238">detectionRules</span><span class="sxs-lookup"><span data-stu-id="86534-238">detectionRules</span></span>|<span data-ttu-id="86534-239">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)集合</span><span class="sxs-lookup"><span data-stu-id="86534-239">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="86534-240">检测到 Win32 业务线 (LoB) 应用程序的检测规则。</span><span class="sxs-lookup"><span data-stu-id="86534-240">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="86534-241">installExperience</span><span class="sxs-lookup"><span data-stu-id="86534-241">installExperience</span></span>|[<span data-ttu-id="86534-242">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="86534-242">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="86534-243">此应用的安装体验。</span><span class="sxs-lookup"><span data-stu-id="86534-243">The install experience for this app.</span></span>|
|<span data-ttu-id="86534-244">returnCodes</span><span class="sxs-lookup"><span data-stu-id="86534-244">returnCodes</span></span>|<span data-ttu-id="86534-245">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)集合</span><span class="sxs-lookup"><span data-stu-id="86534-245">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="86534-246">用于安装后行为的返回代码。</span><span class="sxs-lookup"><span data-stu-id="86534-246">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="86534-247">msiInformation</span><span class="sxs-lookup"><span data-stu-id="86534-247">msiInformation</span></span>|[<span data-ttu-id="86534-248">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="86534-248">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="86534-249">如果此 Win32 应用是 msi 应用程序, 则为 msi 详细信息。</span><span class="sxs-lookup"><span data-stu-id="86534-249">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="86534-250">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="86534-250">setupFilePath</span></span>|<span data-ttu-id="86534-251">String</span><span class="sxs-lookup"><span data-stu-id="86534-251">String</span></span>|<span data-ttu-id="86534-252">加密的 Win32LobApp 包中的安装程序文件的相对路径。</span><span class="sxs-lookup"><span data-stu-id="86534-252">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="86534-253">响应</span><span class="sxs-lookup"><span data-stu-id="86534-253">Response</span></span>
<span data-ttu-id="86534-254">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[win32LobApp](../resources/intune-apps-win32lobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="86534-254">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86534-255">示例</span><span class="sxs-lookup"><span data-stu-id="86534-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="86534-256">请求</span><span class="sxs-lookup"><span data-stu-id="86534-256">Request</span></span>
<span data-ttu-id="86534-257">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86534-257">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2364

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value"
}
```

### <a name="response"></a><span data-ttu-id="86534-258">响应</span><span class="sxs-lookup"><span data-stu-id="86534-258">Response</span></span>
<span data-ttu-id="86534-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86534-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2536

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value"
}
```




