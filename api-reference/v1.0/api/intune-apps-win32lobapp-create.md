---
title: 创建 win32LobApp
description: 创建新的 win32LobApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4720cd7b77ce32e059a5e2754534efee619cfd79
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756741"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="afa67-103">创建 win32LobApp</span><span class="sxs-lookup"><span data-stu-id="afa67-103">Create win32LobApp</span></span>

<span data-ttu-id="afa67-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afa67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afa67-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="afa67-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afa67-106">创建新的 [win32LobApp](../resources/intune-apps-win32lobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="afa67-106">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afa67-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="afa67-107">Prerequisites</span></span>
<span data-ttu-id="afa67-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="afa67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afa67-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="afa67-110">Permission type</span></span>|<span data-ttu-id="afa67-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="afa67-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afa67-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="afa67-112">Delegated (work or school account)</span></span>|<span data-ttu-id="afa67-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afa67-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="afa67-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="afa67-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afa67-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="afa67-115">Not supported.</span></span>|
|<span data-ttu-id="afa67-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="afa67-116">Application</span></span>|<span data-ttu-id="afa67-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afa67-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="afa67-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="afa67-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="afa67-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="afa67-119">Request headers</span></span>
|<span data-ttu-id="afa67-120">标头</span><span class="sxs-lookup"><span data-stu-id="afa67-120">Header</span></span>|<span data-ttu-id="afa67-121">值</span><span class="sxs-lookup"><span data-stu-id="afa67-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afa67-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="afa67-122">Authorization</span></span>|<span data-ttu-id="afa67-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="afa67-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afa67-124">接受</span><span class="sxs-lookup"><span data-stu-id="afa67-124">Accept</span></span>|<span data-ttu-id="afa67-125">application/json</span><span class="sxs-lookup"><span data-stu-id="afa67-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afa67-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="afa67-126">Request body</span></span>
<span data-ttu-id="afa67-127">在请求正文中，提供 win32LobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="afa67-127">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="afa67-128">下表显示创建 win32LobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="afa67-128">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="afa67-129">属性</span><span class="sxs-lookup"><span data-stu-id="afa67-129">Property</span></span>|<span data-ttu-id="afa67-130">类型</span><span class="sxs-lookup"><span data-stu-id="afa67-130">Type</span></span>|<span data-ttu-id="afa67-131">说明</span><span class="sxs-lookup"><span data-stu-id="afa67-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afa67-132">id</span><span class="sxs-lookup"><span data-stu-id="afa67-132">id</span></span>|<span data-ttu-id="afa67-133">String</span><span class="sxs-lookup"><span data-stu-id="afa67-133">String</span></span>|<span data-ttu-id="afa67-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="afa67-134">Key of the entity.</span></span> <span data-ttu-id="afa67-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="afa67-136">displayName</span><span class="sxs-lookup"><span data-stu-id="afa67-136">displayName</span></span>|<span data-ttu-id="afa67-137">String</span><span class="sxs-lookup"><span data-stu-id="afa67-137">String</span></span>|<span data-ttu-id="afa67-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="afa67-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="afa67-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="afa67-140">说明</span><span class="sxs-lookup"><span data-stu-id="afa67-140">description</span></span>|<span data-ttu-id="afa67-141">String</span><span class="sxs-lookup"><span data-stu-id="afa67-141">String</span></span>|<span data-ttu-id="afa67-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="afa67-142">The description of the app.</span></span> <span data-ttu-id="afa67-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="afa67-144">publisher</span><span class="sxs-lookup"><span data-stu-id="afa67-144">publisher</span></span>|<span data-ttu-id="afa67-145">String</span><span class="sxs-lookup"><span data-stu-id="afa67-145">String</span></span>|<span data-ttu-id="afa67-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="afa67-146">The publisher of the app.</span></span> <span data-ttu-id="afa67-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="afa67-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="afa67-148">largeIcon</span></span>|[<span data-ttu-id="afa67-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="afa67-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="afa67-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="afa67-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="afa67-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="afa67-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="afa67-152">createdDateTime</span></span>|<span data-ttu-id="afa67-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afa67-153">DateTimeOffset</span></span>|<span data-ttu-id="afa67-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="afa67-154">The date and time the app was created.</span></span> <span data-ttu-id="afa67-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="afa67-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="afa67-156">lastModifiedDateTime</span></span>|<span data-ttu-id="afa67-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afa67-157">DateTimeOffset</span></span>|<span data-ttu-id="afa67-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="afa67-158">The date and time the app was last modified.</span></span> <span data-ttu-id="afa67-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="afa67-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="afa67-160">isFeatured</span></span>|<span data-ttu-id="afa67-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="afa67-161">Boolean</span></span>|<span data-ttu-id="afa67-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="afa67-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="afa67-163">privacyInformationUrl</span></span>|<span data-ttu-id="afa67-164">String</span><span class="sxs-lookup"><span data-stu-id="afa67-164">String</span></span>|<span data-ttu-id="afa67-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="afa67-165">The privacy statement Url.</span></span> <span data-ttu-id="afa67-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="afa67-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="afa67-167">informationUrl</span></span>|<span data-ttu-id="afa67-168">String</span><span class="sxs-lookup"><span data-stu-id="afa67-168">String</span></span>|<span data-ttu-id="afa67-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="afa67-169">The more information Url.</span></span> <span data-ttu-id="afa67-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="afa67-171">所有者</span><span class="sxs-lookup"><span data-stu-id="afa67-171">owner</span></span>|<span data-ttu-id="afa67-172">String</span><span class="sxs-lookup"><span data-stu-id="afa67-172">String</span></span>|<span data-ttu-id="afa67-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="afa67-173">The owner of the app.</span></span> <span data-ttu-id="afa67-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="afa67-175">developer</span><span class="sxs-lookup"><span data-stu-id="afa67-175">developer</span></span>|<span data-ttu-id="afa67-176">String</span><span class="sxs-lookup"><span data-stu-id="afa67-176">String</span></span>|<span data-ttu-id="afa67-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="afa67-177">The developer of the app.</span></span> <span data-ttu-id="afa67-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="afa67-179">notes</span><span class="sxs-lookup"><span data-stu-id="afa67-179">notes</span></span>|<span data-ttu-id="afa67-180">String</span><span class="sxs-lookup"><span data-stu-id="afa67-180">String</span></span>|<span data-ttu-id="afa67-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="afa67-181">Notes for the app.</span></span> <span data-ttu-id="afa67-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="afa67-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="afa67-183">publishingState</span></span>|[<span data-ttu-id="afa67-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="afa67-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="afa67-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="afa67-185">The publishing state for the app.</span></span> <span data-ttu-id="afa67-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="afa67-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="afa67-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="afa67-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="afa67-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="afa67-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="afa67-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="afa67-189">committedContentVersion</span></span>|<span data-ttu-id="afa67-190">String</span><span class="sxs-lookup"><span data-stu-id="afa67-190">String</span></span>|<span data-ttu-id="afa67-191">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="afa67-191">The internal committed content version.</span></span> <span data-ttu-id="afa67-192">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="afa67-193">fileName</span><span class="sxs-lookup"><span data-stu-id="afa67-193">fileName</span></span>|<span data-ttu-id="afa67-194">String</span><span class="sxs-lookup"><span data-stu-id="afa67-194">String</span></span>|<span data-ttu-id="afa67-195">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="afa67-195">The name of the main Lob application file.</span></span> <span data-ttu-id="afa67-196">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="afa67-197">size</span><span class="sxs-lookup"><span data-stu-id="afa67-197">size</span></span>|<span data-ttu-id="afa67-198">Int64</span><span class="sxs-lookup"><span data-stu-id="afa67-198">Int64</span></span>|<span data-ttu-id="afa67-199">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="afa67-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="afa67-200">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="afa67-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="afa67-201">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="afa67-201">installCommandLine</span></span>|<span data-ttu-id="afa67-202">String</span><span class="sxs-lookup"><span data-stu-id="afa67-202">String</span></span>|<span data-ttu-id="afa67-203">安装此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="afa67-203">The command line to install this app</span></span>|
|<span data-ttu-id="afa67-204">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="afa67-204">uninstallCommandLine</span></span>|<span data-ttu-id="afa67-205">String</span><span class="sxs-lookup"><span data-stu-id="afa67-205">String</span></span>|<span data-ttu-id="afa67-206">卸载此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="afa67-206">The command line to uninstall this app</span></span>|
|<span data-ttu-id="afa67-207">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="afa67-207">applicableArchitectures</span></span>|[<span data-ttu-id="afa67-208">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="afa67-208">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="afa67-209">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="afa67-209">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="afa67-210">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。</span><span class="sxs-lookup"><span data-stu-id="afa67-210">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="afa67-211">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="afa67-211">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="afa67-212">Int32</span><span class="sxs-lookup"><span data-stu-id="afa67-212">Int32</span></span>|<span data-ttu-id="afa67-213">安装此应用程序所需的最小可用磁盘空间的值。</span><span class="sxs-lookup"><span data-stu-id="afa67-213">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="afa67-214">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="afa67-214">minimumMemoryInMB</span></span>|<span data-ttu-id="afa67-215">Int32</span><span class="sxs-lookup"><span data-stu-id="afa67-215">Int32</span></span>|<span data-ttu-id="afa67-216">安装此应用所需的最小物理内存的值。</span><span class="sxs-lookup"><span data-stu-id="afa67-216">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="afa67-217">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="afa67-217">minimumNumberOfProcessors</span></span>|<span data-ttu-id="afa67-218">Int32</span><span class="sxs-lookup"><span data-stu-id="afa67-218">Int32</span></span>|<span data-ttu-id="afa67-219">安装此应用程序所需的最少处理器数的值。</span><span class="sxs-lookup"><span data-stu-id="afa67-219">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="afa67-220">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="afa67-220">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="afa67-221">Int32</span><span class="sxs-lookup"><span data-stu-id="afa67-221">Int32</span></span>|<span data-ttu-id="afa67-222">安装此应用所需的最小 CPU 速度的值。</span><span class="sxs-lookup"><span data-stu-id="afa67-222">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="afa67-223">规则</span><span class="sxs-lookup"><span data-stu-id="afa67-223">rules</span></span>|<span data-ttu-id="afa67-224">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="afa67-224">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="afa67-225">此应用的检测和要求规则。</span><span class="sxs-lookup"><span data-stu-id="afa67-225">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="afa67-226">installExperience</span><span class="sxs-lookup"><span data-stu-id="afa67-226">installExperience</span></span>|[<span data-ttu-id="afa67-227">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="afa67-227">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="afa67-228">此应用的安装体验。</span><span class="sxs-lookup"><span data-stu-id="afa67-228">The install experience for this app.</span></span>|
|<span data-ttu-id="afa67-229">returnCodes</span><span class="sxs-lookup"><span data-stu-id="afa67-229">returnCodes</span></span>|<span data-ttu-id="afa67-230">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) 集合</span><span class="sxs-lookup"><span data-stu-id="afa67-230">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="afa67-231">安装后行为的返回代码。</span><span class="sxs-lookup"><span data-stu-id="afa67-231">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="afa67-232">msiInformation</span><span class="sxs-lookup"><span data-stu-id="afa67-232">msiInformation</span></span>|[<span data-ttu-id="afa67-233">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="afa67-233">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="afa67-234">如果此 Win32 应用是 MSI 应用，则 MSI 详细信息。</span><span class="sxs-lookup"><span data-stu-id="afa67-234">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="afa67-235">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="afa67-235">setupFilePath</span></span>|<span data-ttu-id="afa67-236">String</span><span class="sxs-lookup"><span data-stu-id="afa67-236">String</span></span>|<span data-ttu-id="afa67-237">加密 Win32LobApp 程序包中安装文件的相对路径。</span><span class="sxs-lookup"><span data-stu-id="afa67-237">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="afa67-238">minimumSupportedWindowsRelease</span><span class="sxs-lookup"><span data-stu-id="afa67-238">minimumSupportedWindowsRelease</span></span>|<span data-ttu-id="afa67-239">String</span><span class="sxs-lookup"><span data-stu-id="afa67-239">String</span></span>|<span data-ttu-id="afa67-240">受支持的最低窗口版本的值。</span><span class="sxs-lookup"><span data-stu-id="afa67-240">The value for the minimum supported windows release.</span></span>|



## <a name="response"></a><span data-ttu-id="afa67-241">响应</span><span class="sxs-lookup"><span data-stu-id="afa67-241">Response</span></span>
<span data-ttu-id="afa67-242">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [win32LobApp](../resources/intune-apps-win32lobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="afa67-242">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afa67-243">示例</span><span class="sxs-lookup"><span data-stu-id="afa67-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="afa67-244">请求</span><span class="sxs-lookup"><span data-stu-id="afa67-244">Request</span></span>
<span data-ttu-id="afa67-245">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="afa67-245">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="afa67-246">响应</span><span class="sxs-lookup"><span data-stu-id="afa67-246">Response</span></span>
<span data-ttu-id="afa67-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="afa67-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




