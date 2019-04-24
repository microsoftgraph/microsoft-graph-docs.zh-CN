---
title: 创建 windowsPhoneXAP
description: 创建新的 windowsPhoneXAP 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c148b0df6e5aff01ed5afe4fc61a482ef15530b5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32487824"
---
# <a name="create-windowsphonexap"></a><span data-ttu-id="f36dd-103">创建 windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="f36dd-103">Create windowsPhoneXAP</span></span>

> <span data-ttu-id="f36dd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f36dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f36dd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f36dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f36dd-106">创建新的[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f36dd-106">Create a new [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f36dd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f36dd-107">Prerequisites</span></span>
<span data-ttu-id="f36dd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f36dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f36dd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f36dd-110">Permission type</span></span>|<span data-ttu-id="f36dd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f36dd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f36dd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f36dd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f36dd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f36dd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f36dd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f36dd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f36dd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f36dd-115">Not supported.</span></span>|
|<span data-ttu-id="f36dd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f36dd-116">Application</span></span>|<span data-ttu-id="f36dd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f36dd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f36dd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f36dd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f36dd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f36dd-119">Request headers</span></span>
|<span data-ttu-id="f36dd-120">标头</span><span class="sxs-lookup"><span data-stu-id="f36dd-120">Header</span></span>|<span data-ttu-id="f36dd-121">值</span><span class="sxs-lookup"><span data-stu-id="f36dd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f36dd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f36dd-122">Authorization</span></span>|<span data-ttu-id="f36dd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f36dd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f36dd-124">接受</span><span class="sxs-lookup"><span data-stu-id="f36dd-124">Accept</span></span>|<span data-ttu-id="f36dd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f36dd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f36dd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f36dd-126">Request body</span></span>
<span data-ttu-id="f36dd-127">在请求正文中, 提供 windowsPhoneXAP 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f36dd-127">In the request body, supply a JSON representation for the windowsPhoneXAP object.</span></span>

<span data-ttu-id="f36dd-128">下表显示创建 windowsPhoneXAP 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f36dd-128">The following table shows the properties that are required when you create the windowsPhoneXAP.</span></span>

|<span data-ttu-id="f36dd-129">属性</span><span class="sxs-lookup"><span data-stu-id="f36dd-129">Property</span></span>|<span data-ttu-id="f36dd-130">类型</span><span class="sxs-lookup"><span data-stu-id="f36dd-130">Type</span></span>|<span data-ttu-id="f36dd-131">说明</span><span class="sxs-lookup"><span data-stu-id="f36dd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f36dd-132">id</span><span class="sxs-lookup"><span data-stu-id="f36dd-132">id</span></span>|<span data-ttu-id="f36dd-133">String</span><span class="sxs-lookup"><span data-stu-id="f36dd-133">String</span></span>|<span data-ttu-id="f36dd-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f36dd-134">Key of the entity.</span></span> <span data-ttu-id="f36dd-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f36dd-136">displayName</span></span>|<span data-ttu-id="f36dd-137">字符串</span><span class="sxs-lookup"><span data-stu-id="f36dd-137">String</span></span>|<span data-ttu-id="f36dd-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="f36dd-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f36dd-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-140">description</span><span class="sxs-lookup"><span data-stu-id="f36dd-140">description</span></span>|<span data-ttu-id="f36dd-141">字符串</span><span class="sxs-lookup"><span data-stu-id="f36dd-141">String</span></span>|<span data-ttu-id="f36dd-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="f36dd-142">The description of the app.</span></span> <span data-ttu-id="f36dd-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-144">publisher</span><span class="sxs-lookup"><span data-stu-id="f36dd-144">publisher</span></span>|<span data-ttu-id="f36dd-145">字符串</span><span class="sxs-lookup"><span data-stu-id="f36dd-145">String</span></span>|<span data-ttu-id="f36dd-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="f36dd-146">The publisher of the app.</span></span> <span data-ttu-id="f36dd-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f36dd-148">largeIcon</span></span>|[<span data-ttu-id="f36dd-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f36dd-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f36dd-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="f36dd-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f36dd-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f36dd-152">createdDateTime</span></span>|<span data-ttu-id="f36dd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f36dd-153">DateTimeOffset</span></span>|<span data-ttu-id="f36dd-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f36dd-154">The date and time the app was created.</span></span> <span data-ttu-id="f36dd-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f36dd-156">lastModifiedDateTime</span></span>|<span data-ttu-id="f36dd-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f36dd-157">DateTimeOffset</span></span>|<span data-ttu-id="f36dd-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f36dd-158">The date and time the app was last modified.</span></span> <span data-ttu-id="f36dd-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f36dd-160">isFeatured</span></span>|<span data-ttu-id="f36dd-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="f36dd-161">Boolean</span></span>|<span data-ttu-id="f36dd-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f36dd-163">privacyInformationUrl</span></span>|<span data-ttu-id="f36dd-164">字符串</span><span class="sxs-lookup"><span data-stu-id="f36dd-164">String</span></span>|<span data-ttu-id="f36dd-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="f36dd-165">The privacy statement Url.</span></span> <span data-ttu-id="f36dd-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f36dd-167">informationUrl</span></span>|<span data-ttu-id="f36dd-168">字符串</span><span class="sxs-lookup"><span data-stu-id="f36dd-168">String</span></span>|<span data-ttu-id="f36dd-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="f36dd-169">The more information Url.</span></span> <span data-ttu-id="f36dd-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-171">owner</span><span class="sxs-lookup"><span data-stu-id="f36dd-171">owner</span></span>|<span data-ttu-id="f36dd-172">字符串</span><span class="sxs-lookup"><span data-stu-id="f36dd-172">String</span></span>|<span data-ttu-id="f36dd-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="f36dd-173">The owner of the app.</span></span> <span data-ttu-id="f36dd-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-175">developer</span><span class="sxs-lookup"><span data-stu-id="f36dd-175">developer</span></span>|<span data-ttu-id="f36dd-176">字符串</span><span class="sxs-lookup"><span data-stu-id="f36dd-176">String</span></span>|<span data-ttu-id="f36dd-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="f36dd-177">The developer of the app.</span></span> <span data-ttu-id="f36dd-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-179">notes</span><span class="sxs-lookup"><span data-stu-id="f36dd-179">notes</span></span>|<span data-ttu-id="f36dd-180">字符串</span><span class="sxs-lookup"><span data-stu-id="f36dd-180">String</span></span>|<span data-ttu-id="f36dd-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="f36dd-181">Notes for the app.</span></span> <span data-ttu-id="f36dd-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="f36dd-183">uploadState</span></span>|<span data-ttu-id="f36dd-184">Int32</span><span class="sxs-lookup"><span data-stu-id="f36dd-184">Int32</span></span>|<span data-ttu-id="f36dd-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="f36dd-185">The upload state.</span></span> <span data-ttu-id="f36dd-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="f36dd-187">publishingState</span></span>|[<span data-ttu-id="f36dd-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f36dd-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f36dd-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="f36dd-189">The publishing state for the app.</span></span> <span data-ttu-id="f36dd-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="f36dd-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f36dd-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="f36dd-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f36dd-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="f36dd-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f36dd-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f36dd-193">isAssigned</span></span>|<span data-ttu-id="f36dd-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f36dd-194">Boolean</span></span>|<span data-ttu-id="f36dd-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="f36dd-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f36dd-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f36dd-197">roleScopeTagIds</span></span>|<span data-ttu-id="f36dd-198">String collection</span><span class="sxs-lookup"><span data-stu-id="f36dd-198">String collection</span></span>|<span data-ttu-id="f36dd-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="f36dd-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f36dd-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="f36dd-201">dependentAppCount</span></span>|<span data-ttu-id="f36dd-202">Int32</span><span class="sxs-lookup"><span data-stu-id="f36dd-202">Int32</span></span>|<span data-ttu-id="f36dd-203">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="f36dd-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="f36dd-204">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f36dd-205">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f36dd-205">committedContentVersion</span></span>|<span data-ttu-id="f36dd-206">字符串</span><span class="sxs-lookup"><span data-stu-id="f36dd-206">String</span></span>|<span data-ttu-id="f36dd-207">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="f36dd-207">The internal committed content version.</span></span> <span data-ttu-id="f36dd-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f36dd-209">fileName</span><span class="sxs-lookup"><span data-stu-id="f36dd-209">fileName</span></span>|<span data-ttu-id="f36dd-210">字符串</span><span class="sxs-lookup"><span data-stu-id="f36dd-210">String</span></span>|<span data-ttu-id="f36dd-211">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="f36dd-211">The name of the main Lob application file.</span></span> <span data-ttu-id="f36dd-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f36dd-213">size</span><span class="sxs-lookup"><span data-stu-id="f36dd-213">size</span></span>|<span data-ttu-id="f36dd-214">Int64</span><span class="sxs-lookup"><span data-stu-id="f36dd-214">Int64</span></span>|<span data-ttu-id="f36dd-215">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="f36dd-215">The total size, including all uploaded files.</span></span> <span data-ttu-id="f36dd-216">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f36dd-216">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f36dd-217">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f36dd-217">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f36dd-218">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f36dd-218">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="f36dd-219">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="f36dd-219">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f36dd-220">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="f36dd-220">productIdentifier</span></span>|<span data-ttu-id="f36dd-221">字符串</span><span class="sxs-lookup"><span data-stu-id="f36dd-221">String</span></span>|<span data-ttu-id="f36dd-222">产品标识符。</span><span class="sxs-lookup"><span data-stu-id="f36dd-222">The Product Identifier.</span></span>|
|<span data-ttu-id="f36dd-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f36dd-223">identityVersion</span></span>|<span data-ttu-id="f36dd-224">String</span><span class="sxs-lookup"><span data-stu-id="f36dd-224">String</span></span>|<span data-ttu-id="f36dd-225">标识版本。</span><span class="sxs-lookup"><span data-stu-id="f36dd-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="f36dd-226">响应</span><span class="sxs-lookup"><span data-stu-id="f36dd-226">Response</span></span>
<span data-ttu-id="f36dd-227">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f36dd-227">If successful, this method returns a `201 Created` response code and a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f36dd-228">示例</span><span class="sxs-lookup"><span data-stu-id="f36dd-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="f36dd-229">请求</span><span class="sxs-lookup"><span data-stu-id="f36dd-229">Request</span></span>
<span data-ttu-id="f36dd-230">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f36dd-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f36dd-231">响应</span><span class="sxs-lookup"><span data-stu-id="f36dd-231">Response</span></span>
<span data-ttu-id="f36dd-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f36dd-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





