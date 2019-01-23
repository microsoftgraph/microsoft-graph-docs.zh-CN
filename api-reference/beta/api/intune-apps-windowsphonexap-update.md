---
title: 更新 windowsPhoneXAP
description: 更新 windowsPhoneXAP 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 90943bafd09a31efeb6451ae91aa3f25205e0be4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421254"
---
# <a name="update-windowsphonexap"></a><span data-ttu-id="eaac5-103">更新 windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="eaac5-103">Update windowsPhoneXAP</span></span>

> <span data-ttu-id="eaac5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="eaac5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eaac5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eaac5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eaac5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eaac5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eaac5-107">更新[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eaac5-107">Update the properties of a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eaac5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="eaac5-108">Prerequisites</span></span>
<span data-ttu-id="eaac5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="eaac5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="eaac5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eaac5-111">Permission type</span></span>|<span data-ttu-id="eaac5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eaac5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eaac5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eaac5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eaac5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaac5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eaac5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eaac5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaac5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eaac5-116">Not supported.</span></span>|
|<span data-ttu-id="eaac5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eaac5-117">Application</span></span>|<span data-ttu-id="eaac5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="eaac5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaac5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eaac5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="eaac5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eaac5-120">Request headers</span></span>
|<span data-ttu-id="eaac5-121">标头</span><span class="sxs-lookup"><span data-stu-id="eaac5-121">Header</span></span>|<span data-ttu-id="eaac5-122">值</span><span class="sxs-lookup"><span data-stu-id="eaac5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eaac5-123">授权</span><span class="sxs-lookup"><span data-stu-id="eaac5-123">Authorization</span></span>|<span data-ttu-id="eaac5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eaac5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eaac5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eaac5-125">Accept</span></span>|<span data-ttu-id="eaac5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eaac5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaac5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="eaac5-127">Request body</span></span>
<span data-ttu-id="eaac5-128">在请求正文中，提供[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eaac5-128">In the request body, supply a JSON representation for the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

<span data-ttu-id="eaac5-129">下表显示时创建[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eaac5-129">The following table shows the properties that are required when you create the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span></span>

|<span data-ttu-id="eaac5-130">属性</span><span class="sxs-lookup"><span data-stu-id="eaac5-130">Property</span></span>|<span data-ttu-id="eaac5-131">类型</span><span class="sxs-lookup"><span data-stu-id="eaac5-131">Type</span></span>|<span data-ttu-id="eaac5-132">说明</span><span class="sxs-lookup"><span data-stu-id="eaac5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaac5-133">id</span><span class="sxs-lookup"><span data-stu-id="eaac5-133">id</span></span>|<span data-ttu-id="eaac5-134">String</span><span class="sxs-lookup"><span data-stu-id="eaac5-134">String</span></span>|<span data-ttu-id="eaac5-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="eaac5-135">Key of the entity.</span></span> <span data-ttu-id="eaac5-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="eaac5-137">displayName</span></span>|<span data-ttu-id="eaac5-138">String</span><span class="sxs-lookup"><span data-stu-id="eaac5-138">String</span></span>|<span data-ttu-id="eaac5-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="eaac5-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="eaac5-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-141">description</span><span class="sxs-lookup"><span data-stu-id="eaac5-141">description</span></span>|<span data-ttu-id="eaac5-142">String</span><span class="sxs-lookup"><span data-stu-id="eaac5-142">String</span></span>|<span data-ttu-id="eaac5-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="eaac5-143">The description of the app.</span></span> <span data-ttu-id="eaac5-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-145">publisher</span><span class="sxs-lookup"><span data-stu-id="eaac5-145">publisher</span></span>|<span data-ttu-id="eaac5-146">String</span><span class="sxs-lookup"><span data-stu-id="eaac5-146">String</span></span>|<span data-ttu-id="eaac5-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="eaac5-147">The publisher of the app.</span></span> <span data-ttu-id="eaac5-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="eaac5-149">largeIcon</span></span>|[<span data-ttu-id="eaac5-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="eaac5-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="eaac5-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="eaac5-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="eaac5-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eaac5-153">createdDateTime</span></span>|<span data-ttu-id="eaac5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaac5-154">DateTimeOffset</span></span>|<span data-ttu-id="eaac5-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="eaac5-155">The date and time the app was created.</span></span> <span data-ttu-id="eaac5-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eaac5-157">lastModifiedDateTime</span></span>|<span data-ttu-id="eaac5-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaac5-158">DateTimeOffset</span></span>|<span data-ttu-id="eaac5-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="eaac5-159">The date and time the app was last modified.</span></span> <span data-ttu-id="eaac5-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="eaac5-161">isFeatured</span></span>|<span data-ttu-id="eaac5-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaac5-162">Boolean</span></span>|<span data-ttu-id="eaac5-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="eaac5-164">privacyInformationUrl</span></span>|<span data-ttu-id="eaac5-165">String</span><span class="sxs-lookup"><span data-stu-id="eaac5-165">String</span></span>|<span data-ttu-id="eaac5-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="eaac5-166">The privacy statement Url.</span></span> <span data-ttu-id="eaac5-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="eaac5-168">informationUrl</span></span>|<span data-ttu-id="eaac5-169">String</span><span class="sxs-lookup"><span data-stu-id="eaac5-169">String</span></span>|<span data-ttu-id="eaac5-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="eaac5-170">The more information Url.</span></span> <span data-ttu-id="eaac5-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-172">owner</span><span class="sxs-lookup"><span data-stu-id="eaac5-172">owner</span></span>|<span data-ttu-id="eaac5-173">String</span><span class="sxs-lookup"><span data-stu-id="eaac5-173">String</span></span>|<span data-ttu-id="eaac5-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="eaac5-174">The owner of the app.</span></span> <span data-ttu-id="eaac5-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-176">developer</span><span class="sxs-lookup"><span data-stu-id="eaac5-176">developer</span></span>|<span data-ttu-id="eaac5-177">String</span><span class="sxs-lookup"><span data-stu-id="eaac5-177">String</span></span>|<span data-ttu-id="eaac5-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="eaac5-178">The developer of the app.</span></span> <span data-ttu-id="eaac5-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-180">notes</span><span class="sxs-lookup"><span data-stu-id="eaac5-180">notes</span></span>|<span data-ttu-id="eaac5-181">String</span><span class="sxs-lookup"><span data-stu-id="eaac5-181">String</span></span>|<span data-ttu-id="eaac5-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="eaac5-182">Notes for the app.</span></span> <span data-ttu-id="eaac5-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="eaac5-184">uploadState</span></span>|<span data-ttu-id="eaac5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="eaac5-185">Int32</span></span>|<span data-ttu-id="eaac5-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="eaac5-186">The upload state.</span></span> <span data-ttu-id="eaac5-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="eaac5-188">publishingState</span></span>|[<span data-ttu-id="eaac5-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="eaac5-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="eaac5-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="eaac5-190">The publishing state for the app.</span></span> <span data-ttu-id="eaac5-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="eaac5-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="eaac5-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="eaac5-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="eaac5-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="eaac5-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="eaac5-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="eaac5-194">isAssigned</span></span>|<span data-ttu-id="eaac5-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaac5-195">Boolean</span></span>|<span data-ttu-id="eaac5-196">值，指示是否将应用程序分配给至少一个组。</span><span class="sxs-lookup"><span data-stu-id="eaac5-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="eaac5-197">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eaac5-198">roleScopeTagIds</span></span>|<span data-ttu-id="eaac5-199">String 集合</span><span class="sxs-lookup"><span data-stu-id="eaac5-199">String collection</span></span>|<span data-ttu-id="eaac5-200">此移动应用程序的作用域标记 id 的列表。</span><span class="sxs-lookup"><span data-stu-id="eaac5-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="eaac5-201">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eaac5-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="eaac5-202">committedContentVersion</span></span>|<span data-ttu-id="eaac5-203">String</span><span class="sxs-lookup"><span data-stu-id="eaac5-203">String</span></span>|<span data-ttu-id="eaac5-204">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="eaac5-204">The internal committed content version.</span></span> <span data-ttu-id="eaac5-205">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="eaac5-206">fileName</span><span class="sxs-lookup"><span data-stu-id="eaac5-206">fileName</span></span>|<span data-ttu-id="eaac5-207">String</span><span class="sxs-lookup"><span data-stu-id="eaac5-207">String</span></span>|<span data-ttu-id="eaac5-208">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="eaac5-208">The name of the main Lob application file.</span></span> <span data-ttu-id="eaac5-209">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="eaac5-210">size</span><span class="sxs-lookup"><span data-stu-id="eaac5-210">size</span></span>|<span data-ttu-id="eaac5-211">Int64</span><span class="sxs-lookup"><span data-stu-id="eaac5-211">Int64</span></span>|<span data-ttu-id="eaac5-212">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="eaac5-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="eaac5-213">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="eaac5-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="eaac5-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="eaac5-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="eaac5-215">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="eaac5-215">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="eaac5-216">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="eaac5-216">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="eaac5-217">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="eaac5-217">productIdentifier</span></span>|<span data-ttu-id="eaac5-218">String</span><span class="sxs-lookup"><span data-stu-id="eaac5-218">String</span></span>|<span data-ttu-id="eaac5-219">产品标识符。</span><span class="sxs-lookup"><span data-stu-id="eaac5-219">The Product Identifier.</span></span>|
|<span data-ttu-id="eaac5-220">identityVersion</span><span class="sxs-lookup"><span data-stu-id="eaac5-220">identityVersion</span></span>|<span data-ttu-id="eaac5-221">String</span><span class="sxs-lookup"><span data-stu-id="eaac5-221">String</span></span>|<span data-ttu-id="eaac5-222">标识版本。</span><span class="sxs-lookup"><span data-stu-id="eaac5-222">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="eaac5-223">响应</span><span class="sxs-lookup"><span data-stu-id="eaac5-223">Response</span></span>
<span data-ttu-id="eaac5-224">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eaac5-224">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaac5-225">示例</span><span class="sxs-lookup"><span data-stu-id="eaac5-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="eaac5-226">请求</span><span class="sxs-lookup"><span data-stu-id="eaac5-226">Request</span></span>
<span data-ttu-id="eaac5-227">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eaac5-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1164

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
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
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="eaac5-228">响应</span><span class="sxs-lookup"><span data-stu-id="eaac5-228">Response</span></span>
<span data-ttu-id="eaac5-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eaac5-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1336

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```




