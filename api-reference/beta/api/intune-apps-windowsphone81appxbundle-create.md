---
title: 创建了 windowsphone81appxbundle
description: 创建新的了 windowsphone81appxbundle 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e0130112b9706b041203e5c233d4ec53b78b8b6d
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790985"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="db1af-103">创建了 windowsphone81appxbundle</span><span class="sxs-lookup"><span data-stu-id="db1af-103">Create windowsPhone81AppXBundle</span></span>

<span data-ttu-id="db1af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db1af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="db1af-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db1af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db1af-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db1af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db1af-107">创建新的 [了 windowsphone81appxbundle](../resources/intune-apps-windowsphone81appxbundle.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db1af-107">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db1af-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="db1af-108">Prerequisites</span></span>
<span data-ttu-id="db1af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db1af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db1af-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="db1af-111">Permission type</span></span>|<span data-ttu-id="db1af-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="db1af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db1af-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db1af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db1af-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db1af-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="db1af-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db1af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db1af-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="db1af-116">Not supported.</span></span>|
|<span data-ttu-id="db1af-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="db1af-117">Application</span></span>|<span data-ttu-id="db1af-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db1af-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="db1af-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db1af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="db1af-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="db1af-120">Request headers</span></span>
|<span data-ttu-id="db1af-121">标头</span><span class="sxs-lookup"><span data-stu-id="db1af-121">Header</span></span>|<span data-ttu-id="db1af-122">值</span><span class="sxs-lookup"><span data-stu-id="db1af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db1af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="db1af-123">Authorization</span></span>|<span data-ttu-id="db1af-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db1af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db1af-125">接受</span><span class="sxs-lookup"><span data-stu-id="db1af-125">Accept</span></span>|<span data-ttu-id="db1af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db1af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db1af-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="db1af-127">Request body</span></span>
<span data-ttu-id="db1af-128">在请求正文中，提供了 windowsphone81appxbundle 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db1af-128">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="db1af-129">下表显示创建了 windowsphone81appxbundle 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="db1af-129">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="db1af-130">属性</span><span class="sxs-lookup"><span data-stu-id="db1af-130">Property</span></span>|<span data-ttu-id="db1af-131">类型</span><span class="sxs-lookup"><span data-stu-id="db1af-131">Type</span></span>|<span data-ttu-id="db1af-132">说明</span><span class="sxs-lookup"><span data-stu-id="db1af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db1af-133">id</span><span class="sxs-lookup"><span data-stu-id="db1af-133">id</span></span>|<span data-ttu-id="db1af-134">String</span><span class="sxs-lookup"><span data-stu-id="db1af-134">String</span></span>|<span data-ttu-id="db1af-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="db1af-135">Key of the entity.</span></span> <span data-ttu-id="db1af-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-137">displayName</span><span class="sxs-lookup"><span data-stu-id="db1af-137">displayName</span></span>|<span data-ttu-id="db1af-138">String</span><span class="sxs-lookup"><span data-stu-id="db1af-138">String</span></span>|<span data-ttu-id="db1af-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="db1af-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="db1af-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-141">description</span><span class="sxs-lookup"><span data-stu-id="db1af-141">description</span></span>|<span data-ttu-id="db1af-142">String</span><span class="sxs-lookup"><span data-stu-id="db1af-142">String</span></span>|<span data-ttu-id="db1af-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="db1af-143">The description of the app.</span></span> <span data-ttu-id="db1af-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-145">publisher</span><span class="sxs-lookup"><span data-stu-id="db1af-145">publisher</span></span>|<span data-ttu-id="db1af-146">String</span><span class="sxs-lookup"><span data-stu-id="db1af-146">String</span></span>|<span data-ttu-id="db1af-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="db1af-147">The publisher of the app.</span></span> <span data-ttu-id="db1af-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="db1af-149">largeIcon</span></span>|[<span data-ttu-id="db1af-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="db1af-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="db1af-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="db1af-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="db1af-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db1af-153">createdDateTime</span></span>|<span data-ttu-id="db1af-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db1af-154">DateTimeOffset</span></span>|<span data-ttu-id="db1af-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="db1af-155">The date and time the app was created.</span></span> <span data-ttu-id="db1af-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db1af-157">lastModifiedDateTime</span></span>|<span data-ttu-id="db1af-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db1af-158">DateTimeOffset</span></span>|<span data-ttu-id="db1af-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="db1af-159">The date and time the app was last modified.</span></span> <span data-ttu-id="db1af-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="db1af-161">isFeatured</span></span>|<span data-ttu-id="db1af-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="db1af-162">Boolean</span></span>|<span data-ttu-id="db1af-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="db1af-164">privacyInformationUrl</span></span>|<span data-ttu-id="db1af-165">String</span><span class="sxs-lookup"><span data-stu-id="db1af-165">String</span></span>|<span data-ttu-id="db1af-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="db1af-166">The privacy statement Url.</span></span> <span data-ttu-id="db1af-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="db1af-168">informationUrl</span></span>|<span data-ttu-id="db1af-169">String</span><span class="sxs-lookup"><span data-stu-id="db1af-169">String</span></span>|<span data-ttu-id="db1af-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="db1af-170">The more information Url.</span></span> <span data-ttu-id="db1af-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-172">所有者</span><span class="sxs-lookup"><span data-stu-id="db1af-172">owner</span></span>|<span data-ttu-id="db1af-173">String</span><span class="sxs-lookup"><span data-stu-id="db1af-173">String</span></span>|<span data-ttu-id="db1af-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="db1af-174">The owner of the app.</span></span> <span data-ttu-id="db1af-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-176">developer</span><span class="sxs-lookup"><span data-stu-id="db1af-176">developer</span></span>|<span data-ttu-id="db1af-177">String</span><span class="sxs-lookup"><span data-stu-id="db1af-177">String</span></span>|<span data-ttu-id="db1af-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="db1af-178">The developer of the app.</span></span> <span data-ttu-id="db1af-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-180">notes</span><span class="sxs-lookup"><span data-stu-id="db1af-180">notes</span></span>|<span data-ttu-id="db1af-181">String</span><span class="sxs-lookup"><span data-stu-id="db1af-181">String</span></span>|<span data-ttu-id="db1af-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="db1af-182">Notes for the app.</span></span> <span data-ttu-id="db1af-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="db1af-184">uploadState</span></span>|<span data-ttu-id="db1af-185">Int32</span><span class="sxs-lookup"><span data-stu-id="db1af-185">Int32</span></span>|<span data-ttu-id="db1af-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="db1af-186">The upload state.</span></span> <span data-ttu-id="db1af-187">可能的值包括： 0- `Not Ready` 、1- `Ready` 、2- `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="db1af-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="db1af-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="db1af-189">publishingState</span></span>|[<span data-ttu-id="db1af-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="db1af-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="db1af-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="db1af-191">The publishing state for the app.</span></span> <span data-ttu-id="db1af-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="db1af-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="db1af-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="db1af-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="db1af-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="db1af-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="db1af-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="db1af-195">isAssigned</span></span>|<span data-ttu-id="db1af-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="db1af-196">Boolean</span></span>|<span data-ttu-id="db1af-197">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="db1af-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="db1af-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="db1af-199">roleScopeTagIds</span></span>|<span data-ttu-id="db1af-200">字符串集合</span><span class="sxs-lookup"><span data-stu-id="db1af-200">String collection</span></span>|<span data-ttu-id="db1af-201">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="db1af-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="db1af-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="db1af-203">dependentAppCount</span></span>|<span data-ttu-id="db1af-204">Int32</span><span class="sxs-lookup"><span data-stu-id="db1af-204">Int32</span></span>|<span data-ttu-id="db1af-205">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="db1af-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="db1af-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="db1af-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="db1af-207">committedContentVersion</span></span>|<span data-ttu-id="db1af-208">String</span><span class="sxs-lookup"><span data-stu-id="db1af-208">String</span></span>|<span data-ttu-id="db1af-209">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="db1af-209">The internal committed content version.</span></span> <span data-ttu-id="db1af-210">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="db1af-211">fileName</span><span class="sxs-lookup"><span data-stu-id="db1af-211">fileName</span></span>|<span data-ttu-id="db1af-212">String</span><span class="sxs-lookup"><span data-stu-id="db1af-212">String</span></span>|<span data-ttu-id="db1af-213">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="db1af-213">The name of the main Lob application file.</span></span> <span data-ttu-id="db1af-214">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="db1af-215">size</span><span class="sxs-lookup"><span data-stu-id="db1af-215">size</span></span>|<span data-ttu-id="db1af-216">Int64</span><span class="sxs-lookup"><span data-stu-id="db1af-216">Int64</span></span>|<span data-ttu-id="db1af-217">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="db1af-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="db1af-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="db1af-219">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="db1af-219">applicableArchitectures</span></span>|[<span data-ttu-id="db1af-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="db1af-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="db1af-221">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="db1af-221">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="db1af-222">继承自 [了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)。</span><span class="sxs-lookup"><span data-stu-id="db1af-222">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="db1af-223">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="db1af-223">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="db1af-224">identityName</span><span class="sxs-lookup"><span data-stu-id="db1af-224">identityName</span></span>|<span data-ttu-id="db1af-225">String</span><span class="sxs-lookup"><span data-stu-id="db1af-225">String</span></span>|<span data-ttu-id="db1af-226">标识名称。</span><span class="sxs-lookup"><span data-stu-id="db1af-226">The Identity Name.</span></span> <span data-ttu-id="db1af-227">继承自 [了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-227">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="db1af-228">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="db1af-228">identityPublisherHash</span></span>|<span data-ttu-id="db1af-229">String</span><span class="sxs-lookup"><span data-stu-id="db1af-229">String</span></span>|<span data-ttu-id="db1af-230">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="db1af-230">The Identity Publisher Hash.</span></span> <span data-ttu-id="db1af-231">继承自 [了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-231">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="db1af-232">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="db1af-232">identityResourceIdentifier</span></span>|<span data-ttu-id="db1af-233">String</span><span class="sxs-lookup"><span data-stu-id="db1af-233">String</span></span>|<span data-ttu-id="db1af-234">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="db1af-234">The Identity Resource Identifier.</span></span> <span data-ttu-id="db1af-235">继承自 [了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-235">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="db1af-236">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="db1af-236">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="db1af-237">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="db1af-237">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="db1af-238">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="db1af-238">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="db1af-239">继承自 [了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-239">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="db1af-240">将 phoneproductidentifier</span><span class="sxs-lookup"><span data-stu-id="db1af-240">phoneProductIdentifier</span></span>|<span data-ttu-id="db1af-241">String</span><span class="sxs-lookup"><span data-stu-id="db1af-241">String</span></span>|<span data-ttu-id="db1af-242">电话产品标识符。</span><span class="sxs-lookup"><span data-stu-id="db1af-242">The Phone Product Identifier.</span></span> <span data-ttu-id="db1af-243">继承自 [了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-243">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="db1af-244">将 phonepublisherid</span><span class="sxs-lookup"><span data-stu-id="db1af-244">phonePublisherId</span></span>|<span data-ttu-id="db1af-245">String</span><span class="sxs-lookup"><span data-stu-id="db1af-245">String</span></span>|<span data-ttu-id="db1af-246">电话发布者 Id。继承自 [了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-246">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="db1af-247">identityVersion</span><span class="sxs-lookup"><span data-stu-id="db1af-247">identityVersion</span></span>|<span data-ttu-id="db1af-248">String</span><span class="sxs-lookup"><span data-stu-id="db1af-248">String</span></span>|<span data-ttu-id="db1af-249">标识版本。</span><span class="sxs-lookup"><span data-stu-id="db1af-249">The identity version.</span></span> <span data-ttu-id="db1af-250">继承自 [了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="db1af-250">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="db1af-251">将 appxpackageinformationlist</span><span class="sxs-lookup"><span data-stu-id="db1af-251">appXPackageInformationList</span></span>|<span data-ttu-id="db1af-252">[了 windowspackageinformation](../resources/intune-apps-windowspackageinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="db1af-252">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="db1af-253">AppX 包信息的列表。</span><span class="sxs-lookup"><span data-stu-id="db1af-253">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="db1af-254">响应</span><span class="sxs-lookup"><span data-stu-id="db1af-254">Response</span></span>
<span data-ttu-id="db1af-255">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [了 windowsphone81appxbundle](../resources/intune-apps-windowsphone81appxbundle.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db1af-255">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db1af-256">示例</span><span class="sxs-lookup"><span data-stu-id="db1af-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="db1af-257">请求</span><span class="sxs-lookup"><span data-stu-id="db1af-257">Request</span></span>
<span data-ttu-id="db1af-258">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db1af-258">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2311

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
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
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="db1af-259">响应</span><span class="sxs-lookup"><span data-stu-id="db1af-259">Response</span></span>
<span data-ttu-id="db1af-p129">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db1af-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2483

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
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
      }
    }
  ]
}
```



