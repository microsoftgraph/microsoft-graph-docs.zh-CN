---
title: 创建 win32LobApp
description: 创建新的 win32LobApp 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 52a4bb81518af0c0d78b642ba19ae295d32fa237
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39934061"
---
# <a name="create-win32lobapp"></a><span data-ttu-id="c023a-103">创建 win32LobApp</span><span class="sxs-lookup"><span data-stu-id="c023a-103">Create win32LobApp</span></span>

> <span data-ttu-id="c023a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c023a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c023a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c023a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c023a-106">创建新的[win32LobApp](../resources/intune-apps-win32lobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c023a-106">Create a new [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c023a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c023a-107">Prerequisites</span></span>
<span data-ttu-id="c023a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c023a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c023a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c023a-110">Permission type</span></span>|<span data-ttu-id="c023a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c023a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c023a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c023a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c023a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c023a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c023a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c023a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c023a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c023a-115">Not supported.</span></span>|
|<span data-ttu-id="c023a-116">Application</span><span class="sxs-lookup"><span data-stu-id="c023a-116">Application</span></span>|<span data-ttu-id="c023a-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c023a-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c023a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c023a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c023a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c023a-119">Request headers</span></span>
|<span data-ttu-id="c023a-120">标头</span><span class="sxs-lookup"><span data-stu-id="c023a-120">Header</span></span>|<span data-ttu-id="c023a-121">值</span><span class="sxs-lookup"><span data-stu-id="c023a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c023a-122">授权</span><span class="sxs-lookup"><span data-stu-id="c023a-122">Authorization</span></span>|<span data-ttu-id="c023a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c023a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c023a-124">接受</span><span class="sxs-lookup"><span data-stu-id="c023a-124">Accept</span></span>|<span data-ttu-id="c023a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c023a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c023a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c023a-126">Request body</span></span>
<span data-ttu-id="c023a-127">在请求正文中，提供 win32LobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c023a-127">In the request body, supply a JSON representation for the win32LobApp object.</span></span>

<span data-ttu-id="c023a-128">下表显示创建 win32LobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c023a-128">The following table shows the properties that are required when you create the win32LobApp.</span></span>

|<span data-ttu-id="c023a-129">属性</span><span class="sxs-lookup"><span data-stu-id="c023a-129">Property</span></span>|<span data-ttu-id="c023a-130">类型</span><span class="sxs-lookup"><span data-stu-id="c023a-130">Type</span></span>|<span data-ttu-id="c023a-131">说明</span><span class="sxs-lookup"><span data-stu-id="c023a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c023a-132">id</span><span class="sxs-lookup"><span data-stu-id="c023a-132">id</span></span>|<span data-ttu-id="c023a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c023a-133">String</span></span>|<span data-ttu-id="c023a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c023a-134">Key of the entity.</span></span> <span data-ttu-id="c023a-135">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-135">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c023a-136">displayName</span></span>|<span data-ttu-id="c023a-137">字符串</span><span class="sxs-lookup"><span data-stu-id="c023a-137">String</span></span>|<span data-ttu-id="c023a-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="c023a-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c023a-139">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-139">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-140">说明</span><span class="sxs-lookup"><span data-stu-id="c023a-140">description</span></span>|<span data-ttu-id="c023a-141">字符串</span><span class="sxs-lookup"><span data-stu-id="c023a-141">String</span></span>|<span data-ttu-id="c023a-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="c023a-142">The description of the app.</span></span> <span data-ttu-id="c023a-143">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-143">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-144">publisher</span><span class="sxs-lookup"><span data-stu-id="c023a-144">publisher</span></span>|<span data-ttu-id="c023a-145">字符串</span><span class="sxs-lookup"><span data-stu-id="c023a-145">String</span></span>|<span data-ttu-id="c023a-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="c023a-146">The publisher of the app.</span></span> <span data-ttu-id="c023a-147">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-147">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c023a-148">largeIcon</span></span>|[<span data-ttu-id="c023a-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c023a-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c023a-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="c023a-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c023a-151">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-151">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c023a-152">createdDateTime</span></span>|<span data-ttu-id="c023a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c023a-153">DateTimeOffset</span></span>|<span data-ttu-id="c023a-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c023a-154">The date and time the app was created.</span></span> <span data-ttu-id="c023a-155">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-155">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c023a-156">lastModifiedDateTime</span></span>|<span data-ttu-id="c023a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c023a-157">DateTimeOffset</span></span>|<span data-ttu-id="c023a-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c023a-158">The date and time the app was last modified.</span></span> <span data-ttu-id="c023a-159">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-159">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c023a-160">isFeatured</span></span>|<span data-ttu-id="c023a-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="c023a-161">Boolean</span></span>|<span data-ttu-id="c023a-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c023a-163">privacyInformationUrl</span></span>|<span data-ttu-id="c023a-164">字符串</span><span class="sxs-lookup"><span data-stu-id="c023a-164">String</span></span>|<span data-ttu-id="c023a-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="c023a-165">The privacy statement Url.</span></span> <span data-ttu-id="c023a-166">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-166">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c023a-167">informationUrl</span></span>|<span data-ttu-id="c023a-168">字符串</span><span class="sxs-lookup"><span data-stu-id="c023a-168">String</span></span>|<span data-ttu-id="c023a-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="c023a-169">The more information Url.</span></span> <span data-ttu-id="c023a-170">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-170">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-171">owner</span><span class="sxs-lookup"><span data-stu-id="c023a-171">owner</span></span>|<span data-ttu-id="c023a-172">String</span><span class="sxs-lookup"><span data-stu-id="c023a-172">String</span></span>|<span data-ttu-id="c023a-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="c023a-173">The owner of the app.</span></span> <span data-ttu-id="c023a-174">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-174">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-175">developer</span><span class="sxs-lookup"><span data-stu-id="c023a-175">developer</span></span>|<span data-ttu-id="c023a-176">字符串</span><span class="sxs-lookup"><span data-stu-id="c023a-176">String</span></span>|<span data-ttu-id="c023a-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="c023a-177">The developer of the app.</span></span> <span data-ttu-id="c023a-178">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-178">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-179">notes</span><span class="sxs-lookup"><span data-stu-id="c023a-179">notes</span></span>|<span data-ttu-id="c023a-180">字符串</span><span class="sxs-lookup"><span data-stu-id="c023a-180">String</span></span>|<span data-ttu-id="c023a-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="c023a-181">Notes for the app.</span></span> <span data-ttu-id="c023a-182">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-182">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="c023a-183">uploadState</span></span>|<span data-ttu-id="c023a-184">Int32</span><span class="sxs-lookup"><span data-stu-id="c023a-184">Int32</span></span>|<span data-ttu-id="c023a-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="c023a-185">The upload state.</span></span> <span data-ttu-id="c023a-186">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-186">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="c023a-187">publishingState</span></span>|[<span data-ttu-id="c023a-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c023a-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c023a-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="c023a-189">The publishing state for the app.</span></span> <span data-ttu-id="c023a-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="c023a-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c023a-191">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="c023a-191">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="c023a-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="c023a-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c023a-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c023a-193">isAssigned</span></span>|<span data-ttu-id="c023a-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="c023a-194">Boolean</span></span>|<span data-ttu-id="c023a-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="c023a-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c023a-196">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-196">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c023a-197">roleScopeTagIds</span></span>|<span data-ttu-id="c023a-198">String collection</span><span class="sxs-lookup"><span data-stu-id="c023a-198">String collection</span></span>|<span data-ttu-id="c023a-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="c023a-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c023a-200">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-200">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="c023a-201">dependentAppCount</span></span>|<span data-ttu-id="c023a-202">Int32</span><span class="sxs-lookup"><span data-stu-id="c023a-202">Int32</span></span>|<span data-ttu-id="c023a-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="c023a-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="c023a-204">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-204">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="c023a-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="c023a-205">committedContentVersion</span></span>|<span data-ttu-id="c023a-206">字符串</span><span class="sxs-lookup"><span data-stu-id="c023a-206">String</span></span>|<span data-ttu-id="c023a-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="c023a-207">The internal committed content version.</span></span> <span data-ttu-id="c023a-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c023a-209">fileName</span><span class="sxs-lookup"><span data-stu-id="c023a-209">fileName</span></span>|<span data-ttu-id="c023a-210">String</span><span class="sxs-lookup"><span data-stu-id="c023a-210">String</span></span>|<span data-ttu-id="c023a-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="c023a-211">The name of the main Lob application file.</span></span> <span data-ttu-id="c023a-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c023a-213">size</span><span class="sxs-lookup"><span data-stu-id="c023a-213">size</span></span>|<span data-ttu-id="c023a-214">Int64</span><span class="sxs-lookup"><span data-stu-id="c023a-214">Int64</span></span>|<span data-ttu-id="c023a-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="c023a-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="c023a-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c023a-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c023a-217">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="c023a-217">installCommandLine</span></span>|<span data-ttu-id="c023a-218">字符串</span><span class="sxs-lookup"><span data-stu-id="c023a-218">String</span></span>|<span data-ttu-id="c023a-219">要安装此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="c023a-219">The command line to install this app</span></span>|
|<span data-ttu-id="c023a-220">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="c023a-220">uninstallCommandLine</span></span>|<span data-ttu-id="c023a-221">字符串</span><span class="sxs-lookup"><span data-stu-id="c023a-221">String</span></span>|<span data-ttu-id="c023a-222">要卸载此应用程序的命令行</span><span class="sxs-lookup"><span data-stu-id="c023a-222">The command line to uninstall this app</span></span>|
|<span data-ttu-id="c023a-223">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="c023a-223">applicableArchitectures</span></span>|[<span data-ttu-id="c023a-224">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="c023a-224">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="c023a-225">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="c023a-225">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="c023a-226">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="c023a-226">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="c023a-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c023a-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c023a-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c023a-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="c023a-229">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="c023a-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="c023a-230">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="c023a-230">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="c023a-231">Int32</span><span class="sxs-lookup"><span data-stu-id="c023a-231">Int32</span></span>|<span data-ttu-id="c023a-232">安装此应用程序所需的最小可用磁盘空间的值。</span><span class="sxs-lookup"><span data-stu-id="c023a-232">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="c023a-233">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="c023a-233">minimumMemoryInMB</span></span>|<span data-ttu-id="c023a-234">Int32</span><span class="sxs-lookup"><span data-stu-id="c023a-234">Int32</span></span>|<span data-ttu-id="c023a-235">安装此应用程序所需的最小物理内存的值。</span><span class="sxs-lookup"><span data-stu-id="c023a-235">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="c023a-236">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="c023a-236">minimumNumberOfProcessors</span></span>|<span data-ttu-id="c023a-237">Int32</span><span class="sxs-lookup"><span data-stu-id="c023a-237">Int32</span></span>|<span data-ttu-id="c023a-238">安装此应用程序所需的最小处理器数的值。</span><span class="sxs-lookup"><span data-stu-id="c023a-238">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="c023a-239">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="c023a-239">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="c023a-240">Int32</span><span class="sxs-lookup"><span data-stu-id="c023a-240">Int32</span></span>|<span data-ttu-id="c023a-241">安装此应用程序所需的最低 CPU 速度的值。</span><span class="sxs-lookup"><span data-stu-id="c023a-241">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="c023a-242">detectionRules</span><span class="sxs-lookup"><span data-stu-id="c023a-242">detectionRules</span></span>|<span data-ttu-id="c023a-243">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)集合</span><span class="sxs-lookup"><span data-stu-id="c023a-243">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="c023a-244">检测到 Win32 业务线（LoB）应用程序的检测规则。</span><span class="sxs-lookup"><span data-stu-id="c023a-244">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c023a-245">requirementRules</span><span class="sxs-lookup"><span data-stu-id="c023a-245">requirementRules</span></span>|<span data-ttu-id="c023a-246">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)集合</span><span class="sxs-lookup"><span data-stu-id="c023a-246">[win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md) collection</span></span>|<span data-ttu-id="c023a-247">用于检测 Win32 业务线（LoB）应用程序的要求规则。</span><span class="sxs-lookup"><span data-stu-id="c023a-247">The requirement rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c023a-248">installExperience</span><span class="sxs-lookup"><span data-stu-id="c023a-248">installExperience</span></span>|[<span data-ttu-id="c023a-249">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="c023a-249">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="c023a-250">此应用的安装体验。</span><span class="sxs-lookup"><span data-stu-id="c023a-250">The install experience for this app.</span></span>|
|<span data-ttu-id="c023a-251">returnCodes</span><span class="sxs-lookup"><span data-stu-id="c023a-251">returnCodes</span></span>|<span data-ttu-id="c023a-252">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)集合</span><span class="sxs-lookup"><span data-stu-id="c023a-252">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="c023a-253">用于安装后行为的返回代码。</span><span class="sxs-lookup"><span data-stu-id="c023a-253">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="c023a-254">msiInformation</span><span class="sxs-lookup"><span data-stu-id="c023a-254">msiInformation</span></span>|[<span data-ttu-id="c023a-255">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="c023a-255">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="c023a-256">如果此 Win32 应用是 MSI 应用程序，则为 MSI 详细信息。</span><span class="sxs-lookup"><span data-stu-id="c023a-256">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="c023a-257">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="c023a-257">setupFilePath</span></span>|<span data-ttu-id="c023a-258">字符串</span><span class="sxs-lookup"><span data-stu-id="c023a-258">String</span></span>|<span data-ttu-id="c023a-259">加密的 Win32LobApp 包中的安装程序文件的相对路径。</span><span class="sxs-lookup"><span data-stu-id="c023a-259">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="c023a-260">响应</span><span class="sxs-lookup"><span data-stu-id="c023a-260">Response</span></span>
<span data-ttu-id="c023a-261">如果成功，此方法在响应`201 Created`正文中返回响应代码和[win32LobApp](../resources/intune-apps-win32lobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c023a-261">If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c023a-262">示例</span><span class="sxs-lookup"><span data-stu-id="c023a-262">Example</span></span>

### <a name="request"></a><span data-ttu-id="c023a-263">请求</span><span class="sxs-lookup"><span data-stu-id="c023a-263">Request</span></span>
<span data-ttu-id="c023a-264">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c023a-264">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2817

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
  "setupFilePath": "Setup File Path value"
}
```

### <a name="response"></a><span data-ttu-id="c023a-265">响应</span><span class="sxs-lookup"><span data-stu-id="c023a-265">Response</span></span>
<span data-ttu-id="c023a-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c023a-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2989

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
  "setupFilePath": "Setup File Path value"
}
```





