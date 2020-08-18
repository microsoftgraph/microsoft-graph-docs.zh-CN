---
title: 创建 windowsAppX
description: 创建新的 windowsAppX 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 12854a2bcb5668634eef96a4063a857d460a455a
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791545"
---
# <a name="create-windowsappx"></a><span data-ttu-id="b4603-103">创建 windowsAppX</span><span class="sxs-lookup"><span data-stu-id="b4603-103">Create windowsAppX</span></span>

<span data-ttu-id="b4603-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4603-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4603-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b4603-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4603-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4603-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4603-107">创建新的 [windowsAppX](../resources/intune-apps-windowsappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b4603-107">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4603-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b4603-108">Prerequisites</span></span>
<span data-ttu-id="b4603-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4603-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4603-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4603-111">Permission type</span></span>|<span data-ttu-id="b4603-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b4603-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4603-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4603-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4603-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4603-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b4603-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4603-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4603-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4603-116">Not supported.</span></span>|
|<span data-ttu-id="b4603-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4603-117">Application</span></span>|<span data-ttu-id="b4603-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4603-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4603-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4603-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b4603-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4603-120">Request headers</span></span>
|<span data-ttu-id="b4603-121">标头</span><span class="sxs-lookup"><span data-stu-id="b4603-121">Header</span></span>|<span data-ttu-id="b4603-122">值</span><span class="sxs-lookup"><span data-stu-id="b4603-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4603-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4603-123">Authorization</span></span>|<span data-ttu-id="b4603-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b4603-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4603-125">接受</span><span class="sxs-lookup"><span data-stu-id="b4603-125">Accept</span></span>|<span data-ttu-id="b4603-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4603-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4603-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4603-127">Request body</span></span>
<span data-ttu-id="b4603-128">在请求正文中，提供 windowsAppX 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4603-128">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="b4603-129">下表显示创建 windowsAppX 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b4603-129">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="b4603-130">属性</span><span class="sxs-lookup"><span data-stu-id="b4603-130">Property</span></span>|<span data-ttu-id="b4603-131">类型</span><span class="sxs-lookup"><span data-stu-id="b4603-131">Type</span></span>|<span data-ttu-id="b4603-132">说明</span><span class="sxs-lookup"><span data-stu-id="b4603-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4603-133">id</span><span class="sxs-lookup"><span data-stu-id="b4603-133">id</span></span>|<span data-ttu-id="b4603-134">String</span><span class="sxs-lookup"><span data-stu-id="b4603-134">String</span></span>|<span data-ttu-id="b4603-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b4603-135">Key of the entity.</span></span> <span data-ttu-id="b4603-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b4603-137">displayName</span></span>|<span data-ttu-id="b4603-138">String</span><span class="sxs-lookup"><span data-stu-id="b4603-138">String</span></span>|<span data-ttu-id="b4603-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="b4603-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b4603-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-141">description</span><span class="sxs-lookup"><span data-stu-id="b4603-141">description</span></span>|<span data-ttu-id="b4603-142">String</span><span class="sxs-lookup"><span data-stu-id="b4603-142">String</span></span>|<span data-ttu-id="b4603-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="b4603-143">The description of the app.</span></span> <span data-ttu-id="b4603-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-145">publisher</span><span class="sxs-lookup"><span data-stu-id="b4603-145">publisher</span></span>|<span data-ttu-id="b4603-146">String</span><span class="sxs-lookup"><span data-stu-id="b4603-146">String</span></span>|<span data-ttu-id="b4603-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="b4603-147">The publisher of the app.</span></span> <span data-ttu-id="b4603-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b4603-149">largeIcon</span></span>|[<span data-ttu-id="b4603-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b4603-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b4603-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="b4603-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b4603-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4603-153">createdDateTime</span></span>|<span data-ttu-id="b4603-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4603-154">DateTimeOffset</span></span>|<span data-ttu-id="b4603-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b4603-155">The date and time the app was created.</span></span> <span data-ttu-id="b4603-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4603-157">lastModifiedDateTime</span></span>|<span data-ttu-id="b4603-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4603-158">DateTimeOffset</span></span>|<span data-ttu-id="b4603-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b4603-159">The date and time the app was last modified.</span></span> <span data-ttu-id="b4603-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b4603-161">isFeatured</span></span>|<span data-ttu-id="b4603-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4603-162">Boolean</span></span>|<span data-ttu-id="b4603-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b4603-164">privacyInformationUrl</span></span>|<span data-ttu-id="b4603-165">String</span><span class="sxs-lookup"><span data-stu-id="b4603-165">String</span></span>|<span data-ttu-id="b4603-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="b4603-166">The privacy statement Url.</span></span> <span data-ttu-id="b4603-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b4603-168">informationUrl</span></span>|<span data-ttu-id="b4603-169">String</span><span class="sxs-lookup"><span data-stu-id="b4603-169">String</span></span>|<span data-ttu-id="b4603-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="b4603-170">The more information Url.</span></span> <span data-ttu-id="b4603-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-172">所有者</span><span class="sxs-lookup"><span data-stu-id="b4603-172">owner</span></span>|<span data-ttu-id="b4603-173">String</span><span class="sxs-lookup"><span data-stu-id="b4603-173">String</span></span>|<span data-ttu-id="b4603-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="b4603-174">The owner of the app.</span></span> <span data-ttu-id="b4603-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-176">developer</span><span class="sxs-lookup"><span data-stu-id="b4603-176">developer</span></span>|<span data-ttu-id="b4603-177">String</span><span class="sxs-lookup"><span data-stu-id="b4603-177">String</span></span>|<span data-ttu-id="b4603-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="b4603-178">The developer of the app.</span></span> <span data-ttu-id="b4603-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-180">notes</span><span class="sxs-lookup"><span data-stu-id="b4603-180">notes</span></span>|<span data-ttu-id="b4603-181">String</span><span class="sxs-lookup"><span data-stu-id="b4603-181">String</span></span>|<span data-ttu-id="b4603-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="b4603-182">Notes for the app.</span></span> <span data-ttu-id="b4603-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="b4603-184">uploadState</span></span>|<span data-ttu-id="b4603-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b4603-185">Int32</span></span>|<span data-ttu-id="b4603-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="b4603-186">The upload state.</span></span> <span data-ttu-id="b4603-187">可能的值包括： 0- `Not Ready` 、1- `Ready` 、2- `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="b4603-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="b4603-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="b4603-189">publishingState</span></span>|[<span data-ttu-id="b4603-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b4603-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b4603-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="b4603-191">The publishing state for the app.</span></span> <span data-ttu-id="b4603-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="b4603-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b4603-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="b4603-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="b4603-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="b4603-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b4603-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b4603-195">isAssigned</span></span>|<span data-ttu-id="b4603-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4603-196">Boolean</span></span>|<span data-ttu-id="b4603-197">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="b4603-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b4603-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b4603-199">roleScopeTagIds</span></span>|<span data-ttu-id="b4603-200">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b4603-200">String collection</span></span>|<span data-ttu-id="b4603-201">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="b4603-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b4603-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b4603-203">dependentAppCount</span></span>|<span data-ttu-id="b4603-204">Int32</span><span class="sxs-lookup"><span data-stu-id="b4603-204">Int32</span></span>|<span data-ttu-id="b4603-205">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="b4603-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b4603-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="b4603-207">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b4603-207">committedContentVersion</span></span>|<span data-ttu-id="b4603-208">String</span><span class="sxs-lookup"><span data-stu-id="b4603-208">String</span></span>|<span data-ttu-id="b4603-209">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="b4603-209">The internal committed content version.</span></span> <span data-ttu-id="b4603-210">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-210">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b4603-211">fileName</span><span class="sxs-lookup"><span data-stu-id="b4603-211">fileName</span></span>|<span data-ttu-id="b4603-212">String</span><span class="sxs-lookup"><span data-stu-id="b4603-212">String</span></span>|<span data-ttu-id="b4603-213">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="b4603-213">The name of the main Lob application file.</span></span> <span data-ttu-id="b4603-214">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-214">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b4603-215">size</span><span class="sxs-lookup"><span data-stu-id="b4603-215">size</span></span>|<span data-ttu-id="b4603-216">Int64</span><span class="sxs-lookup"><span data-stu-id="b4603-216">Int64</span></span>|<span data-ttu-id="b4603-217">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="b4603-217">The total size, including all uploaded files.</span></span> <span data-ttu-id="b4603-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b4603-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b4603-219">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="b4603-219">applicableArchitectures</span></span>|[<span data-ttu-id="b4603-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b4603-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b4603-221">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="b4603-221">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="b4603-222">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="b4603-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="b4603-223">identityName</span><span class="sxs-lookup"><span data-stu-id="b4603-223">identityName</span></span>|<span data-ttu-id="b4603-224">String</span><span class="sxs-lookup"><span data-stu-id="b4603-224">String</span></span>|<span data-ttu-id="b4603-225">标识名称。</span><span class="sxs-lookup"><span data-stu-id="b4603-225">The Identity Name.</span></span>|
|<span data-ttu-id="b4603-226">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="b4603-226">identityPublisherHash</span></span>|<span data-ttu-id="b4603-227">String</span><span class="sxs-lookup"><span data-stu-id="b4603-227">String</span></span>|<span data-ttu-id="b4603-228">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="b4603-228">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="b4603-229">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b4603-229">identityResourceIdentifier</span></span>|<span data-ttu-id="b4603-230">String</span><span class="sxs-lookup"><span data-stu-id="b4603-230">String</span></span>|<span data-ttu-id="b4603-231">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="b4603-231">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="b4603-232">isBundle</span><span class="sxs-lookup"><span data-stu-id="b4603-232">isBundle</span></span>|<span data-ttu-id="b4603-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4603-233">Boolean</span></span>|<span data-ttu-id="b4603-234">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="b4603-234">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="b4603-235">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b4603-235">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b4603-236">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b4603-236">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="b4603-237">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="b4603-237">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="b4603-238">identityVersion</span><span class="sxs-lookup"><span data-stu-id="b4603-238">identityVersion</span></span>|<span data-ttu-id="b4603-239">String</span><span class="sxs-lookup"><span data-stu-id="b4603-239">String</span></span>|<span data-ttu-id="b4603-240">标识版本。</span><span class="sxs-lookup"><span data-stu-id="b4603-240">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="b4603-241">响应</span><span class="sxs-lookup"><span data-stu-id="b4603-241">Response</span></span>
<span data-ttu-id="b4603-242">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [windowsAppX](../resources/intune-apps-windowsappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b4603-242">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4603-243">示例</span><span class="sxs-lookup"><span data-stu-id="b4603-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4603-244">请求</span><span class="sxs-lookup"><span data-stu-id="b4603-244">Request</span></span>
<span data-ttu-id="b4603-245">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4603-245">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1413

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="b4603-246">响应</span><span class="sxs-lookup"><span data-stu-id="b4603-246">Response</span></span>
<span data-ttu-id="b4603-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b4603-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1585

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```



