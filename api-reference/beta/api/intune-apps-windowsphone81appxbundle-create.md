---
title: 创建了 windowsphone81appxbundle
description: 创建新的了 windowsphone81appxbundle 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b727c08d71e9ca6e9efd54b040fe7cac8f96e85d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43409271"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="b0a0d-103">创建了 windowsphone81appxbundle</span><span class="sxs-lookup"><span data-stu-id="b0a0d-103">Create windowsPhone81AppXBundle</span></span>

<span data-ttu-id="b0a0d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0a0d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0a0d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0a0d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0a0d-107">创建新的[了 windowsphone81appxbundle](../resources/intune-apps-windowsphone81appxbundle.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-107">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0a0d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b0a0d-108">Prerequisites</span></span>
<span data-ttu-id="b0a0d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0a0d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0a0d-111">Permission type</span></span>|<span data-ttu-id="b0a0d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b0a0d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0a0d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0a0d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0a0d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0a0d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b0a0d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0a0d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0a0d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-116">Not supported.</span></span>|
|<span data-ttu-id="b0a0d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0a0d-117">Application</span></span>|<span data-ttu-id="b0a0d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0a0d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0a0d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0a0d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b0a0d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0a0d-120">Request headers</span></span>
|<span data-ttu-id="b0a0d-121">标头</span><span class="sxs-lookup"><span data-stu-id="b0a0d-121">Header</span></span>|<span data-ttu-id="b0a0d-122">值</span><span class="sxs-lookup"><span data-stu-id="b0a0d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0a0d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0a0d-123">Authorization</span></span>|<span data-ttu-id="b0a0d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0a0d-125">接受</span><span class="sxs-lookup"><span data-stu-id="b0a0d-125">Accept</span></span>|<span data-ttu-id="b0a0d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0a0d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0a0d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0a0d-127">Request body</span></span>
<span data-ttu-id="b0a0d-128">在请求正文中，提供了 windowsphone81appxbundle 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-128">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="b0a0d-129">下表显示创建了 windowsphone81appxbundle 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-129">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="b0a0d-130">属性</span><span class="sxs-lookup"><span data-stu-id="b0a0d-130">Property</span></span>|<span data-ttu-id="b0a0d-131">类型</span><span class="sxs-lookup"><span data-stu-id="b0a0d-131">Type</span></span>|<span data-ttu-id="b0a0d-132">说明</span><span class="sxs-lookup"><span data-stu-id="b0a0d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0a0d-133">id</span><span class="sxs-lookup"><span data-stu-id="b0a0d-133">id</span></span>|<span data-ttu-id="b0a0d-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b0a0d-134">String</span></span>|<span data-ttu-id="b0a0d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-135">Key of the entity.</span></span> <span data-ttu-id="b0a0d-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b0a0d-137">displayName</span></span>|<span data-ttu-id="b0a0d-138">String</span><span class="sxs-lookup"><span data-stu-id="b0a0d-138">String</span></span>|<span data-ttu-id="b0a0d-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b0a0d-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-141">description</span><span class="sxs-lookup"><span data-stu-id="b0a0d-141">description</span></span>|<span data-ttu-id="b0a0d-142">字符串</span><span class="sxs-lookup"><span data-stu-id="b0a0d-142">String</span></span>|<span data-ttu-id="b0a0d-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-143">The description of the app.</span></span> <span data-ttu-id="b0a0d-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-145">publisher</span><span class="sxs-lookup"><span data-stu-id="b0a0d-145">publisher</span></span>|<span data-ttu-id="b0a0d-146">String</span><span class="sxs-lookup"><span data-stu-id="b0a0d-146">String</span></span>|<span data-ttu-id="b0a0d-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-147">The publisher of the app.</span></span> <span data-ttu-id="b0a0d-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b0a0d-149">largeIcon</span></span>|[<span data-ttu-id="b0a0d-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b0a0d-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b0a0d-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b0a0d-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0a0d-153">createdDateTime</span></span>|<span data-ttu-id="b0a0d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0a0d-154">DateTimeOffset</span></span>|<span data-ttu-id="b0a0d-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-155">The date and time the app was created.</span></span> <span data-ttu-id="b0a0d-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0a0d-157">lastModifiedDateTime</span></span>|<span data-ttu-id="b0a0d-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0a0d-158">DateTimeOffset</span></span>|<span data-ttu-id="b0a0d-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-159">The date and time the app was last modified.</span></span> <span data-ttu-id="b0a0d-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b0a0d-161">isFeatured</span></span>|<span data-ttu-id="b0a0d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a0d-162">Boolean</span></span>|<span data-ttu-id="b0a0d-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b0a0d-164">privacyInformationUrl</span></span>|<span data-ttu-id="b0a0d-165">String</span><span class="sxs-lookup"><span data-stu-id="b0a0d-165">String</span></span>|<span data-ttu-id="b0a0d-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-166">The privacy statement Url.</span></span> <span data-ttu-id="b0a0d-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b0a0d-168">informationUrl</span></span>|<span data-ttu-id="b0a0d-169">String</span><span class="sxs-lookup"><span data-stu-id="b0a0d-169">String</span></span>|<span data-ttu-id="b0a0d-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-170">The more information Url.</span></span> <span data-ttu-id="b0a0d-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-172">owner</span><span class="sxs-lookup"><span data-stu-id="b0a0d-172">owner</span></span>|<span data-ttu-id="b0a0d-173">String</span><span class="sxs-lookup"><span data-stu-id="b0a0d-173">String</span></span>|<span data-ttu-id="b0a0d-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-174">The owner of the app.</span></span> <span data-ttu-id="b0a0d-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-176">developer</span><span class="sxs-lookup"><span data-stu-id="b0a0d-176">developer</span></span>|<span data-ttu-id="b0a0d-177">String</span><span class="sxs-lookup"><span data-stu-id="b0a0d-177">String</span></span>|<span data-ttu-id="b0a0d-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-178">The developer of the app.</span></span> <span data-ttu-id="b0a0d-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-180">notes</span><span class="sxs-lookup"><span data-stu-id="b0a0d-180">notes</span></span>|<span data-ttu-id="b0a0d-181">String</span><span class="sxs-lookup"><span data-stu-id="b0a0d-181">String</span></span>|<span data-ttu-id="b0a0d-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-182">Notes for the app.</span></span> <span data-ttu-id="b0a0d-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="b0a0d-184">uploadState</span></span>|<span data-ttu-id="b0a0d-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a0d-185">Int32</span></span>|<span data-ttu-id="b0a0d-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-186">The upload state.</span></span> <span data-ttu-id="b0a0d-187">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-187">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="b0a0d-188">publishingState</span></span>|[<span data-ttu-id="b0a0d-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b0a0d-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b0a0d-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-190">The publishing state for the app.</span></span> <span data-ttu-id="b0a0d-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b0a0d-192">继承自[mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-192">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="b0a0d-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b0a0d-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b0a0d-194">isAssigned</span></span>|<span data-ttu-id="b0a0d-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0a0d-195">Boolean</span></span>|<span data-ttu-id="b0a0d-196">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b0a0d-197">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-197">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b0a0d-198">roleScopeTagIds</span></span>|<span data-ttu-id="b0a0d-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="b0a0d-199">String collection</span></span>|<span data-ttu-id="b0a0d-200">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b0a0d-201">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-201">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-202">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b0a0d-202">dependentAppCount</span></span>|<span data-ttu-id="b0a0d-203">Int32</span><span class="sxs-lookup"><span data-stu-id="b0a0d-203">Int32</span></span>|<span data-ttu-id="b0a0d-204">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-204">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b0a0d-205">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-205">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b0a0d-206">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b0a0d-206">committedContentVersion</span></span>|<span data-ttu-id="b0a0d-207">String</span><span class="sxs-lookup"><span data-stu-id="b0a0d-207">String</span></span>|<span data-ttu-id="b0a0d-208">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-208">The internal committed content version.</span></span> <span data-ttu-id="b0a0d-209">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b0a0d-210">fileName</span><span class="sxs-lookup"><span data-stu-id="b0a0d-210">fileName</span></span>|<span data-ttu-id="b0a0d-211">String</span><span class="sxs-lookup"><span data-stu-id="b0a0d-211">String</span></span>|<span data-ttu-id="b0a0d-212">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-212">The name of the main Lob application file.</span></span> <span data-ttu-id="b0a0d-213">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b0a0d-214">size</span><span class="sxs-lookup"><span data-stu-id="b0a0d-214">size</span></span>|<span data-ttu-id="b0a0d-215">Int64</span><span class="sxs-lookup"><span data-stu-id="b0a0d-215">Int64</span></span>|<span data-ttu-id="b0a0d-216">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-216">The total size, including all uploaded files.</span></span> <span data-ttu-id="b0a0d-217">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-217">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b0a0d-218">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="b0a0d-218">applicableArchitectures</span></span>|[<span data-ttu-id="b0a0d-219">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b0a0d-219">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b0a0d-220">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-220">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="b0a0d-221">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-221">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="b0a0d-222">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="b0a0d-223">identityName</span><span class="sxs-lookup"><span data-stu-id="b0a0d-223">identityName</span></span>|<span data-ttu-id="b0a0d-224">String</span><span class="sxs-lookup"><span data-stu-id="b0a0d-224">String</span></span>|<span data-ttu-id="b0a0d-225">标识名称。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-225">The Identity Name.</span></span> <span data-ttu-id="b0a0d-226">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-226">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b0a0d-227">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="b0a0d-227">identityPublisherHash</span></span>|<span data-ttu-id="b0a0d-228">String</span><span class="sxs-lookup"><span data-stu-id="b0a0d-228">String</span></span>|<span data-ttu-id="b0a0d-229">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-229">The Identity Publisher Hash.</span></span> <span data-ttu-id="b0a0d-230">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b0a0d-231">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b0a0d-231">identityResourceIdentifier</span></span>|<span data-ttu-id="b0a0d-232">String</span><span class="sxs-lookup"><span data-stu-id="b0a0d-232">String</span></span>|<span data-ttu-id="b0a0d-233">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-233">The Identity Resource Identifier.</span></span> <span data-ttu-id="b0a0d-234">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-234">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b0a0d-235">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b0a0d-235">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b0a0d-236">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b0a0d-236">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="b0a0d-237">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-237">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="b0a0d-238">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-238">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b0a0d-239">将 phoneproductidentifier</span><span class="sxs-lookup"><span data-stu-id="b0a0d-239">phoneProductIdentifier</span></span>|<span data-ttu-id="b0a0d-240">String</span><span class="sxs-lookup"><span data-stu-id="b0a0d-240">String</span></span>|<span data-ttu-id="b0a0d-241">电话产品标识符。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-241">The Phone Product Identifier.</span></span> <span data-ttu-id="b0a0d-242">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-242">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b0a0d-243">将 phonepublisherid</span><span class="sxs-lookup"><span data-stu-id="b0a0d-243">phonePublisherId</span></span>|<span data-ttu-id="b0a0d-244">String</span><span class="sxs-lookup"><span data-stu-id="b0a0d-244">String</span></span>|<span data-ttu-id="b0a0d-245">电话发布者 Id。继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-245">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b0a0d-246">identityVersion</span><span class="sxs-lookup"><span data-stu-id="b0a0d-246">identityVersion</span></span>|<span data-ttu-id="b0a0d-247">String</span><span class="sxs-lookup"><span data-stu-id="b0a0d-247">String</span></span>|<span data-ttu-id="b0a0d-248">标识版本。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-248">The identity version.</span></span> <span data-ttu-id="b0a0d-249">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="b0a0d-249">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="b0a0d-250">将 appxpackageinformationlist</span><span class="sxs-lookup"><span data-stu-id="b0a0d-250">appXPackageInformationList</span></span>|<span data-ttu-id="b0a0d-251">[了 windowspackageinformation](../resources/intune-apps-windowspackageinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="b0a0d-251">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="b0a0d-252">AppX 包信息的列表。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-252">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="b0a0d-253">响应</span><span class="sxs-lookup"><span data-stu-id="b0a0d-253">Response</span></span>
<span data-ttu-id="b0a0d-254">如果成功，此方法在响应`201 Created`正文中返回响应代码和[了 windowsphone81appxbundle](../resources/intune-apps-windowsphone81appxbundle.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-254">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0a0d-255">示例</span><span class="sxs-lookup"><span data-stu-id="b0a0d-255">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0a0d-256">请求</span><span class="sxs-lookup"><span data-stu-id="b0a0d-256">Request</span></span>
<span data-ttu-id="b0a0d-257">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-257">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b0a0d-258">响应</span><span class="sxs-lookup"><span data-stu-id="b0a0d-258">Response</span></span>
<span data-ttu-id="b0a0d-p129">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b0a0d-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



