---
title: 更新 windowsPhone81AppXBundle
description: 更新 windowsPhone81AppXBundle 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4bb7f25653f8bf5516b1bdd38eb5b8afaafcefb9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393989"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="fe449-103">更新 windowsPhone81AppXBundle</span><span class="sxs-lookup"><span data-stu-id="fe449-103">Update windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="fe449-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="fe449-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fe449-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fe449-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe449-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fe449-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe449-107">更新[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fe449-107">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe449-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fe449-108">Prerequisites</span></span>
<span data-ttu-id="fe449-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fe449-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fe449-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe449-111">Permission type</span></span>|<span data-ttu-id="fe449-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fe449-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe449-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe449-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe449-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe449-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fe449-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe449-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe449-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe449-116">Not supported.</span></span>|
|<span data-ttu-id="fe449-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe449-117">Application</span></span>|<span data-ttu-id="fe449-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe449-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe449-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe449-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="fe449-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe449-120">Request headers</span></span>
|<span data-ttu-id="fe449-121">标头</span><span class="sxs-lookup"><span data-stu-id="fe449-121">Header</span></span>|<span data-ttu-id="fe449-122">值</span><span class="sxs-lookup"><span data-stu-id="fe449-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe449-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe449-123">Authorization</span></span>|<span data-ttu-id="fe449-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fe449-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe449-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe449-125">Accept</span></span>|<span data-ttu-id="fe449-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe449-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe449-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe449-127">Request body</span></span>
<span data-ttu-id="fe449-128">在请求正文中，提供[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe449-128">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="fe449-129">下表显示时创建[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fe449-129">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="fe449-130">属性</span><span class="sxs-lookup"><span data-stu-id="fe449-130">Property</span></span>|<span data-ttu-id="fe449-131">类型</span><span class="sxs-lookup"><span data-stu-id="fe449-131">Type</span></span>|<span data-ttu-id="fe449-132">说明</span><span class="sxs-lookup"><span data-stu-id="fe449-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe449-133">id</span><span class="sxs-lookup"><span data-stu-id="fe449-133">id</span></span>|<span data-ttu-id="fe449-134">String</span><span class="sxs-lookup"><span data-stu-id="fe449-134">String</span></span>|<span data-ttu-id="fe449-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fe449-135">Key of the entity.</span></span> <span data-ttu-id="fe449-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fe449-137">displayName</span></span>|<span data-ttu-id="fe449-138">String</span><span class="sxs-lookup"><span data-stu-id="fe449-138">String</span></span>|<span data-ttu-id="fe449-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="fe449-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fe449-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-141">description</span><span class="sxs-lookup"><span data-stu-id="fe449-141">description</span></span>|<span data-ttu-id="fe449-142">String</span><span class="sxs-lookup"><span data-stu-id="fe449-142">String</span></span>|<span data-ttu-id="fe449-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="fe449-143">The description of the app.</span></span> <span data-ttu-id="fe449-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-145">publisher</span><span class="sxs-lookup"><span data-stu-id="fe449-145">publisher</span></span>|<span data-ttu-id="fe449-146">String</span><span class="sxs-lookup"><span data-stu-id="fe449-146">String</span></span>|<span data-ttu-id="fe449-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="fe449-147">The publisher of the app.</span></span> <span data-ttu-id="fe449-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fe449-149">largeIcon</span></span>|[<span data-ttu-id="fe449-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fe449-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fe449-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="fe449-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fe449-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe449-153">createdDateTime</span></span>|<span data-ttu-id="fe449-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe449-154">DateTimeOffset</span></span>|<span data-ttu-id="fe449-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fe449-155">The date and time the app was created.</span></span> <span data-ttu-id="fe449-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe449-157">lastModifiedDateTime</span></span>|<span data-ttu-id="fe449-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe449-158">DateTimeOffset</span></span>|<span data-ttu-id="fe449-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fe449-159">The date and time the app was last modified.</span></span> <span data-ttu-id="fe449-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fe449-161">isFeatured</span></span>|<span data-ttu-id="fe449-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe449-162">Boolean</span></span>|<span data-ttu-id="fe449-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fe449-164">privacyInformationUrl</span></span>|<span data-ttu-id="fe449-165">String</span><span class="sxs-lookup"><span data-stu-id="fe449-165">String</span></span>|<span data-ttu-id="fe449-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="fe449-166">The privacy statement Url.</span></span> <span data-ttu-id="fe449-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fe449-168">informationUrl</span></span>|<span data-ttu-id="fe449-169">String</span><span class="sxs-lookup"><span data-stu-id="fe449-169">String</span></span>|<span data-ttu-id="fe449-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="fe449-170">The more information Url.</span></span> <span data-ttu-id="fe449-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-172">owner</span><span class="sxs-lookup"><span data-stu-id="fe449-172">owner</span></span>|<span data-ttu-id="fe449-173">String</span><span class="sxs-lookup"><span data-stu-id="fe449-173">String</span></span>|<span data-ttu-id="fe449-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="fe449-174">The owner of the app.</span></span> <span data-ttu-id="fe449-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-176">developer</span><span class="sxs-lookup"><span data-stu-id="fe449-176">developer</span></span>|<span data-ttu-id="fe449-177">String</span><span class="sxs-lookup"><span data-stu-id="fe449-177">String</span></span>|<span data-ttu-id="fe449-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="fe449-178">The developer of the app.</span></span> <span data-ttu-id="fe449-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-180">notes</span><span class="sxs-lookup"><span data-stu-id="fe449-180">notes</span></span>|<span data-ttu-id="fe449-181">String</span><span class="sxs-lookup"><span data-stu-id="fe449-181">String</span></span>|<span data-ttu-id="fe449-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="fe449-182">Notes for the app.</span></span> <span data-ttu-id="fe449-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="fe449-184">uploadState</span></span>|<span data-ttu-id="fe449-185">Int32</span><span class="sxs-lookup"><span data-stu-id="fe449-185">Int32</span></span>|<span data-ttu-id="fe449-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="fe449-186">The upload state.</span></span> <span data-ttu-id="fe449-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="fe449-188">publishingState</span></span>|[<span data-ttu-id="fe449-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fe449-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fe449-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="fe449-190">The publishing state for the app.</span></span> <span data-ttu-id="fe449-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="fe449-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fe449-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="fe449-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="fe449-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="fe449-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fe449-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="fe449-194">isAssigned</span></span>|<span data-ttu-id="fe449-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe449-195">Boolean</span></span>|<span data-ttu-id="fe449-196">值，指示是否将应用程序分配给至少一个组。</span><span class="sxs-lookup"><span data-stu-id="fe449-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="fe449-197">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fe449-198">roleScopeTagIds</span></span>|<span data-ttu-id="fe449-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="fe449-199">String collection</span></span>|<span data-ttu-id="fe449-200">此移动应用程序的作用域标记 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="fe449-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="fe449-201">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fe449-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="fe449-202">committedContentVersion</span></span>|<span data-ttu-id="fe449-203">String</span><span class="sxs-lookup"><span data-stu-id="fe449-203">String</span></span>|<span data-ttu-id="fe449-204">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="fe449-204">The internal committed content version.</span></span> <span data-ttu-id="fe449-205">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fe449-206">fileName</span><span class="sxs-lookup"><span data-stu-id="fe449-206">fileName</span></span>|<span data-ttu-id="fe449-207">String</span><span class="sxs-lookup"><span data-stu-id="fe449-207">String</span></span>|<span data-ttu-id="fe449-208">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="fe449-208">The name of the main Lob application file.</span></span> <span data-ttu-id="fe449-209">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fe449-210">size</span><span class="sxs-lookup"><span data-stu-id="fe449-210">size</span></span>|<span data-ttu-id="fe449-211">Int64</span><span class="sxs-lookup"><span data-stu-id="fe449-211">Int64</span></span>|<span data-ttu-id="fe449-212">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="fe449-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="fe449-213">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fe449-214">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="fe449-214">applicableArchitectures</span></span>|[<span data-ttu-id="fe449-215">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="fe449-215">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="fe449-216">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="fe449-216">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="fe449-217">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)。</span><span class="sxs-lookup"><span data-stu-id="fe449-217">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="fe449-218">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="fe449-218">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="fe449-219">identityName</span><span class="sxs-lookup"><span data-stu-id="fe449-219">identityName</span></span>|<span data-ttu-id="fe449-220">String</span><span class="sxs-lookup"><span data-stu-id="fe449-220">String</span></span>|<span data-ttu-id="fe449-221">标识名称。</span><span class="sxs-lookup"><span data-stu-id="fe449-221">The Identity Name.</span></span> <span data-ttu-id="fe449-222">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-222">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="fe449-223">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="fe449-223">identityPublisherHash</span></span>|<span data-ttu-id="fe449-224">String</span><span class="sxs-lookup"><span data-stu-id="fe449-224">String</span></span>|<span data-ttu-id="fe449-225">标识发布者哈希。</span><span class="sxs-lookup"><span data-stu-id="fe449-225">The Identity Publisher Hash.</span></span> <span data-ttu-id="fe449-226">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-226">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="fe449-227">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="fe449-227">identityResourceIdentifier</span></span>|<span data-ttu-id="fe449-228">String</span><span class="sxs-lookup"><span data-stu-id="fe449-228">String</span></span>|<span data-ttu-id="fe449-229">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="fe449-229">The Identity Resource Identifier.</span></span> <span data-ttu-id="fe449-230">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="fe449-231">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fe449-231">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="fe449-232">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fe449-232">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="fe449-233">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="fe449-233">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="fe449-234">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-234">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="fe449-235">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="fe449-235">phoneProductIdentifier</span></span>|<span data-ttu-id="fe449-236">String</span><span class="sxs-lookup"><span data-stu-id="fe449-236">String</span></span>|<span data-ttu-id="fe449-237">电话产品标识符。</span><span class="sxs-lookup"><span data-stu-id="fe449-237">The Phone Product Identifier.</span></span> <span data-ttu-id="fe449-238">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-238">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="fe449-239">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="fe449-239">phonePublisherId</span></span>|<span data-ttu-id="fe449-240">String</span><span class="sxs-lookup"><span data-stu-id="fe449-240">String</span></span>|<span data-ttu-id="fe449-241">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)电话 Publisher id。</span><span class="sxs-lookup"><span data-stu-id="fe449-241">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="fe449-242">identityVersion</span><span class="sxs-lookup"><span data-stu-id="fe449-242">identityVersion</span></span>|<span data-ttu-id="fe449-243">String</span><span class="sxs-lookup"><span data-stu-id="fe449-243">String</span></span>|<span data-ttu-id="fe449-244">标识版本。</span><span class="sxs-lookup"><span data-stu-id="fe449-244">The identity version.</span></span> <span data-ttu-id="fe449-245">继承自[windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span><span class="sxs-lookup"><span data-stu-id="fe449-245">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="fe449-246">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="fe449-246">appXPackageInformationList</span></span>|<span data-ttu-id="fe449-247">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)集合</span><span class="sxs-lookup"><span data-stu-id="fe449-247">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="fe449-248">约程序包信息的列表。</span><span class="sxs-lookup"><span data-stu-id="fe449-248">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="fe449-249">响应</span><span class="sxs-lookup"><span data-stu-id="fe449-249">Response</span></span>
<span data-ttu-id="fe449-250">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fe449-250">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe449-251">示例</span><span class="sxs-lookup"><span data-stu-id="fe449-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe449-252">请求</span><span class="sxs-lookup"><span data-stu-id="fe449-252">Request</span></span>
<span data-ttu-id="fe449-253">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fe449-253">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2184

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
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

### <a name="response"></a><span data-ttu-id="fe449-254">响应</span><span class="sxs-lookup"><span data-stu-id="fe449-254">Response</span></span>
<span data-ttu-id="fe449-p129">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fe449-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2356

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




