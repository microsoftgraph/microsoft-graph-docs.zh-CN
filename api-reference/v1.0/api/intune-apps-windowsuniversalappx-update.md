---
title: 更新 windowsUniversalAppX
description: 更新 windowsUniversalAppX 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b684cb53aa514f27391842accea803d409b7d663
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515775"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="9f45e-103">更新 windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="9f45e-103">Update windowsUniversalAppX</span></span>

<span data-ttu-id="9f45e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f45e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f45e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f45e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f45e-106">更新 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9f45e-106">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f45e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9f45e-107">Prerequisites</span></span>
<span data-ttu-id="9f45e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f45e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f45e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f45e-110">Permission type</span></span>|<span data-ttu-id="9f45e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9f45e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f45e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f45e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f45e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f45e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9f45e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f45e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f45e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f45e-115">Not supported.</span></span>|
|<span data-ttu-id="9f45e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9f45e-116">Application</span></span>|<span data-ttu-id="9f45e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9f45e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f45e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f45e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="9f45e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f45e-119">Request headers</span></span>
|<span data-ttu-id="9f45e-120">标头</span><span class="sxs-lookup"><span data-stu-id="9f45e-120">Header</span></span>|<span data-ttu-id="9f45e-121">值</span><span class="sxs-lookup"><span data-stu-id="9f45e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f45e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f45e-122">Authorization</span></span>|<span data-ttu-id="9f45e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9f45e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f45e-124">接受</span><span class="sxs-lookup"><span data-stu-id="9f45e-124">Accept</span></span>|<span data-ttu-id="9f45e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f45e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f45e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f45e-126">Request body</span></span>
<span data-ttu-id="9f45e-127">在请求正文中，提供 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9f45e-127">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="9f45e-128">下表显示创建 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9f45e-128">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="9f45e-129">属性</span><span class="sxs-lookup"><span data-stu-id="9f45e-129">Property</span></span>|<span data-ttu-id="9f45e-130">类型</span><span class="sxs-lookup"><span data-stu-id="9f45e-130">Type</span></span>|<span data-ttu-id="9f45e-131">说明</span><span class="sxs-lookup"><span data-stu-id="9f45e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f45e-132">id</span><span class="sxs-lookup"><span data-stu-id="9f45e-132">id</span></span>|<span data-ttu-id="9f45e-133">字符串</span><span class="sxs-lookup"><span data-stu-id="9f45e-133">String</span></span>|<span data-ttu-id="9f45e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9f45e-134">Key of the entity.</span></span> <span data-ttu-id="9f45e-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9f45e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9f45e-136">displayName</span></span>|<span data-ttu-id="9f45e-137">字符串</span><span class="sxs-lookup"><span data-stu-id="9f45e-137">String</span></span>|<span data-ttu-id="9f45e-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="9f45e-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9f45e-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9f45e-140">说明</span><span class="sxs-lookup"><span data-stu-id="9f45e-140">description</span></span>|<span data-ttu-id="9f45e-141">字符串</span><span class="sxs-lookup"><span data-stu-id="9f45e-141">String</span></span>|<span data-ttu-id="9f45e-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="9f45e-142">The description of the app.</span></span> <span data-ttu-id="9f45e-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9f45e-144">publisher</span><span class="sxs-lookup"><span data-stu-id="9f45e-144">publisher</span></span>|<span data-ttu-id="9f45e-145">字符串</span><span class="sxs-lookup"><span data-stu-id="9f45e-145">String</span></span>|<span data-ttu-id="9f45e-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="9f45e-146">The publisher of the app.</span></span> <span data-ttu-id="9f45e-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9f45e-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9f45e-148">largeIcon</span></span>|[<span data-ttu-id="9f45e-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9f45e-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9f45e-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="9f45e-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9f45e-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9f45e-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f45e-152">createdDateTime</span></span>|<span data-ttu-id="9f45e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f45e-153">DateTimeOffset</span></span>|<span data-ttu-id="9f45e-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9f45e-154">The date and time the app was created.</span></span> <span data-ttu-id="9f45e-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9f45e-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f45e-156">lastModifiedDateTime</span></span>|<span data-ttu-id="9f45e-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f45e-157">DateTimeOffset</span></span>|<span data-ttu-id="9f45e-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9f45e-158">The date and time the app was last modified.</span></span> <span data-ttu-id="9f45e-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9f45e-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9f45e-160">isFeatured</span></span>|<span data-ttu-id="9f45e-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f45e-161">Boolean</span></span>|<span data-ttu-id="9f45e-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9f45e-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9f45e-163">privacyInformationUrl</span></span>|<span data-ttu-id="9f45e-164">字符串</span><span class="sxs-lookup"><span data-stu-id="9f45e-164">String</span></span>|<span data-ttu-id="9f45e-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="9f45e-165">The privacy statement Url.</span></span> <span data-ttu-id="9f45e-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9f45e-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9f45e-167">informationUrl</span></span>|<span data-ttu-id="9f45e-168">字符串</span><span class="sxs-lookup"><span data-stu-id="9f45e-168">String</span></span>|<span data-ttu-id="9f45e-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="9f45e-169">The more information Url.</span></span> <span data-ttu-id="9f45e-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9f45e-171">owner</span><span class="sxs-lookup"><span data-stu-id="9f45e-171">owner</span></span>|<span data-ttu-id="9f45e-172">String</span><span class="sxs-lookup"><span data-stu-id="9f45e-172">String</span></span>|<span data-ttu-id="9f45e-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="9f45e-173">The owner of the app.</span></span> <span data-ttu-id="9f45e-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9f45e-175">developer</span><span class="sxs-lookup"><span data-stu-id="9f45e-175">developer</span></span>|<span data-ttu-id="9f45e-176">字符串</span><span class="sxs-lookup"><span data-stu-id="9f45e-176">String</span></span>|<span data-ttu-id="9f45e-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="9f45e-177">The developer of the app.</span></span> <span data-ttu-id="9f45e-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9f45e-179">notes</span><span class="sxs-lookup"><span data-stu-id="9f45e-179">notes</span></span>|<span data-ttu-id="9f45e-180">字符串</span><span class="sxs-lookup"><span data-stu-id="9f45e-180">String</span></span>|<span data-ttu-id="9f45e-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="9f45e-181">Notes for the app.</span></span> <span data-ttu-id="9f45e-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9f45e-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="9f45e-183">publishingState</span></span>|[<span data-ttu-id="9f45e-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9f45e-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9f45e-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="9f45e-185">The publishing state for the app.</span></span> <span data-ttu-id="9f45e-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="9f45e-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9f45e-187">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="9f45e-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9f45e-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="9f45e-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9f45e-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9f45e-189">committedContentVersion</span></span>|<span data-ttu-id="9f45e-190">字符串</span><span class="sxs-lookup"><span data-stu-id="9f45e-190">String</span></span>|<span data-ttu-id="9f45e-191">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="9f45e-191">The internal committed content version.</span></span> <span data-ttu-id="9f45e-192">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9f45e-193">fileName</span><span class="sxs-lookup"><span data-stu-id="9f45e-193">fileName</span></span>|<span data-ttu-id="9f45e-194">字符串</span><span class="sxs-lookup"><span data-stu-id="9f45e-194">String</span></span>|<span data-ttu-id="9f45e-195">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="9f45e-195">The name of the main Lob application file.</span></span> <span data-ttu-id="9f45e-196">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9f45e-197">size</span><span class="sxs-lookup"><span data-stu-id="9f45e-197">size</span></span>|<span data-ttu-id="9f45e-198">Int64</span><span class="sxs-lookup"><span data-stu-id="9f45e-198">Int64</span></span>|<span data-ttu-id="9f45e-199">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="9f45e-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="9f45e-200">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9f45e-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="9f45e-201">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="9f45e-201">applicableArchitectures</span></span>|[<span data-ttu-id="9f45e-202">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="9f45e-202">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="9f45e-203">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="9f45e-203">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="9f45e-204">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。</span><span class="sxs-lookup"><span data-stu-id="9f45e-204">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="9f45e-205">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="9f45e-205">applicableDeviceTypes</span></span>|[<span data-ttu-id="9f45e-206">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="9f45e-206">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="9f45e-207">可运行此应用的 Windows 设备类型。</span><span class="sxs-lookup"><span data-stu-id="9f45e-207">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="9f45e-208">可取值为：`none`、`desktop`、`mobile`、`holographic`、`team`。</span><span class="sxs-lookup"><span data-stu-id="9f45e-208">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="9f45e-209">identityName</span><span class="sxs-lookup"><span data-stu-id="9f45e-209">identityName</span></span>|<span data-ttu-id="9f45e-210">字符串</span><span class="sxs-lookup"><span data-stu-id="9f45e-210">String</span></span>|<span data-ttu-id="9f45e-211">标识名称。</span><span class="sxs-lookup"><span data-stu-id="9f45e-211">The Identity Name.</span></span>|
|<span data-ttu-id="9f45e-212">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="9f45e-212">identityPublisherHash</span></span>|<span data-ttu-id="9f45e-213">字符串</span><span class="sxs-lookup"><span data-stu-id="9f45e-213">String</span></span>|<span data-ttu-id="9f45e-214">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="9f45e-214">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="9f45e-215">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="9f45e-215">identityResourceIdentifier</span></span>|<span data-ttu-id="9f45e-216">字符串</span><span class="sxs-lookup"><span data-stu-id="9f45e-216">String</span></span>|<span data-ttu-id="9f45e-217">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="9f45e-217">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="9f45e-218">isBundle</span><span class="sxs-lookup"><span data-stu-id="9f45e-218">isBundle</span></span>|<span data-ttu-id="9f45e-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="9f45e-219">Boolean</span></span>|<span data-ttu-id="9f45e-220">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="9f45e-220">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="9f45e-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9f45e-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9f45e-222">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9f45e-222">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="9f45e-223">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="9f45e-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9f45e-224">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9f45e-224">identityVersion</span></span>|<span data-ttu-id="9f45e-225">String</span><span class="sxs-lookup"><span data-stu-id="9f45e-225">String</span></span>|<span data-ttu-id="9f45e-226">标识版本。</span><span class="sxs-lookup"><span data-stu-id="9f45e-226">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="9f45e-227">响应</span><span class="sxs-lookup"><span data-stu-id="9f45e-227">Response</span></span>
<span data-ttu-id="9f45e-228">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9f45e-228">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f45e-229">示例</span><span class="sxs-lookup"><span data-stu-id="9f45e-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f45e-230">请求</span><span class="sxs-lookup"><span data-stu-id="9f45e-230">Request</span></span>
<span data-ttu-id="9f45e-231">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9f45e-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f45e-232">响应</span><span class="sxs-lookup"><span data-stu-id="9f45e-232">Response</span></span>
<span data-ttu-id="9f45e-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9f45e-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




