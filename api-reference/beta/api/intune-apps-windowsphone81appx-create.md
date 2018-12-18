---
title: 创建 windowsPhone81AppX
description: 创建新的 windowsPhone81AppX 对象。
author: tfitzmac
ms.openlocfilehash: ac8501c6c68f1efe2fb99a39c659868944254048
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325709"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="98623-103">创建 windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="98623-103">Create windowsPhone81AppX</span></span>

> <span data-ttu-id="98623-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="98623-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98623-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="98623-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98623-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="98623-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98623-107">创建新的[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)对象。</span><span class="sxs-lookup"><span data-stu-id="98623-107">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="98623-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="98623-108">Prerequisites</span></span>
<span data-ttu-id="98623-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="98623-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98623-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="98623-111">Permission type</span></span>|<span data-ttu-id="98623-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="98623-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98623-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98623-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98623-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98623-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="98623-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98623-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98623-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="98623-116">Not supported.</span></span>|
|<span data-ttu-id="98623-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="98623-117">Application</span></span>|<span data-ttu-id="98623-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="98623-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98623-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98623-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="98623-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="98623-120">Request headers</span></span>
|<span data-ttu-id="98623-121">标头</span><span class="sxs-lookup"><span data-stu-id="98623-121">Header</span></span>|<span data-ttu-id="98623-122">值</span><span class="sxs-lookup"><span data-stu-id="98623-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98623-123">授权</span><span class="sxs-lookup"><span data-stu-id="98623-123">Authorization</span></span>|<span data-ttu-id="98623-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="98623-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98623-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98623-125">Accept</span></span>|<span data-ttu-id="98623-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98623-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98623-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="98623-127">Request body</span></span>
<span data-ttu-id="98623-128">在请求正文中，提供 windowsPhone81AppX 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98623-128">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="98623-129">下表显示时创建 windowsPhone81AppX 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="98623-129">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="98623-130">属性</span><span class="sxs-lookup"><span data-stu-id="98623-130">Property</span></span>|<span data-ttu-id="98623-131">类型</span><span class="sxs-lookup"><span data-stu-id="98623-131">Type</span></span>|<span data-ttu-id="98623-132">说明</span><span class="sxs-lookup"><span data-stu-id="98623-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98623-133">id</span><span class="sxs-lookup"><span data-stu-id="98623-133">id</span></span>|<span data-ttu-id="98623-134">String</span><span class="sxs-lookup"><span data-stu-id="98623-134">String</span></span>|<span data-ttu-id="98623-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="98623-135">Key of the entity.</span></span> <span data-ttu-id="98623-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98623-137">displayName</span><span class="sxs-lookup"><span data-stu-id="98623-137">displayName</span></span>|<span data-ttu-id="98623-138">String</span><span class="sxs-lookup"><span data-stu-id="98623-138">String</span></span>|<span data-ttu-id="98623-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="98623-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="98623-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98623-141">description</span><span class="sxs-lookup"><span data-stu-id="98623-141">description</span></span>|<span data-ttu-id="98623-142">String</span><span class="sxs-lookup"><span data-stu-id="98623-142">String</span></span>|<span data-ttu-id="98623-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="98623-143">The description of the app.</span></span> <span data-ttu-id="98623-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98623-145">publisher</span><span class="sxs-lookup"><span data-stu-id="98623-145">publisher</span></span>|<span data-ttu-id="98623-146">String</span><span class="sxs-lookup"><span data-stu-id="98623-146">String</span></span>|<span data-ttu-id="98623-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="98623-147">The publisher of the app.</span></span> <span data-ttu-id="98623-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98623-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="98623-149">largeIcon</span></span>|[<span data-ttu-id="98623-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="98623-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="98623-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="98623-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="98623-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98623-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="98623-153">createdDateTime</span></span>|<span data-ttu-id="98623-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98623-154">DateTimeOffset</span></span>|<span data-ttu-id="98623-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="98623-155">The date and time the app was created.</span></span> <span data-ttu-id="98623-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98623-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="98623-157">lastModifiedDateTime</span></span>|<span data-ttu-id="98623-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98623-158">DateTimeOffset</span></span>|<span data-ttu-id="98623-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="98623-159">The date and time the app was last modified.</span></span> <span data-ttu-id="98623-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98623-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="98623-161">isFeatured</span></span>|<span data-ttu-id="98623-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="98623-162">Boolean</span></span>|<span data-ttu-id="98623-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98623-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="98623-164">privacyInformationUrl</span></span>|<span data-ttu-id="98623-165">String</span><span class="sxs-lookup"><span data-stu-id="98623-165">String</span></span>|<span data-ttu-id="98623-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="98623-166">The privacy statement Url.</span></span> <span data-ttu-id="98623-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98623-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="98623-168">informationUrl</span></span>|<span data-ttu-id="98623-169">String</span><span class="sxs-lookup"><span data-stu-id="98623-169">String</span></span>|<span data-ttu-id="98623-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="98623-170">The more information Url.</span></span> <span data-ttu-id="98623-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98623-172">owner</span><span class="sxs-lookup"><span data-stu-id="98623-172">owner</span></span>|<span data-ttu-id="98623-173">String</span><span class="sxs-lookup"><span data-stu-id="98623-173">String</span></span>|<span data-ttu-id="98623-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="98623-174">The owner of the app.</span></span> <span data-ttu-id="98623-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98623-176">developer</span><span class="sxs-lookup"><span data-stu-id="98623-176">developer</span></span>|<span data-ttu-id="98623-177">String</span><span class="sxs-lookup"><span data-stu-id="98623-177">String</span></span>|<span data-ttu-id="98623-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="98623-178">The developer of the app.</span></span> <span data-ttu-id="98623-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98623-180">notes</span><span class="sxs-lookup"><span data-stu-id="98623-180">notes</span></span>|<span data-ttu-id="98623-181">String</span><span class="sxs-lookup"><span data-stu-id="98623-181">String</span></span>|<span data-ttu-id="98623-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="98623-182">Notes for the app.</span></span> <span data-ttu-id="98623-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98623-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="98623-184">uploadState</span></span>|<span data-ttu-id="98623-185">Int32</span><span class="sxs-lookup"><span data-stu-id="98623-185">Int32</span></span>|<span data-ttu-id="98623-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="98623-186">The upload state.</span></span> <span data-ttu-id="98623-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="98623-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="98623-188">publishingState</span></span>|[<span data-ttu-id="98623-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="98623-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="98623-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="98623-190">The publishing state for the app.</span></span> <span data-ttu-id="98623-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="98623-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="98623-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="98623-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="98623-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="98623-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="98623-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="98623-194">committedContentVersion</span></span>|<span data-ttu-id="98623-195">String</span><span class="sxs-lookup"><span data-stu-id="98623-195">String</span></span>|<span data-ttu-id="98623-196">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="98623-196">The internal committed content version.</span></span> <span data-ttu-id="98623-197">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="98623-198">fileName</span><span class="sxs-lookup"><span data-stu-id="98623-198">fileName</span></span>|<span data-ttu-id="98623-199">String</span><span class="sxs-lookup"><span data-stu-id="98623-199">String</span></span>|<span data-ttu-id="98623-200">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="98623-200">The name of the main Lob application file.</span></span> <span data-ttu-id="98623-201">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="98623-202">size</span><span class="sxs-lookup"><span data-stu-id="98623-202">size</span></span>|<span data-ttu-id="98623-203">Int64</span><span class="sxs-lookup"><span data-stu-id="98623-203">Int64</span></span>|<span data-ttu-id="98623-204">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="98623-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="98623-205">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="98623-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="98623-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="98623-206">applicableArchitectures</span></span>|[<span data-ttu-id="98623-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="98623-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="98623-208">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="98623-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="98623-209">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。</span><span class="sxs-lookup"><span data-stu-id="98623-209">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="98623-210">identityName</span><span class="sxs-lookup"><span data-stu-id="98623-210">identityName</span></span>|<span data-ttu-id="98623-211">String</span><span class="sxs-lookup"><span data-stu-id="98623-211">String</span></span>|<span data-ttu-id="98623-212">标识名称。</span><span class="sxs-lookup"><span data-stu-id="98623-212">The Identity Name.</span></span>|
|<span data-ttu-id="98623-213">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="98623-213">identityPublisherHash</span></span>|<span data-ttu-id="98623-214">String</span><span class="sxs-lookup"><span data-stu-id="98623-214">String</span></span>|<span data-ttu-id="98623-215">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="98623-215">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="98623-216">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="98623-216">identityResourceIdentifier</span></span>|<span data-ttu-id="98623-217">String</span><span class="sxs-lookup"><span data-stu-id="98623-217">String</span></span>|<span data-ttu-id="98623-218">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="98623-218">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="98623-219">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="98623-219">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="98623-220">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="98623-220">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="98623-221">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="98623-221">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="98623-222">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="98623-222">phoneProductIdentifier</span></span>|<span data-ttu-id="98623-223">字符串</span><span class="sxs-lookup"><span data-stu-id="98623-223">String</span></span>|<span data-ttu-id="98623-224">电话产品标识符。</span><span class="sxs-lookup"><span data-stu-id="98623-224">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="98623-225">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="98623-225">phonePublisherId</span></span>|<span data-ttu-id="98623-226">字符串</span><span class="sxs-lookup"><span data-stu-id="98623-226">String</span></span>|<span data-ttu-id="98623-227">电话 Publisher id。</span><span class="sxs-lookup"><span data-stu-id="98623-227">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="98623-228">identityVersion</span><span class="sxs-lookup"><span data-stu-id="98623-228">identityVersion</span></span>|<span data-ttu-id="98623-229">String</span><span class="sxs-lookup"><span data-stu-id="98623-229">String</span></span>|<span data-ttu-id="98623-230">标识版本。</span><span class="sxs-lookup"><span data-stu-id="98623-230">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="98623-231">响应</span><span class="sxs-lookup"><span data-stu-id="98623-231">Response</span></span>
<span data-ttu-id="98623-232">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)对象。</span><span class="sxs-lookup"><span data-stu-id="98623-232">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98623-233">示例</span><span class="sxs-lookup"><span data-stu-id="98623-233">Example</span></span>
### <a name="request"></a><span data-ttu-id="98623-234">请求</span><span class="sxs-lookup"><span data-stu-id="98623-234">Request</span></span>
<span data-ttu-id="98623-235">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="98623-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1419

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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="98623-236">响应</span><span class="sxs-lookup"><span data-stu-id="98623-236">Response</span></span>
<span data-ttu-id="98623-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="98623-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1527

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





