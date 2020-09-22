---
title: 创建 win32LobApp
description: 创建新的 win32LobApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c903de1e1f2bec92c255d29878eac06d38f4428c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080041"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="29399-103">创建 win32LobApp</span><span class="sxs-lookup"><span data-stu-id="29399-103">Create win32LobApp</span></span>

<span data-ttu-id="29399-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29399-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29399-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29399-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29399-106">创建新的 [win32LobApp](../resources/intune-apps-win32lobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29399-106">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29399-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="29399-107">Prerequisites</span></span>
<span data-ttu-id="29399-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29399-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29399-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="29399-110">Permission type</span></span>|<span data-ttu-id="29399-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="29399-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29399-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29399-112">Delegated (work or school account)</span></span>|<span data-ttu-id="29399-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29399-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="29399-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29399-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29399-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="29399-115">Not supported.</span></span>|
|<span data-ttu-id="29399-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="29399-116">Application</span></span>|<span data-ttu-id="29399-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29399-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29399-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29399-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="29399-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="29399-119">Request headers</span></span>
|<span data-ttu-id="29399-120">标头</span><span class="sxs-lookup"><span data-stu-id="29399-120">Header</span></span>|<span data-ttu-id="29399-121">值</span><span class="sxs-lookup"><span data-stu-id="29399-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29399-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="29399-122">Authorization</span></span>|<span data-ttu-id="29399-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="29399-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29399-124">接受</span><span class="sxs-lookup"><span data-stu-id="29399-124">Accept</span></span>|<span data-ttu-id="29399-125">application/json</span><span class="sxs-lookup"><span data-stu-id="29399-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29399-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="29399-126">Request body</span></span>
<span data-ttu-id="29399-127">在请求正文中，提供 win32LobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29399-127">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="29399-128">下表显示创建 win32LobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="29399-128">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="29399-129">属性</span><span class="sxs-lookup"><span data-stu-id="29399-129">Property</span></span>|<span data-ttu-id="29399-130">类型</span><span class="sxs-lookup"><span data-stu-id="29399-130">Type</span></span>|<span data-ttu-id="29399-131">说明</span><span class="sxs-lookup"><span data-stu-id="29399-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29399-132">id</span><span class="sxs-lookup"><span data-stu-id="29399-132">id</span></span>|<span data-ttu-id="29399-133">String</span><span class="sxs-lookup"><span data-stu-id="29399-133">String</span></span>|<span data-ttu-id="29399-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="29399-134">Key of the entity.</span></span> <span data-ttu-id="29399-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29399-136">displayName</span><span class="sxs-lookup"><span data-stu-id="29399-136">displayName</span></span>|<span data-ttu-id="29399-137">String</span><span class="sxs-lookup"><span data-stu-id="29399-137">String</span></span>|<span data-ttu-id="29399-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="29399-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="29399-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29399-140">description</span><span class="sxs-lookup"><span data-stu-id="29399-140">description</span></span>|<span data-ttu-id="29399-141">String</span><span class="sxs-lookup"><span data-stu-id="29399-141">String</span></span>|<span data-ttu-id="29399-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="29399-142">The description of the app.</span></span> <span data-ttu-id="29399-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29399-144">publisher</span><span class="sxs-lookup"><span data-stu-id="29399-144">publisher</span></span>|<span data-ttu-id="29399-145">String</span><span class="sxs-lookup"><span data-stu-id="29399-145">String</span></span>|<span data-ttu-id="29399-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="29399-146">The publisher of the app.</span></span> <span data-ttu-id="29399-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29399-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="29399-148">largeIcon</span></span>|[<span data-ttu-id="29399-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="29399-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="29399-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="29399-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="29399-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29399-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29399-152">createdDateTime</span></span>|<span data-ttu-id="29399-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29399-153">DateTimeOffset</span></span>|<span data-ttu-id="29399-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="29399-154">The date and time the app was created.</span></span> <span data-ttu-id="29399-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29399-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29399-156">lastModifiedDateTime</span></span>|<span data-ttu-id="29399-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29399-157">DateTimeOffset</span></span>|<span data-ttu-id="29399-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="29399-158">The date and time the app was last modified.</span></span> <span data-ttu-id="29399-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29399-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="29399-160">isFeatured</span></span>|<span data-ttu-id="29399-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="29399-161">Boolean</span></span>|<span data-ttu-id="29399-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29399-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="29399-163">privacyInformationUrl</span></span>|<span data-ttu-id="29399-164">String</span><span class="sxs-lookup"><span data-stu-id="29399-164">String</span></span>|<span data-ttu-id="29399-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="29399-165">The privacy statement Url.</span></span> <span data-ttu-id="29399-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29399-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="29399-167">informationUrl</span></span>|<span data-ttu-id="29399-168">String</span><span class="sxs-lookup"><span data-stu-id="29399-168">String</span></span>|<span data-ttu-id="29399-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="29399-169">The more information Url.</span></span> <span data-ttu-id="29399-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29399-171">owner</span><span class="sxs-lookup"><span data-stu-id="29399-171">owner</span></span>|<span data-ttu-id="29399-172">String</span><span class="sxs-lookup"><span data-stu-id="29399-172">String</span></span>|<span data-ttu-id="29399-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="29399-173">The owner of the app.</span></span> <span data-ttu-id="29399-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29399-175">developer</span><span class="sxs-lookup"><span data-stu-id="29399-175">developer</span></span>|<span data-ttu-id="29399-176">String</span><span class="sxs-lookup"><span data-stu-id="29399-176">String</span></span>|<span data-ttu-id="29399-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="29399-177">The developer of the app.</span></span> <span data-ttu-id="29399-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29399-179">notes</span><span class="sxs-lookup"><span data-stu-id="29399-179">notes</span></span>|<span data-ttu-id="29399-180">String</span><span class="sxs-lookup"><span data-stu-id="29399-180">String</span></span>|<span data-ttu-id="29399-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="29399-181">Notes for the app.</span></span> <span data-ttu-id="29399-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="29399-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="29399-183">publishingState</span></span>|[<span data-ttu-id="29399-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="29399-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="29399-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="29399-185">The publishing state for the app.</span></span> <span data-ttu-id="29399-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="29399-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="29399-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="29399-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="29399-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="29399-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="29399-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="29399-189">committedContentVersion</span></span>|<span data-ttu-id="29399-190">String</span><span class="sxs-lookup"><span data-stu-id="29399-190">String</span></span>|<span data-ttu-id="29399-191">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="29399-191">The internal committed content version.</span></span> <span data-ttu-id="29399-192">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="29399-193">fileName</span><span class="sxs-lookup"><span data-stu-id="29399-193">fileName</span></span>|<span data-ttu-id="29399-194">String</span><span class="sxs-lookup"><span data-stu-id="29399-194">String</span></span>|<span data-ttu-id="29399-195">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="29399-195">The name of the main Lob application file.</span></span> <span data-ttu-id="29399-196">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="29399-197">size</span><span class="sxs-lookup"><span data-stu-id="29399-197">size</span></span>|<span data-ttu-id="29399-198">Int64</span><span class="sxs-lookup"><span data-stu-id="29399-198">Int64</span></span>|<span data-ttu-id="29399-199">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="29399-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="29399-200">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="29399-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="29399-201">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="29399-201">installCommandLine</span></span>|<span data-ttu-id="29399-202">String</span><span class="sxs-lookup"><span data-stu-id="29399-202">String</span></span>|<span data-ttu-id="29399-203">要安装此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="29399-203">The command line to install this app</span></span>|
|<span data-ttu-id="29399-204">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="29399-204">uninstallCommandLine</span></span>|<span data-ttu-id="29399-205">String</span><span class="sxs-lookup"><span data-stu-id="29399-205">String</span></span>|<span data-ttu-id="29399-206">要卸载此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="29399-206">The command line to uninstall this app</span></span>|
|<span data-ttu-id="29399-207">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="29399-207">applicableArchitectures</span></span>|[<span data-ttu-id="29399-208">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="29399-208">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="29399-209">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="29399-209">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="29399-210">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。</span><span class="sxs-lookup"><span data-stu-id="29399-210">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="29399-211">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="29399-211">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="29399-212">Int32</span><span class="sxs-lookup"><span data-stu-id="29399-212">Int32</span></span>|<span data-ttu-id="29399-213">安装此应用程序所需的最小可用磁盘空间的值。</span><span class="sxs-lookup"><span data-stu-id="29399-213">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="29399-214">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="29399-214">minimumMemoryInMB</span></span>|<span data-ttu-id="29399-215">Int32</span><span class="sxs-lookup"><span data-stu-id="29399-215">Int32</span></span>|<span data-ttu-id="29399-216">安装此应用程序所需的最小物理内存的值。</span><span class="sxs-lookup"><span data-stu-id="29399-216">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="29399-217">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="29399-217">minimumNumberOfProcessors</span></span>|<span data-ttu-id="29399-218">Int32</span><span class="sxs-lookup"><span data-stu-id="29399-218">Int32</span></span>|<span data-ttu-id="29399-219">安装此应用程序所需的最小处理器数的值。</span><span class="sxs-lookup"><span data-stu-id="29399-219">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="29399-220">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="29399-220">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="29399-221">Int32</span><span class="sxs-lookup"><span data-stu-id="29399-221">Int32</span></span>|<span data-ttu-id="29399-222">安装此应用程序所需的最低 CPU 速度的值。</span><span class="sxs-lookup"><span data-stu-id="29399-222">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="29399-223">规则</span><span class="sxs-lookup"><span data-stu-id="29399-223">rules</span></span>|<span data-ttu-id="29399-224">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="29399-224">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="29399-225">此应用程序的检测和要求规则。</span><span class="sxs-lookup"><span data-stu-id="29399-225">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="29399-226">installExperience</span><span class="sxs-lookup"><span data-stu-id="29399-226">installExperience</span></span>|[<span data-ttu-id="29399-227">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="29399-227">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="29399-228">此应用的安装体验。</span><span class="sxs-lookup"><span data-stu-id="29399-228">The install experience for this app.</span></span>|
|<span data-ttu-id="29399-229">returnCodes</span><span class="sxs-lookup"><span data-stu-id="29399-229">returnCodes</span></span>|<span data-ttu-id="29399-230">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) 集合</span><span class="sxs-lookup"><span data-stu-id="29399-230">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="29399-231">用于安装后行为的返回代码。</span><span class="sxs-lookup"><span data-stu-id="29399-231">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="29399-232">msiInformation</span><span class="sxs-lookup"><span data-stu-id="29399-232">msiInformation</span></span>|[<span data-ttu-id="29399-233">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="29399-233">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="29399-234">如果此 Win32 应用是 MSI 应用程序，则为 MSI 详细信息。</span><span class="sxs-lookup"><span data-stu-id="29399-234">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="29399-235">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="29399-235">setupFilePath</span></span>|<span data-ttu-id="29399-236">String</span><span class="sxs-lookup"><span data-stu-id="29399-236">String</span></span>|<span data-ttu-id="29399-237">加密的 Win32LobApp 包中的安装程序文件的相对路径。</span><span class="sxs-lookup"><span data-stu-id="29399-237">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="29399-238">minimumSupportedWindowsRelease</span><span class="sxs-lookup"><span data-stu-id="29399-238">minimumSupportedWindowsRelease</span></span>|<span data-ttu-id="29399-239">String</span><span class="sxs-lookup"><span data-stu-id="29399-239">String</span></span>|<span data-ttu-id="29399-240">支持的最小 windows 版本的值。</span><span class="sxs-lookup"><span data-stu-id="29399-240">The value for the minimum supported windows release.</span></span>|



## <a name="response"></a><span data-ttu-id="29399-241">响应</span><span class="sxs-lookup"><span data-stu-id="29399-241">Response</span></span>
<span data-ttu-id="29399-242">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [win32LobApp](../resources/intune-apps-win32lobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29399-242">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29399-243">示例</span><span class="sxs-lookup"><span data-stu-id="29399-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="29399-244">请求</span><span class="sxs-lookup"><span data-stu-id="29399-244">Request</span></span>
<span data-ttu-id="29399-245">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29399-245">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="29399-246">响应</span><span class="sxs-lookup"><span data-stu-id="29399-246">Response</span></span>
<span data-ttu-id="29399-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29399-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






