---
title: 创建 windowsUniversalAppX
description: 创建新的 windowsUniversalAppX 对象。
author: tfitzmac
ms.openlocfilehash: bd1c58c56a3d2801bc5d4aaa9ca34286d6bacedb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348424"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="7dff9-103">创建 windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="7dff9-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="7dff9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7dff9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7dff9-105">创建新的 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7dff9-105">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7dff9-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="7dff9-106">Prerequisites</span></span>
<span data-ttu-id="7dff9-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7dff9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dff9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7dff9-109">Permission type</span></span>|<span data-ttu-id="7dff9-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7dff9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dff9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7dff9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7dff9-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dff9-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7dff9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7dff9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dff9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7dff9-114">Not supported.</span></span>|
|<span data-ttu-id="7dff9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7dff9-115">Application</span></span>|<span data-ttu-id="7dff9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7dff9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dff9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7dff9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7dff9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7dff9-118">Request headers</span></span>
|<span data-ttu-id="7dff9-119">标头</span><span class="sxs-lookup"><span data-stu-id="7dff9-119">Header</span></span>|<span data-ttu-id="7dff9-120">值</span><span class="sxs-lookup"><span data-stu-id="7dff9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dff9-121">授权</span><span class="sxs-lookup"><span data-stu-id="7dff9-121">Authorization</span></span>|<span data-ttu-id="7dff9-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7dff9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dff9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7dff9-123">Accept</span></span>|<span data-ttu-id="7dff9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7dff9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dff9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7dff9-125">Request body</span></span>
<span data-ttu-id="7dff9-126">在请求正文中，提供 windowsUniversalAppX 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7dff9-126">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="7dff9-127">下表显示创建 windowsUniversalAppX 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7dff9-127">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="7dff9-128">属性</span><span class="sxs-lookup"><span data-stu-id="7dff9-128">Property</span></span>|<span data-ttu-id="7dff9-129">类型</span><span class="sxs-lookup"><span data-stu-id="7dff9-129">Type</span></span>|<span data-ttu-id="7dff9-130">说明</span><span class="sxs-lookup"><span data-stu-id="7dff9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dff9-131">id</span><span class="sxs-lookup"><span data-stu-id="7dff9-131">id</span></span>|<span data-ttu-id="7dff9-132">String</span><span class="sxs-lookup"><span data-stu-id="7dff9-132">String</span></span>|<span data-ttu-id="7dff9-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7dff9-133">Key of the entity.</span></span> <span data-ttu-id="7dff9-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dff9-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7dff9-135">displayName</span></span>|<span data-ttu-id="7dff9-136">String</span><span class="sxs-lookup"><span data-stu-id="7dff9-136">String</span></span>|<span data-ttu-id="7dff9-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="7dff9-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7dff9-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dff9-139">description</span><span class="sxs-lookup"><span data-stu-id="7dff9-139">description</span></span>|<span data-ttu-id="7dff9-140">String</span><span class="sxs-lookup"><span data-stu-id="7dff9-140">String</span></span>|<span data-ttu-id="7dff9-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="7dff9-141">The description of the app.</span></span> <span data-ttu-id="7dff9-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dff9-143">publisher</span><span class="sxs-lookup"><span data-stu-id="7dff9-143">publisher</span></span>|<span data-ttu-id="7dff9-144">String</span><span class="sxs-lookup"><span data-stu-id="7dff9-144">String</span></span>|<span data-ttu-id="7dff9-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="7dff9-145">The publisher of the app.</span></span> <span data-ttu-id="7dff9-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dff9-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7dff9-147">largeIcon</span></span>|[<span data-ttu-id="7dff9-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7dff9-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7dff9-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="7dff9-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7dff9-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dff9-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7dff9-151">createdDateTime</span></span>|<span data-ttu-id="7dff9-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dff9-152">DateTimeOffset</span></span>|<span data-ttu-id="7dff9-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7dff9-153">The date and time the app was created.</span></span> <span data-ttu-id="7dff9-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dff9-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7dff9-155">lastModifiedDateTime</span></span>|<span data-ttu-id="7dff9-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dff9-156">DateTimeOffset</span></span>|<span data-ttu-id="7dff9-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7dff9-157">The date and time the app was last modified.</span></span> <span data-ttu-id="7dff9-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dff9-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7dff9-159">isFeatured</span></span>|<span data-ttu-id="7dff9-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dff9-160">Boolean</span></span>|<span data-ttu-id="7dff9-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dff9-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7dff9-162">privacyInformationUrl</span></span>|<span data-ttu-id="7dff9-163">String</span><span class="sxs-lookup"><span data-stu-id="7dff9-163">String</span></span>|<span data-ttu-id="7dff9-164">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="7dff9-164">The privacy statement Url.</span></span> <span data-ttu-id="7dff9-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dff9-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7dff9-166">informationUrl</span></span>|<span data-ttu-id="7dff9-167">String</span><span class="sxs-lookup"><span data-stu-id="7dff9-167">String</span></span>|<span data-ttu-id="7dff9-168">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="7dff9-168">The more information Url.</span></span> <span data-ttu-id="7dff9-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dff9-170">owner</span><span class="sxs-lookup"><span data-stu-id="7dff9-170">owner</span></span>|<span data-ttu-id="7dff9-171">String</span><span class="sxs-lookup"><span data-stu-id="7dff9-171">String</span></span>|<span data-ttu-id="7dff9-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="7dff9-172">The owner of the app.</span></span> <span data-ttu-id="7dff9-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dff9-174">developer</span><span class="sxs-lookup"><span data-stu-id="7dff9-174">developer</span></span>|<span data-ttu-id="7dff9-175">String</span><span class="sxs-lookup"><span data-stu-id="7dff9-175">String</span></span>|<span data-ttu-id="7dff9-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="7dff9-176">The developer of the app.</span></span> <span data-ttu-id="7dff9-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dff9-178">notes</span><span class="sxs-lookup"><span data-stu-id="7dff9-178">notes</span></span>|<span data-ttu-id="7dff9-179">String</span><span class="sxs-lookup"><span data-stu-id="7dff9-179">String</span></span>|<span data-ttu-id="7dff9-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="7dff9-180">Notes for the app.</span></span> <span data-ttu-id="7dff9-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7dff9-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="7dff9-182">publishingState</span></span>|[<span data-ttu-id="7dff9-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7dff9-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7dff9-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="7dff9-184">The publishing state for the app.</span></span> <span data-ttu-id="7dff9-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="7dff9-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7dff9-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="7dff9-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7dff9-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="7dff9-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7dff9-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="7dff9-188">committedContentVersion</span></span>|<span data-ttu-id="7dff9-189">String</span><span class="sxs-lookup"><span data-stu-id="7dff9-189">String</span></span>|<span data-ttu-id="7dff9-190">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="7dff9-190">The internal committed content version.</span></span> <span data-ttu-id="7dff9-191">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7dff9-192">fileName</span><span class="sxs-lookup"><span data-stu-id="7dff9-192">fileName</span></span>|<span data-ttu-id="7dff9-193">String</span><span class="sxs-lookup"><span data-stu-id="7dff9-193">String</span></span>|<span data-ttu-id="7dff9-194">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="7dff9-194">The name of the main Lob application file.</span></span> <span data-ttu-id="7dff9-195">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7dff9-196">size</span><span class="sxs-lookup"><span data-stu-id="7dff9-196">size</span></span>|<span data-ttu-id="7dff9-197">Int64</span><span class="sxs-lookup"><span data-stu-id="7dff9-197">Int64</span></span>|<span data-ttu-id="7dff9-198">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="7dff9-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="7dff9-199">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="7dff9-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="7dff9-200">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="7dff9-200">applicableArchitectures</span></span>|[<span data-ttu-id="7dff9-201">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="7dff9-201">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="7dff9-202">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="7dff9-202">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="7dff9-203">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。</span><span class="sxs-lookup"><span data-stu-id="7dff9-203">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="7dff9-204">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="7dff9-204">applicableDeviceTypes</span></span>|[<span data-ttu-id="7dff9-205">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="7dff9-205">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="7dff9-206">可运行此应用的 Windows 设备类型。</span><span class="sxs-lookup"><span data-stu-id="7dff9-206">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="7dff9-207">可取值为：`none`、`desktop`、`mobile`、`holographic`、`team`。</span><span class="sxs-lookup"><span data-stu-id="7dff9-207">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="7dff9-208">identityName</span><span class="sxs-lookup"><span data-stu-id="7dff9-208">identityName</span></span>|<span data-ttu-id="7dff9-209">String</span><span class="sxs-lookup"><span data-stu-id="7dff9-209">String</span></span>|<span data-ttu-id="7dff9-210">标识名称。</span><span class="sxs-lookup"><span data-stu-id="7dff9-210">The Identity Name.</span></span>|
|<span data-ttu-id="7dff9-211">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="7dff9-211">identityPublisherHash</span></span>|<span data-ttu-id="7dff9-212">String</span><span class="sxs-lookup"><span data-stu-id="7dff9-212">String</span></span>|<span data-ttu-id="7dff9-213">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="7dff9-213">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="7dff9-214">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7dff9-214">identityResourceIdentifier</span></span>|<span data-ttu-id="7dff9-215">String</span><span class="sxs-lookup"><span data-stu-id="7dff9-215">String</span></span>|<span data-ttu-id="7dff9-216">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="7dff9-216">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="7dff9-217">isBundle</span><span class="sxs-lookup"><span data-stu-id="7dff9-217">isBundle</span></span>|<span data-ttu-id="7dff9-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="7dff9-218">Boolean</span></span>|<span data-ttu-id="7dff9-219">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="7dff9-219">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="7dff9-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7dff9-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7dff9-221">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7dff9-221">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="7dff9-222">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="7dff9-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="7dff9-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="7dff9-223">identityVersion</span></span>|<span data-ttu-id="7dff9-224">String</span><span class="sxs-lookup"><span data-stu-id="7dff9-224">String</span></span>|<span data-ttu-id="7dff9-225">标识版本。</span><span class="sxs-lookup"><span data-stu-id="7dff9-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="7dff9-226">响应</span><span class="sxs-lookup"><span data-stu-id="7dff9-226">Response</span></span>
<span data-ttu-id="7dff9-227">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7dff9-227">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dff9-228">示例</span><span class="sxs-lookup"><span data-stu-id="7dff9-228">Example</span></span>
### <a name="request"></a><span data-ttu-id="7dff9-229">请求</span><span class="sxs-lookup"><span data-stu-id="7dff9-229">Request</span></span>
<span data-ttu-id="7dff9-230">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7dff9-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="7dff9-231">响应</span><span class="sxs-lookup"><span data-stu-id="7dff9-231">Response</span></span>
<span data-ttu-id="7dff9-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7dff9-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



