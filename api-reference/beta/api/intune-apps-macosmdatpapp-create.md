---
title: 创建 macOSMdatpApp
description: 创建新的 macOSMdatpApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 797c645cd91e4447b8db3eaa3ec72fc70b172066
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49251505"
---
# <a name="create-macosmdatpapp"></a><span data-ttu-id="028b1-103">创建 macOSMdatpApp</span><span class="sxs-lookup"><span data-stu-id="028b1-103">Create macOSMdatpApp</span></span>

<span data-ttu-id="028b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="028b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="028b1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="028b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="028b1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="028b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="028b1-107">创建新的 [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="028b1-107">Create a new [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="028b1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="028b1-108">Prerequisites</span></span>
<span data-ttu-id="028b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="028b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="028b1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="028b1-111">Permission type</span></span>|<span data-ttu-id="028b1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="028b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="028b1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="028b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="028b1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="028b1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="028b1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="028b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="028b1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="028b1-116">Not supported.</span></span>|
|<span data-ttu-id="028b1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="028b1-117">Application</span></span>|<span data-ttu-id="028b1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="028b1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="028b1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="028b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="028b1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="028b1-120">Request headers</span></span>
|<span data-ttu-id="028b1-121">标头</span><span class="sxs-lookup"><span data-stu-id="028b1-121">Header</span></span>|<span data-ttu-id="028b1-122">值</span><span class="sxs-lookup"><span data-stu-id="028b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="028b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="028b1-123">Authorization</span></span>|<span data-ttu-id="028b1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="028b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="028b1-125">接受</span><span class="sxs-lookup"><span data-stu-id="028b1-125">Accept</span></span>|<span data-ttu-id="028b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="028b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="028b1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="028b1-127">Request body</span></span>
<span data-ttu-id="028b1-128">在请求正文中，提供 macOSMdatpApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="028b1-128">In the request body, supply a JSON representation for the macOSMdatpApp object.</span></span>

<span data-ttu-id="028b1-129">下表显示创建 macOSMdatpApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="028b1-129">The following table shows the properties that are required when you create the macOSMdatpApp.</span></span>

|<span data-ttu-id="028b1-130">属性</span><span class="sxs-lookup"><span data-stu-id="028b1-130">Property</span></span>|<span data-ttu-id="028b1-131">类型</span><span class="sxs-lookup"><span data-stu-id="028b1-131">Type</span></span>|<span data-ttu-id="028b1-132">说明</span><span class="sxs-lookup"><span data-stu-id="028b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="028b1-133">id</span><span class="sxs-lookup"><span data-stu-id="028b1-133">id</span></span>|<span data-ttu-id="028b1-134">String</span><span class="sxs-lookup"><span data-stu-id="028b1-134">String</span></span>|<span data-ttu-id="028b1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="028b1-135">Key of the entity.</span></span> <span data-ttu-id="028b1-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="028b1-137">displayName</span></span>|<span data-ttu-id="028b1-138">String</span><span class="sxs-lookup"><span data-stu-id="028b1-138">String</span></span>|<span data-ttu-id="028b1-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="028b1-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="028b1-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-141">description</span><span class="sxs-lookup"><span data-stu-id="028b1-141">description</span></span>|<span data-ttu-id="028b1-142">String</span><span class="sxs-lookup"><span data-stu-id="028b1-142">String</span></span>|<span data-ttu-id="028b1-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="028b1-143">The description of the app.</span></span> <span data-ttu-id="028b1-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-145">publisher</span><span class="sxs-lookup"><span data-stu-id="028b1-145">publisher</span></span>|<span data-ttu-id="028b1-146">String</span><span class="sxs-lookup"><span data-stu-id="028b1-146">String</span></span>|<span data-ttu-id="028b1-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="028b1-147">The publisher of the app.</span></span> <span data-ttu-id="028b1-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="028b1-149">largeIcon</span></span>|[<span data-ttu-id="028b1-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="028b1-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="028b1-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="028b1-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="028b1-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="028b1-153">createdDateTime</span></span>|<span data-ttu-id="028b1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="028b1-154">DateTimeOffset</span></span>|<span data-ttu-id="028b1-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="028b1-155">The date and time the app was created.</span></span> <span data-ttu-id="028b1-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="028b1-157">lastModifiedDateTime</span></span>|<span data-ttu-id="028b1-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="028b1-158">DateTimeOffset</span></span>|<span data-ttu-id="028b1-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="028b1-159">The date and time the app was last modified.</span></span> <span data-ttu-id="028b1-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="028b1-161">isFeatured</span></span>|<span data-ttu-id="028b1-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="028b1-162">Boolean</span></span>|<span data-ttu-id="028b1-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="028b1-164">privacyInformationUrl</span></span>|<span data-ttu-id="028b1-165">String</span><span class="sxs-lookup"><span data-stu-id="028b1-165">String</span></span>|<span data-ttu-id="028b1-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="028b1-166">The privacy statement Url.</span></span> <span data-ttu-id="028b1-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="028b1-168">informationUrl</span></span>|<span data-ttu-id="028b1-169">String</span><span class="sxs-lookup"><span data-stu-id="028b1-169">String</span></span>|<span data-ttu-id="028b1-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="028b1-170">The more information Url.</span></span> <span data-ttu-id="028b1-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-172">所有者</span><span class="sxs-lookup"><span data-stu-id="028b1-172">owner</span></span>|<span data-ttu-id="028b1-173">String</span><span class="sxs-lookup"><span data-stu-id="028b1-173">String</span></span>|<span data-ttu-id="028b1-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="028b1-174">The owner of the app.</span></span> <span data-ttu-id="028b1-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-176">developer</span><span class="sxs-lookup"><span data-stu-id="028b1-176">developer</span></span>|<span data-ttu-id="028b1-177">String</span><span class="sxs-lookup"><span data-stu-id="028b1-177">String</span></span>|<span data-ttu-id="028b1-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="028b1-178">The developer of the app.</span></span> <span data-ttu-id="028b1-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-180">notes</span><span class="sxs-lookup"><span data-stu-id="028b1-180">notes</span></span>|<span data-ttu-id="028b1-181">String</span><span class="sxs-lookup"><span data-stu-id="028b1-181">String</span></span>|<span data-ttu-id="028b1-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="028b1-182">Notes for the app.</span></span> <span data-ttu-id="028b1-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="028b1-184">uploadState</span></span>|<span data-ttu-id="028b1-185">Int32</span><span class="sxs-lookup"><span data-stu-id="028b1-185">Int32</span></span>|<span data-ttu-id="028b1-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="028b1-186">The upload state.</span></span> <span data-ttu-id="028b1-187">可能的值包括： 0- `Not Ready` 、1- `Ready` 、2- `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="028b1-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="028b1-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="028b1-189">publishingState</span></span>|[<span data-ttu-id="028b1-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="028b1-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="028b1-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="028b1-191">The publishing state for the app.</span></span> <span data-ttu-id="028b1-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="028b1-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="028b1-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="028b1-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="028b1-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="028b1-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="028b1-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="028b1-195">isAssigned</span></span>|<span data-ttu-id="028b1-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="028b1-196">Boolean</span></span>|<span data-ttu-id="028b1-197">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="028b1-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="028b1-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="028b1-199">roleScopeTagIds</span></span>|<span data-ttu-id="028b1-200">String 集合</span><span class="sxs-lookup"><span data-stu-id="028b1-200">String collection</span></span>|<span data-ttu-id="028b1-201">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="028b1-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="028b1-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="028b1-203">dependentAppCount</span></span>|<span data-ttu-id="028b1-204">Int32</span><span class="sxs-lookup"><span data-stu-id="028b1-204">Int32</span></span>|<span data-ttu-id="028b1-205">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="028b1-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="028b1-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="028b1-207">supersedingAppCount</span></span>|<span data-ttu-id="028b1-208">Int32</span><span class="sxs-lookup"><span data-stu-id="028b1-208">Int32</span></span>|<span data-ttu-id="028b1-209">此应用程序直接或间接取代的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="028b1-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="028b1-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="028b1-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="028b1-211">supersededAppCount</span></span>|<span data-ttu-id="028b1-212">Int32</span><span class="sxs-lookup"><span data-stu-id="028b1-212">Int32</span></span>|<span data-ttu-id="028b1-213">此应用程序直接或间接取代的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="028b1-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="028b1-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="028b1-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="028b1-215">响应</span><span class="sxs-lookup"><span data-stu-id="028b1-215">Response</span></span>
<span data-ttu-id="028b1-216">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="028b1-216">If successful, this method returns a `201 Created` response code and a [macOSMdatpApp](../resources/intune-apps-macosmdatpapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="028b1-217">示例</span><span class="sxs-lookup"><span data-stu-id="028b1-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="028b1-218">请求</span><span class="sxs-lookup"><span data-stu-id="028b1-218">Request</span></span>
<span data-ttu-id="028b1-219">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="028b1-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 769

{
  "@odata.type": "#microsoft.graph.macOSMdatpApp",
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
  "supersededAppCount": 2
}
```

### <a name="response"></a><span data-ttu-id="028b1-220">响应</span><span class="sxs-lookup"><span data-stu-id="028b1-220">Response</span></span>
<span data-ttu-id="028b1-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="028b1-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 941

{
  "@odata.type": "#microsoft.graph.macOSMdatpApp",
  "id": "2963b007-b007-2963-07b0-632907b06329",
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
  "supersededAppCount": 2
}
```




