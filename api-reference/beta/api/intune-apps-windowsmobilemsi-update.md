---
title: 更新 windowsMobileMSI
description: 更新 windowsMobileMSI 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 300e1719001e50fcc27145a7fa84512b83340cff
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776701"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="41bfa-103">更新 windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="41bfa-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="41bfa-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="41bfa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41bfa-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41bfa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41bfa-106">更新 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="41bfa-106">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41bfa-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="41bfa-107">Prerequisites</span></span>
<span data-ttu-id="41bfa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41bfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41bfa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="41bfa-110">Permission type</span></span>|<span data-ttu-id="41bfa-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41bfa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41bfa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41bfa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41bfa-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41bfa-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="41bfa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41bfa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41bfa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="41bfa-115">Not supported.</span></span>|
|<span data-ttu-id="41bfa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="41bfa-116">Application</span></span>|<span data-ttu-id="41bfa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="41bfa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41bfa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41bfa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="41bfa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="41bfa-119">Request headers</span></span>
|<span data-ttu-id="41bfa-120">标头</span><span class="sxs-lookup"><span data-stu-id="41bfa-120">Header</span></span>|<span data-ttu-id="41bfa-121">值</span><span class="sxs-lookup"><span data-stu-id="41bfa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41bfa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="41bfa-122">Authorization</span></span>|<span data-ttu-id="41bfa-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41bfa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41bfa-124">接受</span><span class="sxs-lookup"><span data-stu-id="41bfa-124">Accept</span></span>|<span data-ttu-id="41bfa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41bfa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41bfa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="41bfa-126">Request body</span></span>
<span data-ttu-id="41bfa-127">在请求正文中，提供 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41bfa-127">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="41bfa-128">下表显示创建 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="41bfa-128">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="41bfa-129">属性</span><span class="sxs-lookup"><span data-stu-id="41bfa-129">Property</span></span>|<span data-ttu-id="41bfa-130">类型</span><span class="sxs-lookup"><span data-stu-id="41bfa-130">Type</span></span>|<span data-ttu-id="41bfa-131">说明</span><span class="sxs-lookup"><span data-stu-id="41bfa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41bfa-132">id</span><span class="sxs-lookup"><span data-stu-id="41bfa-132">id</span></span>|<span data-ttu-id="41bfa-133">String</span><span class="sxs-lookup"><span data-stu-id="41bfa-133">String</span></span>|<span data-ttu-id="41bfa-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="41bfa-134">Key of the entity.</span></span> <span data-ttu-id="41bfa-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-136">displayName</span><span class="sxs-lookup"><span data-stu-id="41bfa-136">displayName</span></span>|<span data-ttu-id="41bfa-137">String</span><span class="sxs-lookup"><span data-stu-id="41bfa-137">String</span></span>|<span data-ttu-id="41bfa-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="41bfa-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="41bfa-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-140">description</span><span class="sxs-lookup"><span data-stu-id="41bfa-140">description</span></span>|<span data-ttu-id="41bfa-141">String</span><span class="sxs-lookup"><span data-stu-id="41bfa-141">String</span></span>|<span data-ttu-id="41bfa-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="41bfa-142">The description of the app.</span></span> <span data-ttu-id="41bfa-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-144">publisher</span><span class="sxs-lookup"><span data-stu-id="41bfa-144">publisher</span></span>|<span data-ttu-id="41bfa-145">String</span><span class="sxs-lookup"><span data-stu-id="41bfa-145">String</span></span>|<span data-ttu-id="41bfa-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="41bfa-146">The publisher of the app.</span></span> <span data-ttu-id="41bfa-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="41bfa-148">largeIcon</span></span>|[<span data-ttu-id="41bfa-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="41bfa-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="41bfa-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="41bfa-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="41bfa-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="41bfa-152">createdDateTime</span></span>|<span data-ttu-id="41bfa-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41bfa-153">DateTimeOffset</span></span>|<span data-ttu-id="41bfa-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="41bfa-154">The date and time the app was created.</span></span> <span data-ttu-id="41bfa-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="41bfa-156">lastModifiedDateTime</span></span>|<span data-ttu-id="41bfa-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41bfa-157">DateTimeOffset</span></span>|<span data-ttu-id="41bfa-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="41bfa-158">The date and time the app was last modified.</span></span> <span data-ttu-id="41bfa-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="41bfa-160">isFeatured</span></span>|<span data-ttu-id="41bfa-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="41bfa-161">Boolean</span></span>|<span data-ttu-id="41bfa-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="41bfa-163">privacyInformationUrl</span></span>|<span data-ttu-id="41bfa-164">String</span><span class="sxs-lookup"><span data-stu-id="41bfa-164">String</span></span>|<span data-ttu-id="41bfa-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="41bfa-165">The privacy statement Url.</span></span> <span data-ttu-id="41bfa-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="41bfa-167">informationUrl</span></span>|<span data-ttu-id="41bfa-168">String</span><span class="sxs-lookup"><span data-stu-id="41bfa-168">String</span></span>|<span data-ttu-id="41bfa-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="41bfa-169">The more information Url.</span></span> <span data-ttu-id="41bfa-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-171">owner</span><span class="sxs-lookup"><span data-stu-id="41bfa-171">owner</span></span>|<span data-ttu-id="41bfa-172">字符串</span><span class="sxs-lookup"><span data-stu-id="41bfa-172">String</span></span>|<span data-ttu-id="41bfa-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="41bfa-173">The owner of the app.</span></span> <span data-ttu-id="41bfa-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-175">developer</span><span class="sxs-lookup"><span data-stu-id="41bfa-175">developer</span></span>|<span data-ttu-id="41bfa-176">String</span><span class="sxs-lookup"><span data-stu-id="41bfa-176">String</span></span>|<span data-ttu-id="41bfa-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="41bfa-177">The developer of the app.</span></span> <span data-ttu-id="41bfa-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-179">notes</span><span class="sxs-lookup"><span data-stu-id="41bfa-179">notes</span></span>|<span data-ttu-id="41bfa-180">String</span><span class="sxs-lookup"><span data-stu-id="41bfa-180">String</span></span>|<span data-ttu-id="41bfa-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="41bfa-181">Notes for the app.</span></span> <span data-ttu-id="41bfa-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="41bfa-183">uploadState</span></span>|<span data-ttu-id="41bfa-184">Int32</span><span class="sxs-lookup"><span data-stu-id="41bfa-184">Int32</span></span>|<span data-ttu-id="41bfa-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="41bfa-185">The upload state.</span></span> <span data-ttu-id="41bfa-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="41bfa-187">publishingState</span></span>|[<span data-ttu-id="41bfa-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="41bfa-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="41bfa-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="41bfa-189">The publishing state for the app.</span></span> <span data-ttu-id="41bfa-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="41bfa-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="41bfa-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="41bfa-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="41bfa-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="41bfa-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="41bfa-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="41bfa-193">isAssigned</span></span>|<span data-ttu-id="41bfa-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="41bfa-194">Boolean</span></span>|<span data-ttu-id="41bfa-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="41bfa-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="41bfa-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="41bfa-197">roleScopeTagIds</span></span>|<span data-ttu-id="41bfa-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="41bfa-198">String collection</span></span>|<span data-ttu-id="41bfa-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="41bfa-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="41bfa-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="41bfa-201">dependentAppCount</span></span>|<span data-ttu-id="41bfa-202">Int32</span><span class="sxs-lookup"><span data-stu-id="41bfa-202">Int32</span></span>|<span data-ttu-id="41bfa-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="41bfa-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="41bfa-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="41bfa-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="41bfa-205">committedContentVersion</span></span>|<span data-ttu-id="41bfa-206">String</span><span class="sxs-lookup"><span data-stu-id="41bfa-206">String</span></span>|<span data-ttu-id="41bfa-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="41bfa-207">The internal committed content version.</span></span> <span data-ttu-id="41bfa-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="41bfa-209">fileName</span><span class="sxs-lookup"><span data-stu-id="41bfa-209">fileName</span></span>|<span data-ttu-id="41bfa-210">String</span><span class="sxs-lookup"><span data-stu-id="41bfa-210">String</span></span>|<span data-ttu-id="41bfa-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="41bfa-211">The name of the main Lob application file.</span></span> <span data-ttu-id="41bfa-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="41bfa-213">size</span><span class="sxs-lookup"><span data-stu-id="41bfa-213">size</span></span>|<span data-ttu-id="41bfa-214">Int64</span><span class="sxs-lookup"><span data-stu-id="41bfa-214">Int64</span></span>|<span data-ttu-id="41bfa-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="41bfa-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="41bfa-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="41bfa-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="41bfa-217">commandLine</span><span class="sxs-lookup"><span data-stu-id="41bfa-217">commandLine</span></span>|<span data-ttu-id="41bfa-218">String</span><span class="sxs-lookup"><span data-stu-id="41bfa-218">String</span></span>|<span data-ttu-id="41bfa-219">命令行。</span><span class="sxs-lookup"><span data-stu-id="41bfa-219">The command line.</span></span>|
|<span data-ttu-id="41bfa-220">productCode</span><span class="sxs-lookup"><span data-stu-id="41bfa-220">productCode</span></span>|<span data-ttu-id="41bfa-221">String</span><span class="sxs-lookup"><span data-stu-id="41bfa-221">String</span></span>|<span data-ttu-id="41bfa-222">产品代码。</span><span class="sxs-lookup"><span data-stu-id="41bfa-222">The product code.</span></span>|
|<span data-ttu-id="41bfa-223">productVersion</span><span class="sxs-lookup"><span data-stu-id="41bfa-223">productVersion</span></span>|<span data-ttu-id="41bfa-224">String</span><span class="sxs-lookup"><span data-stu-id="41bfa-224">String</span></span>|<span data-ttu-id="41bfa-225">Windows Mobile MSI 业务线 (LoB) 应用的产品版本。</span><span class="sxs-lookup"><span data-stu-id="41bfa-225">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="41bfa-226">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="41bfa-226">ignoreVersionDetection</span></span>|<span data-ttu-id="41bfa-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="41bfa-227">Boolean</span></span>|<span data-ttu-id="41bfa-228">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="41bfa-228">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="41bfa-229">对于使用自更新功能的 Windows Mobile MSI 业务线 (LoB) 应用，将此值设置为 true。</span><span class="sxs-lookup"><span data-stu-id="41bfa-229">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="41bfa-230">identityVersion</span><span class="sxs-lookup"><span data-stu-id="41bfa-230">identityVersion</span></span>|<span data-ttu-id="41bfa-231">String</span><span class="sxs-lookup"><span data-stu-id="41bfa-231">String</span></span>|<span data-ttu-id="41bfa-232">标识版本。</span><span class="sxs-lookup"><span data-stu-id="41bfa-232">The identity version.</span></span>|
|<span data-ttu-id="41bfa-233">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="41bfa-233">useDeviceContext</span></span>|<span data-ttu-id="41bfa-234">布尔值</span><span class="sxs-lookup"><span data-stu-id="41bfa-234">Boolean</span></span>|<span data-ttu-id="41bfa-235">指示是否在设备上下文中安装双模式 MSI。</span><span class="sxs-lookup"><span data-stu-id="41bfa-235">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="41bfa-236">如果为 true, 则将为所有用户安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="41bfa-236">If true, app will be installed for all users.</span></span> <span data-ttu-id="41bfa-237">如果为 false, 将按用户安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="41bfa-237">If false, app will be installed per-user.</span></span> <span data-ttu-id="41bfa-238">如果为 null, 服务将使用 MSI 包的默认安装上下文。</span><span class="sxs-lookup"><span data-stu-id="41bfa-238">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="41bfa-239">在双模式 MSI 的情况下, 此默认值将为每个用户。</span><span class="sxs-lookup"><span data-stu-id="41bfa-239">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="41bfa-240">不能为非双重模式的应用程序进行设置。</span><span class="sxs-lookup"><span data-stu-id="41bfa-240">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="41bfa-241">在首次创建应用程序后, 不能更改。</span><span class="sxs-lookup"><span data-stu-id="41bfa-241">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="41bfa-242">响应</span><span class="sxs-lookup"><span data-stu-id="41bfa-242">Response</span></span>
<span data-ttu-id="41bfa-243">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41bfa-243">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41bfa-244">示例</span><span class="sxs-lookup"><span data-stu-id="41bfa-244">Example</span></span>

### <a name="request"></a><span data-ttu-id="41bfa-245">请求</span><span class="sxs-lookup"><span data-stu-id="41bfa-245">Request</span></span>
<span data-ttu-id="41bfa-246">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41bfa-246">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1066

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="41bfa-247">响应</span><span class="sxs-lookup"><span data-stu-id="41bfa-247">Response</span></span>
<span data-ttu-id="41bfa-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41bfa-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1238

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```





