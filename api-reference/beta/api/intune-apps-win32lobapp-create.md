---
title: 创建 win32LobApp
description: 创建新的 win32LobApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f805e9c41aacbc6c12cc44ad84f2e05db5b4d14
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793267"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="8278c-103">创建 win32LobApp</span><span class="sxs-lookup"><span data-stu-id="8278c-103">Create win32LobApp</span></span>

<span data-ttu-id="8278c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8278c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8278c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8278c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8278c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8278c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8278c-107">创建新的[win32LobApp](../resources/intune-apps-win32lobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8278c-107">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8278c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8278c-108">Prerequisites</span></span>
<span data-ttu-id="8278c-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="8278c-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8278c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8278c-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8278c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8278c-111">Permission type</span></span>|<span data-ttu-id="8278c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8278c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8278c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8278c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8278c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8278c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8278c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8278c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8278c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8278c-116">Not supported.</span></span>|
|<span data-ttu-id="8278c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="8278c-117">Application</span></span>|<span data-ttu-id="8278c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8278c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8278c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8278c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="8278c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8278c-120">Request headers</span></span>
|<span data-ttu-id="8278c-121">标头</span><span class="sxs-lookup"><span data-stu-id="8278c-121">Header</span></span>|<span data-ttu-id="8278c-122">值</span><span class="sxs-lookup"><span data-stu-id="8278c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8278c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8278c-123">Authorization</span></span>|<span data-ttu-id="8278c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8278c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8278c-125">接受</span><span class="sxs-lookup"><span data-stu-id="8278c-125">Accept</span></span>|<span data-ttu-id="8278c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8278c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8278c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8278c-127">Request body</span></span>
<span data-ttu-id="8278c-128">在请求正文中，提供 win32LobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8278c-128">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="8278c-129">下表显示创建 win32LobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8278c-129">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="8278c-130">属性</span><span class="sxs-lookup"><span data-stu-id="8278c-130">Property</span></span>|<span data-ttu-id="8278c-131">类型</span><span class="sxs-lookup"><span data-stu-id="8278c-131">Type</span></span>|<span data-ttu-id="8278c-132">说明</span><span class="sxs-lookup"><span data-stu-id="8278c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8278c-133">id</span><span class="sxs-lookup"><span data-stu-id="8278c-133">id</span></span>|<span data-ttu-id="8278c-134">字符串</span><span class="sxs-lookup"><span data-stu-id="8278c-134">String</span></span>|<span data-ttu-id="8278c-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8278c-135">Key of the entity.</span></span> <span data-ttu-id="8278c-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8278c-137">displayName</span></span>|<span data-ttu-id="8278c-138">String</span><span class="sxs-lookup"><span data-stu-id="8278c-138">String</span></span>|<span data-ttu-id="8278c-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="8278c-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8278c-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-141">说明</span><span class="sxs-lookup"><span data-stu-id="8278c-141">description</span></span>|<span data-ttu-id="8278c-142">字符串</span><span class="sxs-lookup"><span data-stu-id="8278c-142">String</span></span>|<span data-ttu-id="8278c-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="8278c-143">The description of the app.</span></span> <span data-ttu-id="8278c-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8278c-145">publisher</span></span>|<span data-ttu-id="8278c-146">String</span><span class="sxs-lookup"><span data-stu-id="8278c-146">String</span></span>|<span data-ttu-id="8278c-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="8278c-147">The publisher of the app.</span></span> <span data-ttu-id="8278c-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8278c-149">largeIcon</span></span>|[<span data-ttu-id="8278c-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8278c-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8278c-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="8278c-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8278c-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8278c-153">createdDateTime</span></span>|<span data-ttu-id="8278c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8278c-154">DateTimeOffset</span></span>|<span data-ttu-id="8278c-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8278c-155">The date and time the app was created.</span></span> <span data-ttu-id="8278c-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8278c-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8278c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8278c-158">DateTimeOffset</span></span>|<span data-ttu-id="8278c-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8278c-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8278c-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8278c-161">isFeatured</span></span>|<span data-ttu-id="8278c-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8278c-162">Boolean</span></span>|<span data-ttu-id="8278c-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8278c-164">privacyInformationUrl</span></span>|<span data-ttu-id="8278c-165">String</span><span class="sxs-lookup"><span data-stu-id="8278c-165">String</span></span>|<span data-ttu-id="8278c-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="8278c-166">The privacy statement Url.</span></span> <span data-ttu-id="8278c-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8278c-168">informationUrl</span></span>|<span data-ttu-id="8278c-169">String</span><span class="sxs-lookup"><span data-stu-id="8278c-169">String</span></span>|<span data-ttu-id="8278c-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="8278c-170">The more information Url.</span></span> <span data-ttu-id="8278c-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-172">owner</span><span class="sxs-lookup"><span data-stu-id="8278c-172">owner</span></span>|<span data-ttu-id="8278c-173">String</span><span class="sxs-lookup"><span data-stu-id="8278c-173">String</span></span>|<span data-ttu-id="8278c-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="8278c-174">The owner of the app.</span></span> <span data-ttu-id="8278c-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-176">developer</span><span class="sxs-lookup"><span data-stu-id="8278c-176">developer</span></span>|<span data-ttu-id="8278c-177">String</span><span class="sxs-lookup"><span data-stu-id="8278c-177">String</span></span>|<span data-ttu-id="8278c-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="8278c-178">The developer of the app.</span></span> <span data-ttu-id="8278c-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-180">notes</span><span class="sxs-lookup"><span data-stu-id="8278c-180">notes</span></span>|<span data-ttu-id="8278c-181">String</span><span class="sxs-lookup"><span data-stu-id="8278c-181">String</span></span>|<span data-ttu-id="8278c-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="8278c-182">Notes for the app.</span></span> <span data-ttu-id="8278c-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8278c-184">uploadState</span></span>|<span data-ttu-id="8278c-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8278c-185">Int32</span></span>|<span data-ttu-id="8278c-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="8278c-186">The upload state.</span></span> <span data-ttu-id="8278c-187">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8278c-188">publishingState</span></span>|[<span data-ttu-id="8278c-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8278c-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8278c-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="8278c-190">The publishing state for the app.</span></span> <span data-ttu-id="8278c-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="8278c-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8278c-192">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="8278c-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="8278c-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="8278c-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8278c-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="8278c-194">isAssigned</span></span>|<span data-ttu-id="8278c-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="8278c-195">Boolean</span></span>|<span data-ttu-id="8278c-196">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="8278c-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="8278c-197">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8278c-198">roleScopeTagIds</span></span>|<span data-ttu-id="8278c-199">String collection</span><span class="sxs-lookup"><span data-stu-id="8278c-199">String collection</span></span>|<span data-ttu-id="8278c-200">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="8278c-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="8278c-201">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="8278c-202">dependentAppCount</span></span>|<span data-ttu-id="8278c-203">Int32</span><span class="sxs-lookup"><span data-stu-id="8278c-203">Int32</span></span>|<span data-ttu-id="8278c-204">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="8278c-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="8278c-205">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="8278c-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="8278c-206">committedContentVersion</span></span>|<span data-ttu-id="8278c-207">String</span><span class="sxs-lookup"><span data-stu-id="8278c-207">String</span></span>|<span data-ttu-id="8278c-208">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="8278c-208">The internal committed content version.</span></span> <span data-ttu-id="8278c-209">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8278c-210">fileName</span><span class="sxs-lookup"><span data-stu-id="8278c-210">fileName</span></span>|<span data-ttu-id="8278c-211">String</span><span class="sxs-lookup"><span data-stu-id="8278c-211">String</span></span>|<span data-ttu-id="8278c-212">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="8278c-212">The name of the main Lob application file.</span></span> <span data-ttu-id="8278c-213">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8278c-214">size</span><span class="sxs-lookup"><span data-stu-id="8278c-214">size</span></span>|<span data-ttu-id="8278c-215">Int64</span><span class="sxs-lookup"><span data-stu-id="8278c-215">Int64</span></span>|<span data-ttu-id="8278c-216">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="8278c-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="8278c-217">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="8278c-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="8278c-218">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="8278c-218">installCommandLine</span></span>|<span data-ttu-id="8278c-219">String</span><span class="sxs-lookup"><span data-stu-id="8278c-219">String</span></span>|<span data-ttu-id="8278c-220">要安装此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="8278c-220">The command line to install this app</span></span>|
|<span data-ttu-id="8278c-221">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="8278c-221">uninstallCommandLine</span></span>|<span data-ttu-id="8278c-222">String</span><span class="sxs-lookup"><span data-stu-id="8278c-222">String</span></span>|<span data-ttu-id="8278c-223">要卸载此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="8278c-223">The command line to uninstall this app</span></span>|
|<span data-ttu-id="8278c-224">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="8278c-224">applicableArchitectures</span></span>|[<span data-ttu-id="8278c-225">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="8278c-225">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="8278c-226">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="8278c-226">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="8278c-227">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="8278c-227">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="8278c-228">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8278c-228">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="8278c-229">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="8278c-229">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="8278c-230">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="8278c-230">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="8278c-231">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="8278c-231">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="8278c-232">Int32</span><span class="sxs-lookup"><span data-stu-id="8278c-232">Int32</span></span>|<span data-ttu-id="8278c-233">安装此应用程序所需的最小可用磁盘空间的值。</span><span class="sxs-lookup"><span data-stu-id="8278c-233">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="8278c-234">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="8278c-234">minimumMemoryInMB</span></span>|<span data-ttu-id="8278c-235">Int32</span><span class="sxs-lookup"><span data-stu-id="8278c-235">Int32</span></span>|<span data-ttu-id="8278c-236">安装此应用程序所需的最小物理内存的值。</span><span class="sxs-lookup"><span data-stu-id="8278c-236">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="8278c-237">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="8278c-237">minimumNumberOfProcessors</span></span>|<span data-ttu-id="8278c-238">Int32</span><span class="sxs-lookup"><span data-stu-id="8278c-238">Int32</span></span>|<span data-ttu-id="8278c-239">安装此应用程序所需的最小处理器数的值。</span><span class="sxs-lookup"><span data-stu-id="8278c-239">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="8278c-240">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="8278c-240">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="8278c-241">Int32</span><span class="sxs-lookup"><span data-stu-id="8278c-241">Int32</span></span>|<span data-ttu-id="8278c-242">安装此应用程序所需的最低 CPU 速度的值。</span><span class="sxs-lookup"><span data-stu-id="8278c-242">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="8278c-243">detectionRules</span><span class="sxs-lookup"><span data-stu-id="8278c-243">detectionRules</span></span>|<span data-ttu-id="8278c-244">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)集合</span><span class="sxs-lookup"><span data-stu-id="8278c-244">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="8278c-245">检测到 Win32 业务线（LoB）应用程序的检测规则。</span><span class="sxs-lookup"><span data-stu-id="8278c-245">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8278c-246">requirementRules</span><span class="sxs-lookup"><span data-stu-id="8278c-246">requirementRules</span></span>|<span data-ttu-id="8278c-247">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)集合</span><span class="sxs-lookup"><span data-stu-id="8278c-247">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="8278c-248">用于检测 Win32 业务线（LoB）应用程序的要求规则。</span><span class="sxs-lookup"><span data-stu-id="8278c-248">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="8278c-249">规则</span><span class="sxs-lookup"><span data-stu-id="8278c-249">rules</span></span>|<span data-ttu-id="8278c-250">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md)集合</span><span class="sxs-lookup"><span data-stu-id="8278c-250">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="8278c-251">此应用程序的检测和要求规则。</span><span class="sxs-lookup"><span data-stu-id="8278c-251">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="8278c-252">installExperience</span><span class="sxs-lookup"><span data-stu-id="8278c-252">installExperience</span></span>|[<span data-ttu-id="8278c-253">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="8278c-253">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="8278c-254">此应用的安装体验。</span><span class="sxs-lookup"><span data-stu-id="8278c-254">The install experience for this app.</span></span>|
|<span data-ttu-id="8278c-255">returnCodes</span><span class="sxs-lookup"><span data-stu-id="8278c-255">returnCodes</span></span>|<span data-ttu-id="8278c-256">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)集合</span><span class="sxs-lookup"><span data-stu-id="8278c-256">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="8278c-257">用于安装后行为的返回代码。</span><span class="sxs-lookup"><span data-stu-id="8278c-257">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="8278c-258">msiInformation</span><span class="sxs-lookup"><span data-stu-id="8278c-258">msiInformation</span></span>|[<span data-ttu-id="8278c-259">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="8278c-259">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="8278c-260">如果此 Win32 应用是 MSI 应用程序，则为 MSI 详细信息。</span><span class="sxs-lookup"><span data-stu-id="8278c-260">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="8278c-261">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="8278c-261">setupFilePath</span></span>|<span data-ttu-id="8278c-262">String</span><span class="sxs-lookup"><span data-stu-id="8278c-262">String</span></span>|<span data-ttu-id="8278c-263">加密的 Win32LobApp 包中的安装程序文件的相对路径。</span><span class="sxs-lookup"><span data-stu-id="8278c-263">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="8278c-264">installLanguage</span><span class="sxs-lookup"><span data-stu-id="8278c-264">installLanguage</span></span>|<span data-ttu-id="8278c-265">String</span><span class="sxs-lookup"><span data-stu-id="8278c-265">String</span></span>|<span data-ttu-id="8278c-266">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8278c-266">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8278c-267">响应</span><span class="sxs-lookup"><span data-stu-id="8278c-267">Response</span></span>
<span data-ttu-id="8278c-268">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[win32LobApp](../resources/intune-apps-win32lobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8278c-268">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8278c-269">示例</span><span class="sxs-lookup"><span data-stu-id="8278c-269">Example</span></span>

### <a name="request"></a><span data-ttu-id="8278c-270">请求</span><span class="sxs-lookup"><span data-stu-id="8278c-270">Request</span></span>
<span data-ttu-id="8278c-271">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8278c-271">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 3224

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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
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
  "installLanguage": "Install Language value"
}
```

### <a name="response"></a><span data-ttu-id="8278c-272">响应</span><span class="sxs-lookup"><span data-stu-id="8278c-272">Response</span></span>
<span data-ttu-id="8278c-273">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="8278c-273">Here is an example of the response.</span></span> <span data-ttu-id="8278c-274">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="8278c-274">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8278c-275">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="8278c-275">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3396

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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
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
  "installLanguage": "Install Language value"
}
```



