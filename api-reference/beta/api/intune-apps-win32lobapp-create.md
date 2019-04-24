---
title: 创建 win32LobApp
description: 创建新的 win32LobApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b4249ff5579ea29ca7c756956f6260df079a3a6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32488334"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="382d7-103">创建 win32LobApp</span><span class="sxs-lookup"><span data-stu-id="382d7-103">Create win32LobApp</span></span>

> <span data-ttu-id="382d7-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="382d7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="382d7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="382d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="382d7-106">创建新的[win32LobApp](../resources/intune-apps-win32lobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="382d7-106">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="382d7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="382d7-107">Prerequisites</span></span>
<span data-ttu-id="382d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="382d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="382d7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="382d7-110">Permission type</span></span>|<span data-ttu-id="382d7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="382d7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="382d7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="382d7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="382d7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="382d7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="382d7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="382d7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="382d7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="382d7-115">Not supported.</span></span>|
|<span data-ttu-id="382d7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="382d7-116">Application</span></span>|<span data-ttu-id="382d7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="382d7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="382d7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="382d7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="382d7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="382d7-119">Request headers</span></span>
|<span data-ttu-id="382d7-120">标头</span><span class="sxs-lookup"><span data-stu-id="382d7-120">Header</span></span>|<span data-ttu-id="382d7-121">值</span><span class="sxs-lookup"><span data-stu-id="382d7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="382d7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="382d7-122">Authorization</span></span>|<span data-ttu-id="382d7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="382d7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="382d7-124">接受</span><span class="sxs-lookup"><span data-stu-id="382d7-124">Accept</span></span>|<span data-ttu-id="382d7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="382d7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="382d7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="382d7-126">Request body</span></span>
<span data-ttu-id="382d7-127">在请求正文中, 提供 win32LobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="382d7-127">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="382d7-128">下表显示创建 win32LobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="382d7-128">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="382d7-129">属性</span><span class="sxs-lookup"><span data-stu-id="382d7-129">Property</span></span>|<span data-ttu-id="382d7-130">类型</span><span class="sxs-lookup"><span data-stu-id="382d7-130">Type</span></span>|<span data-ttu-id="382d7-131">说明</span><span class="sxs-lookup"><span data-stu-id="382d7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="382d7-132">id</span><span class="sxs-lookup"><span data-stu-id="382d7-132">id</span></span>|<span data-ttu-id="382d7-133">String</span><span class="sxs-lookup"><span data-stu-id="382d7-133">String</span></span>|<span data-ttu-id="382d7-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="382d7-134">Key of the entity.</span></span> <span data-ttu-id="382d7-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="382d7-136">displayName</span></span>|<span data-ttu-id="382d7-137">字符串</span><span class="sxs-lookup"><span data-stu-id="382d7-137">String</span></span>|<span data-ttu-id="382d7-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="382d7-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="382d7-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-140">description</span><span class="sxs-lookup"><span data-stu-id="382d7-140">description</span></span>|<span data-ttu-id="382d7-141">字符串</span><span class="sxs-lookup"><span data-stu-id="382d7-141">String</span></span>|<span data-ttu-id="382d7-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="382d7-142">The description of the app.</span></span> <span data-ttu-id="382d7-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-144">publisher</span><span class="sxs-lookup"><span data-stu-id="382d7-144">publisher</span></span>|<span data-ttu-id="382d7-145">字符串</span><span class="sxs-lookup"><span data-stu-id="382d7-145">String</span></span>|<span data-ttu-id="382d7-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="382d7-146">The publisher of the app.</span></span> <span data-ttu-id="382d7-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="382d7-148">largeIcon</span></span>|[<span data-ttu-id="382d7-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="382d7-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="382d7-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="382d7-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="382d7-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="382d7-152">createdDateTime</span></span>|<span data-ttu-id="382d7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="382d7-153">DateTimeOffset</span></span>|<span data-ttu-id="382d7-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="382d7-154">The date and time the app was created.</span></span> <span data-ttu-id="382d7-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="382d7-156">lastModifiedDateTime</span></span>|<span data-ttu-id="382d7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="382d7-157">DateTimeOffset</span></span>|<span data-ttu-id="382d7-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="382d7-158">The date and time the app was last modified.</span></span> <span data-ttu-id="382d7-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="382d7-160">isFeatured</span></span>|<span data-ttu-id="382d7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="382d7-161">Boolean</span></span>|<span data-ttu-id="382d7-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="382d7-163">privacyInformationUrl</span></span>|<span data-ttu-id="382d7-164">字符串</span><span class="sxs-lookup"><span data-stu-id="382d7-164">String</span></span>|<span data-ttu-id="382d7-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="382d7-165">The privacy statement Url.</span></span> <span data-ttu-id="382d7-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="382d7-167">informationUrl</span></span>|<span data-ttu-id="382d7-168">字符串</span><span class="sxs-lookup"><span data-stu-id="382d7-168">String</span></span>|<span data-ttu-id="382d7-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="382d7-169">The more information Url.</span></span> <span data-ttu-id="382d7-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-171">owner</span><span class="sxs-lookup"><span data-stu-id="382d7-171">owner</span></span>|<span data-ttu-id="382d7-172">字符串</span><span class="sxs-lookup"><span data-stu-id="382d7-172">String</span></span>|<span data-ttu-id="382d7-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="382d7-173">The owner of the app.</span></span> <span data-ttu-id="382d7-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-175">developer</span><span class="sxs-lookup"><span data-stu-id="382d7-175">developer</span></span>|<span data-ttu-id="382d7-176">字符串</span><span class="sxs-lookup"><span data-stu-id="382d7-176">String</span></span>|<span data-ttu-id="382d7-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="382d7-177">The developer of the app.</span></span> <span data-ttu-id="382d7-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-179">notes</span><span class="sxs-lookup"><span data-stu-id="382d7-179">notes</span></span>|<span data-ttu-id="382d7-180">字符串</span><span class="sxs-lookup"><span data-stu-id="382d7-180">String</span></span>|<span data-ttu-id="382d7-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="382d7-181">Notes for the app.</span></span> <span data-ttu-id="382d7-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="382d7-183">uploadState</span></span>|<span data-ttu-id="382d7-184">Int32</span><span class="sxs-lookup"><span data-stu-id="382d7-184">Int32</span></span>|<span data-ttu-id="382d7-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="382d7-185">The upload state.</span></span> <span data-ttu-id="382d7-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="382d7-187">publishingState</span></span>|[<span data-ttu-id="382d7-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="382d7-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="382d7-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="382d7-189">The publishing state for the app.</span></span> <span data-ttu-id="382d7-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="382d7-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="382d7-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="382d7-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="382d7-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="382d7-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="382d7-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="382d7-193">isAssigned</span></span>|<span data-ttu-id="382d7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="382d7-194">Boolean</span></span>|<span data-ttu-id="382d7-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="382d7-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="382d7-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="382d7-197">roleScopeTagIds</span></span>|<span data-ttu-id="382d7-198">String collection</span><span class="sxs-lookup"><span data-stu-id="382d7-198">String collection</span></span>|<span data-ttu-id="382d7-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="382d7-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="382d7-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="382d7-201">dependentAppCount</span></span>|<span data-ttu-id="382d7-202">Int32</span><span class="sxs-lookup"><span data-stu-id="382d7-202">Int32</span></span>|<span data-ttu-id="382d7-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="382d7-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="382d7-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="382d7-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="382d7-205">committedContentVersion</span></span>|<span data-ttu-id="382d7-206">字符串</span><span class="sxs-lookup"><span data-stu-id="382d7-206">String</span></span>|<span data-ttu-id="382d7-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="382d7-207">The internal committed content version.</span></span> <span data-ttu-id="382d7-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="382d7-209">fileName</span><span class="sxs-lookup"><span data-stu-id="382d7-209">fileName</span></span>|<span data-ttu-id="382d7-210">String</span><span class="sxs-lookup"><span data-stu-id="382d7-210">String</span></span>|<span data-ttu-id="382d7-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="382d7-211">The name of the main Lob application file.</span></span> <span data-ttu-id="382d7-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="382d7-213">size</span><span class="sxs-lookup"><span data-stu-id="382d7-213">size</span></span>|<span data-ttu-id="382d7-214">Int64</span><span class="sxs-lookup"><span data-stu-id="382d7-214">Int64</span></span>|<span data-ttu-id="382d7-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="382d7-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="382d7-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="382d7-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="382d7-217">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="382d7-217">installCommandLine</span></span>|<span data-ttu-id="382d7-218">字符串</span><span class="sxs-lookup"><span data-stu-id="382d7-218">String</span></span>|<span data-ttu-id="382d7-219">要安装此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="382d7-219">The command line to install this app</span></span>|
|<span data-ttu-id="382d7-220">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="382d7-220">uninstallCommandLine</span></span>|<span data-ttu-id="382d7-221">字符串</span><span class="sxs-lookup"><span data-stu-id="382d7-221">String</span></span>|<span data-ttu-id="382d7-222">要卸载此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="382d7-222">The command line to uninstall this app</span></span>|
|<span data-ttu-id="382d7-223">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="382d7-223">applicableArchitectures</span></span>|[<span data-ttu-id="382d7-224">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="382d7-224">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="382d7-225">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="382d7-225">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="382d7-226">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="382d7-226">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="382d7-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="382d7-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="382d7-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="382d7-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="382d7-229">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="382d7-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="382d7-230">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="382d7-230">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="382d7-231">Int32</span><span class="sxs-lookup"><span data-stu-id="382d7-231">Int32</span></span>|<span data-ttu-id="382d7-232">安装此应用程序所需的最小可用磁盘空间的值。</span><span class="sxs-lookup"><span data-stu-id="382d7-232">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="382d7-233">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="382d7-233">minimumMemoryInMB</span></span>|<span data-ttu-id="382d7-234">Int32</span><span class="sxs-lookup"><span data-stu-id="382d7-234">Int32</span></span>|<span data-ttu-id="382d7-235">安装此应用程序所需的最小物理内存的值。</span><span class="sxs-lookup"><span data-stu-id="382d7-235">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="382d7-236">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="382d7-236">minimumNumberOfProcessors</span></span>|<span data-ttu-id="382d7-237">Int32</span><span class="sxs-lookup"><span data-stu-id="382d7-237">Int32</span></span>|<span data-ttu-id="382d7-238">安装此应用程序所需的最小处理器数的值。</span><span class="sxs-lookup"><span data-stu-id="382d7-238">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="382d7-239">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="382d7-239">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="382d7-240">Int32</span><span class="sxs-lookup"><span data-stu-id="382d7-240">Int32</span></span>|<span data-ttu-id="382d7-241">安装此应用程序所需的最低 CPU 速度的值。</span><span class="sxs-lookup"><span data-stu-id="382d7-241">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="382d7-242">detectionRules</span><span class="sxs-lookup"><span data-stu-id="382d7-242">detectionRules</span></span>|<span data-ttu-id="382d7-243">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)集合</span><span class="sxs-lookup"><span data-stu-id="382d7-243">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="382d7-244">检测到 Win32 业务线 (LoB) 应用程序的检测规则。</span><span class="sxs-lookup"><span data-stu-id="382d7-244">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="382d7-245">requirementRules</span><span class="sxs-lookup"><span data-stu-id="382d7-245">requirementRules</span></span>|<span data-ttu-id="382d7-246">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)集合</span><span class="sxs-lookup"><span data-stu-id="382d7-246">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="382d7-247">用于检测 Win32 业务线 (LoB) 应用程序的要求规则。</span><span class="sxs-lookup"><span data-stu-id="382d7-247">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="382d7-248">installExperience</span><span class="sxs-lookup"><span data-stu-id="382d7-248">installExperience</span></span>|[<span data-ttu-id="382d7-249">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="382d7-249">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="382d7-250">此应用的安装体验。</span><span class="sxs-lookup"><span data-stu-id="382d7-250">The install experience for this app.</span></span>|
|<span data-ttu-id="382d7-251">returnCodes</span><span class="sxs-lookup"><span data-stu-id="382d7-251">returnCodes</span></span>|<span data-ttu-id="382d7-252">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)集合</span><span class="sxs-lookup"><span data-stu-id="382d7-252">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="382d7-253">用于安装后行为的返回代码。</span><span class="sxs-lookup"><span data-stu-id="382d7-253">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="382d7-254">msiInformation</span><span class="sxs-lookup"><span data-stu-id="382d7-254">msiInformation</span></span>|[<span data-ttu-id="382d7-255">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="382d7-255">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="382d7-256">如果此 Win32 应用是 msi 应用程序, 则为 msi 详细信息。</span><span class="sxs-lookup"><span data-stu-id="382d7-256">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="382d7-257">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="382d7-257">setupFilePath</span></span>|<span data-ttu-id="382d7-258">字符串</span><span class="sxs-lookup"><span data-stu-id="382d7-258">String</span></span>|<span data-ttu-id="382d7-259">加密的 Win32LobApp 包中的安装程序文件的相对路径。</span><span class="sxs-lookup"><span data-stu-id="382d7-259">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="382d7-260">响应</span><span class="sxs-lookup"><span data-stu-id="382d7-260">Response</span></span>
<span data-ttu-id="382d7-261">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[win32LobApp](../resources/intune-apps-win32lobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="382d7-261">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="382d7-262">示例</span><span class="sxs-lookup"><span data-stu-id="382d7-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="382d7-263">请求</span><span class="sxs-lookup"><span data-stu-id="382d7-263">Request</span></span>
<span data-ttu-id="382d7-264">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="382d7-264">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2732

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
  "dependentAppCount": 1,
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
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
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

### <a name="response"></a><span data-ttu-id="382d7-265">响应</span><span class="sxs-lookup"><span data-stu-id="382d7-265">Response</span></span>
<span data-ttu-id="382d7-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="382d7-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2904

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
  "dependentAppCount": 1,
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
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
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





