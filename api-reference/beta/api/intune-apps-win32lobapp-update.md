---
title: 更新 win32LobApp
description: 更新 win32LobApp 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 962059965abb2691ba1777518ad8aabc64adafe7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405336"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="f20c3-103">更新 win32LobApp</span><span class="sxs-lookup"><span data-stu-id="f20c3-103">Update win32LobApp</span></span>

> <span data-ttu-id="f20c3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f20c3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f20c3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f20c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f20c3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f20c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f20c3-107">更新[win32LobApp](../resources/intune-apps-win32lobapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f20c3-107">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f20c3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f20c3-108">Prerequisites</span></span>
<span data-ttu-id="f20c3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f20c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f20c3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f20c3-111">Permission type</span></span>|<span data-ttu-id="f20c3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f20c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f20c3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f20c3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f20c3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f20c3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f20c3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f20c3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f20c3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f20c3-116">Not supported.</span></span>|
|<span data-ttu-id="f20c3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f20c3-117">Application</span></span>|<span data-ttu-id="f20c3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f20c3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f20c3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f20c3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f20c3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f20c3-120">Request headers</span></span>
|<span data-ttu-id="f20c3-121">标头</span><span class="sxs-lookup"><span data-stu-id="f20c3-121">Header</span></span>|<span data-ttu-id="f20c3-122">值</span><span class="sxs-lookup"><span data-stu-id="f20c3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f20c3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f20c3-123">Authorization</span></span>|<span data-ttu-id="f20c3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f20c3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f20c3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f20c3-125">Accept</span></span>|<span data-ttu-id="f20c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f20c3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f20c3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f20c3-127">Request body</span></span>
<span data-ttu-id="f20c3-128">在请求正文中，提供[win32LobApp](../resources/intune-apps-win32lobapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f20c3-128">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="f20c3-129">下表显示时创建[win32LobApp](../resources/intune-apps-win32lobapp.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f20c3-129">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="f20c3-130">属性</span><span class="sxs-lookup"><span data-stu-id="f20c3-130">Property</span></span>|<span data-ttu-id="f20c3-131">类型</span><span class="sxs-lookup"><span data-stu-id="f20c3-131">Type</span></span>|<span data-ttu-id="f20c3-132">说明</span><span class="sxs-lookup"><span data-stu-id="f20c3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f20c3-133">id</span><span class="sxs-lookup"><span data-stu-id="f20c3-133">id</span></span>|<span data-ttu-id="f20c3-134">String</span><span class="sxs-lookup"><span data-stu-id="f20c3-134">String</span></span>|<span data-ttu-id="f20c3-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f20c3-135">Key of the entity.</span></span> <span data-ttu-id="f20c3-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f20c3-137">displayName</span></span>|<span data-ttu-id="f20c3-138">String</span><span class="sxs-lookup"><span data-stu-id="f20c3-138">String</span></span>|<span data-ttu-id="f20c3-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="f20c3-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f20c3-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-141">description</span><span class="sxs-lookup"><span data-stu-id="f20c3-141">description</span></span>|<span data-ttu-id="f20c3-142">String</span><span class="sxs-lookup"><span data-stu-id="f20c3-142">String</span></span>|<span data-ttu-id="f20c3-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="f20c3-143">The description of the app.</span></span> <span data-ttu-id="f20c3-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f20c3-145">publisher</span></span>|<span data-ttu-id="f20c3-146">String</span><span class="sxs-lookup"><span data-stu-id="f20c3-146">String</span></span>|<span data-ttu-id="f20c3-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="f20c3-147">The publisher of the app.</span></span> <span data-ttu-id="f20c3-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f20c3-149">largeIcon</span></span>|[<span data-ttu-id="f20c3-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f20c3-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f20c3-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="f20c3-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f20c3-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f20c3-153">createdDateTime</span></span>|<span data-ttu-id="f20c3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f20c3-154">DateTimeOffset</span></span>|<span data-ttu-id="f20c3-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f20c3-155">The date and time the app was created.</span></span> <span data-ttu-id="f20c3-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f20c3-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f20c3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f20c3-158">DateTimeOffset</span></span>|<span data-ttu-id="f20c3-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f20c3-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f20c3-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f20c3-161">isFeatured</span></span>|<span data-ttu-id="f20c3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f20c3-162">Boolean</span></span>|<span data-ttu-id="f20c3-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f20c3-164">privacyInformationUrl</span></span>|<span data-ttu-id="f20c3-165">String</span><span class="sxs-lookup"><span data-stu-id="f20c3-165">String</span></span>|<span data-ttu-id="f20c3-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="f20c3-166">The privacy statement Url.</span></span> <span data-ttu-id="f20c3-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f20c3-168">informationUrl</span></span>|<span data-ttu-id="f20c3-169">String</span><span class="sxs-lookup"><span data-stu-id="f20c3-169">String</span></span>|<span data-ttu-id="f20c3-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="f20c3-170">The more information Url.</span></span> <span data-ttu-id="f20c3-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-172">owner</span><span class="sxs-lookup"><span data-stu-id="f20c3-172">owner</span></span>|<span data-ttu-id="f20c3-173">String</span><span class="sxs-lookup"><span data-stu-id="f20c3-173">String</span></span>|<span data-ttu-id="f20c3-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="f20c3-174">The owner of the app.</span></span> <span data-ttu-id="f20c3-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-176">developer</span><span class="sxs-lookup"><span data-stu-id="f20c3-176">developer</span></span>|<span data-ttu-id="f20c3-177">String</span><span class="sxs-lookup"><span data-stu-id="f20c3-177">String</span></span>|<span data-ttu-id="f20c3-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="f20c3-178">The developer of the app.</span></span> <span data-ttu-id="f20c3-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-180">notes</span><span class="sxs-lookup"><span data-stu-id="f20c3-180">notes</span></span>|<span data-ttu-id="f20c3-181">String</span><span class="sxs-lookup"><span data-stu-id="f20c3-181">String</span></span>|<span data-ttu-id="f20c3-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="f20c3-182">Notes for the app.</span></span> <span data-ttu-id="f20c3-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f20c3-184">uploadState</span></span>|<span data-ttu-id="f20c3-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f20c3-185">Int32</span></span>|<span data-ttu-id="f20c3-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="f20c3-186">The upload state.</span></span> <span data-ttu-id="f20c3-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="f20c3-188">publishingState</span></span>|[<span data-ttu-id="f20c3-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f20c3-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f20c3-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="f20c3-190">The publishing state for the app.</span></span> <span data-ttu-id="f20c3-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="f20c3-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f20c3-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="f20c3-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f20c3-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="f20c3-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f20c3-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f20c3-194">isAssigned</span></span>|<span data-ttu-id="f20c3-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="f20c3-195">Boolean</span></span>|<span data-ttu-id="f20c3-196">值，指示是否将应用程序分配给至少一个组。</span><span class="sxs-lookup"><span data-stu-id="f20c3-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f20c3-197">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f20c3-198">roleScopeTagIds</span></span>|<span data-ttu-id="f20c3-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="f20c3-199">String collection</span></span>|<span data-ttu-id="f20c3-200">此移动应用程序的作用域标记 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="f20c3-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f20c3-201">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c3-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f20c3-202">committedContentVersion</span></span>|<span data-ttu-id="f20c3-203">String</span><span class="sxs-lookup"><span data-stu-id="f20c3-203">String</span></span>|<span data-ttu-id="f20c3-204">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="f20c3-204">The internal committed content version.</span></span> <span data-ttu-id="f20c3-205">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f20c3-206">fileName</span><span class="sxs-lookup"><span data-stu-id="f20c3-206">fileName</span></span>|<span data-ttu-id="f20c3-207">String</span><span class="sxs-lookup"><span data-stu-id="f20c3-207">String</span></span>|<span data-ttu-id="f20c3-208">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="f20c3-208">The name of the main Lob application file.</span></span> <span data-ttu-id="f20c3-209">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f20c3-210">size</span><span class="sxs-lookup"><span data-stu-id="f20c3-210">size</span></span>|<span data-ttu-id="f20c3-211">Int64</span><span class="sxs-lookup"><span data-stu-id="f20c3-211">Int64</span></span>|<span data-ttu-id="f20c3-212">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="f20c3-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="f20c3-213">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f20c3-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f20c3-214">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="f20c3-214">installCommandLine</span></span>|<span data-ttu-id="f20c3-215">String</span><span class="sxs-lookup"><span data-stu-id="f20c3-215">String</span></span>|<span data-ttu-id="f20c3-216">命令行安装此应用程序</span><span class="sxs-lookup"><span data-stu-id="f20c3-216">The command line to install this app</span></span>|
|<span data-ttu-id="f20c3-217">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="f20c3-217">uninstallCommandLine</span></span>|<span data-ttu-id="f20c3-218">String</span><span class="sxs-lookup"><span data-stu-id="f20c3-218">String</span></span>|<span data-ttu-id="f20c3-219">命令行来卸载此应用程序</span><span class="sxs-lookup"><span data-stu-id="f20c3-219">The command line to uninstall this app</span></span>|
|<span data-ttu-id="f20c3-220">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="f20c3-220">applicableArchitectures</span></span>|[<span data-ttu-id="f20c3-221">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="f20c3-221">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="f20c3-222">可运行此应用的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="f20c3-222">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="f20c3-223">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="f20c3-223">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="f20c3-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f20c3-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f20c3-225">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f20c3-225">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="f20c3-226">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="f20c3-226">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f20c3-227">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="f20c3-227">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="f20c3-228">Int32</span><span class="sxs-lookup"><span data-stu-id="f20c3-228">Int32</span></span>|<span data-ttu-id="f20c3-229">所需安装此应用程序的最小可用磁盘空间的值。</span><span class="sxs-lookup"><span data-stu-id="f20c3-229">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="f20c3-230">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="f20c3-230">minimumMemoryInMB</span></span>|<span data-ttu-id="f20c3-231">Int32</span><span class="sxs-lookup"><span data-stu-id="f20c3-231">Int32</span></span>|<span data-ttu-id="f20c3-232">安装此应用程序所需的最低物理内存值。</span><span class="sxs-lookup"><span data-stu-id="f20c3-232">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="f20c3-233">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="f20c3-233">minimumNumberOfProcessors</span></span>|<span data-ttu-id="f20c3-234">Int32</span><span class="sxs-lookup"><span data-stu-id="f20c3-234">Int32</span></span>|<span data-ttu-id="f20c3-235">最小处理器的数量需安装此应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="f20c3-235">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="f20c3-236">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="f20c3-236">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="f20c3-237">Int32</span><span class="sxs-lookup"><span data-stu-id="f20c3-237">Int32</span></span>|<span data-ttu-id="f20c3-238">最小的 CPU 速度，需安装此应用程序的值。</span><span class="sxs-lookup"><span data-stu-id="f20c3-238">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="f20c3-239">detectionRules</span><span class="sxs-lookup"><span data-stu-id="f20c3-239">detectionRules</span></span>|<span data-ttu-id="f20c3-240">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)集合</span><span class="sxs-lookup"><span data-stu-id="f20c3-240">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="f20c3-241">若要检测 Win32 业务线 (LoB) 应用程序检测规则。</span><span class="sxs-lookup"><span data-stu-id="f20c3-241">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f20c3-242">installExperience</span><span class="sxs-lookup"><span data-stu-id="f20c3-242">installExperience</span></span>|[<span data-ttu-id="f20c3-243">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="f20c3-243">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="f20c3-244">此应用程序安装体验。</span><span class="sxs-lookup"><span data-stu-id="f20c3-244">The install experience for this app.</span></span>|
|<span data-ttu-id="f20c3-245">returnCodes</span><span class="sxs-lookup"><span data-stu-id="f20c3-245">returnCodes</span></span>|<span data-ttu-id="f20c3-246">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)集合</span><span class="sxs-lookup"><span data-stu-id="f20c3-246">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="f20c3-247">开机自检安装行为返回代码。</span><span class="sxs-lookup"><span data-stu-id="f20c3-247">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="f20c3-248">msiInformation</span><span class="sxs-lookup"><span data-stu-id="f20c3-248">msiInformation</span></span>|[<span data-ttu-id="f20c3-249">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="f20c3-249">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="f20c3-250">MSI 详细信息此 Win32 应用程序是否 MSI 应用程序。</span><span class="sxs-lookup"><span data-stu-id="f20c3-250">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="f20c3-251">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="f20c3-251">setupFilePath</span></span>|<span data-ttu-id="f20c3-252">String</span><span class="sxs-lookup"><span data-stu-id="f20c3-252">String</span></span>|<span data-ttu-id="f20c3-253">加密 Win32LobApp 包中的安装程序文件的相对路径。</span><span class="sxs-lookup"><span data-stu-id="f20c3-253">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="f20c3-254">响应</span><span class="sxs-lookup"><span data-stu-id="f20c3-254">Response</span></span>
<span data-ttu-id="f20c3-255">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[win32LobApp](../resources/intune-apps-win32lobapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f20c3-255">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f20c3-256">示例</span><span class="sxs-lookup"><span data-stu-id="f20c3-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="f20c3-257">请求</span><span class="sxs-lookup"><span data-stu-id="f20c3-257">Request</span></span>
<span data-ttu-id="f20c3-258">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f20c3-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2285

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser"
  },
  "setupFilePath": "Setup File Path value"
}
```

### <a name="response"></a><span data-ttu-id="f20c3-259">响应</span><span class="sxs-lookup"><span data-stu-id="f20c3-259">Response</span></span>
<span data-ttu-id="f20c3-p123">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f20c3-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2457

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser"
  },
  "setupFilePath": "Setup File Path value"
}
```




