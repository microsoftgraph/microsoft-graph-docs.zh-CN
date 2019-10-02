---
title: 更新 windowsUniversalAppX
description: 更新 windowsUniversalAppX 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0c11c649b6ce7e56dab0aa5556874dfa619055a4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354894"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="e28f8-103">更新 windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="e28f8-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="e28f8-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e28f8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e28f8-105">更新 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e28f8-105">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e28f8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="e28f8-106">Prerequisites</span></span>
<span data-ttu-id="e28f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e28f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e28f8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e28f8-109">Permission type</span></span>|<span data-ttu-id="e28f8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e28f8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e28f8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e28f8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e28f8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e28f8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e28f8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e28f8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e28f8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e28f8-114">Not supported.</span></span>|
|<span data-ttu-id="e28f8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e28f8-115">Application</span></span>|<span data-ttu-id="e28f8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e28f8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e28f8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e28f8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="e28f8-118">请求头</span><span class="sxs-lookup"><span data-stu-id="e28f8-118">Request headers</span></span>
|<span data-ttu-id="e28f8-119">标头</span><span class="sxs-lookup"><span data-stu-id="e28f8-119">Header</span></span>|<span data-ttu-id="e28f8-120">值</span><span class="sxs-lookup"><span data-stu-id="e28f8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e28f8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e28f8-121">Authorization</span></span>|<span data-ttu-id="e28f8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e28f8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e28f8-123">接受</span><span class="sxs-lookup"><span data-stu-id="e28f8-123">Accept</span></span>|<span data-ttu-id="e28f8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e28f8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e28f8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e28f8-125">Request body</span></span>
<span data-ttu-id="e28f8-126">在请求正文中，提供 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e28f8-126">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="e28f8-127">下表显示创建 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e28f8-127">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="e28f8-128">属性</span><span class="sxs-lookup"><span data-stu-id="e28f8-128">Property</span></span>|<span data-ttu-id="e28f8-129">类型</span><span class="sxs-lookup"><span data-stu-id="e28f8-129">Type</span></span>|<span data-ttu-id="e28f8-130">说明</span><span class="sxs-lookup"><span data-stu-id="e28f8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e28f8-131">id</span><span class="sxs-lookup"><span data-stu-id="e28f8-131">id</span></span>|<span data-ttu-id="e28f8-132">字符串</span><span class="sxs-lookup"><span data-stu-id="e28f8-132">String</span></span>|<span data-ttu-id="e28f8-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e28f8-133">Key of the entity.</span></span> <span data-ttu-id="e28f8-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e28f8-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e28f8-135">displayName</span></span>|<span data-ttu-id="e28f8-136">String</span><span class="sxs-lookup"><span data-stu-id="e28f8-136">String</span></span>|<span data-ttu-id="e28f8-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="e28f8-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e28f8-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e28f8-139">说明</span><span class="sxs-lookup"><span data-stu-id="e28f8-139">description</span></span>|<span data-ttu-id="e28f8-140">字符串</span><span class="sxs-lookup"><span data-stu-id="e28f8-140">String</span></span>|<span data-ttu-id="e28f8-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="e28f8-141">The description of the app.</span></span> <span data-ttu-id="e28f8-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e28f8-143">publisher</span><span class="sxs-lookup"><span data-stu-id="e28f8-143">publisher</span></span>|<span data-ttu-id="e28f8-144">String</span><span class="sxs-lookup"><span data-stu-id="e28f8-144">String</span></span>|<span data-ttu-id="e28f8-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="e28f8-145">The publisher of the app.</span></span> <span data-ttu-id="e28f8-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e28f8-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e28f8-147">largeIcon</span></span>|[<span data-ttu-id="e28f8-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e28f8-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e28f8-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="e28f8-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e28f8-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e28f8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e28f8-151">createdDateTime</span></span>|<span data-ttu-id="e28f8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e28f8-152">DateTimeOffset</span></span>|<span data-ttu-id="e28f8-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e28f8-153">The date and time the app was created.</span></span> <span data-ttu-id="e28f8-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e28f8-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e28f8-155">lastModifiedDateTime</span></span>|<span data-ttu-id="e28f8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e28f8-156">DateTimeOffset</span></span>|<span data-ttu-id="e28f8-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e28f8-157">The date and time the app was last modified.</span></span> <span data-ttu-id="e28f8-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e28f8-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e28f8-159">isFeatured</span></span>|<span data-ttu-id="e28f8-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="e28f8-160">Boolean</span></span>|<span data-ttu-id="e28f8-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e28f8-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e28f8-162">privacyInformationUrl</span></span>|<span data-ttu-id="e28f8-163">String</span><span class="sxs-lookup"><span data-stu-id="e28f8-163">String</span></span>|<span data-ttu-id="e28f8-164">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="e28f8-164">The privacy statement Url.</span></span> <span data-ttu-id="e28f8-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e28f8-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e28f8-166">informationUrl</span></span>|<span data-ttu-id="e28f8-167">String</span><span class="sxs-lookup"><span data-stu-id="e28f8-167">String</span></span>|<span data-ttu-id="e28f8-168">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="e28f8-168">The more information Url.</span></span> <span data-ttu-id="e28f8-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e28f8-170">owner</span><span class="sxs-lookup"><span data-stu-id="e28f8-170">owner</span></span>|<span data-ttu-id="e28f8-171">String</span><span class="sxs-lookup"><span data-stu-id="e28f8-171">String</span></span>|<span data-ttu-id="e28f8-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="e28f8-172">The owner of the app.</span></span> <span data-ttu-id="e28f8-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e28f8-174">developer</span><span class="sxs-lookup"><span data-stu-id="e28f8-174">developer</span></span>|<span data-ttu-id="e28f8-175">String</span><span class="sxs-lookup"><span data-stu-id="e28f8-175">String</span></span>|<span data-ttu-id="e28f8-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="e28f8-176">The developer of the app.</span></span> <span data-ttu-id="e28f8-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e28f8-178">notes</span><span class="sxs-lookup"><span data-stu-id="e28f8-178">notes</span></span>|<span data-ttu-id="e28f8-179">String</span><span class="sxs-lookup"><span data-stu-id="e28f8-179">String</span></span>|<span data-ttu-id="e28f8-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="e28f8-180">Notes for the app.</span></span> <span data-ttu-id="e28f8-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e28f8-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="e28f8-182">publishingState</span></span>|[<span data-ttu-id="e28f8-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e28f8-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e28f8-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="e28f8-184">The publishing state for the app.</span></span> <span data-ttu-id="e28f8-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="e28f8-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e28f8-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="e28f8-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e28f8-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="e28f8-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e28f8-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e28f8-188">committedContentVersion</span></span>|<span data-ttu-id="e28f8-189">String</span><span class="sxs-lookup"><span data-stu-id="e28f8-189">String</span></span>|<span data-ttu-id="e28f8-190">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="e28f8-190">The internal committed content version.</span></span> <span data-ttu-id="e28f8-191">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e28f8-192">fileName</span><span class="sxs-lookup"><span data-stu-id="e28f8-192">fileName</span></span>|<span data-ttu-id="e28f8-193">String</span><span class="sxs-lookup"><span data-stu-id="e28f8-193">String</span></span>|<span data-ttu-id="e28f8-194">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="e28f8-194">The name of the main Lob application file.</span></span> <span data-ttu-id="e28f8-195">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e28f8-196">size</span><span class="sxs-lookup"><span data-stu-id="e28f8-196">size</span></span>|<span data-ttu-id="e28f8-197">Int64</span><span class="sxs-lookup"><span data-stu-id="e28f8-197">Int64</span></span>|<span data-ttu-id="e28f8-198">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="e28f8-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="e28f8-199">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="e28f8-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e28f8-200">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="e28f8-200">applicableArchitectures</span></span>|[<span data-ttu-id="e28f8-201">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="e28f8-201">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="e28f8-202">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="e28f8-202">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="e28f8-203">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。</span><span class="sxs-lookup"><span data-stu-id="e28f8-203">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="e28f8-204">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="e28f8-204">applicableDeviceTypes</span></span>|[<span data-ttu-id="e28f8-205">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="e28f8-205">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="e28f8-206">可运行此应用的 Windows 设备类型。</span><span class="sxs-lookup"><span data-stu-id="e28f8-206">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="e28f8-207">可取值为：`none`、`desktop`、`mobile`、`holographic`、`team`。</span><span class="sxs-lookup"><span data-stu-id="e28f8-207">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="e28f8-208">identityName</span><span class="sxs-lookup"><span data-stu-id="e28f8-208">identityName</span></span>|<span data-ttu-id="e28f8-209">String</span><span class="sxs-lookup"><span data-stu-id="e28f8-209">String</span></span>|<span data-ttu-id="e28f8-210">标识名称。</span><span class="sxs-lookup"><span data-stu-id="e28f8-210">The Identity Name.</span></span>|
|<span data-ttu-id="e28f8-211">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="e28f8-211">identityPublisherHash</span></span>|<span data-ttu-id="e28f8-212">String</span><span class="sxs-lookup"><span data-stu-id="e28f8-212">String</span></span>|<span data-ttu-id="e28f8-213">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="e28f8-213">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="e28f8-214">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="e28f8-214">identityResourceIdentifier</span></span>|<span data-ttu-id="e28f8-215">String</span><span class="sxs-lookup"><span data-stu-id="e28f8-215">String</span></span>|<span data-ttu-id="e28f8-216">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="e28f8-216">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="e28f8-217">isBundle</span><span class="sxs-lookup"><span data-stu-id="e28f8-217">isBundle</span></span>|<span data-ttu-id="e28f8-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="e28f8-218">Boolean</span></span>|<span data-ttu-id="e28f8-219">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="e28f8-219">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="e28f8-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e28f8-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e28f8-221">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e28f8-221">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="e28f8-222">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="e28f8-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e28f8-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="e28f8-223">identityVersion</span></span>|<span data-ttu-id="e28f8-224">String</span><span class="sxs-lookup"><span data-stu-id="e28f8-224">String</span></span>|<span data-ttu-id="e28f8-225">标识版本。</span><span class="sxs-lookup"><span data-stu-id="e28f8-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="e28f8-226">响应</span><span class="sxs-lookup"><span data-stu-id="e28f8-226">Response</span></span>
<span data-ttu-id="e28f8-227">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e28f8-227">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e28f8-228">示例</span><span class="sxs-lookup"><span data-stu-id="e28f8-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="e28f8-229">请求</span><span class="sxs-lookup"><span data-stu-id="e28f8-229">Request</span></span>
<span data-ttu-id="e28f8-230">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e28f8-230">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e28f8-231">响应</span><span class="sxs-lookup"><span data-stu-id="e28f8-231">Response</span></span>
<span data-ttu-id="e28f8-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e28f8-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




