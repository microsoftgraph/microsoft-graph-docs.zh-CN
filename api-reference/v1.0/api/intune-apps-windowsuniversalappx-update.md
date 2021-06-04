---
title: 更新 windowsUniversalAppX
description: 更新 windowsUniversalAppX 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 095e06dc55f8528bb677051a0831ef91b82a4336
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754019"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="06810-103">更新 windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="06810-103">Update windowsUniversalAppX</span></span>

<span data-ttu-id="06810-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06810-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06810-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06810-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06810-106">更新 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="06810-106">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06810-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="06810-107">Prerequisites</span></span>
<span data-ttu-id="06810-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06810-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06810-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="06810-110">Permission type</span></span>|<span data-ttu-id="06810-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06810-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06810-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06810-112">Delegated (work or school account)</span></span>|<span data-ttu-id="06810-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06810-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="06810-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06810-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06810-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="06810-115">Not supported.</span></span>|
|<span data-ttu-id="06810-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="06810-116">Application</span></span>|<span data-ttu-id="06810-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06810-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="06810-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06810-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="06810-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="06810-119">Request headers</span></span>
|<span data-ttu-id="06810-120">标头</span><span class="sxs-lookup"><span data-stu-id="06810-120">Header</span></span>|<span data-ttu-id="06810-121">值</span><span class="sxs-lookup"><span data-stu-id="06810-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06810-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="06810-122">Authorization</span></span>|<span data-ttu-id="06810-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="06810-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06810-124">接受</span><span class="sxs-lookup"><span data-stu-id="06810-124">Accept</span></span>|<span data-ttu-id="06810-125">application/json</span><span class="sxs-lookup"><span data-stu-id="06810-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06810-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="06810-126">Request body</span></span>
<span data-ttu-id="06810-127">在请求正文中，提供 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06810-127">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="06810-128">下表显示创建 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="06810-128">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="06810-129">属性</span><span class="sxs-lookup"><span data-stu-id="06810-129">Property</span></span>|<span data-ttu-id="06810-130">类型</span><span class="sxs-lookup"><span data-stu-id="06810-130">Type</span></span>|<span data-ttu-id="06810-131">说明</span><span class="sxs-lookup"><span data-stu-id="06810-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06810-132">id</span><span class="sxs-lookup"><span data-stu-id="06810-132">id</span></span>|<span data-ttu-id="06810-133">String</span><span class="sxs-lookup"><span data-stu-id="06810-133">String</span></span>|<span data-ttu-id="06810-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="06810-134">Key of the entity.</span></span> <span data-ttu-id="06810-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06810-136">displayName</span><span class="sxs-lookup"><span data-stu-id="06810-136">displayName</span></span>|<span data-ttu-id="06810-137">String</span><span class="sxs-lookup"><span data-stu-id="06810-137">String</span></span>|<span data-ttu-id="06810-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="06810-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="06810-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06810-140">说明</span><span class="sxs-lookup"><span data-stu-id="06810-140">description</span></span>|<span data-ttu-id="06810-141">String</span><span class="sxs-lookup"><span data-stu-id="06810-141">String</span></span>|<span data-ttu-id="06810-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="06810-142">The description of the app.</span></span> <span data-ttu-id="06810-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06810-144">publisher</span><span class="sxs-lookup"><span data-stu-id="06810-144">publisher</span></span>|<span data-ttu-id="06810-145">String</span><span class="sxs-lookup"><span data-stu-id="06810-145">String</span></span>|<span data-ttu-id="06810-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="06810-146">The publisher of the app.</span></span> <span data-ttu-id="06810-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06810-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="06810-148">largeIcon</span></span>|[<span data-ttu-id="06810-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="06810-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="06810-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="06810-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="06810-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06810-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06810-152">createdDateTime</span></span>|<span data-ttu-id="06810-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06810-153">DateTimeOffset</span></span>|<span data-ttu-id="06810-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="06810-154">The date and time the app was created.</span></span> <span data-ttu-id="06810-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06810-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06810-156">lastModifiedDateTime</span></span>|<span data-ttu-id="06810-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06810-157">DateTimeOffset</span></span>|<span data-ttu-id="06810-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="06810-158">The date and time the app was last modified.</span></span> <span data-ttu-id="06810-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06810-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="06810-160">isFeatured</span></span>|<span data-ttu-id="06810-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="06810-161">Boolean</span></span>|<span data-ttu-id="06810-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06810-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="06810-163">privacyInformationUrl</span></span>|<span data-ttu-id="06810-164">String</span><span class="sxs-lookup"><span data-stu-id="06810-164">String</span></span>|<span data-ttu-id="06810-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="06810-165">The privacy statement Url.</span></span> <span data-ttu-id="06810-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06810-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="06810-167">informationUrl</span></span>|<span data-ttu-id="06810-168">String</span><span class="sxs-lookup"><span data-stu-id="06810-168">String</span></span>|<span data-ttu-id="06810-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="06810-169">The more information Url.</span></span> <span data-ttu-id="06810-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06810-171">所有者</span><span class="sxs-lookup"><span data-stu-id="06810-171">owner</span></span>|<span data-ttu-id="06810-172">String</span><span class="sxs-lookup"><span data-stu-id="06810-172">String</span></span>|<span data-ttu-id="06810-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="06810-173">The owner of the app.</span></span> <span data-ttu-id="06810-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06810-175">developer</span><span class="sxs-lookup"><span data-stu-id="06810-175">developer</span></span>|<span data-ttu-id="06810-176">String</span><span class="sxs-lookup"><span data-stu-id="06810-176">String</span></span>|<span data-ttu-id="06810-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="06810-177">The developer of the app.</span></span> <span data-ttu-id="06810-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06810-179">notes</span><span class="sxs-lookup"><span data-stu-id="06810-179">notes</span></span>|<span data-ttu-id="06810-180">String</span><span class="sxs-lookup"><span data-stu-id="06810-180">String</span></span>|<span data-ttu-id="06810-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="06810-181">Notes for the app.</span></span> <span data-ttu-id="06810-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="06810-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="06810-183">publishingState</span></span>|[<span data-ttu-id="06810-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="06810-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="06810-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="06810-185">The publishing state for the app.</span></span> <span data-ttu-id="06810-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="06810-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="06810-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="06810-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="06810-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="06810-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="06810-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="06810-189">committedContentVersion</span></span>|<span data-ttu-id="06810-190">String</span><span class="sxs-lookup"><span data-stu-id="06810-190">String</span></span>|<span data-ttu-id="06810-191">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="06810-191">The internal committed content version.</span></span> <span data-ttu-id="06810-192">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="06810-193">fileName</span><span class="sxs-lookup"><span data-stu-id="06810-193">fileName</span></span>|<span data-ttu-id="06810-194">String</span><span class="sxs-lookup"><span data-stu-id="06810-194">String</span></span>|<span data-ttu-id="06810-195">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="06810-195">The name of the main Lob application file.</span></span> <span data-ttu-id="06810-196">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="06810-197">size</span><span class="sxs-lookup"><span data-stu-id="06810-197">size</span></span>|<span data-ttu-id="06810-198">Int64</span><span class="sxs-lookup"><span data-stu-id="06810-198">Int64</span></span>|<span data-ttu-id="06810-199">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="06810-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="06810-200">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="06810-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="06810-201">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="06810-201">applicableArchitectures</span></span>|[<span data-ttu-id="06810-202">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="06810-202">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="06810-203">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="06810-203">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="06810-204">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。</span><span class="sxs-lookup"><span data-stu-id="06810-204">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="06810-205">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="06810-205">applicableDeviceTypes</span></span>|[<span data-ttu-id="06810-206">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="06810-206">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="06810-207">可运行此应用的 Windows 设备类型。</span><span class="sxs-lookup"><span data-stu-id="06810-207">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="06810-208">可取值为：`none`、`desktop`、`mobile`、`holographic`、`team`。</span><span class="sxs-lookup"><span data-stu-id="06810-208">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="06810-209">identityName</span><span class="sxs-lookup"><span data-stu-id="06810-209">identityName</span></span>|<span data-ttu-id="06810-210">String</span><span class="sxs-lookup"><span data-stu-id="06810-210">String</span></span>|<span data-ttu-id="06810-211">标识名称。</span><span class="sxs-lookup"><span data-stu-id="06810-211">The Identity Name.</span></span>|
|<span data-ttu-id="06810-212">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="06810-212">identityPublisherHash</span></span>|<span data-ttu-id="06810-213">String</span><span class="sxs-lookup"><span data-stu-id="06810-213">String</span></span>|<span data-ttu-id="06810-214">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="06810-214">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="06810-215">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="06810-215">identityResourceIdentifier</span></span>|<span data-ttu-id="06810-216">String</span><span class="sxs-lookup"><span data-stu-id="06810-216">String</span></span>|<span data-ttu-id="06810-217">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="06810-217">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="06810-218">isBundle</span><span class="sxs-lookup"><span data-stu-id="06810-218">isBundle</span></span>|<span data-ttu-id="06810-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="06810-219">Boolean</span></span>|<span data-ttu-id="06810-220">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="06810-220">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="06810-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="06810-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="06810-222">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="06810-222">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="06810-223">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="06810-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="06810-224">identityVersion</span><span class="sxs-lookup"><span data-stu-id="06810-224">identityVersion</span></span>|<span data-ttu-id="06810-225">String</span><span class="sxs-lookup"><span data-stu-id="06810-225">String</span></span>|<span data-ttu-id="06810-226">标识版本。</span><span class="sxs-lookup"><span data-stu-id="06810-226">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="06810-227">响应</span><span class="sxs-lookup"><span data-stu-id="06810-227">Response</span></span>
<span data-ttu-id="06810-228">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06810-228">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06810-229">示例</span><span class="sxs-lookup"><span data-stu-id="06810-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="06810-230">请求</span><span class="sxs-lookup"><span data-stu-id="06810-230">Request</span></span>
<span data-ttu-id="06810-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="06810-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="06810-232">响应</span><span class="sxs-lookup"><span data-stu-id="06810-232">Response</span></span>
<span data-ttu-id="06810-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="06810-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```




