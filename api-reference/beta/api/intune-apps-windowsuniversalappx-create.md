---
title: 创建 windowsUniversalAppX
description: 创建新的 windowsUniversalAppX 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc6678b950ca5894b5fd480e74f8a4ab4ed371dd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971561"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="1f7ed-103">创建 windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="1f7ed-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="1f7ed-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f7ed-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f7ed-106">创建新的 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-106">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f7ed-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="1f7ed-107">Prerequisites</span></span>
<span data-ttu-id="1f7ed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f7ed-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f7ed-110">Permission type</span></span>|<span data-ttu-id="1f7ed-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1f7ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f7ed-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f7ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f7ed-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f7ed-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1f7ed-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f7ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f7ed-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-115">Not supported.</span></span>|
|<span data-ttu-id="1f7ed-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f7ed-116">Application</span></span>|<span data-ttu-id="1f7ed-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f7ed-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f7ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1f7ed-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f7ed-119">Request headers</span></span>
|<span data-ttu-id="1f7ed-120">标头</span><span class="sxs-lookup"><span data-stu-id="1f7ed-120">Header</span></span>|<span data-ttu-id="1f7ed-121">值</span><span class="sxs-lookup"><span data-stu-id="1f7ed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f7ed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f7ed-122">Authorization</span></span>|<span data-ttu-id="1f7ed-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f7ed-124">接受</span><span class="sxs-lookup"><span data-stu-id="1f7ed-124">Accept</span></span>|<span data-ttu-id="1f7ed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f7ed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f7ed-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f7ed-126">Request body</span></span>
<span data-ttu-id="1f7ed-127">在请求正文中，提供 windowsUniversalAppX 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-127">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="1f7ed-128">下表显示创建 windowsUniversalAppX 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-128">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="1f7ed-129">属性</span><span class="sxs-lookup"><span data-stu-id="1f7ed-129">Property</span></span>|<span data-ttu-id="1f7ed-130">类型</span><span class="sxs-lookup"><span data-stu-id="1f7ed-130">Type</span></span>|<span data-ttu-id="1f7ed-131">说明</span><span class="sxs-lookup"><span data-stu-id="1f7ed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f7ed-132">id</span><span class="sxs-lookup"><span data-stu-id="1f7ed-132">id</span></span>|<span data-ttu-id="1f7ed-133">String</span><span class="sxs-lookup"><span data-stu-id="1f7ed-133">String</span></span>|<span data-ttu-id="1f7ed-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-134">Key of the entity.</span></span> <span data-ttu-id="1f7ed-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1f7ed-136">displayName</span></span>|<span data-ttu-id="1f7ed-137">String</span><span class="sxs-lookup"><span data-stu-id="1f7ed-137">String</span></span>|<span data-ttu-id="1f7ed-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1f7ed-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-140">description</span><span class="sxs-lookup"><span data-stu-id="1f7ed-140">description</span></span>|<span data-ttu-id="1f7ed-141">String</span><span class="sxs-lookup"><span data-stu-id="1f7ed-141">String</span></span>|<span data-ttu-id="1f7ed-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-142">The description of the app.</span></span> <span data-ttu-id="1f7ed-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-144">publisher</span><span class="sxs-lookup"><span data-stu-id="1f7ed-144">publisher</span></span>|<span data-ttu-id="1f7ed-145">String</span><span class="sxs-lookup"><span data-stu-id="1f7ed-145">String</span></span>|<span data-ttu-id="1f7ed-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-146">The publisher of the app.</span></span> <span data-ttu-id="1f7ed-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1f7ed-148">largeIcon</span></span>|[<span data-ttu-id="1f7ed-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1f7ed-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1f7ed-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1f7ed-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f7ed-152">createdDateTime</span></span>|<span data-ttu-id="1f7ed-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f7ed-153">DateTimeOffset</span></span>|<span data-ttu-id="1f7ed-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-154">The date and time the app was created.</span></span> <span data-ttu-id="1f7ed-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f7ed-156">lastModifiedDateTime</span></span>|<span data-ttu-id="1f7ed-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f7ed-157">DateTimeOffset</span></span>|<span data-ttu-id="1f7ed-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-158">The date and time the app was last modified.</span></span> <span data-ttu-id="1f7ed-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1f7ed-160">isFeatured</span></span>|<span data-ttu-id="1f7ed-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f7ed-161">Boolean</span></span>|<span data-ttu-id="1f7ed-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1f7ed-163">privacyInformationUrl</span></span>|<span data-ttu-id="1f7ed-164">String</span><span class="sxs-lookup"><span data-stu-id="1f7ed-164">String</span></span>|<span data-ttu-id="1f7ed-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-165">The privacy statement Url.</span></span> <span data-ttu-id="1f7ed-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1f7ed-167">informationUrl</span></span>|<span data-ttu-id="1f7ed-168">String</span><span class="sxs-lookup"><span data-stu-id="1f7ed-168">String</span></span>|<span data-ttu-id="1f7ed-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-169">The more information Url.</span></span> <span data-ttu-id="1f7ed-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-171">owner</span><span class="sxs-lookup"><span data-stu-id="1f7ed-171">owner</span></span>|<span data-ttu-id="1f7ed-172">字符串</span><span class="sxs-lookup"><span data-stu-id="1f7ed-172">String</span></span>|<span data-ttu-id="1f7ed-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-173">The owner of the app.</span></span> <span data-ttu-id="1f7ed-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-175">developer</span><span class="sxs-lookup"><span data-stu-id="1f7ed-175">developer</span></span>|<span data-ttu-id="1f7ed-176">String</span><span class="sxs-lookup"><span data-stu-id="1f7ed-176">String</span></span>|<span data-ttu-id="1f7ed-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-177">The developer of the app.</span></span> <span data-ttu-id="1f7ed-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-179">notes</span><span class="sxs-lookup"><span data-stu-id="1f7ed-179">notes</span></span>|<span data-ttu-id="1f7ed-180">String</span><span class="sxs-lookup"><span data-stu-id="1f7ed-180">String</span></span>|<span data-ttu-id="1f7ed-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-181">Notes for the app.</span></span> <span data-ttu-id="1f7ed-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="1f7ed-183">uploadState</span></span>|<span data-ttu-id="1f7ed-184">Int32</span><span class="sxs-lookup"><span data-stu-id="1f7ed-184">Int32</span></span>|<span data-ttu-id="1f7ed-185">上载状态。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-185">The upload state.</span></span> <span data-ttu-id="1f7ed-186">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="1f7ed-187">publishingState</span></span>|[<span data-ttu-id="1f7ed-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1f7ed-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1f7ed-189">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-189">The publishing state for the app.</span></span> <span data-ttu-id="1f7ed-190">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1f7ed-191">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1f7ed-192">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1f7ed-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1f7ed-193">isAssigned</span></span>|<span data-ttu-id="1f7ed-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f7ed-194">Boolean</span></span>|<span data-ttu-id="1f7ed-195">指示是否至少向一个组分配了应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1f7ed-196">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1f7ed-197">roleScopeTagIds</span></span>|<span data-ttu-id="1f7ed-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="1f7ed-198">String collection</span></span>|<span data-ttu-id="1f7ed-199">此移动应用的作用域标记 id 列表。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1f7ed-200">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1f7ed-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1f7ed-201">committedContentVersion</span></span>|<span data-ttu-id="1f7ed-202">String</span><span class="sxs-lookup"><span data-stu-id="1f7ed-202">String</span></span>|<span data-ttu-id="1f7ed-203">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-203">The internal committed content version.</span></span> <span data-ttu-id="1f7ed-204">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1f7ed-205">fileName</span><span class="sxs-lookup"><span data-stu-id="1f7ed-205">fileName</span></span>|<span data-ttu-id="1f7ed-206">String</span><span class="sxs-lookup"><span data-stu-id="1f7ed-206">String</span></span>|<span data-ttu-id="1f7ed-207">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-207">The name of the main Lob application file.</span></span> <span data-ttu-id="1f7ed-208">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1f7ed-209">size</span><span class="sxs-lookup"><span data-stu-id="1f7ed-209">size</span></span>|<span data-ttu-id="1f7ed-210">Int64</span><span class="sxs-lookup"><span data-stu-id="1f7ed-210">Int64</span></span>|<span data-ttu-id="1f7ed-211">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="1f7ed-212">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f7ed-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1f7ed-213">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="1f7ed-213">applicableArchitectures</span></span>|[<span data-ttu-id="1f7ed-214">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="1f7ed-214">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="1f7ed-215">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-215">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="1f7ed-216">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-216">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="1f7ed-217">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="1f7ed-217">applicableDeviceTypes</span></span>|[<span data-ttu-id="1f7ed-218">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="1f7ed-218">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="1f7ed-219">可运行此应用的 Windows 设备类型。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-219">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="1f7ed-220">可取值为：`none`、`desktop`、`mobile`、`holographic`、`team`。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-220">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="1f7ed-221">identityName</span><span class="sxs-lookup"><span data-stu-id="1f7ed-221">identityName</span></span>|<span data-ttu-id="1f7ed-222">String</span><span class="sxs-lookup"><span data-stu-id="1f7ed-222">String</span></span>|<span data-ttu-id="1f7ed-223">标识名称。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-223">The Identity Name.</span></span>|
|<span data-ttu-id="1f7ed-224">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="1f7ed-224">identityPublisherHash</span></span>|<span data-ttu-id="1f7ed-225">String</span><span class="sxs-lookup"><span data-stu-id="1f7ed-225">String</span></span>|<span data-ttu-id="1f7ed-226">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-226">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="1f7ed-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="1f7ed-227">identityResourceIdentifier</span></span>|<span data-ttu-id="1f7ed-228">String</span><span class="sxs-lookup"><span data-stu-id="1f7ed-228">String</span></span>|<span data-ttu-id="1f7ed-229">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-229">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="1f7ed-230">isBundle</span><span class="sxs-lookup"><span data-stu-id="1f7ed-230">isBundle</span></span>|<span data-ttu-id="1f7ed-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f7ed-231">Boolean</span></span>|<span data-ttu-id="1f7ed-232">应用是否为捆绑包。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-232">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="1f7ed-233">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1f7ed-233">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1f7ed-234">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1f7ed-234">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="1f7ed-235">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-235">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="1f7ed-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1f7ed-236">identityVersion</span></span>|<span data-ttu-id="1f7ed-237">String</span><span class="sxs-lookup"><span data-stu-id="1f7ed-237">String</span></span>|<span data-ttu-id="1f7ed-238">标识版本。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="1f7ed-239">响应</span><span class="sxs-lookup"><span data-stu-id="1f7ed-239">Response</span></span>
<span data-ttu-id="1f7ed-240">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-240">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f7ed-241">示例</span><span class="sxs-lookup"><span data-stu-id="1f7ed-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f7ed-242">请求</span><span class="sxs-lookup"><span data-stu-id="1f7ed-242">Request</span></span>
<span data-ttu-id="1f7ed-243">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-243">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1f7ed-244">响应</span><span class="sxs-lookup"><span data-stu-id="1f7ed-244">Response</span></span>
<span data-ttu-id="1f7ed-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1f7ed-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




