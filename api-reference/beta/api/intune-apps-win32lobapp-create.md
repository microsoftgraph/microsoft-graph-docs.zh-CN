---
title: 创建 win32LobApp
description: 创建新的 win32LobApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc05e7b86c50018b7576a7839867d2896b590443
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791531"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="79e07-103">创建 win32LobApp</span><span class="sxs-lookup"><span data-stu-id="79e07-103">Create win32LobApp</span></span>

<span data-ttu-id="79e07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79e07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79e07-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="79e07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79e07-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79e07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79e07-107">创建新的 [win32LobApp](../resources/intune-apps-win32lobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79e07-107">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79e07-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="79e07-108">Prerequisites</span></span>
<span data-ttu-id="79e07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79e07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79e07-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="79e07-111">Permission type</span></span>|<span data-ttu-id="79e07-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="79e07-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79e07-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79e07-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79e07-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79e07-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="79e07-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79e07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79e07-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="79e07-116">Not supported.</span></span>|
|<span data-ttu-id="79e07-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="79e07-117">Application</span></span>|<span data-ttu-id="79e07-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79e07-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79e07-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79e07-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="79e07-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="79e07-120">Request headers</span></span>
|<span data-ttu-id="79e07-121">标头</span><span class="sxs-lookup"><span data-stu-id="79e07-121">Header</span></span>|<span data-ttu-id="79e07-122">值</span><span class="sxs-lookup"><span data-stu-id="79e07-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79e07-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79e07-123">Authorization</span></span>|<span data-ttu-id="79e07-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="79e07-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79e07-125">接受</span><span class="sxs-lookup"><span data-stu-id="79e07-125">Accept</span></span>|<span data-ttu-id="79e07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79e07-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79e07-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="79e07-127">Request body</span></span>
<span data-ttu-id="79e07-128">在请求正文中，提供 win32LobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79e07-128">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="79e07-129">下表显示创建 win32LobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="79e07-129">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="79e07-130">属性</span><span class="sxs-lookup"><span data-stu-id="79e07-130">Property</span></span>|<span data-ttu-id="79e07-131">类型</span><span class="sxs-lookup"><span data-stu-id="79e07-131">Type</span></span>|<span data-ttu-id="79e07-132">说明</span><span class="sxs-lookup"><span data-stu-id="79e07-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79e07-133">id</span><span class="sxs-lookup"><span data-stu-id="79e07-133">id</span></span>|<span data-ttu-id="79e07-134">String</span><span class="sxs-lookup"><span data-stu-id="79e07-134">String</span></span>|<span data-ttu-id="79e07-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="79e07-135">Key of the entity.</span></span> <span data-ttu-id="79e07-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-137">displayName</span><span class="sxs-lookup"><span data-stu-id="79e07-137">displayName</span></span>|<span data-ttu-id="79e07-138">String</span><span class="sxs-lookup"><span data-stu-id="79e07-138">String</span></span>|<span data-ttu-id="79e07-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="79e07-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="79e07-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-141">description</span><span class="sxs-lookup"><span data-stu-id="79e07-141">description</span></span>|<span data-ttu-id="79e07-142">String</span><span class="sxs-lookup"><span data-stu-id="79e07-142">String</span></span>|<span data-ttu-id="79e07-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="79e07-143">The description of the app.</span></span> <span data-ttu-id="79e07-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-145">publisher</span><span class="sxs-lookup"><span data-stu-id="79e07-145">publisher</span></span>|<span data-ttu-id="79e07-146">String</span><span class="sxs-lookup"><span data-stu-id="79e07-146">String</span></span>|<span data-ttu-id="79e07-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="79e07-147">The publisher of the app.</span></span> <span data-ttu-id="79e07-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="79e07-149">largeIcon</span></span>|[<span data-ttu-id="79e07-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="79e07-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="79e07-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="79e07-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="79e07-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79e07-153">createdDateTime</span></span>|<span data-ttu-id="79e07-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79e07-154">DateTimeOffset</span></span>|<span data-ttu-id="79e07-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="79e07-155">The date and time the app was created.</span></span> <span data-ttu-id="79e07-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79e07-157">lastModifiedDateTime</span></span>|<span data-ttu-id="79e07-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79e07-158">DateTimeOffset</span></span>|<span data-ttu-id="79e07-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="79e07-159">The date and time the app was last modified.</span></span> <span data-ttu-id="79e07-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="79e07-161">isFeatured</span></span>|<span data-ttu-id="79e07-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="79e07-162">Boolean</span></span>|<span data-ttu-id="79e07-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="79e07-164">privacyInformationUrl</span></span>|<span data-ttu-id="79e07-165">String</span><span class="sxs-lookup"><span data-stu-id="79e07-165">String</span></span>|<span data-ttu-id="79e07-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="79e07-166">The privacy statement Url.</span></span> <span data-ttu-id="79e07-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="79e07-168">informationUrl</span></span>|<span data-ttu-id="79e07-169">String</span><span class="sxs-lookup"><span data-stu-id="79e07-169">String</span></span>|<span data-ttu-id="79e07-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="79e07-170">The more information Url.</span></span> <span data-ttu-id="79e07-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-172">所有者</span><span class="sxs-lookup"><span data-stu-id="79e07-172">owner</span></span>|<span data-ttu-id="79e07-173">String</span><span class="sxs-lookup"><span data-stu-id="79e07-173">String</span></span>|<span data-ttu-id="79e07-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="79e07-174">The owner of the app.</span></span> <span data-ttu-id="79e07-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-176">developer</span><span class="sxs-lookup"><span data-stu-id="79e07-176">developer</span></span>|<span data-ttu-id="79e07-177">String</span><span class="sxs-lookup"><span data-stu-id="79e07-177">String</span></span>|<span data-ttu-id="79e07-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="79e07-178">The developer of the app.</span></span> <span data-ttu-id="79e07-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-180">notes</span><span class="sxs-lookup"><span data-stu-id="79e07-180">notes</span></span>|<span data-ttu-id="79e07-181">String</span><span class="sxs-lookup"><span data-stu-id="79e07-181">String</span></span>|<span data-ttu-id="79e07-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="79e07-182">Notes for the app.</span></span> <span data-ttu-id="79e07-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="79e07-184">uploadState</span></span>|<span data-ttu-id="79e07-185">Int32</span><span class="sxs-lookup"><span data-stu-id="79e07-185">Int32</span></span>|<span data-ttu-id="79e07-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="79e07-186">The upload state.</span></span> <span data-ttu-id="79e07-187">可能的值包括： 0- `Not Ready` 、1- `Ready` 、2- `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="79e07-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="79e07-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="79e07-189">publishingState</span></span>|[<span data-ttu-id="79e07-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="79e07-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="79e07-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="79e07-191">The publishing state for the app.</span></span> <span data-ttu-id="79e07-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="79e07-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="79e07-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="79e07-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="79e07-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="79e07-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="79e07-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="79e07-195">isAssigned</span></span>|<span data-ttu-id="79e07-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="79e07-196">Boolean</span></span>|<span data-ttu-id="79e07-197">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="79e07-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="79e07-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="79e07-199">roleScopeTagIds</span></span>|<span data-ttu-id="79e07-200">字符串集合</span><span class="sxs-lookup"><span data-stu-id="79e07-200">String collection</span></span>|<span data-ttu-id="79e07-201">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="79e07-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="79e07-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="79e07-203">dependentAppCount</span></span>|<span data-ttu-id="79e07-204">Int32</span><span class="sxs-lookup"><span data-stu-id="79e07-204">Int32</span></span>|<span data-ttu-id="79e07-205">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="79e07-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="79e07-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="79e07-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="79e07-207">committedContentVersion</span></span>|<span data-ttu-id="79e07-208">String</span><span class="sxs-lookup"><span data-stu-id="79e07-208">String</span></span>|<span data-ttu-id="79e07-209">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="79e07-209">The internal committed content version.</span></span> <span data-ttu-id="79e07-210">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="79e07-211">fileName</span><span class="sxs-lookup"><span data-stu-id="79e07-211">fileName</span></span>|<span data-ttu-id="79e07-212">String</span><span class="sxs-lookup"><span data-stu-id="79e07-212">String</span></span>|<span data-ttu-id="79e07-213">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="79e07-213">The name of the main Lob application file.</span></span> <span data-ttu-id="79e07-214">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="79e07-215">size</span><span class="sxs-lookup"><span data-stu-id="79e07-215">size</span></span>|<span data-ttu-id="79e07-216">Int64</span><span class="sxs-lookup"><span data-stu-id="79e07-216">Int64</span></span>|<span data-ttu-id="79e07-217">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="79e07-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="79e07-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="79e07-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="79e07-219">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="79e07-219">installCommandLine</span></span>|<span data-ttu-id="79e07-220">String</span><span class="sxs-lookup"><span data-stu-id="79e07-220">String</span></span>|<span data-ttu-id="79e07-221">要安装此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="79e07-221">The command line to install this app</span></span>|
|<span data-ttu-id="79e07-222">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="79e07-222">uninstallCommandLine</span></span>|<span data-ttu-id="79e07-223">String</span><span class="sxs-lookup"><span data-stu-id="79e07-223">String</span></span>|<span data-ttu-id="79e07-224">要卸载此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="79e07-224">The command line to uninstall this app</span></span>|
|<span data-ttu-id="79e07-225">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="79e07-225">applicableArchitectures</span></span>|[<span data-ttu-id="79e07-226">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="79e07-226">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="79e07-227">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="79e07-227">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="79e07-228">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="79e07-228">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="79e07-229">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="79e07-229">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="79e07-230">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="79e07-230">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="79e07-231">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="79e07-231">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="79e07-232">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="79e07-232">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="79e07-233">Int32</span><span class="sxs-lookup"><span data-stu-id="79e07-233">Int32</span></span>|<span data-ttu-id="79e07-234">安装此应用程序所需的最小可用磁盘空间的值。</span><span class="sxs-lookup"><span data-stu-id="79e07-234">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="79e07-235">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="79e07-235">minimumMemoryInMB</span></span>|<span data-ttu-id="79e07-236">Int32</span><span class="sxs-lookup"><span data-stu-id="79e07-236">Int32</span></span>|<span data-ttu-id="79e07-237">安装此应用程序所需的最小物理内存的值。</span><span class="sxs-lookup"><span data-stu-id="79e07-237">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="79e07-238">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="79e07-238">minimumNumberOfProcessors</span></span>|<span data-ttu-id="79e07-239">Int32</span><span class="sxs-lookup"><span data-stu-id="79e07-239">Int32</span></span>|<span data-ttu-id="79e07-240">安装此应用程序所需的最小处理器数的值。</span><span class="sxs-lookup"><span data-stu-id="79e07-240">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="79e07-241">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="79e07-241">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="79e07-242">Int32</span><span class="sxs-lookup"><span data-stu-id="79e07-242">Int32</span></span>|<span data-ttu-id="79e07-243">安装此应用程序所需的最低 CPU 速度的值。</span><span class="sxs-lookup"><span data-stu-id="79e07-243">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="79e07-244">detectionRules</span><span class="sxs-lookup"><span data-stu-id="79e07-244">detectionRules</span></span>|<span data-ttu-id="79e07-245">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="79e07-245">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="79e07-246">用于检测 Win32 业务线 (LoB) 应用程序的检测规则。</span><span class="sxs-lookup"><span data-stu-id="79e07-246">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="79e07-247">requirementRules</span><span class="sxs-lookup"><span data-stu-id="79e07-247">requirementRules</span></span>|<span data-ttu-id="79e07-248">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) 集合</span><span class="sxs-lookup"><span data-stu-id="79e07-248">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="79e07-249">用于检测 Win32 业务线 (LoB) 应用程序的要求规则。</span><span class="sxs-lookup"><span data-stu-id="79e07-249">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="79e07-250">规则</span><span class="sxs-lookup"><span data-stu-id="79e07-250">rules</span></span>|<span data-ttu-id="79e07-251">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="79e07-251">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="79e07-252">此应用程序的检测和要求规则。</span><span class="sxs-lookup"><span data-stu-id="79e07-252">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="79e07-253">installExperience</span><span class="sxs-lookup"><span data-stu-id="79e07-253">installExperience</span></span>|[<span data-ttu-id="79e07-254">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="79e07-254">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="79e07-255">此应用的安装体验。</span><span class="sxs-lookup"><span data-stu-id="79e07-255">The install experience for this app.</span></span>|
|<span data-ttu-id="79e07-256">returnCodes</span><span class="sxs-lookup"><span data-stu-id="79e07-256">returnCodes</span></span>|<span data-ttu-id="79e07-257">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) 集合</span><span class="sxs-lookup"><span data-stu-id="79e07-257">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="79e07-258">用于安装后行为的返回代码。</span><span class="sxs-lookup"><span data-stu-id="79e07-258">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="79e07-259">msiInformation</span><span class="sxs-lookup"><span data-stu-id="79e07-259">msiInformation</span></span>|[<span data-ttu-id="79e07-260">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="79e07-260">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="79e07-261">如果此 Win32 应用是 MSI 应用程序，则为 MSI 详细信息。</span><span class="sxs-lookup"><span data-stu-id="79e07-261">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="79e07-262">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="79e07-262">setupFilePath</span></span>|<span data-ttu-id="79e07-263">String</span><span class="sxs-lookup"><span data-stu-id="79e07-263">String</span></span>|<span data-ttu-id="79e07-264">加密的 Win32LobApp 包中的安装程序文件的相对路径。</span><span class="sxs-lookup"><span data-stu-id="79e07-264">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="79e07-265">installLanguage</span><span class="sxs-lookup"><span data-stu-id="79e07-265">installLanguage</span></span>|<span data-ttu-id="79e07-266">String</span><span class="sxs-lookup"><span data-stu-id="79e07-266">String</span></span>|<span data-ttu-id="79e07-267">尚未记录</span><span class="sxs-lookup"><span data-stu-id="79e07-267">Not yet documented</span></span>|
|<span data-ttu-id="79e07-268">minimumSupportedWindowsRelease</span><span class="sxs-lookup"><span data-stu-id="79e07-268">minimumSupportedWindowsRelease</span></span>|<span data-ttu-id="79e07-269">String</span><span class="sxs-lookup"><span data-stu-id="79e07-269">String</span></span>|<span data-ttu-id="79e07-270">支持的最小 windows 版本的值。</span><span class="sxs-lookup"><span data-stu-id="79e07-270">The value for the minimum supported windows release.</span></span>|



## <a name="response"></a><span data-ttu-id="79e07-271">响应</span><span class="sxs-lookup"><span data-stu-id="79e07-271">Response</span></span>
<span data-ttu-id="79e07-272">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [win32LobApp](../resources/intune-apps-win32lobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79e07-272">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79e07-273">示例</span><span class="sxs-lookup"><span data-stu-id="79e07-273">Example</span></span>

### <a name="request"></a><span data-ttu-id="79e07-274">请求</span><span class="sxs-lookup"><span data-stu-id="79e07-274">Request</span></span>
<span data-ttu-id="79e07-275">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79e07-275">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 3304

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
  "installLanguage": "Install Language value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```

### <a name="response"></a><span data-ttu-id="79e07-276">响应</span><span class="sxs-lookup"><span data-stu-id="79e07-276">Response</span></span>
<span data-ttu-id="79e07-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="79e07-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3476

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
  "installLanguage": "Install Language value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```



