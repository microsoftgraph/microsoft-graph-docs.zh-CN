---
title: 更新 windowsAppX
description: 更新 windowsAppX 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7123364c618dbbdf0eb37dd9e080f54a67b6809b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946166"
---
# <a name="update-windowsappx"></a><span data-ttu-id="f2e64-103">更新 windowsAppX</span><span class="sxs-lookup"><span data-stu-id="f2e64-103">Update windowsAppX</span></span>

> <span data-ttu-id="f2e64-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f2e64-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2e64-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f2e64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2e64-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f2e64-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2e64-107">更新[windowsAppX](../resources/intune-apps-windowsappx.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f2e64-107">Update the properties of a [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2e64-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f2e64-108">Prerequisites</span></span>
<span data-ttu-id="f2e64-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f2e64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2e64-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2e64-111">Permission type</span></span>|<span data-ttu-id="f2e64-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f2e64-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2e64-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2e64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2e64-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2e64-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2e64-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2e64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2e64-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2e64-116">Not supported.</span></span>|
|<span data-ttu-id="f2e64-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2e64-117">Application</span></span>|<span data-ttu-id="f2e64-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2e64-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2e64-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2e64-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f2e64-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2e64-120">Request headers</span></span>
|<span data-ttu-id="f2e64-121">标头</span><span class="sxs-lookup"><span data-stu-id="f2e64-121">Header</span></span>|<span data-ttu-id="f2e64-122">值</span><span class="sxs-lookup"><span data-stu-id="f2e64-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2e64-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2e64-123">Authorization</span></span>|<span data-ttu-id="f2e64-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f2e64-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2e64-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f2e64-125">Accept</span></span>|<span data-ttu-id="f2e64-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2e64-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2e64-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2e64-127">Request body</span></span>
<span data-ttu-id="f2e64-128">在请求正文中，提供[windowsAppX](../resources/intune-apps-windowsappx.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2e64-128">In the request body, supply a JSON representation for the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

<span data-ttu-id="f2e64-129">下表显示时创建[windowsAppX](../resources/intune-apps-windowsappx.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f2e64-129">The following table shows the properties that are required when you create the [windowsAppX](../resources/intune-apps-windowsappx.md).</span></span>

|<span data-ttu-id="f2e64-130">属性</span><span class="sxs-lookup"><span data-stu-id="f2e64-130">Property</span></span>|<span data-ttu-id="f2e64-131">类型</span><span class="sxs-lookup"><span data-stu-id="f2e64-131">Type</span></span>|<span data-ttu-id="f2e64-132">说明</span><span class="sxs-lookup"><span data-stu-id="f2e64-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2e64-133">id</span><span class="sxs-lookup"><span data-stu-id="f2e64-133">id</span></span>|<span data-ttu-id="f2e64-134">String</span><span class="sxs-lookup"><span data-stu-id="f2e64-134">String</span></span>|<span data-ttu-id="f2e64-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f2e64-135">Key of the entity.</span></span> <span data-ttu-id="f2e64-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2e64-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f2e64-137">displayName</span></span>|<span data-ttu-id="f2e64-138">String</span><span class="sxs-lookup"><span data-stu-id="f2e64-138">String</span></span>|<span data-ttu-id="f2e64-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="f2e64-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f2e64-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2e64-141">description</span><span class="sxs-lookup"><span data-stu-id="f2e64-141">description</span></span>|<span data-ttu-id="f2e64-142">String</span><span class="sxs-lookup"><span data-stu-id="f2e64-142">String</span></span>|<span data-ttu-id="f2e64-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="f2e64-143">The description of the app.</span></span> <span data-ttu-id="f2e64-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2e64-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f2e64-145">publisher</span></span>|<span data-ttu-id="f2e64-146">String</span><span class="sxs-lookup"><span data-stu-id="f2e64-146">String</span></span>|<span data-ttu-id="f2e64-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="f2e64-147">The publisher of the app.</span></span> <span data-ttu-id="f2e64-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2e64-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f2e64-149">largeIcon</span></span>|[<span data-ttu-id="f2e64-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f2e64-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f2e64-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="f2e64-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f2e64-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2e64-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2e64-153">createdDateTime</span></span>|<span data-ttu-id="f2e64-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2e64-154">DateTimeOffset</span></span>|<span data-ttu-id="f2e64-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f2e64-155">The date and time the app was created.</span></span> <span data-ttu-id="f2e64-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2e64-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2e64-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f2e64-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2e64-158">DateTimeOffset</span></span>|<span data-ttu-id="f2e64-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f2e64-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f2e64-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2e64-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f2e64-161">isFeatured</span></span>|<span data-ttu-id="f2e64-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2e64-162">Boolean</span></span>|<span data-ttu-id="f2e64-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2e64-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f2e64-164">privacyInformationUrl</span></span>|<span data-ttu-id="f2e64-165">String</span><span class="sxs-lookup"><span data-stu-id="f2e64-165">String</span></span>|<span data-ttu-id="f2e64-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="f2e64-166">The privacy statement Url.</span></span> <span data-ttu-id="f2e64-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2e64-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f2e64-168">informationUrl</span></span>|<span data-ttu-id="f2e64-169">String</span><span class="sxs-lookup"><span data-stu-id="f2e64-169">String</span></span>|<span data-ttu-id="f2e64-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="f2e64-170">The more information Url.</span></span> <span data-ttu-id="f2e64-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2e64-172">owner</span><span class="sxs-lookup"><span data-stu-id="f2e64-172">owner</span></span>|<span data-ttu-id="f2e64-173">String</span><span class="sxs-lookup"><span data-stu-id="f2e64-173">String</span></span>|<span data-ttu-id="f2e64-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="f2e64-174">The owner of the app.</span></span> <span data-ttu-id="f2e64-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2e64-176">developer</span><span class="sxs-lookup"><span data-stu-id="f2e64-176">developer</span></span>|<span data-ttu-id="f2e64-177">String</span><span class="sxs-lookup"><span data-stu-id="f2e64-177">String</span></span>|<span data-ttu-id="f2e64-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="f2e64-178">The developer of the app.</span></span> <span data-ttu-id="f2e64-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2e64-180">notes</span><span class="sxs-lookup"><span data-stu-id="f2e64-180">notes</span></span>|<span data-ttu-id="f2e64-181">String</span><span class="sxs-lookup"><span data-stu-id="f2e64-181">String</span></span>|<span data-ttu-id="f2e64-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="f2e64-182">Notes for the app.</span></span> <span data-ttu-id="f2e64-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2e64-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f2e64-184">uploadState</span></span>|<span data-ttu-id="f2e64-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f2e64-185">Int32</span></span>|<span data-ttu-id="f2e64-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="f2e64-186">The upload state.</span></span> <span data-ttu-id="f2e64-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2e64-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="f2e64-188">publishingState</span></span>|[<span data-ttu-id="f2e64-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f2e64-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f2e64-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="f2e64-190">The publishing state for the app.</span></span> <span data-ttu-id="f2e64-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="f2e64-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f2e64-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="f2e64-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f2e64-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="f2e64-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f2e64-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f2e64-194">committedContentVersion</span></span>|<span data-ttu-id="f2e64-195">String</span><span class="sxs-lookup"><span data-stu-id="f2e64-195">String</span></span>|<span data-ttu-id="f2e64-196">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="f2e64-196">The internal committed content version.</span></span> <span data-ttu-id="f2e64-197">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f2e64-198">fileName</span><span class="sxs-lookup"><span data-stu-id="f2e64-198">fileName</span></span>|<span data-ttu-id="f2e64-199">String</span><span class="sxs-lookup"><span data-stu-id="f2e64-199">String</span></span>|<span data-ttu-id="f2e64-200">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="f2e64-200">The name of the main Lob application file.</span></span> <span data-ttu-id="f2e64-201">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f2e64-202">size</span><span class="sxs-lookup"><span data-stu-id="f2e64-202">size</span></span>|<span data-ttu-id="f2e64-203">Int64</span><span class="sxs-lookup"><span data-stu-id="f2e64-203">Int64</span></span>|<span data-ttu-id="f2e64-204">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="f2e64-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="f2e64-205">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f2e64-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f2e64-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="f2e64-206">applicableArchitectures</span></span>|[<span data-ttu-id="f2e64-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="f2e64-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="f2e64-208">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="f2e64-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="f2e64-209">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。</span><span class="sxs-lookup"><span data-stu-id="f2e64-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="f2e64-210">identityName</span><span class="sxs-lookup"><span data-stu-id="f2e64-210">identityName</span></span>|<span data-ttu-id="f2e64-211">String</span><span class="sxs-lookup"><span data-stu-id="f2e64-211">String</span></span>|<span data-ttu-id="f2e64-212">标识名称。</span><span class="sxs-lookup"><span data-stu-id="f2e64-212">The Identity Name.</span></span>|
|<span data-ttu-id="f2e64-213">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="f2e64-213">identityPublisherHash</span></span>|<span data-ttu-id="f2e64-214">String</span><span class="sxs-lookup"><span data-stu-id="f2e64-214">String</span></span>|<span data-ttu-id="f2e64-215">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="f2e64-215">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="f2e64-216">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f2e64-216">identityResourceIdentifier</span></span>|<span data-ttu-id="f2e64-217">String</span><span class="sxs-lookup"><span data-stu-id="f2e64-217">String</span></span>|<span data-ttu-id="f2e64-218">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="f2e64-218">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="f2e64-219">isBundle</span><span class="sxs-lookup"><span data-stu-id="f2e64-219">isBundle</span></span>|<span data-ttu-id="f2e64-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2e64-220">Boolean</span></span>|<span data-ttu-id="f2e64-221">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="f2e64-221">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="f2e64-222">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2e64-222">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f2e64-223">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f2e64-223">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="f2e64-224">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="f2e64-224">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f2e64-225">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f2e64-225">identityVersion</span></span>|<span data-ttu-id="f2e64-226">String</span><span class="sxs-lookup"><span data-stu-id="f2e64-226">String</span></span>|<span data-ttu-id="f2e64-227">标识版本。</span><span class="sxs-lookup"><span data-stu-id="f2e64-227">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="f2e64-228">响应</span><span class="sxs-lookup"><span data-stu-id="f2e64-228">Response</span></span>
<span data-ttu-id="f2e64-229">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsAppX](../resources/intune-apps-windowsappx.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f2e64-229">If successful, this method returns a `200 OK` response code and an updated [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2e64-230">示例</span><span class="sxs-lookup"><span data-stu-id="f2e64-230">Example</span></span>
### <a name="request"></a><span data-ttu-id="f2e64-231">请求</span><span class="sxs-lookup"><span data-stu-id="f2e64-231">Request</span></span>
<span data-ttu-id="f2e64-232">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2e64-232">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1269

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
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="f2e64-233">响应</span><span class="sxs-lookup"><span data-stu-id="f2e64-233">Response</span></span>
<span data-ttu-id="f2e64-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2e64-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1427

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```





