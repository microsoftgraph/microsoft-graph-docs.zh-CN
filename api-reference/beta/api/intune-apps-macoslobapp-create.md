---
title: 创建 macOSLobApp
description: 创建新的 macOSLobApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a82e0d63789a2edef8cf2eb267bafeba29b2117d
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792112"
---
# <a name="create-macoslobapp"></a><span data-ttu-id="563f7-103">创建 macOSLobApp</span><span class="sxs-lookup"><span data-stu-id="563f7-103">Create macOSLobApp</span></span>

<span data-ttu-id="563f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="563f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="563f7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="563f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="563f7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="563f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="563f7-107">创建新的 [macOSLobApp](../resources/intune-apps-macoslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="563f7-107">Create a new [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="563f7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="563f7-108">Prerequisites</span></span>
<span data-ttu-id="563f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="563f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="563f7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="563f7-111">Permission type</span></span>|<span data-ttu-id="563f7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="563f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="563f7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="563f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="563f7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="563f7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="563f7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="563f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="563f7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="563f7-116">Not supported.</span></span>|
|<span data-ttu-id="563f7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="563f7-117">Application</span></span>|<span data-ttu-id="563f7-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="563f7-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="563f7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="563f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="563f7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="563f7-120">Request headers</span></span>
|<span data-ttu-id="563f7-121">标头</span><span class="sxs-lookup"><span data-stu-id="563f7-121">Header</span></span>|<span data-ttu-id="563f7-122">值</span><span class="sxs-lookup"><span data-stu-id="563f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="563f7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="563f7-123">Authorization</span></span>|<span data-ttu-id="563f7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="563f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="563f7-125">接受</span><span class="sxs-lookup"><span data-stu-id="563f7-125">Accept</span></span>|<span data-ttu-id="563f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="563f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="563f7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="563f7-127">Request body</span></span>
<span data-ttu-id="563f7-128">在请求正文中，提供 macOSLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="563f7-128">In the request body, supply a JSON representation for the macOSLobApp object.</span></span>

<span data-ttu-id="563f7-129">下表显示创建 macOSLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="563f7-129">The following table shows the properties that are required when you create the macOSLobApp.</span></span>

|<span data-ttu-id="563f7-130">属性</span><span class="sxs-lookup"><span data-stu-id="563f7-130">Property</span></span>|<span data-ttu-id="563f7-131">类型</span><span class="sxs-lookup"><span data-stu-id="563f7-131">Type</span></span>|<span data-ttu-id="563f7-132">说明</span><span class="sxs-lookup"><span data-stu-id="563f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="563f7-133">id</span><span class="sxs-lookup"><span data-stu-id="563f7-133">id</span></span>|<span data-ttu-id="563f7-134">String</span><span class="sxs-lookup"><span data-stu-id="563f7-134">String</span></span>|<span data-ttu-id="563f7-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="563f7-135">Key of the entity.</span></span> <span data-ttu-id="563f7-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="563f7-137">displayName</span></span>|<span data-ttu-id="563f7-138">String</span><span class="sxs-lookup"><span data-stu-id="563f7-138">String</span></span>|<span data-ttu-id="563f7-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="563f7-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="563f7-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-141">description</span><span class="sxs-lookup"><span data-stu-id="563f7-141">description</span></span>|<span data-ttu-id="563f7-142">String</span><span class="sxs-lookup"><span data-stu-id="563f7-142">String</span></span>|<span data-ttu-id="563f7-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="563f7-143">The description of the app.</span></span> <span data-ttu-id="563f7-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-145">publisher</span><span class="sxs-lookup"><span data-stu-id="563f7-145">publisher</span></span>|<span data-ttu-id="563f7-146">String</span><span class="sxs-lookup"><span data-stu-id="563f7-146">String</span></span>|<span data-ttu-id="563f7-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="563f7-147">The publisher of the app.</span></span> <span data-ttu-id="563f7-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="563f7-149">largeIcon</span></span>|[<span data-ttu-id="563f7-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="563f7-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="563f7-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="563f7-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="563f7-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="563f7-153">createdDateTime</span></span>|<span data-ttu-id="563f7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="563f7-154">DateTimeOffset</span></span>|<span data-ttu-id="563f7-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="563f7-155">The date and time the app was created.</span></span> <span data-ttu-id="563f7-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="563f7-157">lastModifiedDateTime</span></span>|<span data-ttu-id="563f7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="563f7-158">DateTimeOffset</span></span>|<span data-ttu-id="563f7-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="563f7-159">The date and time the app was last modified.</span></span> <span data-ttu-id="563f7-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="563f7-161">isFeatured</span></span>|<span data-ttu-id="563f7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="563f7-162">Boolean</span></span>|<span data-ttu-id="563f7-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="563f7-164">privacyInformationUrl</span></span>|<span data-ttu-id="563f7-165">String</span><span class="sxs-lookup"><span data-stu-id="563f7-165">String</span></span>|<span data-ttu-id="563f7-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="563f7-166">The privacy statement Url.</span></span> <span data-ttu-id="563f7-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="563f7-168">informationUrl</span></span>|<span data-ttu-id="563f7-169">String</span><span class="sxs-lookup"><span data-stu-id="563f7-169">String</span></span>|<span data-ttu-id="563f7-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="563f7-170">The more information Url.</span></span> <span data-ttu-id="563f7-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-172">所有者</span><span class="sxs-lookup"><span data-stu-id="563f7-172">owner</span></span>|<span data-ttu-id="563f7-173">String</span><span class="sxs-lookup"><span data-stu-id="563f7-173">String</span></span>|<span data-ttu-id="563f7-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="563f7-174">The owner of the app.</span></span> <span data-ttu-id="563f7-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-176">developer</span><span class="sxs-lookup"><span data-stu-id="563f7-176">developer</span></span>|<span data-ttu-id="563f7-177">String</span><span class="sxs-lookup"><span data-stu-id="563f7-177">String</span></span>|<span data-ttu-id="563f7-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="563f7-178">The developer of the app.</span></span> <span data-ttu-id="563f7-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-180">notes</span><span class="sxs-lookup"><span data-stu-id="563f7-180">notes</span></span>|<span data-ttu-id="563f7-181">String</span><span class="sxs-lookup"><span data-stu-id="563f7-181">String</span></span>|<span data-ttu-id="563f7-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="563f7-182">Notes for the app.</span></span> <span data-ttu-id="563f7-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="563f7-184">uploadState</span></span>|<span data-ttu-id="563f7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="563f7-185">Int32</span></span>|<span data-ttu-id="563f7-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="563f7-186">The upload state.</span></span> <span data-ttu-id="563f7-187">可能的值包括： 0- `Not Ready` 、1- `Ready` 、2- `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="563f7-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="563f7-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="563f7-189">publishingState</span></span>|[<span data-ttu-id="563f7-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="563f7-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="563f7-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="563f7-191">The publishing state for the app.</span></span> <span data-ttu-id="563f7-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="563f7-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="563f7-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="563f7-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="563f7-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="563f7-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="563f7-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="563f7-195">isAssigned</span></span>|<span data-ttu-id="563f7-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="563f7-196">Boolean</span></span>|<span data-ttu-id="563f7-197">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="563f7-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="563f7-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="563f7-199">roleScopeTagIds</span></span>|<span data-ttu-id="563f7-200">字符串集合</span><span class="sxs-lookup"><span data-stu-id="563f7-200">String collection</span></span>|<span data-ttu-id="563f7-201">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="563f7-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="563f7-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="563f7-203">dependentAppCount</span></span>|<span data-ttu-id="563f7-204">Int32</span><span class="sxs-lookup"><span data-stu-id="563f7-204">Int32</span></span>|<span data-ttu-id="563f7-205">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="563f7-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="563f7-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="563f7-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="563f7-207">committedContentVersion</span></span>|<span data-ttu-id="563f7-208">String</span><span class="sxs-lookup"><span data-stu-id="563f7-208">String</span></span>|<span data-ttu-id="563f7-209">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="563f7-209">The internal committed content version.</span></span> <span data-ttu-id="563f7-210">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="563f7-211">fileName</span><span class="sxs-lookup"><span data-stu-id="563f7-211">fileName</span></span>|<span data-ttu-id="563f7-212">String</span><span class="sxs-lookup"><span data-stu-id="563f7-212">String</span></span>|<span data-ttu-id="563f7-213">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="563f7-213">The name of the main Lob application file.</span></span> <span data-ttu-id="563f7-214">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="563f7-215">size</span><span class="sxs-lookup"><span data-stu-id="563f7-215">size</span></span>|<span data-ttu-id="563f7-216">Int64</span><span class="sxs-lookup"><span data-stu-id="563f7-216">Int64</span></span>|<span data-ttu-id="563f7-217">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="563f7-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="563f7-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="563f7-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="563f7-219">bundleId</span><span class="sxs-lookup"><span data-stu-id="563f7-219">bundleId</span></span>|<span data-ttu-id="563f7-220">String</span><span class="sxs-lookup"><span data-stu-id="563f7-220">String</span></span>|<span data-ttu-id="563f7-221">捆绑包 id。</span><span class="sxs-lookup"><span data-stu-id="563f7-221">The bundle id.</span></span>|
|<span data-ttu-id="563f7-222">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="563f7-222">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="563f7-223">macOSMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="563f7-223">macOSMinimumOperatingSystem</span></span>](../resources/intune-apps-macosminimumoperatingsystem.md)|<span data-ttu-id="563f7-224">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="563f7-224">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="563f7-225">buildNumber</span><span class="sxs-lookup"><span data-stu-id="563f7-225">buildNumber</span></span>|<span data-ttu-id="563f7-226">String</span><span class="sxs-lookup"><span data-stu-id="563f7-226">String</span></span>|<span data-ttu-id="563f7-227">MacOS 业务线 (LoB) 应用程序的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="563f7-227">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="563f7-228">versionNumber</span><span class="sxs-lookup"><span data-stu-id="563f7-228">versionNumber</span></span>|<span data-ttu-id="563f7-229">String</span><span class="sxs-lookup"><span data-stu-id="563f7-229">String</span></span>|<span data-ttu-id="563f7-230">MacOS 业务线 (LoB) 应用程序的版本号。</span><span class="sxs-lookup"><span data-stu-id="563f7-230">The version number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="563f7-231">childApps</span><span class="sxs-lookup"><span data-stu-id="563f7-231">childApps</span></span>|<span data-ttu-id="563f7-232">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="563f7-232">[macOSLobChildApp](../resources/intune-apps-macoslobchildapp.md) collection</span></span>|<span data-ttu-id="563f7-233">此捆绑包包中的应用程序列表</span><span class="sxs-lookup"><span data-stu-id="563f7-233">The app list in this bundle package</span></span>|
|<span data-ttu-id="563f7-234">identityVersion</span><span class="sxs-lookup"><span data-stu-id="563f7-234">identityVersion</span></span>|<span data-ttu-id="563f7-235">String</span><span class="sxs-lookup"><span data-stu-id="563f7-235">String</span></span>|<span data-ttu-id="563f7-236">标识版本。</span><span class="sxs-lookup"><span data-stu-id="563f7-236">The identity version.</span></span>|
|<span data-ttu-id="563f7-237">md5HashChunkSize</span><span class="sxs-lookup"><span data-stu-id="563f7-237">md5HashChunkSize</span></span>|<span data-ttu-id="563f7-238">Int32</span><span class="sxs-lookup"><span data-stu-id="563f7-238">Int32</span></span>|<span data-ttu-id="563f7-239">MD5 哈希的块大小</span><span class="sxs-lookup"><span data-stu-id="563f7-239">The chunk size for MD5 hash</span></span>|
|<span data-ttu-id="563f7-240">md5Hash</span><span class="sxs-lookup"><span data-stu-id="563f7-240">md5Hash</span></span>|<span data-ttu-id="563f7-241">字符串集合</span><span class="sxs-lookup"><span data-stu-id="563f7-241">String collection</span></span>|<span data-ttu-id="563f7-242">MD5 哈希代码</span><span class="sxs-lookup"><span data-stu-id="563f7-242">The MD5 hash codes</span></span>|
|<span data-ttu-id="563f7-243">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="563f7-243">ignoreVersionDetection</span></span>|<span data-ttu-id="563f7-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="563f7-244">Boolean</span></span>|<span data-ttu-id="563f7-245">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="563f7-245">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="563f7-246">将此值设置为 true，以便 macOS 业务线 (LoB) 使用自我更新功能的应用程序。</span><span class="sxs-lookup"><span data-stu-id="563f7-246">Set this to true for macOS Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="563f7-247">响应</span><span class="sxs-lookup"><span data-stu-id="563f7-247">Response</span></span>
<span data-ttu-id="563f7-248">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [macOSLobApp](../resources/intune-apps-macoslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="563f7-248">If successful, this method returns a `201 Created` response code and a [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="563f7-249">示例</span><span class="sxs-lookup"><span data-stu-id="563f7-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="563f7-250">请求</span><span class="sxs-lookup"><span data-stu-id="563f7-250">Request</span></span>
<span data-ttu-id="563f7-251">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="563f7-251">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1616

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
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
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="563f7-252">响应</span><span class="sxs-lookup"><span data-stu-id="563f7-252">Response</span></span>
<span data-ttu-id="563f7-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="563f7-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1788

{
  "@odata.type": "#microsoft.graph.macOSLobApp",
  "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
  "bundleId": "Bundle Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
    "v10_7": true,
    "v10_8": true,
    "v10_9": true,
    "v10_10": true,
    "v10_11": true,
    "v10_12": true,
    "v10_13": true,
    "v10_14": true,
    "v10_15": true
  },
  "buildNumber": "Build Number value",
  "versionNumber": "Version Number value",
  "childApps": [
    {
      "@odata.type": "microsoft.graph.macOSLobChildApp",
      "bundleId": "Bundle Id value",
      "buildNumber": "Build Number value",
      "versionNumber": "Version Number value"
    }
  ],
  "identityVersion": "Identity Version value",
  "md5HashChunkSize": 0,
  "md5Hash": [
    "Md5Hash value"
  ],
  "ignoreVersionDetection": true
}
```



