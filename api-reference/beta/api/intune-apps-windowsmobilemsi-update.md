---
title: 更新 windowsMobileMSI
description: 更新 windowsMobileMSI 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4c1683bff6d0212deff060193aa624f56143246e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409095"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="b5fdd-103">更新 windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="b5fdd-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="b5fdd-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b5fdd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5fdd-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5fdd-107">更新 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-107">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5fdd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b5fdd-108">Prerequisites</span></span>
<span data-ttu-id="b5fdd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b5fdd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5fdd-111">Permission type</span></span>|<span data-ttu-id="b5fdd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b5fdd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5fdd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5fdd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5fdd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5fdd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b5fdd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5fdd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5fdd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-116">Not supported.</span></span>|
|<span data-ttu-id="b5fdd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5fdd-117">Application</span></span>|<span data-ttu-id="b5fdd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5fdd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5fdd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="b5fdd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5fdd-120">Request headers</span></span>
|<span data-ttu-id="b5fdd-121">标头</span><span class="sxs-lookup"><span data-stu-id="b5fdd-121">Header</span></span>|<span data-ttu-id="b5fdd-122">值</span><span class="sxs-lookup"><span data-stu-id="b5fdd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5fdd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5fdd-123">Authorization</span></span>|<span data-ttu-id="b5fdd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5fdd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b5fdd-125">Accept</span></span>|<span data-ttu-id="b5fdd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5fdd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5fdd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5fdd-127">Request body</span></span>
<span data-ttu-id="b5fdd-128">在请求正文中，提供 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-128">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="b5fdd-129">下表显示创建 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-129">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="b5fdd-130">属性</span><span class="sxs-lookup"><span data-stu-id="b5fdd-130">Property</span></span>|<span data-ttu-id="b5fdd-131">类型</span><span class="sxs-lookup"><span data-stu-id="b5fdd-131">Type</span></span>|<span data-ttu-id="b5fdd-132">说明</span><span class="sxs-lookup"><span data-stu-id="b5fdd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5fdd-133">id</span><span class="sxs-lookup"><span data-stu-id="b5fdd-133">id</span></span>|<span data-ttu-id="b5fdd-134">String</span><span class="sxs-lookup"><span data-stu-id="b5fdd-134">String</span></span>|<span data-ttu-id="b5fdd-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-135">Key of the entity.</span></span> <span data-ttu-id="b5fdd-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b5fdd-137">displayName</span></span>|<span data-ttu-id="b5fdd-138">String</span><span class="sxs-lookup"><span data-stu-id="b5fdd-138">String</span></span>|<span data-ttu-id="b5fdd-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b5fdd-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-141">description</span><span class="sxs-lookup"><span data-stu-id="b5fdd-141">description</span></span>|<span data-ttu-id="b5fdd-142">String</span><span class="sxs-lookup"><span data-stu-id="b5fdd-142">String</span></span>|<span data-ttu-id="b5fdd-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-143">The description of the app.</span></span> <span data-ttu-id="b5fdd-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-145">publisher</span><span class="sxs-lookup"><span data-stu-id="b5fdd-145">publisher</span></span>|<span data-ttu-id="b5fdd-146">String</span><span class="sxs-lookup"><span data-stu-id="b5fdd-146">String</span></span>|<span data-ttu-id="b5fdd-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-147">The publisher of the app.</span></span> <span data-ttu-id="b5fdd-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b5fdd-149">largeIcon</span></span>|[<span data-ttu-id="b5fdd-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b5fdd-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b5fdd-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b5fdd-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5fdd-153">createdDateTime</span></span>|<span data-ttu-id="b5fdd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5fdd-154">DateTimeOffset</span></span>|<span data-ttu-id="b5fdd-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-155">The date and time the app was created.</span></span> <span data-ttu-id="b5fdd-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5fdd-157">lastModifiedDateTime</span></span>|<span data-ttu-id="b5fdd-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5fdd-158">DateTimeOffset</span></span>|<span data-ttu-id="b5fdd-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-159">The date and time the app was last modified.</span></span> <span data-ttu-id="b5fdd-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b5fdd-161">isFeatured</span></span>|<span data-ttu-id="b5fdd-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5fdd-162">Boolean</span></span>|<span data-ttu-id="b5fdd-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b5fdd-164">privacyInformationUrl</span></span>|<span data-ttu-id="b5fdd-165">String</span><span class="sxs-lookup"><span data-stu-id="b5fdd-165">String</span></span>|<span data-ttu-id="b5fdd-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-166">The privacy statement Url.</span></span> <span data-ttu-id="b5fdd-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b5fdd-168">informationUrl</span></span>|<span data-ttu-id="b5fdd-169">String</span><span class="sxs-lookup"><span data-stu-id="b5fdd-169">String</span></span>|<span data-ttu-id="b5fdd-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-170">The more information Url.</span></span> <span data-ttu-id="b5fdd-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-172">owner</span><span class="sxs-lookup"><span data-stu-id="b5fdd-172">owner</span></span>|<span data-ttu-id="b5fdd-173">String</span><span class="sxs-lookup"><span data-stu-id="b5fdd-173">String</span></span>|<span data-ttu-id="b5fdd-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-174">The owner of the app.</span></span> <span data-ttu-id="b5fdd-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-176">developer</span><span class="sxs-lookup"><span data-stu-id="b5fdd-176">developer</span></span>|<span data-ttu-id="b5fdd-177">String</span><span class="sxs-lookup"><span data-stu-id="b5fdd-177">String</span></span>|<span data-ttu-id="b5fdd-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-178">The developer of the app.</span></span> <span data-ttu-id="b5fdd-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-180">notes</span><span class="sxs-lookup"><span data-stu-id="b5fdd-180">notes</span></span>|<span data-ttu-id="b5fdd-181">String</span><span class="sxs-lookup"><span data-stu-id="b5fdd-181">String</span></span>|<span data-ttu-id="b5fdd-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-182">Notes for the app.</span></span> <span data-ttu-id="b5fdd-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="b5fdd-184">uploadState</span></span>|<span data-ttu-id="b5fdd-185">Int32</span><span class="sxs-lookup"><span data-stu-id="b5fdd-185">Int32</span></span>|<span data-ttu-id="b5fdd-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-186">The upload state.</span></span> <span data-ttu-id="b5fdd-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="b5fdd-188">publishingState</span></span>|[<span data-ttu-id="b5fdd-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b5fdd-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b5fdd-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-190">The publishing state for the app.</span></span> <span data-ttu-id="b5fdd-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b5fdd-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b5fdd-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b5fdd-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b5fdd-194">isAssigned</span></span>|<span data-ttu-id="b5fdd-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5fdd-195">Boolean</span></span>|<span data-ttu-id="b5fdd-196">值，指示是否将应用程序分配给至少一个组。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b5fdd-197">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b5fdd-198">roleScopeTagIds</span></span>|<span data-ttu-id="b5fdd-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="b5fdd-199">String collection</span></span>|<span data-ttu-id="b5fdd-200">此移动应用程序的作用域标记 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b5fdd-201">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b5fdd-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b5fdd-202">committedContentVersion</span></span>|<span data-ttu-id="b5fdd-203">String</span><span class="sxs-lookup"><span data-stu-id="b5fdd-203">String</span></span>|<span data-ttu-id="b5fdd-204">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-204">The internal committed content version.</span></span> <span data-ttu-id="b5fdd-205">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b5fdd-206">fileName</span><span class="sxs-lookup"><span data-stu-id="b5fdd-206">fileName</span></span>|<span data-ttu-id="b5fdd-207">String</span><span class="sxs-lookup"><span data-stu-id="b5fdd-207">String</span></span>|<span data-ttu-id="b5fdd-208">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-208">The name of the main Lob application file.</span></span> <span data-ttu-id="b5fdd-209">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b5fdd-210">size</span><span class="sxs-lookup"><span data-stu-id="b5fdd-210">size</span></span>|<span data-ttu-id="b5fdd-211">Int64</span><span class="sxs-lookup"><span data-stu-id="b5fdd-211">Int64</span></span>|<span data-ttu-id="b5fdd-212">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="b5fdd-213">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b5fdd-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="b5fdd-214">commandLine</span><span class="sxs-lookup"><span data-stu-id="b5fdd-214">commandLine</span></span>|<span data-ttu-id="b5fdd-215">String</span><span class="sxs-lookup"><span data-stu-id="b5fdd-215">String</span></span>|<span data-ttu-id="b5fdd-216">命令行。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-216">The command line.</span></span>|
|<span data-ttu-id="b5fdd-217">productCode</span><span class="sxs-lookup"><span data-stu-id="b5fdd-217">productCode</span></span>|<span data-ttu-id="b5fdd-218">String</span><span class="sxs-lookup"><span data-stu-id="b5fdd-218">String</span></span>|<span data-ttu-id="b5fdd-219">产品代码。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-219">The product code.</span></span>|
|<span data-ttu-id="b5fdd-220">productVersion</span><span class="sxs-lookup"><span data-stu-id="b5fdd-220">productVersion</span></span>|<span data-ttu-id="b5fdd-221">String</span><span class="sxs-lookup"><span data-stu-id="b5fdd-221">String</span></span>|<span data-ttu-id="b5fdd-222">Windows Mobile MSI 业务线 (LoB) 应用的产品版本。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-222">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b5fdd-223">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="b5fdd-223">ignoreVersionDetection</span></span>|<span data-ttu-id="b5fdd-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5fdd-224">Boolean</span></span>|<span data-ttu-id="b5fdd-225">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-225">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="b5fdd-226">对于使用自更新功能的 Windows Mobile MSI 业务线 (LoB) 应用，将此值设置为 true。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-226">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="b5fdd-227">identityVersion</span><span class="sxs-lookup"><span data-stu-id="b5fdd-227">identityVersion</span></span>|<span data-ttu-id="b5fdd-228">String</span><span class="sxs-lookup"><span data-stu-id="b5fdd-228">String</span></span>|<span data-ttu-id="b5fdd-229">标识版本。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-229">The identity version.</span></span>|
|<span data-ttu-id="b5fdd-230">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="b5fdd-230">useDeviceContext</span></span>|<span data-ttu-id="b5fdd-231">布尔值</span><span class="sxs-lookup"><span data-stu-id="b5fdd-231">Boolean</span></span>|<span data-ttu-id="b5fdd-232">指示是否双模式 MSI 安装设备上下文中。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-232">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="b5fdd-233">如果为 true，则将为所有用户安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-233">If true, app will be installed for all users.</span></span> <span data-ttu-id="b5fdd-234">如果为 false，应用程序将安装的每个用户。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-234">If false, app will be installed per-user.</span></span> <span data-ttu-id="b5fdd-235">如果为空，服务将使用 MSI 数据包的默认安装上下文。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-235">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="b5fdd-236">双模式 MSI 时此默认值将为每个用户。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-236">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="b5fdd-237">不能设置为非双协议模式应用程序。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-237">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="b5fdd-238">不能更改首次创建的应用程序后。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-238">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="b5fdd-239">响应</span><span class="sxs-lookup"><span data-stu-id="b5fdd-239">Response</span></span>
<span data-ttu-id="b5fdd-240">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-240">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5fdd-241">示例</span><span class="sxs-lookup"><span data-stu-id="b5fdd-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5fdd-242">请求</span><span class="sxs-lookup"><span data-stu-id="b5fdd-242">Request</span></span>
<span data-ttu-id="b5fdd-243">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1039

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="b5fdd-244">响应</span><span class="sxs-lookup"><span data-stu-id="b5fdd-244">Response</span></span>
<span data-ttu-id="b5fdd-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5fdd-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1211

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```




