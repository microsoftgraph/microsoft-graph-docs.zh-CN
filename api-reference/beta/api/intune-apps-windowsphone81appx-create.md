---
title: 创建 windowsPhone81AppX
description: 创建新的 windowsPhone81AppX 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 629f06f372b85e50a7c239184c058fb0ff5005a2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401479"
---
# <a name="create-windowsphone81appx"></a><span data-ttu-id="31d25-103">创建 windowsPhone81AppX</span><span class="sxs-lookup"><span data-stu-id="31d25-103">Create windowsPhone81AppX</span></span>

> <span data-ttu-id="31d25-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="31d25-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="31d25-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="31d25-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31d25-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="31d25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31d25-107">创建新的[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)对象。</span><span class="sxs-lookup"><span data-stu-id="31d25-107">Create a new [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31d25-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="31d25-108">Prerequisites</span></span>
<span data-ttu-id="31d25-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="31d25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="31d25-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="31d25-111">Permission type</span></span>|<span data-ttu-id="31d25-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="31d25-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31d25-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="31d25-113">Delegated (work or school account)</span></span>|<span data-ttu-id="31d25-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31d25-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="31d25-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="31d25-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31d25-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="31d25-116">Not supported.</span></span>|
|<span data-ttu-id="31d25-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="31d25-117">Application</span></span>|<span data-ttu-id="31d25-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="31d25-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31d25-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="31d25-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="31d25-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="31d25-120">Request headers</span></span>
|<span data-ttu-id="31d25-121">标头</span><span class="sxs-lookup"><span data-stu-id="31d25-121">Header</span></span>|<span data-ttu-id="31d25-122">值</span><span class="sxs-lookup"><span data-stu-id="31d25-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31d25-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="31d25-123">Authorization</span></span>|<span data-ttu-id="31d25-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="31d25-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31d25-125">Accept</span><span class="sxs-lookup"><span data-stu-id="31d25-125">Accept</span></span>|<span data-ttu-id="31d25-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31d25-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31d25-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="31d25-127">Request body</span></span>
<span data-ttu-id="31d25-128">在请求正文中，提供 windowsPhone81AppX 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31d25-128">In the request body, supply a JSON representation for the windowsPhone81AppX object.</span></span>

<span data-ttu-id="31d25-129">下表显示时创建 windowsPhone81AppX 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="31d25-129">The following table shows the properties that are required when you create the windowsPhone81AppX.</span></span>

|<span data-ttu-id="31d25-130">属性</span><span class="sxs-lookup"><span data-stu-id="31d25-130">Property</span></span>|<span data-ttu-id="31d25-131">类型</span><span class="sxs-lookup"><span data-stu-id="31d25-131">Type</span></span>|<span data-ttu-id="31d25-132">说明</span><span class="sxs-lookup"><span data-stu-id="31d25-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31d25-133">id</span><span class="sxs-lookup"><span data-stu-id="31d25-133">id</span></span>|<span data-ttu-id="31d25-134">String</span><span class="sxs-lookup"><span data-stu-id="31d25-134">String</span></span>|<span data-ttu-id="31d25-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="31d25-135">Key of the entity.</span></span> <span data-ttu-id="31d25-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-137">displayName</span><span class="sxs-lookup"><span data-stu-id="31d25-137">displayName</span></span>|<span data-ttu-id="31d25-138">String</span><span class="sxs-lookup"><span data-stu-id="31d25-138">String</span></span>|<span data-ttu-id="31d25-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="31d25-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="31d25-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-141">description</span><span class="sxs-lookup"><span data-stu-id="31d25-141">description</span></span>|<span data-ttu-id="31d25-142">String</span><span class="sxs-lookup"><span data-stu-id="31d25-142">String</span></span>|<span data-ttu-id="31d25-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="31d25-143">The description of the app.</span></span> <span data-ttu-id="31d25-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-145">publisher</span><span class="sxs-lookup"><span data-stu-id="31d25-145">publisher</span></span>|<span data-ttu-id="31d25-146">String</span><span class="sxs-lookup"><span data-stu-id="31d25-146">String</span></span>|<span data-ttu-id="31d25-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="31d25-147">The publisher of the app.</span></span> <span data-ttu-id="31d25-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="31d25-149">largeIcon</span></span>|[<span data-ttu-id="31d25-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="31d25-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="31d25-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="31d25-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="31d25-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31d25-153">createdDateTime</span></span>|<span data-ttu-id="31d25-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31d25-154">DateTimeOffset</span></span>|<span data-ttu-id="31d25-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="31d25-155">The date and time the app was created.</span></span> <span data-ttu-id="31d25-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31d25-157">lastModifiedDateTime</span></span>|<span data-ttu-id="31d25-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31d25-158">DateTimeOffset</span></span>|<span data-ttu-id="31d25-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="31d25-159">The date and time the app was last modified.</span></span> <span data-ttu-id="31d25-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="31d25-161">isFeatured</span></span>|<span data-ttu-id="31d25-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="31d25-162">Boolean</span></span>|<span data-ttu-id="31d25-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="31d25-164">privacyInformationUrl</span></span>|<span data-ttu-id="31d25-165">String</span><span class="sxs-lookup"><span data-stu-id="31d25-165">String</span></span>|<span data-ttu-id="31d25-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="31d25-166">The privacy statement Url.</span></span> <span data-ttu-id="31d25-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="31d25-168">informationUrl</span></span>|<span data-ttu-id="31d25-169">String</span><span class="sxs-lookup"><span data-stu-id="31d25-169">String</span></span>|<span data-ttu-id="31d25-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="31d25-170">The more information Url.</span></span> <span data-ttu-id="31d25-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-172">owner</span><span class="sxs-lookup"><span data-stu-id="31d25-172">owner</span></span>|<span data-ttu-id="31d25-173">String</span><span class="sxs-lookup"><span data-stu-id="31d25-173">String</span></span>|<span data-ttu-id="31d25-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="31d25-174">The owner of the app.</span></span> <span data-ttu-id="31d25-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-176">developer</span><span class="sxs-lookup"><span data-stu-id="31d25-176">developer</span></span>|<span data-ttu-id="31d25-177">String</span><span class="sxs-lookup"><span data-stu-id="31d25-177">String</span></span>|<span data-ttu-id="31d25-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="31d25-178">The developer of the app.</span></span> <span data-ttu-id="31d25-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-180">notes</span><span class="sxs-lookup"><span data-stu-id="31d25-180">notes</span></span>|<span data-ttu-id="31d25-181">String</span><span class="sxs-lookup"><span data-stu-id="31d25-181">String</span></span>|<span data-ttu-id="31d25-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="31d25-182">Notes for the app.</span></span> <span data-ttu-id="31d25-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="31d25-184">uploadState</span></span>|<span data-ttu-id="31d25-185">Int32</span><span class="sxs-lookup"><span data-stu-id="31d25-185">Int32</span></span>|<span data-ttu-id="31d25-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="31d25-186">The upload state.</span></span> <span data-ttu-id="31d25-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="31d25-188">publishingState</span></span>|[<span data-ttu-id="31d25-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="31d25-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="31d25-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="31d25-190">The publishing state for the app.</span></span> <span data-ttu-id="31d25-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="31d25-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="31d25-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="31d25-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="31d25-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="31d25-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="31d25-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="31d25-194">isAssigned</span></span>|<span data-ttu-id="31d25-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="31d25-195">Boolean</span></span>|<span data-ttu-id="31d25-196">值，指示是否将应用程序分配给至少一个组。</span><span class="sxs-lookup"><span data-stu-id="31d25-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="31d25-197">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="31d25-198">roleScopeTagIds</span></span>|<span data-ttu-id="31d25-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="31d25-199">String collection</span></span>|<span data-ttu-id="31d25-200">此移动应用程序的作用域标记 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="31d25-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="31d25-201">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31d25-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="31d25-202">committedContentVersion</span></span>|<span data-ttu-id="31d25-203">String</span><span class="sxs-lookup"><span data-stu-id="31d25-203">String</span></span>|<span data-ttu-id="31d25-204">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="31d25-204">The internal committed content version.</span></span> <span data-ttu-id="31d25-205">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="31d25-206">fileName</span><span class="sxs-lookup"><span data-stu-id="31d25-206">fileName</span></span>|<span data-ttu-id="31d25-207">String</span><span class="sxs-lookup"><span data-stu-id="31d25-207">String</span></span>|<span data-ttu-id="31d25-208">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="31d25-208">The name of the main Lob application file.</span></span> <span data-ttu-id="31d25-209">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="31d25-210">size</span><span class="sxs-lookup"><span data-stu-id="31d25-210">size</span></span>|<span data-ttu-id="31d25-211">Int64</span><span class="sxs-lookup"><span data-stu-id="31d25-211">Int64</span></span>|<span data-ttu-id="31d25-212">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="31d25-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="31d25-213">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="31d25-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="31d25-214">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="31d25-214">applicableArchitectures</span></span>|[<span data-ttu-id="31d25-215">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="31d25-215">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="31d25-216">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="31d25-216">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="31d25-217">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="31d25-217">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="31d25-218">identityName</span><span class="sxs-lookup"><span data-stu-id="31d25-218">identityName</span></span>|<span data-ttu-id="31d25-219">String</span><span class="sxs-lookup"><span data-stu-id="31d25-219">String</span></span>|<span data-ttu-id="31d25-220">标识名称。</span><span class="sxs-lookup"><span data-stu-id="31d25-220">The Identity Name.</span></span>|
|<span data-ttu-id="31d25-221">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="31d25-221">identityPublisherHash</span></span>|<span data-ttu-id="31d25-222">String</span><span class="sxs-lookup"><span data-stu-id="31d25-222">String</span></span>|<span data-ttu-id="31d25-223">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="31d25-223">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="31d25-224">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="31d25-224">identityResourceIdentifier</span></span>|<span data-ttu-id="31d25-225">String</span><span class="sxs-lookup"><span data-stu-id="31d25-225">String</span></span>|<span data-ttu-id="31d25-226">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="31d25-226">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="31d25-227">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="31d25-227">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="31d25-228">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="31d25-228">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="31d25-229">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="31d25-229">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="31d25-230">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="31d25-230">phoneProductIdentifier</span></span>|<span data-ttu-id="31d25-231">String</span><span class="sxs-lookup"><span data-stu-id="31d25-231">String</span></span>|<span data-ttu-id="31d25-232">电话产品标识符。</span><span class="sxs-lookup"><span data-stu-id="31d25-232">The Phone Product Identifier.</span></span>|
|<span data-ttu-id="31d25-233">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="31d25-233">phonePublisherId</span></span>|<span data-ttu-id="31d25-234">String</span><span class="sxs-lookup"><span data-stu-id="31d25-234">String</span></span>|<span data-ttu-id="31d25-235">电话 Publisher id。</span><span class="sxs-lookup"><span data-stu-id="31d25-235">The Phone Publisher Id.</span></span>|
|<span data-ttu-id="31d25-236">identityVersion</span><span class="sxs-lookup"><span data-stu-id="31d25-236">identityVersion</span></span>|<span data-ttu-id="31d25-237">String</span><span class="sxs-lookup"><span data-stu-id="31d25-237">String</span></span>|<span data-ttu-id="31d25-238">标识版本。</span><span class="sxs-lookup"><span data-stu-id="31d25-238">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="31d25-239">响应</span><span class="sxs-lookup"><span data-stu-id="31d25-239">Response</span></span>
<span data-ttu-id="31d25-240">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)对象。</span><span class="sxs-lookup"><span data-stu-id="31d25-240">If successful, this method returns a `201 Created` response code and a [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31d25-241">示例</span><span class="sxs-lookup"><span data-stu-id="31d25-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="31d25-242">请求</span><span class="sxs-lookup"><span data-stu-id="31d25-242">Request</span></span>
<span data-ttu-id="31d25-243">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="31d25-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1440

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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="31d25-244">响应</span><span class="sxs-lookup"><span data-stu-id="31d25-244">Response</span></span>
<span data-ttu-id="31d25-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="31d25-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1612

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
  "identityVersion": "Identity Version value"
}
```




