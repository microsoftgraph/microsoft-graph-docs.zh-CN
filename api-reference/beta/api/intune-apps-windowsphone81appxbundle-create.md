---
title: 创建了 windowsphone81appxbundle
description: 创建新的了 windowsphone81appxbundle 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b37d04f4c08d562529943ada7a64937c25ede324
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969902"
---
# <a name="create-windowsphone81appxbundle"></a><span data-ttu-id="6b08f-103">创建了 windowsphone81appxbundle</span><span class="sxs-lookup"><span data-stu-id="6b08f-103">Create windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="6b08f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6b08f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b08f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b08f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b08f-106">创建新的[了 windowsphone81appxbundle](../resources/intune-apps-windowsphone81appxbundle.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6b08f-106">Create a new [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b08f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6b08f-107">Prerequisites</span></span>
<span data-ttu-id="6b08f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b08f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b08f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b08f-110">Permission type</span></span>|<span data-ttu-id="6b08f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6b08f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b08f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b08f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b08f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b08f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6b08f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b08f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b08f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b08f-115">Not supported.</span></span>|
|<span data-ttu-id="6b08f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b08f-116">Application</span></span>|<span data-ttu-id="6b08f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b08f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b08f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b08f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="6b08f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b08f-119">Request headers</span></span>
|<span data-ttu-id="6b08f-120">标头</span><span class="sxs-lookup"><span data-stu-id="6b08f-120">Header</span></span>|<span data-ttu-id="6b08f-121">值</span><span class="sxs-lookup"><span data-stu-id="6b08f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b08f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b08f-122">Authorization</span></span>|<span data-ttu-id="6b08f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6b08f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b08f-124">接受</span><span class="sxs-lookup"><span data-stu-id="6b08f-124">Accept</span></span>|<span data-ttu-id="6b08f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b08f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b08f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b08f-126">Request body</span></span>
<span data-ttu-id="6b08f-127">在请求正文中, 提供了 windowsphone81appxbundle 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b08f-127">In the request body, supply a JSON representation for the windowsPhone81AppXBundle object.</span></span>

<span data-ttu-id="6b08f-128">下表显示创建了 windowsphone81appxbundle 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6b08f-128">The following table shows the properties that are required when you create the windowsPhone81AppXBundle.</span></span>

