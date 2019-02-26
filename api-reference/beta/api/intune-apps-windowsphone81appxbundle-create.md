---
title: 创建了 windowsphone81appxbundle
description: 创建新的了 windowsphone81appxbundle 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cac7c3b6c46d17fe494098acf0b8a8656c65237
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154444"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="83325-103">创建了 windowsphone81appxbundle</span><span class="sxs-lookup"><span data-stu-id="83325-103">Create windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="83325-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="83325-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83325-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83325-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83325-106">创建新的[了 windowsphone81appxbundle](../resources/intune-apps-windowsphone81appxbundle.md)对象。</span><span class="sxs-lookup"><span data-stu-id="83325-106">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83325-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="83325-107">Prerequisites</span></span>
<span data-ttu-id="83325-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="83325-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="83325-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="83325-110">Permission type</span></span>|<span data-ttu-id="83325-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="83325-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83325-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83325-112">Delegated (work or school account)</span></span>|<span data-ttu-id="83325-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83325-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="83325-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83325-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83325-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="83325-115">Not supported.</span></span>|
|<span data-ttu-id="83325-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="83325-116">Application</span></span>|<span data-ttu-id="83325-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="83325-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83325-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83325-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="83325-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="83325-119">Request headers</span></span>
|<span data-ttu-id="83325-120">标头</span><span class="sxs-lookup"><span data-stu-id="83325-120">Header</span></span>|<span data-ttu-id="83325-121">值</span><span class="sxs-lookup"><span data-stu-id="83325-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83325-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="83325-122">Authorization</span></span>|<span data-ttu-id="83325-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="83325-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83325-124">Accept</span><span class="sxs-lookup"><span data-stu-id="83325-124">Accept</span></span>|<span data-ttu-id="83325-125">application/json</span><span class="sxs-lookup"><span data-stu-id="83325-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83325-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="83325-126">Request body</span></span>
<span data-ttu-id="83325-127">在请求正文中, 提供了 windowsphone81appxbundle 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83325-127">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="83325-128">下表显示创建了 windowsphone81appxbundle 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="83325-128">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="83325-129">属性</span><span class="sxs-lookup"><span data-stu-id="83325-129">Property</span></span>|<span data-ttu-id="83325-130">类型</span><span class="sxs-lookup"><span data-stu-id="83325-130">Type</span></span>|<span data-ttu-id="83325-131">说明</span><span class="sxs-lookup"><span data-stu-id="83325-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83325-132">id</span><span class="sxs-lookup"><span data-stu-id="83325-132">id</span></span>|<span data-ttu-id="83325-133">字符串</span><span class="sxs-lookup"><span data-stu-id="83325-133">String</span></span>|<span data-ttu-id="83325-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="83325-134">Key of the entity.</span></span> <span data-ttu-id="83325-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-136">displayName</span><span class="sxs-lookup"><span data-stu-id="83325-136">displayName</span></span>|<span data-ttu-id="83325-137">String</span><span class="sxs-lookup"><span data-stu-id="83325-137">String</span></span>|<span data-ttu-id="83325-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="83325-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="83325-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-140">description</span><span class="sxs-lookup"><span data-stu-id="83325-140">description</span></span>|<span data-ttu-id="83325-141">字符串</span><span class="sxs-lookup"><span data-stu-id="83325-141">String</span></span>|<span data-ttu-id="83325-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="83325-142">The description of the app.</span></span> <span data-ttu-id="83325-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-144">publisher</span><span class="sxs-lookup"><span data-stu-id="83325-144">publisher</span></span>|<span data-ttu-id="83325-145">String</span><span class="sxs-lookup"><span data-stu-id="83325-145">String</span></span>|<span data-ttu-id="83325-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="83325-146">The publisher of the app.</span></span> <span data-ttu-id="83325-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="83325-148">largeIcon</span></span>|[<span data-ttu-id="83325-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="83325-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="83325-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="83325-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="83325-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83325-152">createdDateTime</span></span>|<span data-ttu-id="83325-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83325-153">DateTimeOffset</span></span>|<span data-ttu-id="83325-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="83325-154">The date and time the app was created.</span></span> <span data-ttu-id="83325-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83325-156">lastModifiedDateTime</span></span>|<span data-ttu-id="83325-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83325-157">DateTimeOffset</span></span>|<span data-ttu-id="83325-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="83325-158">The date and time the app was last modified.</span></span> <span data-ttu-id="83325-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="83325-160">isFeatured</span></span>|<span data-ttu-id="83325-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="83325-161">Boolean</span></span>|<span data-ttu-id="83325-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="83325-163">privacyInformationUrl</span></span>|<span data-ttu-id="83325-164">String</span><span class="sxs-lookup"><span data-stu-id="83325-164">String</span></span>|<span data-ttu-id="83325-165">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="83325-165">The privacy statement Url.</span></span> <span data-ttu-id="83325-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="83325-167">informationUrl</span></span>|<span data-ttu-id="83325-168">String</span><span class="sxs-lookup"><span data-stu-id="83325-168">String</span></span>|<span data-ttu-id="83325-169">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="83325-169">The more information Url.</span></span> <span data-ttu-id="83325-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-171">owner</span><span class="sxs-lookup"><span data-stu-id="83325-171">owner</span></span>|<span data-ttu-id="83325-172">String</span><span class="sxs-lookup"><span data-stu-id="83325-172">String</span></span>|<span data-ttu-id="83325-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="83325-173">The owner of the app.</span></span> <span data-ttu-id="83325-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-175">developer</span><span class="sxs-lookup"><span data-stu-id="83325-175">developer</span></span>|<span data-ttu-id="83325-176">String</span><span class="sxs-lookup"><span data-stu-id="83325-176">String</span></span>|<span data-ttu-id="83325-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="83325-177">The developer of the app.</span></span> <span data-ttu-id="83325-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-179">notes</span><span class="sxs-lookup"><span data-stu-id="83325-179">notes</span></span>|<span data-ttu-id="83325-180">String</span><span class="sxs-lookup"><span data-stu-id="83325-180">String</span></span>|<span data-ttu-id="83325-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="83325-181">Notes for the app.</span></span> <span data-ttu-id="83325-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="83325-183">uploadState</span></span>|<span data-ttu-id="83325-184">Int32</span><span class="sxs-lookup"><span data-stu-id="83325-184">Int32</span></span>|<span data-ttu-id="83325-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="83325-185">The upload state.</span></span> <span data-ttu-id="83325-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="83325-187">publishingState</span></span>|[<span data-ttu-id="83325-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="83325-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="83325-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="83325-189">The publishing state for the app.</span></span> <span data-ttu-id="83325-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="83325-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="83325-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="83325-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="83325-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="83325-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="83325-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="83325-193">isAssigned</span></span>|<span data-ttu-id="83325-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="83325-194">Boolean</span></span>|<span data-ttu-id="83325-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="83325-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="83325-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83325-197">roleScopeTagIds</span></span>|<span data-ttu-id="83325-198">String collection</span><span class="sxs-lookup"><span data-stu-id="83325-198">String collection</span></span>|<span data-ttu-id="83325-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="83325-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="83325-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83325-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="83325-201">committedContentVersion</span></span>|<span data-ttu-id="83325-202">String</span><span class="sxs-lookup"><span data-stu-id="83325-202">String</span></span>|<span data-ttu-id="83325-203">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="83325-203">The internal committed content version.</span></span> <span data-ttu-id="83325-204">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="83325-205">fileName</span><span class="sxs-lookup"><span data-stu-id="83325-205">fileName</span></span>|<span data-ttu-id="83325-206">String</span><span class="sxs-lookup"><span data-stu-id="83325-206">String</span></span>|<span data-ttu-id="83325-207">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="83325-207">The name of the main Lob application file.</span></span> <span data-ttu-id="83325-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="83325-209">size</span><span class="sxs-lookup"><span data-stu-id="83325-209">size</span></span>|<span data-ttu-id="83325-210">Int64</span><span class="sxs-lookup"><span data-stu-id="83325-210">Int64</span></span>|<span data-ttu-id="83325-211">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="83325-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="83325-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="83325-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="83325-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="83325-213">applicableArchitectures</span></span>|[<span data-ttu-id="83325-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="83325-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="83325-215">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="83325-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="83325-216">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)。</span><span class="sxs-lookup"><span data-stu-id="83325-216">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="83325-217">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="83325-217">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="83325-218">identityName</span><span class="sxs-lookup"><span data-stu-id="83325-218">identityName</span></span>|<span data-ttu-id="83325-219">String</span><span class="sxs-lookup"><span data-stu-id="83325-219">String</span></span>|<span data-ttu-id="83325-220">标识名称。</span><span class="sxs-lookup"><span data-stu-id="83325-220">The Identity Name.</span></span> <span data-ttu-id="83325-221">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="83325-221">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="83325-222">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="83325-222">identityPublisherHash</span></span>|<span data-ttu-id="83325-223">String</span><span class="sxs-lookup"><span data-stu-id="83325-223">String</span></span>|<span data-ttu-id="83325-224">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="83325-224">The Identity Publisher Hash.</span></span> <span data-ttu-id="83325-225">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="83325-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="83325-226">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="83325-226">identityResourceIdentifier</span></span>|<span data-ttu-id="83325-227">String</span><span class="sxs-lookup"><span data-stu-id="83325-227">String</span></span>|<span data-ttu-id="83325-228">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="83325-228">The Identity Resource Identifier.</span></span> <span data-ttu-id="83325-229">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="83325-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="83325-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="83325-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="83325-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="83325-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="83325-232">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="83325-232">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="83325-233">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="83325-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="83325-234">将 phoneproductidentifier</span><span class="sxs-lookup"><span data-stu-id="83325-234">phoneProductIdentifier</span></span>|<span data-ttu-id="83325-235">String</span><span class="sxs-lookup"><span data-stu-id="83325-235">String</span></span>|<span data-ttu-id="83325-236">电话产品标识符。</span><span class="sxs-lookup"><span data-stu-id="83325-236">The Phone Product Identifier.</span></span> <span data-ttu-id="83325-237">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="83325-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="83325-238">将 phonepublisherid</span><span class="sxs-lookup"><span data-stu-id="83325-238">phonePublisherId</span></span>|<span data-ttu-id="83325-239">String</span><span class="sxs-lookup"><span data-stu-id="83325-239">String</span></span>|<span data-ttu-id="83325-240">电话发布者 Id。继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="83325-240">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="83325-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="83325-241">identityVersion</span></span>|<span data-ttu-id="83325-242">String</span><span class="sxs-lookup"><span data-stu-id="83325-242">String</span></span>|<span data-ttu-id="83325-243">标识版本。</span><span class="sxs-lookup"><span data-stu-id="83325-243">The identity version.</span></span> <span data-ttu-id="83325-244">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="83325-244">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="83325-245">将 appxpackageinformationlist</span><span class="sxs-lookup"><span data-stu-id="83325-245">appXPackageInformationList</span></span>|<span data-ttu-id="83325-246">[了 windowspackageinformation](../resources/intune-apps-windowspackageinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="83325-246">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="83325-247">AppX 包信息的列表。</span><span class="sxs-lookup"><span data-stu-id="83325-247">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="83325-248">响应</span><span class="sxs-lookup"><span data-stu-id="83325-248">Response</span></span>
<span data-ttu-id="83325-249">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[了 windowsphone81appxbundle](../resources/intune-apps-windowsphone81appxbundle.md)对象。</span><span class="sxs-lookup"><span data-stu-id="83325-249">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83325-250">示例</span><span class="sxs-lookup"><span data-stu-id="83325-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="83325-251">请求</span><span class="sxs-lookup"><span data-stu-id="83325-251">Request</span></span>
<span data-ttu-id="83325-252">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="83325-252">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 2184

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
        "v10_1803": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="83325-253">响应</span><span class="sxs-lookup"><span data-stu-id="83325-253">Response</span></span>
<span data-ttu-id="83325-p128">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="83325-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2356

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
        "v10_1803": true
      }
    }
  ]
}
```




