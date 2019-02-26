---
title: 创建了 windowsphone81appx
description: 创建新的了 windowsphone81appx 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 678e21a2d3b662ed322dc26a07f2f110312a4ff1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166484"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="a8586-103">创建了 windowsphone81appx</span><span class="sxs-lookup"><span data-stu-id="a8586-103">Create windowsPhone81AppX</span></span>

> <span data-ttu-id="a8586-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a8586-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8586-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a8586-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8586-106">创建新的[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a8586-106">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8586-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a8586-107">Prerequisites</span></span>
<span data-ttu-id="a8586-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a8586-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a8586-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8586-110">Permission type</span></span>|<span data-ttu-id="a8586-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a8586-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8586-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8586-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8586-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8586-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a8586-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8586-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8586-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8586-115">Not supported.</span></span>|
|<span data-ttu-id="a8586-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8586-116">Application</span></span>|<span data-ttu-id="a8586-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8586-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8586-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8586-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a8586-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8586-119">Request headers</span></span>
|<span data-ttu-id="a8586-120">标头</span><span class="sxs-lookup"><span data-stu-id="a8586-120">Header</span></span>|<span data-ttu-id="a8586-121">值</span><span class="sxs-lookup"><span data-stu-id="a8586-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8586-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8586-122">Authorization</span></span>|<span data-ttu-id="a8586-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a8586-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8586-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a8586-124">Accept</span></span>|<span data-ttu-id="a8586-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a8586-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8586-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8586-126">Request body</span></span>
<span data-ttu-id="a8586-127">在请求正文中, 提供了 windowsphone81appx 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8586-127">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="a8586-128">下表显示创建了 windowsphone81appx 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a8586-128">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="a8586-129">属性</span><span class="sxs-lookup"><span data-stu-id="a8586-129">Property</span></span>|<span data-ttu-id="a8586-130">类型</span><span class="sxs-lookup"><span data-stu-id="a8586-130">Type</span></span>|<span data-ttu-id="a8586-131">说明</span><span class="sxs-lookup"><span data-stu-id="a8586-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8586-132">id</span><span class="sxs-lookup"><span data-stu-id="a8586-132">id</span></span>|<span data-ttu-id="a8586-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a8586-133">String</span></span>|<span data-ttu-id="a8586-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a8586-134">Key of the entity.</span></span> <span data-ttu-id="a8586-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a8586-136">displayName</span></span>|<span data-ttu-id="a8586-137">String</span><span class="sxs-lookup"><span data-stu-id="a8586-137">String</span></span>|<span data-ttu-id="a8586-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="a8586-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a8586-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-140">description</span><span class="sxs-lookup"><span data-stu-id="a8586-140">description</span></span>|<span data-ttu-id="a8586-141">字符串</span><span class="sxs-lookup"><span data-stu-id="a8586-141">String</span></span>|<span data-ttu-id="a8586-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="a8586-142">The description of the app.</span></span> <span data-ttu-id="a8586-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-144">publisher</span><span class="sxs-lookup"><span data-stu-id="a8586-144">publisher</span></span>|<span data-ttu-id="a8586-145">String</span><span class="sxs-lookup"><span data-stu-id="a8586-145">String</span></span>|<span data-ttu-id="a8586-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="a8586-146">The publisher of the app.</span></span> <span data-ttu-id="a8586-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a8586-148">largeIcon</span></span>|[<span data-ttu-id="a8586-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a8586-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a8586-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="a8586-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a8586-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8586-152">createdDateTime</span></span>|<span data-ttu-id="a8586-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8586-153">DateTimeOffset</span></span>|<span data-ttu-id="a8586-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a8586-154">The date and time the app was created.</span></span> <span data-ttu-id="a8586-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8586-156">lastModifiedDateTime</span></span>|<span data-ttu-id="a8586-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8586-157">DateTimeOffset</span></span>|<span data-ttu-id="a8586-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a8586-158">The date and time the app was last modified.</span></span> <span data-ttu-id="a8586-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a8586-160">isFeatured</span></span>|<span data-ttu-id="a8586-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8586-161">Boolean</span></span>|<span data-ttu-id="a8586-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a8586-163">privacyInformationUrl</span></span>|<span data-ttu-id="a8586-164">String</span><span class="sxs-lookup"><span data-stu-id="a8586-164">String</span></span>|<span data-ttu-id="a8586-165">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="a8586-165">The privacy statement Url.</span></span> <span data-ttu-id="a8586-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a8586-167">informationUrl</span></span>|<span data-ttu-id="a8586-168">String</span><span class="sxs-lookup"><span data-stu-id="a8586-168">String</span></span>|<span data-ttu-id="a8586-169">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="a8586-169">The more information Url.</span></span> <span data-ttu-id="a8586-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-171">owner</span><span class="sxs-lookup"><span data-stu-id="a8586-171">owner</span></span>|<span data-ttu-id="a8586-172">String</span><span class="sxs-lookup"><span data-stu-id="a8586-172">String</span></span>|<span data-ttu-id="a8586-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="a8586-173">The owner of the app.</span></span> <span data-ttu-id="a8586-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-175">developer</span><span class="sxs-lookup"><span data-stu-id="a8586-175">developer</span></span>|<span data-ttu-id="a8586-176">String</span><span class="sxs-lookup"><span data-stu-id="a8586-176">String</span></span>|<span data-ttu-id="a8586-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="a8586-177">The developer of the app.</span></span> <span data-ttu-id="a8586-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-179">notes</span><span class="sxs-lookup"><span data-stu-id="a8586-179">notes</span></span>|<span data-ttu-id="a8586-180">String</span><span class="sxs-lookup"><span data-stu-id="a8586-180">String</span></span>|<span data-ttu-id="a8586-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="a8586-181">Notes for the app.</span></span> <span data-ttu-id="a8586-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="a8586-183">uploadState</span></span>|<span data-ttu-id="a8586-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a8586-184">Int32</span></span>|<span data-ttu-id="a8586-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="a8586-185">The upload state.</span></span> <span data-ttu-id="a8586-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="a8586-187">publishingState</span></span>|[<span data-ttu-id="a8586-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a8586-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a8586-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="a8586-189">The publishing state for the app.</span></span> <span data-ttu-id="a8586-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="a8586-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a8586-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="a8586-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a8586-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="a8586-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a8586-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a8586-193">isAssigned</span></span>|<span data-ttu-id="a8586-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8586-194">Boolean</span></span>|<span data-ttu-id="a8586-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="a8586-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a8586-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a8586-197">roleScopeTagIds</span></span>|<span data-ttu-id="a8586-198">String collection</span><span class="sxs-lookup"><span data-stu-id="a8586-198">String collection</span></span>|<span data-ttu-id="a8586-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="a8586-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a8586-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8586-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a8586-201">committedContentVersion</span></span>|<span data-ttu-id="a8586-202">String</span><span class="sxs-lookup"><span data-stu-id="a8586-202">String</span></span>|<span data-ttu-id="a8586-203">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="a8586-203">The internal committed content version.</span></span> <span data-ttu-id="a8586-204">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a8586-205">fileName</span><span class="sxs-lookup"><span data-stu-id="a8586-205">fileName</span></span>|<span data-ttu-id="a8586-206">String</span><span class="sxs-lookup"><span data-stu-id="a8586-206">String</span></span>|<span data-ttu-id="a8586-207">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="a8586-207">The name of the main Lob application file.</span></span> <span data-ttu-id="a8586-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a8586-209">size</span><span class="sxs-lookup"><span data-stu-id="a8586-209">size</span></span>|<span data-ttu-id="a8586-210">Int64</span><span class="sxs-lookup"><span data-stu-id="a8586-210">Int64</span></span>|<span data-ttu-id="a8586-211">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="a8586-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="a8586-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a8586-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a8586-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="a8586-213">applicableArchitectures</span></span>|[<span data-ttu-id="a8586-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="a8586-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="a8586-215">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="a8586-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="a8586-216">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="a8586-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="a8586-217">identityName</span><span class="sxs-lookup"><span data-stu-id="a8586-217">identityName</span></span>|<span data-ttu-id="a8586-218">String</span><span class="sxs-lookup"><span data-stu-id="a8586-218">String</span></span>|<span data-ttu-id="a8586-219">标识名称。</span><span class="sxs-lookup"><span data-stu-id="a8586-219">The Identity Name.</span></span>|
|<span data-ttu-id="a8586-220">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="a8586-220">identityPublisherHash</span></span>|<span data-ttu-id="a8586-221">String</span><span class="sxs-lookup"><span data-stu-id="a8586-221">String</span></span>|<span data-ttu-id="a8586-222">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="a8586-222">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="a8586-223">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="a8586-223">identityResourceIdentifier</span></span>|<span data-ttu-id="a8586-224">String</span><span class="sxs-lookup"><span data-stu-id="a8586-224">String</span></span>|<span data-ttu-id="a8586-225">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="a8586-225">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="a8586-226">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a8586-226">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="a8586-227">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="a8586-227">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="a8586-228">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="a8586-228">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="a8586-229">将 phoneproductidentifier</span><span class="sxs-lookup"><span data-stu-id="a8586-229">phoneProductIdentifier</span></span>|<span data-ttu-id="a8586-230">String</span><span class="sxs-lookup"><span data-stu-id="a8586-230">String</span></span>|<span data-ttu-id="a8586-231">电话产品标识符。</span><span class="sxs-lookup"><span data-stu-id="a8586-231">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="a8586-232">将 phonepublisherid</span><span class="sxs-lookup"><span data-stu-id="a8586-232">phonePublisherId</span></span>|<span data-ttu-id="a8586-233">String</span><span class="sxs-lookup"><span data-stu-id="a8586-233">String</span></span>|<span data-ttu-id="a8586-234">电话发布者 Id。</span><span class="sxs-lookup"><span data-stu-id="a8586-234">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="a8586-235">identityVersion</span><span class="sxs-lookup"><span data-stu-id="a8586-235">identityVersion</span></span>|<span data-ttu-id="a8586-236">String</span><span class="sxs-lookup"><span data-stu-id="a8586-236">String</span></span>|<span data-ttu-id="a8586-237">标识版本。</span><span class="sxs-lookup"><span data-stu-id="a8586-237">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="a8586-238">响应</span><span class="sxs-lookup"><span data-stu-id="a8586-238">Response</span></span>
<span data-ttu-id="a8586-239">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a8586-239">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8586-240">示例</span><span class="sxs-lookup"><span data-stu-id="a8586-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8586-241">请求</span><span class="sxs-lookup"><span data-stu-id="a8586-241">Request</span></span>
<span data-ttu-id="a8586-242">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8586-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1440

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
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
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="a8586-243">响应</span><span class="sxs-lookup"><span data-stu-id="a8586-243">Response</span></span>
<span data-ttu-id="a8586-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a8586-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1612

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppX",
  "id": "4ff27f80-7f80-4ff2-807f-f24f807ff24f",
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
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value"
}
```




