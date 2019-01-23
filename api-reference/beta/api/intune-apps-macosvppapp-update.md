---
title: 更新 macOsVppApp
description: 更新 macOsVppApp 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b34a8e4ae3e179cfa8674abb08565b5fbe0c72a3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431367"
---
# <a name="update-macosvppapp"></a><span data-ttu-id="48b3a-103">更新 macOsVppApp</span><span class="sxs-lookup"><span data-stu-id="48b3a-103">Update macOsVppApp</span></span>

> <span data-ttu-id="48b3a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="48b3a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="48b3a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="48b3a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48b3a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="48b3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48b3a-107">更新[macOsVppApp](../resources/intune-apps-macosvppapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="48b3a-107">Update the properties of a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48b3a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="48b3a-108">Prerequisites</span></span>
<span data-ttu-id="48b3a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="48b3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="48b3a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="48b3a-111">Permission type</span></span>|<span data-ttu-id="48b3a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="48b3a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48b3a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48b3a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48b3a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48b3a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="48b3a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48b3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48b3a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="48b3a-116">Not supported.</span></span>|
|<span data-ttu-id="48b3a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="48b3a-117">Application</span></span>|<span data-ttu-id="48b3a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="48b3a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48b3a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48b3a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="48b3a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="48b3a-120">Request headers</span></span>
|<span data-ttu-id="48b3a-121">标头</span><span class="sxs-lookup"><span data-stu-id="48b3a-121">Header</span></span>|<span data-ttu-id="48b3a-122">值</span><span class="sxs-lookup"><span data-stu-id="48b3a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48b3a-123">授权</span><span class="sxs-lookup"><span data-stu-id="48b3a-123">Authorization</span></span>|<span data-ttu-id="48b3a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="48b3a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48b3a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="48b3a-125">Accept</span></span>|<span data-ttu-id="48b3a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48b3a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48b3a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="48b3a-127">Request body</span></span>
<span data-ttu-id="48b3a-128">在请求正文中，提供[macOsVppApp](../resources/intune-apps-macosvppapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48b3a-128">In the request body, supply a JSON representation for the [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

<span data-ttu-id="48b3a-129">下表显示时创建[macOsVppApp](../resources/intune-apps-macosvppapp.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="48b3a-129">The following table shows the properties that are required when you create the [macOsVppApp](../resources/intune-apps-macosvppapp.md).</span></span>

|<span data-ttu-id="48b3a-130">属性</span><span class="sxs-lookup"><span data-stu-id="48b3a-130">Property</span></span>|<span data-ttu-id="48b3a-131">类型</span><span class="sxs-lookup"><span data-stu-id="48b3a-131">Type</span></span>|<span data-ttu-id="48b3a-132">说明</span><span class="sxs-lookup"><span data-stu-id="48b3a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48b3a-133">id</span><span class="sxs-lookup"><span data-stu-id="48b3a-133">id</span></span>|<span data-ttu-id="48b3a-134">String</span><span class="sxs-lookup"><span data-stu-id="48b3a-134">String</span></span>|<span data-ttu-id="48b3a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="48b3a-135">Key of the entity.</span></span> <span data-ttu-id="48b3a-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="48b3a-137">displayName</span></span>|<span data-ttu-id="48b3a-138">String</span><span class="sxs-lookup"><span data-stu-id="48b3a-138">String</span></span>|<span data-ttu-id="48b3a-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="48b3a-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="48b3a-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-141">description</span><span class="sxs-lookup"><span data-stu-id="48b3a-141">description</span></span>|<span data-ttu-id="48b3a-142">String</span><span class="sxs-lookup"><span data-stu-id="48b3a-142">String</span></span>|<span data-ttu-id="48b3a-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="48b3a-143">The description of the app.</span></span> <span data-ttu-id="48b3a-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-145">publisher</span><span class="sxs-lookup"><span data-stu-id="48b3a-145">publisher</span></span>|<span data-ttu-id="48b3a-146">String</span><span class="sxs-lookup"><span data-stu-id="48b3a-146">String</span></span>|<span data-ttu-id="48b3a-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="48b3a-147">The publisher of the app.</span></span> <span data-ttu-id="48b3a-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="48b3a-149">largeIcon</span></span>|[<span data-ttu-id="48b3a-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="48b3a-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="48b3a-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="48b3a-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="48b3a-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="48b3a-153">createdDateTime</span></span>|<span data-ttu-id="48b3a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48b3a-154">DateTimeOffset</span></span>|<span data-ttu-id="48b3a-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="48b3a-155">The date and time the app was created.</span></span> <span data-ttu-id="48b3a-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48b3a-157">lastModifiedDateTime</span></span>|<span data-ttu-id="48b3a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48b3a-158">DateTimeOffset</span></span>|<span data-ttu-id="48b3a-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="48b3a-159">The date and time the app was last modified.</span></span> <span data-ttu-id="48b3a-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="48b3a-161">isFeatured</span></span>|<span data-ttu-id="48b3a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="48b3a-162">Boolean</span></span>|<span data-ttu-id="48b3a-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="48b3a-164">privacyInformationUrl</span></span>|<span data-ttu-id="48b3a-165">String</span><span class="sxs-lookup"><span data-stu-id="48b3a-165">String</span></span>|<span data-ttu-id="48b3a-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="48b3a-166">The privacy statement Url.</span></span> <span data-ttu-id="48b3a-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="48b3a-168">informationUrl</span></span>|<span data-ttu-id="48b3a-169">String</span><span class="sxs-lookup"><span data-stu-id="48b3a-169">String</span></span>|<span data-ttu-id="48b3a-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="48b3a-170">The more information Url.</span></span> <span data-ttu-id="48b3a-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-172">owner</span><span class="sxs-lookup"><span data-stu-id="48b3a-172">owner</span></span>|<span data-ttu-id="48b3a-173">String</span><span class="sxs-lookup"><span data-stu-id="48b3a-173">String</span></span>|<span data-ttu-id="48b3a-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="48b3a-174">The owner of the app.</span></span> <span data-ttu-id="48b3a-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-176">developer</span><span class="sxs-lookup"><span data-stu-id="48b3a-176">developer</span></span>|<span data-ttu-id="48b3a-177">String</span><span class="sxs-lookup"><span data-stu-id="48b3a-177">String</span></span>|<span data-ttu-id="48b3a-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="48b3a-178">The developer of the app.</span></span> <span data-ttu-id="48b3a-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-180">notes</span><span class="sxs-lookup"><span data-stu-id="48b3a-180">notes</span></span>|<span data-ttu-id="48b3a-181">String</span><span class="sxs-lookup"><span data-stu-id="48b3a-181">String</span></span>|<span data-ttu-id="48b3a-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="48b3a-182">Notes for the app.</span></span> <span data-ttu-id="48b3a-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="48b3a-184">uploadState</span></span>|<span data-ttu-id="48b3a-185">Int32</span><span class="sxs-lookup"><span data-stu-id="48b3a-185">Int32</span></span>|<span data-ttu-id="48b3a-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="48b3a-186">The upload state.</span></span> <span data-ttu-id="48b3a-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="48b3a-188">publishingState</span></span>|[<span data-ttu-id="48b3a-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="48b3a-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="48b3a-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="48b3a-190">The publishing state for the app.</span></span> <span data-ttu-id="48b3a-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="48b3a-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="48b3a-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="48b3a-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="48b3a-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="48b3a-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="48b3a-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="48b3a-194">isAssigned</span></span>|<span data-ttu-id="48b3a-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="48b3a-195">Boolean</span></span>|<span data-ttu-id="48b3a-196">值，指示是否将应用程序分配给至少一个组。</span><span class="sxs-lookup"><span data-stu-id="48b3a-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="48b3a-197">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="48b3a-198">roleScopeTagIds</span></span>|<span data-ttu-id="48b3a-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="48b3a-199">String collection</span></span>|<span data-ttu-id="48b3a-200">此移动应用程序的作用域标记 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="48b3a-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="48b3a-201">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="48b3a-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="48b3a-202">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="48b3a-202">usedLicenseCount</span></span>|<span data-ttu-id="48b3a-203">Int32</span><span class="sxs-lookup"><span data-stu-id="48b3a-203">Int32</span></span>|<span data-ttu-id="48b3a-204">使用中的 VPP 许可证数量。</span><span class="sxs-lookup"><span data-stu-id="48b3a-204">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="48b3a-205">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="48b3a-205">totalLicenseCount</span></span>|<span data-ttu-id="48b3a-206">Int32</span><span class="sxs-lookup"><span data-stu-id="48b3a-206">Int32</span></span>|<span data-ttu-id="48b3a-207">VPP 许可证的总数。</span><span class="sxs-lookup"><span data-stu-id="48b3a-207">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="48b3a-208">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="48b3a-208">releaseDateTime</span></span>|<span data-ttu-id="48b3a-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48b3a-209">DateTimeOffset</span></span>|<span data-ttu-id="48b3a-210">VPP 应用程序的发布日期和时间。</span><span class="sxs-lookup"><span data-stu-id="48b3a-210">The VPP application release date and time.</span></span>|
|<span data-ttu-id="48b3a-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="48b3a-211">appStoreUrl</span></span>|<span data-ttu-id="48b3a-212">String</span><span class="sxs-lookup"><span data-stu-id="48b3a-212">String</span></span>|<span data-ttu-id="48b3a-213">存储 URL。</span><span class="sxs-lookup"><span data-stu-id="48b3a-213">The store URL.</span></span>|
|<span data-ttu-id="48b3a-214">licensingType</span><span class="sxs-lookup"><span data-stu-id="48b3a-214">licensingType</span></span>|[<span data-ttu-id="48b3a-215">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="48b3a-215">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="48b3a-216">受支持的许可证类型。</span><span class="sxs-lookup"><span data-stu-id="48b3a-216">The supported License Type.</span></span>|
|<span data-ttu-id="48b3a-217">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="48b3a-217">vppTokenOrganizationName</span></span>|<span data-ttu-id="48b3a-218">String</span><span class="sxs-lookup"><span data-stu-id="48b3a-218">String</span></span>|<span data-ttu-id="48b3a-219">与 Apple Volume Purchase Program 令牌关联的组织</span><span class="sxs-lookup"><span data-stu-id="48b3a-219">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="48b3a-220">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="48b3a-220">vppTokenAccountType</span></span>|[<span data-ttu-id="48b3a-221">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="48b3a-221">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="48b3a-222">与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。</span><span class="sxs-lookup"><span data-stu-id="48b3a-222">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="48b3a-223">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="48b3a-223">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="48b3a-224">可取值为：`business`、`education`。</span><span class="sxs-lookup"><span data-stu-id="48b3a-224">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="48b3a-225">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="48b3a-225">vppTokenAppleId</span></span>|<span data-ttu-id="48b3a-226">String</span><span class="sxs-lookup"><span data-stu-id="48b3a-226">String</span></span>|<span data-ttu-id="48b3a-227">与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。</span><span class="sxs-lookup"><span data-stu-id="48b3a-227">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="48b3a-228">bundleId</span><span class="sxs-lookup"><span data-stu-id="48b3a-228">bundleId</span></span>|<span data-ttu-id="48b3a-229">String</span><span class="sxs-lookup"><span data-stu-id="48b3a-229">String</span></span>|<span data-ttu-id="48b3a-230">标识名称。</span><span class="sxs-lookup"><span data-stu-id="48b3a-230">The Identity Name.</span></span>|
|<span data-ttu-id="48b3a-231">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="48b3a-231">vppTokenId</span></span>|<span data-ttu-id="48b3a-232">String</span><span class="sxs-lookup"><span data-stu-id="48b3a-232">String</span></span>|<span data-ttu-id="48b3a-233">与此应用程序关联的 VPP 标记的标识符。</span><span class="sxs-lookup"><span data-stu-id="48b3a-233">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="48b3a-234">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="48b3a-234">revokeLicenseActionResults</span></span>|<span data-ttu-id="48b3a-235">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="48b3a-235">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="48b3a-236">结果的撤消此应用程序许可证操作。</span><span class="sxs-lookup"><span data-stu-id="48b3a-236">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="48b3a-237">响应</span><span class="sxs-lookup"><span data-stu-id="48b3a-237">Response</span></span>
<span data-ttu-id="48b3a-238">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[macOsVppApp](../resources/intune-apps-macosvppapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="48b3a-238">If successful, this method returns a `200 OK` response code and an updated [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48b3a-239">示例</span><span class="sxs-lookup"><span data-stu-id="48b3a-239">Example</span></span>

### <a name="request"></a><span data-ttu-id="48b3a-240">请求</span><span class="sxs-lookup"><span data-stu-id="48b3a-240">Request</span></span>
<span data-ttu-id="48b3a-241">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="48b3a-241">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1842

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="48b3a-242">响应</span><span class="sxs-lookup"><span data-stu-id="48b3a-242">Response</span></span>
<span data-ttu-id="48b3a-p120">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="48b3a-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2014

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
  "id": "10b95265-5265-10b9-6552-b9106552b910",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```