|<span data-ttu-id="6b08f-129">属性</span><span class="sxs-lookup"><span data-stu-id="6b08f-129">Property</span></span>|<span data-ttu-id="6b08f-130">类型</span><span class="sxs-lookup"><span data-stu-id="6b08f-130">Type</span></span>|<span data-ttu-id="6b08f-131">说明</span><span class="sxs-lookup"><span data-stu-id="6b08f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b08f-132">id</span><span class="sxs-lookup"><span data-stu-id="6b08f-132">id</span></span>|<span data-ttu-id="6b08f-133">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-133">String</span></span>|<span data-ttu-id="6b08f-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6b08f-134">Key of the entity.</span></span> <span data-ttu-id="6b08f-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6b08f-136">displayName</span></span>|<span data-ttu-id="6b08f-137">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-137">String</span></span>|<span data-ttu-id="6b08f-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="6b08f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6b08f-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-140">description</span><span class="sxs-lookup"><span data-stu-id="6b08f-140">description</span></span>|<span data-ttu-id="6b08f-141">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-141">String</span></span>|<span data-ttu-id="6b08f-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="6b08f-142">The description of the app.</span></span> <span data-ttu-id="6b08f-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-144">publisher</span><span class="sxs-lookup"><span data-stu-id="6b08f-144">publisher</span></span>|<span data-ttu-id="6b08f-145">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-145">String</span></span>|<span data-ttu-id="6b08f-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="6b08f-146">The publisher of the app.</span></span> <span data-ttu-id="6b08f-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6b08f-148">largeIcon</span></span>|[<span data-ttu-id="6b08f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6b08f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6b08f-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="6b08f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6b08f-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b08f-152">createdDateTime</span></span>|<span data-ttu-id="6b08f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b08f-153">DateTimeOffset</span></span>|<span data-ttu-id="6b08f-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6b08f-154">The date and time the app was created.</span></span> <span data-ttu-id="6b08f-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b08f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="6b08f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b08f-157">DateTimeOffset</span></span>|<span data-ttu-id="6b08f-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6b08f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="6b08f-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6b08f-160">isFeatured</span></span>|<span data-ttu-id="6b08f-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b08f-161">Boolean</span></span>|<span data-ttu-id="6b08f-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6b08f-163">privacyInformationUrl</span></span>|<span data-ttu-id="6b08f-164">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-164">String</span></span>|<span data-ttu-id="6b08f-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="6b08f-165">The privacy statement Url.</span></span> <span data-ttu-id="6b08f-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6b08f-167">informationUrl</span></span>|<span data-ttu-id="6b08f-168">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-168">String</span></span>|<span data-ttu-id="6b08f-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="6b08f-169">The more information Url.</span></span> <span data-ttu-id="6b08f-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-171">owner</span><span class="sxs-lookup"><span data-stu-id="6b08f-171">owner</span></span>|<span data-ttu-id="6b08f-172">字符串</span><span class="sxs-lookup"><span data-stu-id="6b08f-172">String</span></span>|<span data-ttu-id="6b08f-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="6b08f-173">The owner of the app.</span></span> <span data-ttu-id="6b08f-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-175">developer</span><span class="sxs-lookup"><span data-stu-id="6b08f-175">developer</span></span>|<span data-ttu-id="6b08f-176">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-176">String</span></span>|<span data-ttu-id="6b08f-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="6b08f-177">The developer of the app.</span></span> <span data-ttu-id="6b08f-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-179">notes</span><span class="sxs-lookup"><span data-stu-id="6b08f-179">notes</span></span>|<span data-ttu-id="6b08f-180">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-180">String</span></span>|<span data-ttu-id="6b08f-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="6b08f-181">Notes for the app.</span></span> <span data-ttu-id="6b08f-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="6b08f-183">uploadState</span></span>|<span data-ttu-id="6b08f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="6b08f-184">Int32</span></span>|<span data-ttu-id="6b08f-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="6b08f-185">The upload state.</span></span> <span data-ttu-id="6b08f-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="6b08f-187">publishingState</span></span>|[<span data-ttu-id="6b08f-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6b08f-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6b08f-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="6b08f-189">The publishing state for the app.</span></span> <span data-ttu-id="6b08f-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="6b08f-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6b08f-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="6b08f-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="6b08f-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="6b08f-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6b08f-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6b08f-193">isAssigned</span></span>|<span data-ttu-id="6b08f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b08f-194">Boolean</span></span>|<span data-ttu-id="6b08f-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="6b08f-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6b08f-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6b08f-197">roleScopeTagIds</span></span>|<span data-ttu-id="6b08f-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="6b08f-198">String collection</span></span>|<span data-ttu-id="6b08f-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="6b08f-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6b08f-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6b08f-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="6b08f-201">committedContentVersion</span></span>|<span data-ttu-id="6b08f-202">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-202">String</span></span>|<span data-ttu-id="6b08f-203">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="6b08f-203">The internal committed content version.</span></span> <span data-ttu-id="6b08f-204">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6b08f-205">fileName</span><span class="sxs-lookup"><span data-stu-id="6b08f-205">fileName</span></span>|<span data-ttu-id="6b08f-206">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-206">String</span></span>|<span data-ttu-id="6b08f-207">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="6b08f-207">The name of the main Lob application file.</span></span> <span data-ttu-id="6b08f-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6b08f-209">size</span><span class="sxs-lookup"><span data-stu-id="6b08f-209">size</span></span>|<span data-ttu-id="6b08f-210">Int64</span><span class="sxs-lookup"><span data-stu-id="6b08f-210">Int64</span></span>|<span data-ttu-id="6b08f-211">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="6b08f-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="6b08f-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="6b08f-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="6b08f-213">applicableArchitectures</span></span>|[<span data-ttu-id="6b08f-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="6b08f-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="6b08f-215">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="6b08f-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="6b08f-216">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)。</span><span class="sxs-lookup"><span data-stu-id="6b08f-216">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="6b08f-217">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="6b08f-217">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="6b08f-218">identityName</span><span class="sxs-lookup"><span data-stu-id="6b08f-218">identityName</span></span>|<span data-ttu-id="6b08f-219">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-219">String</span></span>|<span data-ttu-id="6b08f-220">标识名称。</span><span class="sxs-lookup"><span data-stu-id="6b08f-220">The Identity Name.</span></span> <span data-ttu-id="6b08f-221">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-221">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="6b08f-222">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="6b08f-222">identityPublisherHash</span></span>|<span data-ttu-id="6b08f-223">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-223">String</span></span>|<span data-ttu-id="6b08f-224">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="6b08f-224">The Identity Publisher Hash.</span></span> <span data-ttu-id="6b08f-225">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-225">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="6b08f-226">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="6b08f-226">identityResourceIdentifier</span></span>|<span data-ttu-id="6b08f-227">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-227">String</span></span>|<span data-ttu-id="6b08f-228">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="6b08f-228">The Identity Resource Identifier.</span></span> <span data-ttu-id="6b08f-229">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-229">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="6b08f-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6b08f-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="6b08f-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="6b08f-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="6b08f-232">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="6b08f-232">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="6b08f-233">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-233">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="6b08f-234">将 phoneproductidentifier</span><span class="sxs-lookup"><span data-stu-id="6b08f-234">phoneProductIdentifier</span></span>|<span data-ttu-id="6b08f-235">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-235">String</span></span>|<span data-ttu-id="6b08f-236">电话产品标识符。</span><span class="sxs-lookup"><span data-stu-id="6b08f-236">The Phone Product Identifier.</span></span> <span data-ttu-id="6b08f-237">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="6b08f-238">将 phonepublisherid</span><span class="sxs-lookup"><span data-stu-id="6b08f-238">phonePublisherId</span></span>|<span data-ttu-id="6b08f-239">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-239">String</span></span>|<span data-ttu-id="6b08f-240">电话发布者 Id。继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-240">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="6b08f-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="6b08f-241">identityVersion</span></span>|<span data-ttu-id="6b08f-242">String</span><span class="sxs-lookup"><span data-stu-id="6b08f-242">String</span></span>|<span data-ttu-id="6b08f-243">标识版本。</span><span class="sxs-lookup"><span data-stu-id="6b08f-243">The identity version.</span></span> <span data-ttu-id="6b08f-244">继承自[了 windowsphone81appx](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="6b08f-244">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="6b08f-245">将 appxpackageinformationlist</span><span class="sxs-lookup"><span data-stu-id="6b08f-245">appXPackageInformationList</span></span>|<span data-ttu-id="6b08f-246">[了 windowspackageinformation](../resources/intune-apps-windowspackageinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="6b08f-246">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="6b08f-247">AppX 包信息的列表。</span><span class="sxs-lookup"><span data-stu-id="6b08f-247">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="6b08f-248">响应</span><span class="sxs-lookup"><span data-stu-id="6b08f-248">Response</span></span>
<span data-ttu-id="6b08f-249">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[了 windowsphone81appxbundle](../resources/intune-apps-windowsphone81appxbundle.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6b08f-249">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b08f-250">示例</span><span class="sxs-lookup"><span data-stu-id="6b08f-250">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b08f-251">请求</span><span class="sxs-lookup"><span data-stu-id="6b08f-251">Request</span></span>
<span data-ttu-id="6b08f-252">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b08f-252">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6b08f-253">响应</span><span class="sxs-lookup"><span data-stu-id="6b08f-253">Response</span></span>
<span data-ttu-id="6b08f-p128">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b08f-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




