---
title: 创建 androidLobApp
description: 创建新的 androidLobApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 42b8cd15c34a2d9fe677a3aff3cd4d629a94d5b8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49253920"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="ff0c0-103">创建 androidLobApp</span><span class="sxs-lookup"><span data-stu-id="ff0c0-103">Create androidLobApp</span></span>

<span data-ttu-id="ff0c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff0c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff0c0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff0c0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff0c0-107">创建新的 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-107">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff0c0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ff0c0-108">Prerequisites</span></span>
<span data-ttu-id="ff0c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff0c0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff0c0-111">Permission type</span></span>|<span data-ttu-id="ff0c0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ff0c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff0c0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff0c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff0c0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff0c0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ff0c0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff0c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff0c0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-116">Not supported.</span></span>|
|<span data-ttu-id="ff0c0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff0c0-117">Application</span></span>|<span data-ttu-id="ff0c0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff0c0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff0c0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff0c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ff0c0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff0c0-120">Request headers</span></span>
|<span data-ttu-id="ff0c0-121">标头</span><span class="sxs-lookup"><span data-stu-id="ff0c0-121">Header</span></span>|<span data-ttu-id="ff0c0-122">值</span><span class="sxs-lookup"><span data-stu-id="ff0c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff0c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff0c0-123">Authorization</span></span>|<span data-ttu-id="ff0c0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff0c0-125">接受</span><span class="sxs-lookup"><span data-stu-id="ff0c0-125">Accept</span></span>|<span data-ttu-id="ff0c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff0c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff0c0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff0c0-127">Request body</span></span>
<span data-ttu-id="ff0c0-128">在请求正文中，提供 androidLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-128">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="ff0c0-129">下表显示了创建 androidLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-129">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="ff0c0-130">属性</span><span class="sxs-lookup"><span data-stu-id="ff0c0-130">Property</span></span>|<span data-ttu-id="ff0c0-131">类型</span><span class="sxs-lookup"><span data-stu-id="ff0c0-131">Type</span></span>|<span data-ttu-id="ff0c0-132">说明</span><span class="sxs-lookup"><span data-stu-id="ff0c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff0c0-133">id</span><span class="sxs-lookup"><span data-stu-id="ff0c0-133">id</span></span>|<span data-ttu-id="ff0c0-134">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-134">String</span></span>|<span data-ttu-id="ff0c0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-135">Key of the entity.</span></span> <span data-ttu-id="ff0c0-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ff0c0-137">displayName</span></span>|<span data-ttu-id="ff0c0-138">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-138">String</span></span>|<span data-ttu-id="ff0c0-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ff0c0-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-141">description</span><span class="sxs-lookup"><span data-stu-id="ff0c0-141">description</span></span>|<span data-ttu-id="ff0c0-142">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-142">String</span></span>|<span data-ttu-id="ff0c0-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-143">The description of the app.</span></span> <span data-ttu-id="ff0c0-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ff0c0-145">publisher</span></span>|<span data-ttu-id="ff0c0-146">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-146">String</span></span>|<span data-ttu-id="ff0c0-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-147">The publisher of the app.</span></span> <span data-ttu-id="ff0c0-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ff0c0-149">largeIcon</span></span>|[<span data-ttu-id="ff0c0-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ff0c0-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ff0c0-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ff0c0-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff0c0-153">createdDateTime</span></span>|<span data-ttu-id="ff0c0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff0c0-154">DateTimeOffset</span></span>|<span data-ttu-id="ff0c0-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-155">The date and time the app was created.</span></span> <span data-ttu-id="ff0c0-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff0c0-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ff0c0-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff0c0-158">DateTimeOffset</span></span>|<span data-ttu-id="ff0c0-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ff0c0-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ff0c0-161">isFeatured</span></span>|<span data-ttu-id="ff0c0-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff0c0-162">Boolean</span></span>|<span data-ttu-id="ff0c0-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ff0c0-164">privacyInformationUrl</span></span>|<span data-ttu-id="ff0c0-165">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-165">String</span></span>|<span data-ttu-id="ff0c0-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-166">The privacy statement Url.</span></span> <span data-ttu-id="ff0c0-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ff0c0-168">informationUrl</span></span>|<span data-ttu-id="ff0c0-169">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-169">String</span></span>|<span data-ttu-id="ff0c0-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-170">The more information Url.</span></span> <span data-ttu-id="ff0c0-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-172">所有者</span><span class="sxs-lookup"><span data-stu-id="ff0c0-172">owner</span></span>|<span data-ttu-id="ff0c0-173">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-173">String</span></span>|<span data-ttu-id="ff0c0-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-174">The owner of the app.</span></span> <span data-ttu-id="ff0c0-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-176">developer</span><span class="sxs-lookup"><span data-stu-id="ff0c0-176">developer</span></span>|<span data-ttu-id="ff0c0-177">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-177">String</span></span>|<span data-ttu-id="ff0c0-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-178">The developer of the app.</span></span> <span data-ttu-id="ff0c0-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-180">notes</span><span class="sxs-lookup"><span data-stu-id="ff0c0-180">notes</span></span>|<span data-ttu-id="ff0c0-181">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-181">String</span></span>|<span data-ttu-id="ff0c0-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-182">Notes for the app.</span></span> <span data-ttu-id="ff0c0-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ff0c0-184">uploadState</span></span>|<span data-ttu-id="ff0c0-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ff0c0-185">Int32</span></span>|<span data-ttu-id="ff0c0-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-186">The upload state.</span></span> <span data-ttu-id="ff0c0-187">可能的值包括： 0- `Not Ready` 、1- `Ready` 、2- `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="ff0c0-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="ff0c0-189">publishingState</span></span>|[<span data-ttu-id="ff0c0-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ff0c0-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ff0c0-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-191">The publishing state for the app.</span></span> <span data-ttu-id="ff0c0-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ff0c0-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="ff0c0-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ff0c0-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ff0c0-195">isAssigned</span></span>|<span data-ttu-id="ff0c0-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff0c0-196">Boolean</span></span>|<span data-ttu-id="ff0c0-197">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ff0c0-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ff0c0-199">roleScopeTagIds</span></span>|<span data-ttu-id="ff0c0-200">String 集合</span><span class="sxs-lookup"><span data-stu-id="ff0c0-200">String collection</span></span>|<span data-ttu-id="ff0c0-201">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ff0c0-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="ff0c0-203">dependentAppCount</span></span>|<span data-ttu-id="ff0c0-204">Int32</span><span class="sxs-lookup"><span data-stu-id="ff0c0-204">Int32</span></span>|<span data-ttu-id="ff0c0-205">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="ff0c0-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="ff0c0-207">supersedingAppCount</span></span>|<span data-ttu-id="ff0c0-208">Int32</span><span class="sxs-lookup"><span data-stu-id="ff0c0-208">Int32</span></span>|<span data-ttu-id="ff0c0-209">此应用程序直接或间接取代的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="ff0c0-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="ff0c0-211">supersededAppCount</span></span>|<span data-ttu-id="ff0c0-212">Int32</span><span class="sxs-lookup"><span data-stu-id="ff0c0-212">Int32</span></span>|<span data-ttu-id="ff0c0-213">此应用程序直接或间接取代的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="ff0c0-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="ff0c0-215">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ff0c0-215">committedContentVersion</span></span>|<span data-ttu-id="ff0c0-216">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-216">String</span></span>|<span data-ttu-id="ff0c0-217">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-217">The internal committed content version.</span></span> <span data-ttu-id="ff0c0-218">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-218">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ff0c0-219">fileName</span><span class="sxs-lookup"><span data-stu-id="ff0c0-219">fileName</span></span>|<span data-ttu-id="ff0c0-220">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-220">String</span></span>|<span data-ttu-id="ff0c0-221">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-221">The name of the main Lob application file.</span></span> <span data-ttu-id="ff0c0-222">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-222">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ff0c0-223">size</span><span class="sxs-lookup"><span data-stu-id="ff0c0-223">size</span></span>|<span data-ttu-id="ff0c0-224">Int64</span><span class="sxs-lookup"><span data-stu-id="ff0c0-224">Int64</span></span>|<span data-ttu-id="ff0c0-225">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-225">The total size, including all uploaded files.</span></span> <span data-ttu-id="ff0c0-226">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="ff0c0-226">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ff0c0-227">packageId</span><span class="sxs-lookup"><span data-stu-id="ff0c0-227">packageId</span></span>|<span data-ttu-id="ff0c0-228">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-228">String</span></span>|<span data-ttu-id="ff0c0-229">包标识符。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-229">The package identifier.</span></span>|
|<span data-ttu-id="ff0c0-230">identityName</span><span class="sxs-lookup"><span data-stu-id="ff0c0-230">identityName</span></span>|<span data-ttu-id="ff0c0-231">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-231">String</span></span>|<span data-ttu-id="ff0c0-232">标识名称。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-232">The Identity Name.</span></span>|
|<span data-ttu-id="ff0c0-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ff0c0-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ff0c0-234">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ff0c0-234">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="ff0c0-235">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ff0c0-236">versionName</span><span class="sxs-lookup"><span data-stu-id="ff0c0-236">versionName</span></span>|<span data-ttu-id="ff0c0-237">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-237">String</span></span>|<span data-ttu-id="ff0c0-238">Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-238">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ff0c0-239">versionCode</span><span class="sxs-lookup"><span data-stu-id="ff0c0-239">versionCode</span></span>|<span data-ttu-id="ff0c0-240">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-240">String</span></span>|<span data-ttu-id="ff0c0-241">Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-241">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ff0c0-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ff0c0-242">identityVersion</span></span>|<span data-ttu-id="ff0c0-243">String</span><span class="sxs-lookup"><span data-stu-id="ff0c0-243">String</span></span>|<span data-ttu-id="ff0c0-244">标识版本。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-244">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ff0c0-245">响应</span><span class="sxs-lookup"><span data-stu-id="ff0c0-245">Response</span></span>
<span data-ttu-id="ff0c0-246">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-246">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff0c0-247">示例</span><span class="sxs-lookup"><span data-stu-id="ff0c0-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff0c0-248">请求</span><span class="sxs-lookup"><span data-stu-id="ff0c0-248">Request</span></span>
<span data-ttu-id="ff0c0-249">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-249">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1470

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="ff0c0-250">响应</span><span class="sxs-lookup"><span data-stu-id="ff0c0-250">Response</span></span>
<span data-ttu-id="ff0c0-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ff0c0-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1642

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "supersedingAppCount": 3,
  "supersededAppCount": 2,
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




