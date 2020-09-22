---
title: 更新 win32LobApp
description: 更新 win32LobApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a0ff0313b13b7d3b2e094b4918fa68367051cf85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080037"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="ff945-103">更新 win32LobApp</span><span class="sxs-lookup"><span data-stu-id="ff945-103">Update win32LobApp</span></span>

<span data-ttu-id="ff945-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff945-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff945-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff945-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff945-106">更新 [win32LobApp](../resources/intune-apps-win32lobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ff945-106">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff945-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ff945-107">Prerequisites</span></span>
<span data-ttu-id="ff945-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff945-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff945-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff945-110">Permission type</span></span>|<span data-ttu-id="ff945-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ff945-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff945-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff945-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff945-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff945-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ff945-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff945-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff945-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff945-115">Not supported.</span></span>|
|<span data-ttu-id="ff945-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff945-116">Application</span></span>|<span data-ttu-id="ff945-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff945-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff945-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff945-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ff945-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff945-119">Request headers</span></span>
|<span data-ttu-id="ff945-120">标头</span><span class="sxs-lookup"><span data-stu-id="ff945-120">Header</span></span>|<span data-ttu-id="ff945-121">值</span><span class="sxs-lookup"><span data-stu-id="ff945-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff945-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff945-122">Authorization</span></span>|<span data-ttu-id="ff945-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ff945-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff945-124">接受</span><span class="sxs-lookup"><span data-stu-id="ff945-124">Accept</span></span>|<span data-ttu-id="ff945-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff945-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff945-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff945-126">Request body</span></span>
<span data-ttu-id="ff945-127">在请求正文中，提供 [win32LobApp](../resources/intune-apps-win32lobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff945-127">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="ff945-128">下表显示创建 [win32LobApp](../resources/intune-apps-win32lobapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ff945-128">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="ff945-129">属性</span><span class="sxs-lookup"><span data-stu-id="ff945-129">Property</span></span>|<span data-ttu-id="ff945-130">类型</span><span class="sxs-lookup"><span data-stu-id="ff945-130">Type</span></span>|<span data-ttu-id="ff945-131">说明</span><span class="sxs-lookup"><span data-stu-id="ff945-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff945-132">id</span><span class="sxs-lookup"><span data-stu-id="ff945-132">id</span></span>|<span data-ttu-id="ff945-133">String</span><span class="sxs-lookup"><span data-stu-id="ff945-133">String</span></span>|<span data-ttu-id="ff945-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ff945-134">Key of the entity.</span></span> <span data-ttu-id="ff945-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff945-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ff945-136">displayName</span></span>|<span data-ttu-id="ff945-137">String</span><span class="sxs-lookup"><span data-stu-id="ff945-137">String</span></span>|<span data-ttu-id="ff945-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="ff945-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ff945-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff945-140">description</span><span class="sxs-lookup"><span data-stu-id="ff945-140">description</span></span>|<span data-ttu-id="ff945-141">String</span><span class="sxs-lookup"><span data-stu-id="ff945-141">String</span></span>|<span data-ttu-id="ff945-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="ff945-142">The description of the app.</span></span> <span data-ttu-id="ff945-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff945-144">publisher</span><span class="sxs-lookup"><span data-stu-id="ff945-144">publisher</span></span>|<span data-ttu-id="ff945-145">String</span><span class="sxs-lookup"><span data-stu-id="ff945-145">String</span></span>|<span data-ttu-id="ff945-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="ff945-146">The publisher of the app.</span></span> <span data-ttu-id="ff945-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff945-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ff945-148">largeIcon</span></span>|[<span data-ttu-id="ff945-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ff945-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ff945-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="ff945-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ff945-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff945-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff945-152">createdDateTime</span></span>|<span data-ttu-id="ff945-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff945-153">DateTimeOffset</span></span>|<span data-ttu-id="ff945-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ff945-154">The date and time the app was created.</span></span> <span data-ttu-id="ff945-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff945-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff945-156">lastModifiedDateTime</span></span>|<span data-ttu-id="ff945-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff945-157">DateTimeOffset</span></span>|<span data-ttu-id="ff945-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ff945-158">The date and time the app was last modified.</span></span> <span data-ttu-id="ff945-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff945-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ff945-160">isFeatured</span></span>|<span data-ttu-id="ff945-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff945-161">Boolean</span></span>|<span data-ttu-id="ff945-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff945-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ff945-163">privacyInformationUrl</span></span>|<span data-ttu-id="ff945-164">String</span><span class="sxs-lookup"><span data-stu-id="ff945-164">String</span></span>|<span data-ttu-id="ff945-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="ff945-165">The privacy statement Url.</span></span> <span data-ttu-id="ff945-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff945-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ff945-167">informationUrl</span></span>|<span data-ttu-id="ff945-168">String</span><span class="sxs-lookup"><span data-stu-id="ff945-168">String</span></span>|<span data-ttu-id="ff945-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="ff945-169">The more information Url.</span></span> <span data-ttu-id="ff945-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff945-171">owner</span><span class="sxs-lookup"><span data-stu-id="ff945-171">owner</span></span>|<span data-ttu-id="ff945-172">String</span><span class="sxs-lookup"><span data-stu-id="ff945-172">String</span></span>|<span data-ttu-id="ff945-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="ff945-173">The owner of the app.</span></span> <span data-ttu-id="ff945-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff945-175">developer</span><span class="sxs-lookup"><span data-stu-id="ff945-175">developer</span></span>|<span data-ttu-id="ff945-176">String</span><span class="sxs-lookup"><span data-stu-id="ff945-176">String</span></span>|<span data-ttu-id="ff945-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="ff945-177">The developer of the app.</span></span> <span data-ttu-id="ff945-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff945-179">notes</span><span class="sxs-lookup"><span data-stu-id="ff945-179">notes</span></span>|<span data-ttu-id="ff945-180">String</span><span class="sxs-lookup"><span data-stu-id="ff945-180">String</span></span>|<span data-ttu-id="ff945-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="ff945-181">Notes for the app.</span></span> <span data-ttu-id="ff945-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ff945-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="ff945-183">publishingState</span></span>|[<span data-ttu-id="ff945-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ff945-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ff945-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="ff945-185">The publishing state for the app.</span></span> <span data-ttu-id="ff945-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="ff945-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ff945-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="ff945-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ff945-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="ff945-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ff945-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ff945-189">committedContentVersion</span></span>|<span data-ttu-id="ff945-190">String</span><span class="sxs-lookup"><span data-stu-id="ff945-190">String</span></span>|<span data-ttu-id="ff945-191">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="ff945-191">The internal committed content version.</span></span> <span data-ttu-id="ff945-192">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ff945-193">fileName</span><span class="sxs-lookup"><span data-stu-id="ff945-193">fileName</span></span>|<span data-ttu-id="ff945-194">String</span><span class="sxs-lookup"><span data-stu-id="ff945-194">String</span></span>|<span data-ttu-id="ff945-195">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="ff945-195">The name of the main Lob application file.</span></span> <span data-ttu-id="ff945-196">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ff945-197">size</span><span class="sxs-lookup"><span data-stu-id="ff945-197">size</span></span>|<span data-ttu-id="ff945-198">Int64</span><span class="sxs-lookup"><span data-stu-id="ff945-198">Int64</span></span>|<span data-ttu-id="ff945-199">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="ff945-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="ff945-200">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff945-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ff945-201">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="ff945-201">installCommandLine</span></span>|<span data-ttu-id="ff945-202">String</span><span class="sxs-lookup"><span data-stu-id="ff945-202">String</span></span>|<span data-ttu-id="ff945-203">要安装此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="ff945-203">The command line to install this app</span></span>|
|<span data-ttu-id="ff945-204">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="ff945-204">uninstallCommandLine</span></span>|<span data-ttu-id="ff945-205">String</span><span class="sxs-lookup"><span data-stu-id="ff945-205">String</span></span>|<span data-ttu-id="ff945-206">要卸载此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="ff945-206">The command line to uninstall this app</span></span>|
|<span data-ttu-id="ff945-207">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="ff945-207">applicableArchitectures</span></span>|[<span data-ttu-id="ff945-208">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="ff945-208">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="ff945-209">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="ff945-209">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="ff945-210">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。</span><span class="sxs-lookup"><span data-stu-id="ff945-210">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="ff945-211">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="ff945-211">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="ff945-212">Int32</span><span class="sxs-lookup"><span data-stu-id="ff945-212">Int32</span></span>|<span data-ttu-id="ff945-213">安装此应用程序所需的最小可用磁盘空间的值。</span><span class="sxs-lookup"><span data-stu-id="ff945-213">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="ff945-214">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="ff945-214">minimumMemoryInMB</span></span>|<span data-ttu-id="ff945-215">Int32</span><span class="sxs-lookup"><span data-stu-id="ff945-215">Int32</span></span>|<span data-ttu-id="ff945-216">安装此应用程序所需的最小物理内存的值。</span><span class="sxs-lookup"><span data-stu-id="ff945-216">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="ff945-217">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="ff945-217">minimumNumberOfProcessors</span></span>|<span data-ttu-id="ff945-218">Int32</span><span class="sxs-lookup"><span data-stu-id="ff945-218">Int32</span></span>|<span data-ttu-id="ff945-219">安装此应用程序所需的最小处理器数的值。</span><span class="sxs-lookup"><span data-stu-id="ff945-219">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="ff945-220">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="ff945-220">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="ff945-221">Int32</span><span class="sxs-lookup"><span data-stu-id="ff945-221">Int32</span></span>|<span data-ttu-id="ff945-222">安装此应用程序所需的最低 CPU 速度的值。</span><span class="sxs-lookup"><span data-stu-id="ff945-222">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="ff945-223">规则</span><span class="sxs-lookup"><span data-stu-id="ff945-223">rules</span></span>|<span data-ttu-id="ff945-224">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff945-224">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="ff945-225">此应用程序的检测和要求规则。</span><span class="sxs-lookup"><span data-stu-id="ff945-225">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="ff945-226">installExperience</span><span class="sxs-lookup"><span data-stu-id="ff945-226">installExperience</span></span>|[<span data-ttu-id="ff945-227">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="ff945-227">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="ff945-228">此应用的安装体验。</span><span class="sxs-lookup"><span data-stu-id="ff945-228">The install experience for this app.</span></span>|
|<span data-ttu-id="ff945-229">returnCodes</span><span class="sxs-lookup"><span data-stu-id="ff945-229">returnCodes</span></span>|<span data-ttu-id="ff945-230">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ff945-230">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="ff945-231">用于安装后行为的返回代码。</span><span class="sxs-lookup"><span data-stu-id="ff945-231">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="ff945-232">msiInformation</span><span class="sxs-lookup"><span data-stu-id="ff945-232">msiInformation</span></span>|[<span data-ttu-id="ff945-233">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="ff945-233">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="ff945-234">如果此 Win32 应用是 MSI 应用程序，则为 MSI 详细信息。</span><span class="sxs-lookup"><span data-stu-id="ff945-234">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="ff945-235">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="ff945-235">setupFilePath</span></span>|<span data-ttu-id="ff945-236">String</span><span class="sxs-lookup"><span data-stu-id="ff945-236">String</span></span>|<span data-ttu-id="ff945-237">加密的 Win32LobApp 包中的安装程序文件的相对路径。</span><span class="sxs-lookup"><span data-stu-id="ff945-237">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="ff945-238">minimumSupportedWindowsRelease</span><span class="sxs-lookup"><span data-stu-id="ff945-238">minimumSupportedWindowsRelease</span></span>|<span data-ttu-id="ff945-239">String</span><span class="sxs-lookup"><span data-stu-id="ff945-239">String</span></span>|<span data-ttu-id="ff945-240">支持的最小 windows 版本的值。</span><span class="sxs-lookup"><span data-stu-id="ff945-240">The value for the minimum supported windows release.</span></span>|



## <a name="response"></a><span data-ttu-id="ff945-241">响应</span><span class="sxs-lookup"><span data-stu-id="ff945-241">Response</span></span>
<span data-ttu-id="ff945-242">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [win32LobApp](../resources/intune-apps-win32lobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ff945-242">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff945-243">示例</span><span class="sxs-lookup"><span data-stu-id="ff945-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff945-244">请求</span><span class="sxs-lookup"><span data-stu-id="ff945-244">Request</span></span>
<span data-ttu-id="ff945-245">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ff945-245">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2134

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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
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
  "setupFilePath": "Setup File Path value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```

### <a name="response"></a><span data-ttu-id="ff945-246">响应</span><span class="sxs-lookup"><span data-stu-id="ff945-246">Response</span></span>
<span data-ttu-id="ff945-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ff945-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2306

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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
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
  "setupFilePath": "Setup File Path value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```






