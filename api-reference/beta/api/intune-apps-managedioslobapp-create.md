---
title: 创建 managedIOSLobApp
description: 创建新的 managedIOSLobApp 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e51887909019e6c42767e03cf44e275a364b60b5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32493207"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="dadb4-103">创建 managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="dadb4-103">Create managedIOSLobApp</span></span>

> <span data-ttu-id="dadb4-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dadb4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dadb4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dadb4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dadb4-106">创建新的 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dadb4-106">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dadb4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="dadb4-107">Prerequisites</span></span>
<span data-ttu-id="dadb4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dadb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dadb4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dadb4-110">Permission type</span></span>|<span data-ttu-id="dadb4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dadb4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dadb4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dadb4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dadb4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dadb4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dadb4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dadb4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dadb4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dadb4-115">Not supported.</span></span>|
|<span data-ttu-id="dadb4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dadb4-116">Application</span></span>|<span data-ttu-id="dadb4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="dadb4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dadb4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dadb4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="dadb4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dadb4-119">Request headers</span></span>
|<span data-ttu-id="dadb4-120">标头</span><span class="sxs-lookup"><span data-stu-id="dadb4-120">Header</span></span>|<span data-ttu-id="dadb4-121">值</span><span class="sxs-lookup"><span data-stu-id="dadb4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dadb4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dadb4-122">Authorization</span></span>|<span data-ttu-id="dadb4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dadb4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dadb4-124">接受</span><span class="sxs-lookup"><span data-stu-id="dadb4-124">Accept</span></span>|<span data-ttu-id="dadb4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dadb4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dadb4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dadb4-126">Request body</span></span>
<span data-ttu-id="dadb4-127">在请求正文中，提供 managedIOSLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dadb4-127">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="dadb4-128">下表显示创建 managedIOSLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dadb4-128">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="dadb4-129">属性</span><span class="sxs-lookup"><span data-stu-id="dadb4-129">Property</span></span>|<span data-ttu-id="dadb4-130">类型</span><span class="sxs-lookup"><span data-stu-id="dadb4-130">Type</span></span>|<span data-ttu-id="dadb4-131">说明</span><span class="sxs-lookup"><span data-stu-id="dadb4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dadb4-132">id</span><span class="sxs-lookup"><span data-stu-id="dadb4-132">id</span></span>|<span data-ttu-id="dadb4-133">String</span><span class="sxs-lookup"><span data-stu-id="dadb4-133">String</span></span>|<span data-ttu-id="dadb4-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dadb4-134">Key of the entity.</span></span> <span data-ttu-id="dadb4-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="dadb4-136">displayName</span></span>|<span data-ttu-id="dadb4-137">字符串</span><span class="sxs-lookup"><span data-stu-id="dadb4-137">String</span></span>|<span data-ttu-id="dadb4-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="dadb4-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="dadb4-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-140">description</span><span class="sxs-lookup"><span data-stu-id="dadb4-140">description</span></span>|<span data-ttu-id="dadb4-141">字符串</span><span class="sxs-lookup"><span data-stu-id="dadb4-141">String</span></span>|<span data-ttu-id="dadb4-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="dadb4-142">The description of the app.</span></span> <span data-ttu-id="dadb4-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-144">publisher</span><span class="sxs-lookup"><span data-stu-id="dadb4-144">publisher</span></span>|<span data-ttu-id="dadb4-145">字符串</span><span class="sxs-lookup"><span data-stu-id="dadb4-145">String</span></span>|<span data-ttu-id="dadb4-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="dadb4-146">The publisher of the app.</span></span> <span data-ttu-id="dadb4-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="dadb4-148">largeIcon</span></span>|[<span data-ttu-id="dadb4-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dadb4-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dadb4-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="dadb4-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="dadb4-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dadb4-152">createdDateTime</span></span>|<span data-ttu-id="dadb4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dadb4-153">DateTimeOffset</span></span>|<span data-ttu-id="dadb4-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="dadb4-154">The date and time the app was created.</span></span> <span data-ttu-id="dadb4-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dadb4-156">lastModifiedDateTime</span></span>|<span data-ttu-id="dadb4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dadb4-157">DateTimeOffset</span></span>|<span data-ttu-id="dadb4-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="dadb4-158">The date and time the app was last modified.</span></span> <span data-ttu-id="dadb4-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="dadb4-160">isFeatured</span></span>|<span data-ttu-id="dadb4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="dadb4-161">Boolean</span></span>|<span data-ttu-id="dadb4-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="dadb4-163">privacyInformationUrl</span></span>|<span data-ttu-id="dadb4-164">字符串</span><span class="sxs-lookup"><span data-stu-id="dadb4-164">String</span></span>|<span data-ttu-id="dadb4-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="dadb4-165">The privacy statement Url.</span></span> <span data-ttu-id="dadb4-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="dadb4-167">informationUrl</span></span>|<span data-ttu-id="dadb4-168">字符串</span><span class="sxs-lookup"><span data-stu-id="dadb4-168">String</span></span>|<span data-ttu-id="dadb4-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="dadb4-169">The more information Url.</span></span> <span data-ttu-id="dadb4-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-171">owner</span><span class="sxs-lookup"><span data-stu-id="dadb4-171">owner</span></span>|<span data-ttu-id="dadb4-172">字符串</span><span class="sxs-lookup"><span data-stu-id="dadb4-172">String</span></span>|<span data-ttu-id="dadb4-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="dadb4-173">The owner of the app.</span></span> <span data-ttu-id="dadb4-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-175">developer</span><span class="sxs-lookup"><span data-stu-id="dadb4-175">developer</span></span>|<span data-ttu-id="dadb4-176">字符串</span><span class="sxs-lookup"><span data-stu-id="dadb4-176">String</span></span>|<span data-ttu-id="dadb4-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="dadb4-177">The developer of the app.</span></span> <span data-ttu-id="dadb4-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-179">notes</span><span class="sxs-lookup"><span data-stu-id="dadb4-179">notes</span></span>|<span data-ttu-id="dadb4-180">字符串</span><span class="sxs-lookup"><span data-stu-id="dadb4-180">String</span></span>|<span data-ttu-id="dadb4-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="dadb4-181">Notes for the app.</span></span> <span data-ttu-id="dadb4-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="dadb4-183">uploadState</span></span>|<span data-ttu-id="dadb4-184">Int32</span><span class="sxs-lookup"><span data-stu-id="dadb4-184">Int32</span></span>|<span data-ttu-id="dadb4-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="dadb4-185">The upload state.</span></span> <span data-ttu-id="dadb4-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="dadb4-187">publishingState</span></span>|[<span data-ttu-id="dadb4-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="dadb4-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="dadb4-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="dadb4-189">The publishing state for the app.</span></span> <span data-ttu-id="dadb4-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="dadb4-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="dadb4-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="dadb4-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="dadb4-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="dadb4-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="dadb4-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="dadb4-193">isAssigned</span></span>|<span data-ttu-id="dadb4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="dadb4-194">Boolean</span></span>|<span data-ttu-id="dadb4-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="dadb4-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="dadb4-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dadb4-197">roleScopeTagIds</span></span>|<span data-ttu-id="dadb4-198">String collection</span><span class="sxs-lookup"><span data-stu-id="dadb4-198">String collection</span></span>|<span data-ttu-id="dadb4-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="dadb4-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="dadb4-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="dadb4-201">dependentAppCount</span></span>|<span data-ttu-id="dadb4-202">Int32</span><span class="sxs-lookup"><span data-stu-id="dadb4-202">Int32</span></span>|<span data-ttu-id="dadb4-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="dadb4-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="dadb4-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dadb4-205">appAvailability</span><span class="sxs-lookup"><span data-stu-id="dadb4-205">appAvailability</span></span>|[<span data-ttu-id="dadb4-206">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="dadb4-206">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="dadb4-207">应用程序的可用性。</span><span class="sxs-lookup"><span data-stu-id="dadb4-207">The Application's availability.</span></span> <span data-ttu-id="dadb4-208">继承自[managedApp](../resources/intune-apps-managedapp.md)。</span><span class="sxs-lookup"><span data-stu-id="dadb4-208">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="dadb4-209">可取值为：`global`、`lineOfBusiness`。</span><span class="sxs-lookup"><span data-stu-id="dadb4-209">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="dadb4-210">version</span><span class="sxs-lookup"><span data-stu-id="dadb4-210">version</span></span>|<span data-ttu-id="dadb4-211">String</span><span class="sxs-lookup"><span data-stu-id="dadb4-211">String</span></span>|<span data-ttu-id="dadb4-212">应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="dadb4-212">The Application's version.</span></span> <span data-ttu-id="dadb4-213">继承自 [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-213">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="dadb4-214">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="dadb4-214">committedContentVersion</span></span>|<span data-ttu-id="dadb4-215">字符串</span><span class="sxs-lookup"><span data-stu-id="dadb4-215">String</span></span>|<span data-ttu-id="dadb4-216">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="dadb4-216">The internal committed content version.</span></span> <span data-ttu-id="dadb4-217">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-217">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="dadb4-218">fileName</span><span class="sxs-lookup"><span data-stu-id="dadb4-218">fileName</span></span>|<span data-ttu-id="dadb4-219">字符串</span><span class="sxs-lookup"><span data-stu-id="dadb4-219">String</span></span>|<span data-ttu-id="dadb4-220">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="dadb4-220">The name of the main Lob application file.</span></span> <span data-ttu-id="dadb4-221">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-221">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="dadb4-222">size</span><span class="sxs-lookup"><span data-stu-id="dadb4-222">size</span></span>|<span data-ttu-id="dadb4-223">Int64</span><span class="sxs-lookup"><span data-stu-id="dadb4-223">Int64</span></span>|<span data-ttu-id="dadb4-224">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="dadb4-224">The total size, including all uploaded files.</span></span> <span data-ttu-id="dadb4-225">继承自 [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="dadb4-225">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="dadb4-226">bundleId</span><span class="sxs-lookup"><span data-stu-id="dadb4-226">bundleId</span></span>|<span data-ttu-id="dadb4-227">字符串</span><span class="sxs-lookup"><span data-stu-id="dadb4-227">String</span></span>|<span data-ttu-id="dadb4-228">标识名称。</span><span class="sxs-lookup"><span data-stu-id="dadb4-228">The Identity Name.</span></span>|
|<span data-ttu-id="dadb4-229">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="dadb4-229">applicableDeviceType</span></span>|[<span data-ttu-id="dadb4-230">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="dadb4-230">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="dadb4-231">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="dadb4-231">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="dadb4-232">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dadb4-232">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="dadb4-233">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dadb4-233">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="dadb4-234">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="dadb4-234">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="dadb4-235">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="dadb4-235">expirationDateTime</span></span>|<span data-ttu-id="dadb4-236">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dadb4-236">DateTimeOffset</span></span>|<span data-ttu-id="dadb4-237">过期时间。</span><span class="sxs-lookup"><span data-stu-id="dadb4-237">The expiration time.</span></span>|
|<span data-ttu-id="dadb4-238">versionNumber</span><span class="sxs-lookup"><span data-stu-id="dadb4-238">versionNumber</span></span>|<span data-ttu-id="dadb4-239">字符串</span><span class="sxs-lookup"><span data-stu-id="dadb4-239">String</span></span>|<span data-ttu-id="dadb4-240">托管 iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="dadb4-240">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="dadb4-241">buildNumber</span><span class="sxs-lookup"><span data-stu-id="dadb4-241">buildNumber</span></span>|<span data-ttu-id="dadb4-242">字符串</span><span class="sxs-lookup"><span data-stu-id="dadb4-242">String</span></span>|<span data-ttu-id="dadb4-243">托管 iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="dadb4-243">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="dadb4-244">identityVersion</span><span class="sxs-lookup"><span data-stu-id="dadb4-244">identityVersion</span></span>|<span data-ttu-id="dadb4-245">String</span><span class="sxs-lookup"><span data-stu-id="dadb4-245">String</span></span>|<span data-ttu-id="dadb4-246">标识版本。</span><span class="sxs-lookup"><span data-stu-id="dadb4-246">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="dadb4-247">响应</span><span class="sxs-lookup"><span data-stu-id="dadb4-247">Response</span></span>
<span data-ttu-id="dadb4-248">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dadb4-248">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dadb4-249">示例</span><span class="sxs-lookup"><span data-stu-id="dadb4-249">Example</span></span>

### <a name="request"></a><span data-ttu-id="dadb4-250">请求</span><span class="sxs-lookup"><span data-stu-id="dadb4-250">Request</span></span>
<span data-ttu-id="dadb4-251">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dadb4-251">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1469

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="dadb4-252">响应</span><span class="sxs-lookup"><span data-stu-id="dadb4-252">Response</span></span>
<span data-ttu-id="dadb4-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dadb4-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1641

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```





