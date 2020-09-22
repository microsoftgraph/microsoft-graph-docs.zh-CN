---
title: 更新 macOSOfficeSuiteApp
description: 更新 macOSOfficeSuiteApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cd1b83b0e92b434d5509e48c030f10298b333e11
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48012031"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="e2809-103">更新 macOSOfficeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="e2809-103">Update macOSOfficeSuiteApp</span></span>

<span data-ttu-id="e2809-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2809-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2809-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e2809-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2809-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2809-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2809-107">更新 [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e2809-107">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2809-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e2809-108">Prerequisites</span></span>
<span data-ttu-id="e2809-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2809-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2809-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2809-111">Permission type</span></span>|<span data-ttu-id="e2809-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e2809-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2809-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2809-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2809-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2809-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e2809-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2809-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2809-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2809-116">Not supported.</span></span>|
|<span data-ttu-id="e2809-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2809-117">Application</span></span>|<span data-ttu-id="e2809-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2809-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2809-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2809-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="e2809-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2809-120">Request headers</span></span>
|<span data-ttu-id="e2809-121">标头</span><span class="sxs-lookup"><span data-stu-id="e2809-121">Header</span></span>|<span data-ttu-id="e2809-122">值</span><span class="sxs-lookup"><span data-stu-id="e2809-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2809-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2809-123">Authorization</span></span>|<span data-ttu-id="e2809-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e2809-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2809-125">接受</span><span class="sxs-lookup"><span data-stu-id="e2809-125">Accept</span></span>|<span data-ttu-id="e2809-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2809-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2809-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2809-127">Request body</span></span>
<span data-ttu-id="e2809-128">在请求正文中，提供 [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2809-128">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="e2809-129">下表显示创建 [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e2809-129">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="e2809-130">属性</span><span class="sxs-lookup"><span data-stu-id="e2809-130">Property</span></span>|<span data-ttu-id="e2809-131">类型</span><span class="sxs-lookup"><span data-stu-id="e2809-131">Type</span></span>|<span data-ttu-id="e2809-132">说明</span><span class="sxs-lookup"><span data-stu-id="e2809-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2809-133">id</span><span class="sxs-lookup"><span data-stu-id="e2809-133">id</span></span>|<span data-ttu-id="e2809-134">String</span><span class="sxs-lookup"><span data-stu-id="e2809-134">String</span></span>|<span data-ttu-id="e2809-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e2809-135">Key of the entity.</span></span> <span data-ttu-id="e2809-136">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-136">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e2809-137">displayName</span></span>|<span data-ttu-id="e2809-138">String</span><span class="sxs-lookup"><span data-stu-id="e2809-138">String</span></span>|<span data-ttu-id="e2809-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="e2809-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e2809-140">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-140">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-141">description</span><span class="sxs-lookup"><span data-stu-id="e2809-141">description</span></span>|<span data-ttu-id="e2809-142">String</span><span class="sxs-lookup"><span data-stu-id="e2809-142">String</span></span>|<span data-ttu-id="e2809-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="e2809-143">The description of the app.</span></span> <span data-ttu-id="e2809-144">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-144">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-145">publisher</span><span class="sxs-lookup"><span data-stu-id="e2809-145">publisher</span></span>|<span data-ttu-id="e2809-146">String</span><span class="sxs-lookup"><span data-stu-id="e2809-146">String</span></span>|<span data-ttu-id="e2809-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="e2809-147">The publisher of the app.</span></span> <span data-ttu-id="e2809-148">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-148">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e2809-149">largeIcon</span></span>|[<span data-ttu-id="e2809-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e2809-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e2809-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="e2809-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e2809-152">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-152">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e2809-153">createdDateTime</span></span>|<span data-ttu-id="e2809-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2809-154">DateTimeOffset</span></span>|<span data-ttu-id="e2809-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e2809-155">The date and time the app was created.</span></span> <span data-ttu-id="e2809-156">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-156">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2809-157">lastModifiedDateTime</span></span>|<span data-ttu-id="e2809-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2809-158">DateTimeOffset</span></span>|<span data-ttu-id="e2809-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e2809-159">The date and time the app was last modified.</span></span> <span data-ttu-id="e2809-160">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-160">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e2809-161">isFeatured</span></span>|<span data-ttu-id="e2809-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2809-162">Boolean</span></span>|<span data-ttu-id="e2809-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e2809-164">privacyInformationUrl</span></span>|<span data-ttu-id="e2809-165">String</span><span class="sxs-lookup"><span data-stu-id="e2809-165">String</span></span>|<span data-ttu-id="e2809-166">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="e2809-166">The privacy statement Url.</span></span> <span data-ttu-id="e2809-167">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-167">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e2809-168">informationUrl</span></span>|<span data-ttu-id="e2809-169">String</span><span class="sxs-lookup"><span data-stu-id="e2809-169">String</span></span>|<span data-ttu-id="e2809-170">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="e2809-170">The more information Url.</span></span> <span data-ttu-id="e2809-171">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-171">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-172">所有者</span><span class="sxs-lookup"><span data-stu-id="e2809-172">owner</span></span>|<span data-ttu-id="e2809-173">String</span><span class="sxs-lookup"><span data-stu-id="e2809-173">String</span></span>|<span data-ttu-id="e2809-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="e2809-174">The owner of the app.</span></span> <span data-ttu-id="e2809-175">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-175">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-176">developer</span><span class="sxs-lookup"><span data-stu-id="e2809-176">developer</span></span>|<span data-ttu-id="e2809-177">String</span><span class="sxs-lookup"><span data-stu-id="e2809-177">String</span></span>|<span data-ttu-id="e2809-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="e2809-178">The developer of the app.</span></span> <span data-ttu-id="e2809-179">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-179">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-180">notes</span><span class="sxs-lookup"><span data-stu-id="e2809-180">notes</span></span>|<span data-ttu-id="e2809-181">String</span><span class="sxs-lookup"><span data-stu-id="e2809-181">String</span></span>|<span data-ttu-id="e2809-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="e2809-182">Notes for the app.</span></span> <span data-ttu-id="e2809-183">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-183">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="e2809-184">uploadState</span></span>|<span data-ttu-id="e2809-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e2809-185">Int32</span></span>|<span data-ttu-id="e2809-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="e2809-186">The upload state.</span></span> <span data-ttu-id="e2809-187">可能的值包括： 0- `Not Ready` 、1- `Ready` 、2- `Processing` 。</span><span class="sxs-lookup"><span data-stu-id="e2809-187">Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`.</span></span> <span data-ttu-id="e2809-188">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-188">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-189">publishingState</span><span class="sxs-lookup"><span data-stu-id="e2809-189">publishingState</span></span>|[<span data-ttu-id="e2809-190">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e2809-190">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e2809-191">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="e2809-191">The publishing state for the app.</span></span> <span data-ttu-id="e2809-192">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="e2809-192">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e2809-193">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="e2809-193">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md).</span></span> <span data-ttu-id="e2809-194">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="e2809-194">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e2809-195">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e2809-195">isAssigned</span></span>|<span data-ttu-id="e2809-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2809-196">Boolean</span></span>|<span data-ttu-id="e2809-197">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="e2809-197">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e2809-198">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-198">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-199">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e2809-199">roleScopeTagIds</span></span>|<span data-ttu-id="e2809-200">String collection</span><span class="sxs-lookup"><span data-stu-id="e2809-200">String collection</span></span>|<span data-ttu-id="e2809-201">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="e2809-201">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e2809-202">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-202">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-203">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e2809-203">dependentAppCount</span></span>|<span data-ttu-id="e2809-204">Int32</span><span class="sxs-lookup"><span data-stu-id="e2809-204">Int32</span></span>|<span data-ttu-id="e2809-205">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="e2809-205">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e2809-206">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-206">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-207">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="e2809-207">supersedingAppCount</span></span>|<span data-ttu-id="e2809-208">Int32</span><span class="sxs-lookup"><span data-stu-id="e2809-208">Int32</span></span>|<span data-ttu-id="e2809-209">此应用程序直接或间接取代的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="e2809-209">The total number of apps this app directly or indirectly supersedes.</span></span> <span data-ttu-id="e2809-210">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-210">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|
|<span data-ttu-id="e2809-211">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="e2809-211">supersededAppCount</span></span>|<span data-ttu-id="e2809-212">Int32</span><span class="sxs-lookup"><span data-stu-id="e2809-212">Int32</span></span>|<span data-ttu-id="e2809-213">此应用程序直接或间接取代的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="e2809-213">The total number of apps this app is directly or indirectly superseded by.</span></span> <span data-ttu-id="e2809-214">继承自 [mobileApp](../resources/intune-shared-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e2809-214">Inherited from [mobileApp](../resources/intune-shared-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e2809-215">响应</span><span class="sxs-lookup"><span data-stu-id="e2809-215">Response</span></span>
<span data-ttu-id="e2809-216">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e2809-216">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2809-217">示例</span><span class="sxs-lookup"><span data-stu-id="e2809-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2809-218">请求</span><span class="sxs-lookup"><span data-stu-id="e2809-218">Request</span></span>
<span data-ttu-id="e2809-219">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e2809-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 775

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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

### <a name="response"></a><span data-ttu-id="e2809-220">响应</span><span class="sxs-lookup"><span data-stu-id="e2809-220">Response</span></span>
<span data-ttu-id="e2809-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e2809-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 947

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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






