---
title: 创建 windowsUniversalAppX
description: 创建新的 windowsUniversalAppX 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a8a089791ea8535f14fd8e4c1b80d83588ed735
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424964"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="48219-103">创建 windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="48219-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="48219-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="48219-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="48219-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="48219-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48219-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="48219-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48219-107">创建新的 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="48219-107">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48219-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="48219-108">Prerequisites</span></span>
<span data-ttu-id="48219-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="48219-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="48219-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="48219-111">Permission type</span></span>|<span data-ttu-id="48219-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="48219-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48219-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48219-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48219-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48219-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="48219-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48219-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48219-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="48219-116">Not supported.</span></span>|
|<span data-ttu-id="48219-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="48219-117">Application</span></span>|<span data-ttu-id="48219-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="48219-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48219-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48219-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="48219-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="48219-120">Request headers</span></span>
|<span data-ttu-id="48219-121">标头</span><span class="sxs-lookup"><span data-stu-id="48219-121">Header</span></span>|<span data-ttu-id="48219-122">值</span><span class="sxs-lookup"><span data-stu-id="48219-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48219-123">授权</span><span class="sxs-lookup"><span data-stu-id="48219-123">Authorization</span></span>|<span data-ttu-id="48219-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="48219-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48219-125">Accept</span><span class="sxs-lookup"><span data-stu-id="48219-125">Accept</span></span>|<span data-ttu-id="48219-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48219-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48219-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="48219-127">Request body</span></span>
<span data-ttu-id="48219-128">在请求正文中，提供 windowsUniversalAppX 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48219-128">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="48219-129">下表显示创建 windowsUniversalAppX 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="48219-129">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="48219-130">属性</span><span class="sxs-lookup"><span data-stu-id="48219-130">Property</span></span>|<span data-ttu-id="48219-131">类型</span><span class="sxs-lookup"><span data-stu-id="48219-131">Type</span></span>|<span data-ttu-id="48219-132">说明</span><span class="sxs-lookup"><span data-stu-id="48219-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48219-133">id</span><span class="sxs-lookup"><span data-stu-id="48219-133">id</span></span>|<span data-ttu-id="48219-134">String</span><span class="sxs-lookup"><span data-stu-id="48219-134">String</span></span>|<span data-ttu-id="48219-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="48219-135">Key of the entity.</span></span> <span data-ttu-id="48219-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-137">displayName</span><span class="sxs-lookup"><span data-stu-id="48219-137">displayName</span></span>|<span data-ttu-id="48219-138">String</span><span class="sxs-lookup"><span data-stu-id="48219-138">String</span></span>|<span data-ttu-id="48219-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="48219-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="48219-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-141">description</span><span class="sxs-lookup"><span data-stu-id="48219-141">description</span></span>|<span data-ttu-id="48219-142">String</span><span class="sxs-lookup"><span data-stu-id="48219-142">String</span></span>|<span data-ttu-id="48219-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="48219-143">The description of the app.</span></span> <span data-ttu-id="48219-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-145">publisher</span><span class="sxs-lookup"><span data-stu-id="48219-145">publisher</span></span>|<span data-ttu-id="48219-146">String</span><span class="sxs-lookup"><span data-stu-id="48219-146">String</span></span>|<span data-ttu-id="48219-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="48219-147">The publisher of the app.</span></span> <span data-ttu-id="48219-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="48219-149">largeIcon</span></span>|[<span data-ttu-id="48219-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="48219-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="48219-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="48219-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="48219-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48219-153">createdDateTime</span></span>|<span data-ttu-id="48219-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48219-154">DateTimeOffset</span></span>|<span data-ttu-id="48219-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="48219-155">The date and time the app was created.</span></span> <span data-ttu-id="48219-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48219-157">lastModifiedDateTime</span></span>|<span data-ttu-id="48219-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48219-158">DateTimeOffset</span></span>|<span data-ttu-id="48219-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="48219-159">The date and time the app was last modified.</span></span> <span data-ttu-id="48219-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="48219-161">isFeatured</span></span>|<span data-ttu-id="48219-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="48219-162">Boolean</span></span>|<span data-ttu-id="48219-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="48219-164">privacyInformationUrl</span></span>|<span data-ttu-id="48219-165">String</span><span class="sxs-lookup"><span data-stu-id="48219-165">String</span></span>|<span data-ttu-id="48219-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="48219-166">The privacy statement Url.</span></span> <span data-ttu-id="48219-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="48219-168">informationUrl</span></span>|<span data-ttu-id="48219-169">String</span><span class="sxs-lookup"><span data-stu-id="48219-169">String</span></span>|<span data-ttu-id="48219-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="48219-170">The more information Url.</span></span> <span data-ttu-id="48219-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-172">owner</span><span class="sxs-lookup"><span data-stu-id="48219-172">owner</span></span>|<span data-ttu-id="48219-173">String</span><span class="sxs-lookup"><span data-stu-id="48219-173">String</span></span>|<span data-ttu-id="48219-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="48219-174">The owner of the app.</span></span> <span data-ttu-id="48219-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-176">developer</span><span class="sxs-lookup"><span data-stu-id="48219-176">developer</span></span>|<span data-ttu-id="48219-177">String</span><span class="sxs-lookup"><span data-stu-id="48219-177">String</span></span>|<span data-ttu-id="48219-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="48219-178">The developer of the app.</span></span> <span data-ttu-id="48219-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-180">notes</span><span class="sxs-lookup"><span data-stu-id="48219-180">notes</span></span>|<span data-ttu-id="48219-181">String</span><span class="sxs-lookup"><span data-stu-id="48219-181">String</span></span>|<span data-ttu-id="48219-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="48219-182">Notes for the app.</span></span> <span data-ttu-id="48219-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="48219-184">uploadState</span></span>|<span data-ttu-id="48219-185">Int32</span><span class="sxs-lookup"><span data-stu-id="48219-185">Int32</span></span>|<span data-ttu-id="48219-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="48219-186">The upload state.</span></span> <span data-ttu-id="48219-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="48219-188">publishingState</span></span>|[<span data-ttu-id="48219-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="48219-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="48219-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="48219-190">The publishing state for the app.</span></span> <span data-ttu-id="48219-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="48219-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="48219-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="48219-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="48219-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="48219-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="48219-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="48219-194">isAssigned</span></span>|<span data-ttu-id="48219-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="48219-195">Boolean</span></span>|<span data-ttu-id="48219-196">值，指示是否将应用程序分配给至少一个组。</span><span class="sxs-lookup"><span data-stu-id="48219-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="48219-197">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="48219-198">roleScopeTagIds</span></span>|<span data-ttu-id="48219-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="48219-199">String collection</span></span>|<span data-ttu-id="48219-200">此移动应用程序的作用域标记 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="48219-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="48219-201">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48219-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="48219-202">committedContentVersion</span></span>|<span data-ttu-id="48219-203">String</span><span class="sxs-lookup"><span data-stu-id="48219-203">String</span></span>|<span data-ttu-id="48219-204">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="48219-204">The internal committed content version.</span></span> <span data-ttu-id="48219-205">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="48219-206">fileName</span><span class="sxs-lookup"><span data-stu-id="48219-206">fileName</span></span>|<span data-ttu-id="48219-207">String</span><span class="sxs-lookup"><span data-stu-id="48219-207">String</span></span>|<span data-ttu-id="48219-208">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="48219-208">The name of the main Lob application file.</span></span> <span data-ttu-id="48219-209">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="48219-210">size</span><span class="sxs-lookup"><span data-stu-id="48219-210">size</span></span>|<span data-ttu-id="48219-211">Int64</span><span class="sxs-lookup"><span data-stu-id="48219-211">Int64</span></span>|<span data-ttu-id="48219-212">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="48219-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="48219-213">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="48219-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="48219-214">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="48219-214">applicableArchitectures</span></span>|[<span data-ttu-id="48219-215">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="48219-215">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="48219-216">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="48219-216">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="48219-217">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="48219-217">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="48219-218">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="48219-218">applicableDeviceTypes</span></span>|[<span data-ttu-id="48219-219">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="48219-219">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="48219-220">可运行此应用的 Windows 设备类型。</span><span class="sxs-lookup"><span data-stu-id="48219-220">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="48219-221">可取值为：`none`、`desktop`、`mobile`、`holographic`、`team`。</span><span class="sxs-lookup"><span data-stu-id="48219-221">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="48219-222">identityName</span><span class="sxs-lookup"><span data-stu-id="48219-222">identityName</span></span>|<span data-ttu-id="48219-223">String</span><span class="sxs-lookup"><span data-stu-id="48219-223">String</span></span>|<span data-ttu-id="48219-224">标识名称。</span><span class="sxs-lookup"><span data-stu-id="48219-224">The Identity Name.</span></span>|
|<span data-ttu-id="48219-225">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="48219-225">identityPublisherHash</span></span>|<span data-ttu-id="48219-226">String</span><span class="sxs-lookup"><span data-stu-id="48219-226">String</span></span>|<span data-ttu-id="48219-227">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="48219-227">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="48219-228">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="48219-228">identityResourceIdentifier</span></span>|<span data-ttu-id="48219-229">String</span><span class="sxs-lookup"><span data-stu-id="48219-229">String</span></span>|<span data-ttu-id="48219-230">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="48219-230">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="48219-231">isBundle</span><span class="sxs-lookup"><span data-stu-id="48219-231">isBundle</span></span>|<span data-ttu-id="48219-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="48219-232">Boolean</span></span>|<span data-ttu-id="48219-233">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="48219-233">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="48219-234">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="48219-234">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="48219-235">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="48219-235">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="48219-236">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="48219-236">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="48219-237">identityVersion</span><span class="sxs-lookup"><span data-stu-id="48219-237">identityVersion</span></span>|<span data-ttu-id="48219-238">String</span><span class="sxs-lookup"><span data-stu-id="48219-238">String</span></span>|<span data-ttu-id="48219-239">标识版本。</span><span class="sxs-lookup"><span data-stu-id="48219-239">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="48219-240">响应</span><span class="sxs-lookup"><span data-stu-id="48219-240">Response</span></span>
<span data-ttu-id="48219-241">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="48219-241">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48219-242">示例</span><span class="sxs-lookup"><span data-stu-id="48219-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="48219-243">请求</span><span class="sxs-lookup"><span data-stu-id="48219-243">Request</span></span>
<span data-ttu-id="48219-244">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="48219-244">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1388

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
  "applicableDeviceTypes": "desktop",
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

### <a name="response"></a><span data-ttu-id="48219-245">响应</span><span class="sxs-lookup"><span data-stu-id="48219-245">Response</span></span>
<span data-ttu-id="48219-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="48219-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1560

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
  "applicableDeviceTypes": "desktop",
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




