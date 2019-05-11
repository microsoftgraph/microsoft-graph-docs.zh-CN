---
title: 创建 windowsPhoneXAP
description: 创建新的 windowsPhoneXAP 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ebdd779fb8b0280d46df8fa74d7debed1085cd8a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934556"
---
# <a name="create-windowsphonexap"></a><span data-ttu-id="9d6c0-103">创建 windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="9d6c0-103">Create windowsPhoneXAP</span></span>

> <span data-ttu-id="9d6c0-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d6c0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d6c0-106">创建新的[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-106">Create a new [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d6c0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9d6c0-107">Prerequisites</span></span>
<span data-ttu-id="9d6c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d6c0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d6c0-110">Permission type</span></span>|<span data-ttu-id="9d6c0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9d6c0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d6c0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d6c0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9d6c0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d6c0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9d6c0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d6c0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d6c0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-115">Not supported.</span></span>|
|<span data-ttu-id="9d6c0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d6c0-116">Application</span></span>|<span data-ttu-id="9d6c0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d6c0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d6c0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="9d6c0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d6c0-119">Request headers</span></span>
|<span data-ttu-id="9d6c0-120">标头</span><span class="sxs-lookup"><span data-stu-id="9d6c0-120">Header</span></span>|<span data-ttu-id="9d6c0-121">值</span><span class="sxs-lookup"><span data-stu-id="9d6c0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d6c0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d6c0-122">Authorization</span></span>|<span data-ttu-id="9d6c0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d6c0-124">接受</span><span class="sxs-lookup"><span data-stu-id="9d6c0-124">Accept</span></span>|<span data-ttu-id="9d6c0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9d6c0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d6c0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d6c0-126">Request body</span></span>
<span data-ttu-id="9d6c0-127">在请求正文中, 提供 windowsPhoneXAP 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-127">In the request body, supply a JSON representation for the windowsPhoneXAP object.</span></span>

<span data-ttu-id="9d6c0-128">下表显示创建 windowsPhoneXAP 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-128">The following table shows the properties that are required when you create the windowsPhoneXAP.</span></span>

|<span data-ttu-id="9d6c0-129">属性</span><span class="sxs-lookup"><span data-stu-id="9d6c0-129">Property</span></span>|<span data-ttu-id="9d6c0-130">类型</span><span class="sxs-lookup"><span data-stu-id="9d6c0-130">Type</span></span>|<span data-ttu-id="9d6c0-131">说明</span><span class="sxs-lookup"><span data-stu-id="9d6c0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d6c0-132">id</span><span class="sxs-lookup"><span data-stu-id="9d6c0-132">id</span></span>|<span data-ttu-id="9d6c0-133">字符串</span><span class="sxs-lookup"><span data-stu-id="9d6c0-133">String</span></span>|<span data-ttu-id="9d6c0-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-134">Key of the entity.</span></span> <span data-ttu-id="9d6c0-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9d6c0-136">displayName</span></span>|<span data-ttu-id="9d6c0-137">String</span><span class="sxs-lookup"><span data-stu-id="9d6c0-137">String</span></span>|<span data-ttu-id="9d6c0-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9d6c0-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-140">说明</span><span class="sxs-lookup"><span data-stu-id="9d6c0-140">description</span></span>|<span data-ttu-id="9d6c0-141">字符串</span><span class="sxs-lookup"><span data-stu-id="9d6c0-141">String</span></span>|<span data-ttu-id="9d6c0-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-142">The description of the app.</span></span> <span data-ttu-id="9d6c0-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-144">publisher</span><span class="sxs-lookup"><span data-stu-id="9d6c0-144">publisher</span></span>|<span data-ttu-id="9d6c0-145">String</span><span class="sxs-lookup"><span data-stu-id="9d6c0-145">String</span></span>|<span data-ttu-id="9d6c0-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-146">The publisher of the app.</span></span> <span data-ttu-id="9d6c0-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9d6c0-148">largeIcon</span></span>|[<span data-ttu-id="9d6c0-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9d6c0-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9d6c0-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9d6c0-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d6c0-152">createdDateTime</span></span>|<span data-ttu-id="9d6c0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d6c0-153">DateTimeOffset</span></span>|<span data-ttu-id="9d6c0-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-154">The date and time the app was created.</span></span> <span data-ttu-id="9d6c0-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d6c0-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9d6c0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d6c0-157">DateTimeOffset</span></span>|<span data-ttu-id="9d6c0-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-158">The date and time the app was last modified.</span></span> <span data-ttu-id="9d6c0-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9d6c0-160">isFeatured</span></span>|<span data-ttu-id="9d6c0-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d6c0-161">Boolean</span></span>|<span data-ttu-id="9d6c0-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9d6c0-163">privacyInformationUrl</span></span>|<span data-ttu-id="9d6c0-164">String</span><span class="sxs-lookup"><span data-stu-id="9d6c0-164">String</span></span>|<span data-ttu-id="9d6c0-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-165">The privacy statement Url.</span></span> <span data-ttu-id="9d6c0-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9d6c0-167">informationUrl</span></span>|<span data-ttu-id="9d6c0-168">String</span><span class="sxs-lookup"><span data-stu-id="9d6c0-168">String</span></span>|<span data-ttu-id="9d6c0-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-169">The more information Url.</span></span> <span data-ttu-id="9d6c0-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-171">owner</span><span class="sxs-lookup"><span data-stu-id="9d6c0-171">owner</span></span>|<span data-ttu-id="9d6c0-172">String</span><span class="sxs-lookup"><span data-stu-id="9d6c0-172">String</span></span>|<span data-ttu-id="9d6c0-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-173">The owner of the app.</span></span> <span data-ttu-id="9d6c0-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-175">developer</span><span class="sxs-lookup"><span data-stu-id="9d6c0-175">developer</span></span>|<span data-ttu-id="9d6c0-176">String</span><span class="sxs-lookup"><span data-stu-id="9d6c0-176">String</span></span>|<span data-ttu-id="9d6c0-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-177">The developer of the app.</span></span> <span data-ttu-id="9d6c0-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-179">notes</span><span class="sxs-lookup"><span data-stu-id="9d6c0-179">notes</span></span>|<span data-ttu-id="9d6c0-180">String</span><span class="sxs-lookup"><span data-stu-id="9d6c0-180">String</span></span>|<span data-ttu-id="9d6c0-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-181">Notes for the app.</span></span> <span data-ttu-id="9d6c0-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="9d6c0-183">uploadState</span></span>|<span data-ttu-id="9d6c0-184">Int32</span><span class="sxs-lookup"><span data-stu-id="9d6c0-184">Int32</span></span>|<span data-ttu-id="9d6c0-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-185">The upload state.</span></span> <span data-ttu-id="9d6c0-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="9d6c0-187">publishingState</span></span>|[<span data-ttu-id="9d6c0-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9d6c0-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9d6c0-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-189">The publishing state for the app.</span></span> <span data-ttu-id="9d6c0-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9d6c0-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9d6c0-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9d6c0-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="9d6c0-193">isAssigned</span></span>|<span data-ttu-id="9d6c0-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d6c0-194">Boolean</span></span>|<span data-ttu-id="9d6c0-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="9d6c0-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9d6c0-197">roleScopeTagIds</span></span>|<span data-ttu-id="9d6c0-198">String collection</span><span class="sxs-lookup"><span data-stu-id="9d6c0-198">String collection</span></span>|<span data-ttu-id="9d6c0-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="9d6c0-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="9d6c0-201">dependentAppCount</span></span>|<span data-ttu-id="9d6c0-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9d6c0-202">Int32</span></span>|<span data-ttu-id="9d6c0-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="9d6c0-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9d6c0-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9d6c0-205">committedContentVersion</span></span>|<span data-ttu-id="9d6c0-206">String</span><span class="sxs-lookup"><span data-stu-id="9d6c0-206">String</span></span>|<span data-ttu-id="9d6c0-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-207">The internal committed content version.</span></span> <span data-ttu-id="9d6c0-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9d6c0-209">fileName</span><span class="sxs-lookup"><span data-stu-id="9d6c0-209">fileName</span></span>|<span data-ttu-id="9d6c0-210">String</span><span class="sxs-lookup"><span data-stu-id="9d6c0-210">String</span></span>|<span data-ttu-id="9d6c0-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-211">The name of the main Lob application file.</span></span> <span data-ttu-id="9d6c0-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9d6c0-213">size</span><span class="sxs-lookup"><span data-stu-id="9d6c0-213">size</span></span>|<span data-ttu-id="9d6c0-214">Int64</span><span class="sxs-lookup"><span data-stu-id="9d6c0-214">Int64</span></span>|<span data-ttu-id="9d6c0-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="9d6c0-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d6c0-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9d6c0-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9d6c0-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9d6c0-218">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9d6c0-218">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="9d6c0-219">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-219">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9d6c0-220">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="9d6c0-220">productIdentifier</span></span>|<span data-ttu-id="9d6c0-221">String</span><span class="sxs-lookup"><span data-stu-id="9d6c0-221">String</span></span>|<span data-ttu-id="9d6c0-222">产品标识符。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-222">The Product Identifier.</span></span>|
|<span data-ttu-id="9d6c0-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9d6c0-223">identityVersion</span></span>|<span data-ttu-id="9d6c0-224">String</span><span class="sxs-lookup"><span data-stu-id="9d6c0-224">String</span></span>|<span data-ttu-id="9d6c0-225">标识版本。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="9d6c0-226">响应</span><span class="sxs-lookup"><span data-stu-id="9d6c0-226">Response</span></span>
<span data-ttu-id="9d6c0-227">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-227">If successful, this method returns a `201 Created` response code and a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d6c0-228">示例</span><span class="sxs-lookup"><span data-stu-id="9d6c0-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d6c0-229">请求</span><span class="sxs-lookup"><span data-stu-id="9d6c0-229">Request</span></span>
<span data-ttu-id="9d6c0-230">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1191

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
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
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="9d6c0-231">响应</span><span class="sxs-lookup"><span data-stu-id="9d6c0-231">Response</span></span>
<span data-ttu-id="9d6c0-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9d6c0-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1363

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```




