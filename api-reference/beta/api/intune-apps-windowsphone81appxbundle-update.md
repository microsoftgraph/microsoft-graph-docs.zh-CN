---
title: 更新 windowsPhone81AppXBundle
description: 更新 windowsPhone81AppXBundle 对象的属性。
author: tfitzmac
ms.openlocfilehash: 7e377b7ec81d16df768c42555cbdd17b9f2fdd64
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336671"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="dd77f-103">更新 windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="dd77f-103">Update windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="dd77f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dd77f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd77f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dd77f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd77f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dd77f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd77f-107">更新[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dd77f-107">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd77f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dd77f-108">Prerequisites</span></span>
<span data-ttu-id="dd77f-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="dd77f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd77f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd77f-111">Permission type</span></span>|<span data-ttu-id="dd77f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dd77f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd77f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd77f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd77f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd77f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dd77f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd77f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd77f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd77f-116">Not supported.</span></span>|
|<span data-ttu-id="dd77f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd77f-117">Application</span></span>|<span data-ttu-id="dd77f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd77f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd77f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd77f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="dd77f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd77f-120">Request headers</span></span>
|<span data-ttu-id="dd77f-121">标头</span><span class="sxs-lookup"><span data-stu-id="dd77f-121">Header</span></span>|<span data-ttu-id="dd77f-122">值</span><span class="sxs-lookup"><span data-stu-id="dd77f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd77f-123">授权</span><span class="sxs-lookup"><span data-stu-id="dd77f-123">Authorization</span></span>|<span data-ttu-id="dd77f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dd77f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd77f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dd77f-125">Accept</span></span>|<span data-ttu-id="dd77f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd77f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd77f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd77f-127">Request body</span></span>
<span data-ttu-id="dd77f-128">在请求正文中，提供[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd77f-128">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="dd77f-129">下表显示时创建[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dd77f-129">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="dd77f-130">属性</span><span class="sxs-lookup"><span data-stu-id="dd77f-130">Property</span></span>|<span data-ttu-id="dd77f-131">类型</span><span class="sxs-lookup"><span data-stu-id="dd77f-131">Type</span></span>|<span data-ttu-id="dd77f-132">说明</span><span class="sxs-lookup"><span data-stu-id="dd77f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd77f-133">id</span><span class="sxs-lookup"><span data-stu-id="dd77f-133">id</span></span>|<span data-ttu-id="dd77f-134">String</span><span class="sxs-lookup"><span data-stu-id="dd77f-134">String</span></span>|<span data-ttu-id="dd77f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dd77f-135">Key of the entity.</span></span> <span data-ttu-id="dd77f-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd77f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="dd77f-137">displayName</span></span>|<span data-ttu-id="dd77f-138">String</span><span class="sxs-lookup"><span data-stu-id="dd77f-138">String</span></span>|<span data-ttu-id="dd77f-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="dd77f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="dd77f-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd77f-141">description</span><span class="sxs-lookup"><span data-stu-id="dd77f-141">description</span></span>|<span data-ttu-id="dd77f-142">String</span><span class="sxs-lookup"><span data-stu-id="dd77f-142">String</span></span>|<span data-ttu-id="dd77f-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="dd77f-143">The description of the app.</span></span> <span data-ttu-id="dd77f-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd77f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="dd77f-145">publisher</span></span>|<span data-ttu-id="dd77f-146">String</span><span class="sxs-lookup"><span data-stu-id="dd77f-146">String</span></span>|<span data-ttu-id="dd77f-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="dd77f-147">The publisher of the app.</span></span> <span data-ttu-id="dd77f-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd77f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="dd77f-149">largeIcon</span></span>|[<span data-ttu-id="dd77f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="dd77f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="dd77f-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="dd77f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="dd77f-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd77f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd77f-153">createdDateTime</span></span>|<span data-ttu-id="dd77f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd77f-154">DateTimeOffset</span></span>|<span data-ttu-id="dd77f-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="dd77f-155">The date and time the app was created.</span></span> <span data-ttu-id="dd77f-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd77f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd77f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="dd77f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd77f-158">DateTimeOffset</span></span>|<span data-ttu-id="dd77f-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="dd77f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="dd77f-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd77f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="dd77f-161">isFeatured</span></span>|<span data-ttu-id="dd77f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd77f-162">Boolean</span></span>|<span data-ttu-id="dd77f-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd77f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="dd77f-164">privacyInformationUrl</span></span>|<span data-ttu-id="dd77f-165">String</span><span class="sxs-lookup"><span data-stu-id="dd77f-165">String</span></span>|<span data-ttu-id="dd77f-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="dd77f-166">The privacy statement Url.</span></span> <span data-ttu-id="dd77f-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd77f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="dd77f-168">informationUrl</span></span>|<span data-ttu-id="dd77f-169">String</span><span class="sxs-lookup"><span data-stu-id="dd77f-169">String</span></span>|<span data-ttu-id="dd77f-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="dd77f-170">The more information Url.</span></span> <span data-ttu-id="dd77f-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd77f-172">owner</span><span class="sxs-lookup"><span data-stu-id="dd77f-172">owner</span></span>|<span data-ttu-id="dd77f-173">String</span><span class="sxs-lookup"><span data-stu-id="dd77f-173">String</span></span>|<span data-ttu-id="dd77f-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="dd77f-174">The owner of the app.</span></span> <span data-ttu-id="dd77f-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd77f-176">developer</span><span class="sxs-lookup"><span data-stu-id="dd77f-176">developer</span></span>|<span data-ttu-id="dd77f-177">String</span><span class="sxs-lookup"><span data-stu-id="dd77f-177">String</span></span>|<span data-ttu-id="dd77f-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="dd77f-178">The developer of the app.</span></span> <span data-ttu-id="dd77f-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd77f-180">notes</span><span class="sxs-lookup"><span data-stu-id="dd77f-180">notes</span></span>|<span data-ttu-id="dd77f-181">String</span><span class="sxs-lookup"><span data-stu-id="dd77f-181">String</span></span>|<span data-ttu-id="dd77f-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="dd77f-182">Notes for the app.</span></span> <span data-ttu-id="dd77f-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd77f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="dd77f-184">uploadState</span></span>|<span data-ttu-id="dd77f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="dd77f-185">Int32</span></span>|<span data-ttu-id="dd77f-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="dd77f-186">The upload state.</span></span> <span data-ttu-id="dd77f-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="dd77f-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="dd77f-188">publishingState</span></span>|[<span data-ttu-id="dd77f-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="dd77f-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="dd77f-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="dd77f-190">The publishing state for the app.</span></span> <span data-ttu-id="dd77f-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="dd77f-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="dd77f-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="dd77f-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="dd77f-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="dd77f-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="dd77f-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="dd77f-194">committedContentVersion</span></span>|<span data-ttu-id="dd77f-195">String</span><span class="sxs-lookup"><span data-stu-id="dd77f-195">String</span></span>|<span data-ttu-id="dd77f-196">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="dd77f-196">The internal committed content version.</span></span> <span data-ttu-id="dd77f-197">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="dd77f-198">fileName</span><span class="sxs-lookup"><span data-stu-id="dd77f-198">fileName</span></span>|<span data-ttu-id="dd77f-199">String</span><span class="sxs-lookup"><span data-stu-id="dd77f-199">String</span></span>|<span data-ttu-id="dd77f-200">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="dd77f-200">The name of the main Lob application file.</span></span> <span data-ttu-id="dd77f-201">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="dd77f-202">size</span><span class="sxs-lookup"><span data-stu-id="dd77f-202">size</span></span>|<span data-ttu-id="dd77f-203">Int64</span><span class="sxs-lookup"><span data-stu-id="dd77f-203">Int64</span></span>|<span data-ttu-id="dd77f-204">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="dd77f-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="dd77f-205">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="dd77f-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="dd77f-206">applicableArchitectures</span></span>|[<span data-ttu-id="dd77f-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="dd77f-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="dd77f-208">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="dd77f-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="dd77f-209">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)。</span><span class="sxs-lookup"><span data-stu-id="dd77f-209">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="dd77f-210">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。</span><span class="sxs-lookup"><span data-stu-id="dd77f-210">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="dd77f-211">identityName</span><span class="sxs-lookup"><span data-stu-id="dd77f-211">identityName</span></span>|<span data-ttu-id="dd77f-212">String</span><span class="sxs-lookup"><span data-stu-id="dd77f-212">String</span></span>|<span data-ttu-id="dd77f-213">标识名称。</span><span class="sxs-lookup"><span data-stu-id="dd77f-213">The Identity Name.</span></span> <span data-ttu-id="dd77f-214">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-214">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="dd77f-215">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="dd77f-215">identityPublisherHash</span></span>|<span data-ttu-id="dd77f-216">String</span><span class="sxs-lookup"><span data-stu-id="dd77f-216">String</span></span>|<span data-ttu-id="dd77f-217">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="dd77f-217">The Identity Publisher Hash.</span></span> <span data-ttu-id="dd77f-218">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-218">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="dd77f-219">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="dd77f-219">identityResourceIdentifier</span></span>|<span data-ttu-id="dd77f-220">String</span><span class="sxs-lookup"><span data-stu-id="dd77f-220">String</span></span>|<span data-ttu-id="dd77f-221">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="dd77f-221">The Identity Resource Identifier.</span></span> <span data-ttu-id="dd77f-222">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-222">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="dd77f-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dd77f-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="dd77f-224">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="dd77f-224">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="dd77f-225">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="dd77f-225">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="dd77f-226">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-226">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="dd77f-227">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="dd77f-227">phoneProductIdentifier</span></span>|<span data-ttu-id="dd77f-228">字符串</span><span class="sxs-lookup"><span data-stu-id="dd77f-228">String</span></span>|<span data-ttu-id="dd77f-229">电话产品标识符。</span><span class="sxs-lookup"><span data-stu-id="dd77f-229">The Phone Product Identifier.</span></span> <span data-ttu-id="dd77f-230">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="dd77f-231">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="dd77f-231">phonePublisherId</span></span>|<span data-ttu-id="dd77f-232">字符串</span><span class="sxs-lookup"><span data-stu-id="dd77f-232">String</span></span>|<span data-ttu-id="dd77f-233">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)电话 Publisher id。</span><span class="sxs-lookup"><span data-stu-id="dd77f-233">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="dd77f-234">identityVersion</span><span class="sxs-lookup"><span data-stu-id="dd77f-234">identityVersion</span></span>|<span data-ttu-id="dd77f-235">String</span><span class="sxs-lookup"><span data-stu-id="dd77f-235">String</span></span>|<span data-ttu-id="dd77f-236">标识版本。</span><span class="sxs-lookup"><span data-stu-id="dd77f-236">The identity version.</span></span> <span data-ttu-id="dd77f-237">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="dd77f-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="dd77f-238">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="dd77f-238">appXPackageInformationList</span></span>|<span data-ttu-id="dd77f-239">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="dd77f-239">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="dd77f-240">约程序包信息的列表。</span><span class="sxs-lookup"><span data-stu-id="dd77f-240">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="dd77f-241">响应</span><span class="sxs-lookup"><span data-stu-id="dd77f-241">Response</span></span>
<span data-ttu-id="dd77f-242">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dd77f-242">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd77f-243">示例</span><span class="sxs-lookup"><span data-stu-id="dd77f-243">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd77f-244">请求</span><span class="sxs-lookup"><span data-stu-id="dd77f-244">Request</span></span>
<span data-ttu-id="dd77f-245">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dd77f-245">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2100

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
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

### <a name="response"></a><span data-ttu-id="dd77f-246">响应</span><span class="sxs-lookup"><span data-stu-id="dd77f-246">Response</span></span>
<span data-ttu-id="dd77f-p127">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dd77f-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2271

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





