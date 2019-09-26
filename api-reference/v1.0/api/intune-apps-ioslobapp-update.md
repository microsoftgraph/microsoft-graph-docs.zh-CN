---
title: 更新 iosLobApp
description: 更新 iosLobApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a41f95873cd0b0bbfdcc5439053ce00c71fa27a1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196215"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="5cc74-103">更新 iosLobApp</span><span class="sxs-lookup"><span data-stu-id="5cc74-103">Update iosLobApp</span></span>

> <span data-ttu-id="5cc74-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5cc74-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cc74-105">更新 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5cc74-105">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cc74-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="5cc74-106">Prerequisites</span></span>
<span data-ttu-id="5cc74-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5cc74-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5cc74-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5cc74-109">Permission type</span></span>|<span data-ttu-id="5cc74-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5cc74-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cc74-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5cc74-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5cc74-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cc74-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5cc74-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5cc74-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cc74-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5cc74-114">Not supported.</span></span>|
|<span data-ttu-id="5cc74-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5cc74-115">Application</span></span>|<span data-ttu-id="5cc74-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cc74-116">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cc74-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5cc74-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="5cc74-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5cc74-118">Request headers</span></span>
|<span data-ttu-id="5cc74-119">标头</span><span class="sxs-lookup"><span data-stu-id="5cc74-119">Header</span></span>|<span data-ttu-id="5cc74-120">值</span><span class="sxs-lookup"><span data-stu-id="5cc74-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cc74-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cc74-121">Authorization</span></span>|<span data-ttu-id="5cc74-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5cc74-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cc74-123">接受</span><span class="sxs-lookup"><span data-stu-id="5cc74-123">Accept</span></span>|<span data-ttu-id="5cc74-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5cc74-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cc74-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5cc74-125">Request body</span></span>
<span data-ttu-id="5cc74-126">在请求正文中，提供 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cc74-126">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="5cc74-127">下表显示了创建 [iosLobApp](../resources/intune-apps-ioslobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5cc74-127">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="5cc74-128">属性</span><span class="sxs-lookup"><span data-stu-id="5cc74-128">Property</span></span>|<span data-ttu-id="5cc74-129">类型</span><span class="sxs-lookup"><span data-stu-id="5cc74-129">Type</span></span>|<span data-ttu-id="5cc74-130">说明</span><span class="sxs-lookup"><span data-stu-id="5cc74-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cc74-131">id</span><span class="sxs-lookup"><span data-stu-id="5cc74-131">id</span></span>|<span data-ttu-id="5cc74-132">字符串</span><span class="sxs-lookup"><span data-stu-id="5cc74-132">String</span></span>|<span data-ttu-id="5cc74-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5cc74-133">Key of the entity.</span></span> <span data-ttu-id="5cc74-134">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc74-135">displayName</span><span class="sxs-lookup"><span data-stu-id="5cc74-135">displayName</span></span>|<span data-ttu-id="5cc74-136">String</span><span class="sxs-lookup"><span data-stu-id="5cc74-136">String</span></span>|<span data-ttu-id="5cc74-137">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="5cc74-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5cc74-138">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc74-139">说明</span><span class="sxs-lookup"><span data-stu-id="5cc74-139">description</span></span>|<span data-ttu-id="5cc74-140">字符串</span><span class="sxs-lookup"><span data-stu-id="5cc74-140">String</span></span>|<span data-ttu-id="5cc74-141">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="5cc74-141">The description of the app.</span></span> <span data-ttu-id="5cc74-142">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc74-143">publisher</span><span class="sxs-lookup"><span data-stu-id="5cc74-143">publisher</span></span>|<span data-ttu-id="5cc74-144">String</span><span class="sxs-lookup"><span data-stu-id="5cc74-144">String</span></span>|<span data-ttu-id="5cc74-145">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="5cc74-145">The publisher of the app.</span></span> <span data-ttu-id="5cc74-146">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc74-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5cc74-147">largeIcon</span></span>|[<span data-ttu-id="5cc74-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5cc74-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5cc74-149">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="5cc74-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5cc74-150">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc74-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5cc74-151">createdDateTime</span></span>|<span data-ttu-id="5cc74-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cc74-152">DateTimeOffset</span></span>|<span data-ttu-id="5cc74-153">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5cc74-153">The date and time the app was created.</span></span> <span data-ttu-id="5cc74-154">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc74-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5cc74-155">lastModifiedDateTime</span></span>|<span data-ttu-id="5cc74-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cc74-156">DateTimeOffset</span></span>|<span data-ttu-id="5cc74-157">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5cc74-157">The date and time the app was last modified.</span></span> <span data-ttu-id="5cc74-158">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc74-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5cc74-159">isFeatured</span></span>|<span data-ttu-id="5cc74-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="5cc74-160">Boolean</span></span>|<span data-ttu-id="5cc74-161">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc74-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5cc74-162">privacyInformationUrl</span></span>|<span data-ttu-id="5cc74-163">String</span><span class="sxs-lookup"><span data-stu-id="5cc74-163">String</span></span>|<span data-ttu-id="5cc74-164">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="5cc74-164">The privacy statement Url.</span></span> <span data-ttu-id="5cc74-165">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc74-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5cc74-166">informationUrl</span></span>|<span data-ttu-id="5cc74-167">String</span><span class="sxs-lookup"><span data-stu-id="5cc74-167">String</span></span>|<span data-ttu-id="5cc74-168">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="5cc74-168">The more information Url.</span></span> <span data-ttu-id="5cc74-169">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc74-170">owner</span><span class="sxs-lookup"><span data-stu-id="5cc74-170">owner</span></span>|<span data-ttu-id="5cc74-171">String</span><span class="sxs-lookup"><span data-stu-id="5cc74-171">String</span></span>|<span data-ttu-id="5cc74-172">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="5cc74-172">The owner of the app.</span></span> <span data-ttu-id="5cc74-173">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc74-174">developer</span><span class="sxs-lookup"><span data-stu-id="5cc74-174">developer</span></span>|<span data-ttu-id="5cc74-175">String</span><span class="sxs-lookup"><span data-stu-id="5cc74-175">String</span></span>|<span data-ttu-id="5cc74-176">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="5cc74-176">The developer of the app.</span></span> <span data-ttu-id="5cc74-177">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc74-178">notes</span><span class="sxs-lookup"><span data-stu-id="5cc74-178">notes</span></span>|<span data-ttu-id="5cc74-179">String</span><span class="sxs-lookup"><span data-stu-id="5cc74-179">String</span></span>|<span data-ttu-id="5cc74-180">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="5cc74-180">Notes for the app.</span></span> <span data-ttu-id="5cc74-181">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5cc74-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="5cc74-182">publishingState</span></span>|[<span data-ttu-id="5cc74-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5cc74-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5cc74-184">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="5cc74-184">The publishing state for the app.</span></span> <span data-ttu-id="5cc74-185">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="5cc74-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5cc74-186">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="5cc74-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5cc74-187">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="5cc74-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5cc74-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="5cc74-188">committedContentVersion</span></span>|<span data-ttu-id="5cc74-189">String</span><span class="sxs-lookup"><span data-stu-id="5cc74-189">String</span></span>|<span data-ttu-id="5cc74-190">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="5cc74-190">The internal committed content version.</span></span> <span data-ttu-id="5cc74-191">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5cc74-192">fileName</span><span class="sxs-lookup"><span data-stu-id="5cc74-192">fileName</span></span>|<span data-ttu-id="5cc74-193">String</span><span class="sxs-lookup"><span data-stu-id="5cc74-193">String</span></span>|<span data-ttu-id="5cc74-194">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="5cc74-194">The name of the main Lob application file.</span></span> <span data-ttu-id="5cc74-195">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5cc74-196">size</span><span class="sxs-lookup"><span data-stu-id="5cc74-196">size</span></span>|<span data-ttu-id="5cc74-197">Int64</span><span class="sxs-lookup"><span data-stu-id="5cc74-197">Int64</span></span>|<span data-ttu-id="5cc74-198">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="5cc74-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="5cc74-199">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5cc74-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5cc74-200">bundleId</span><span class="sxs-lookup"><span data-stu-id="5cc74-200">bundleId</span></span>|<span data-ttu-id="5cc74-201">String</span><span class="sxs-lookup"><span data-stu-id="5cc74-201">String</span></span>|<span data-ttu-id="5cc74-202">标识名称。</span><span class="sxs-lookup"><span data-stu-id="5cc74-202">The Identity Name.</span></span>|
|<span data-ttu-id="5cc74-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="5cc74-203">applicableDeviceType</span></span>|[<span data-ttu-id="5cc74-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="5cc74-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="5cc74-205">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="5cc74-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="5cc74-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5cc74-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="5cc74-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="5cc74-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="5cc74-208">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="5cc74-208">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="5cc74-209">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5cc74-209">expirationDateTime</span></span>|<span data-ttu-id="5cc74-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5cc74-210">DateTimeOffset</span></span>|<span data-ttu-id="5cc74-211">过期时间。</span><span class="sxs-lookup"><span data-stu-id="5cc74-211">The expiration time.</span></span>|
|<span data-ttu-id="5cc74-212">versionNumber</span><span class="sxs-lookup"><span data-stu-id="5cc74-212">versionNumber</span></span>|<span data-ttu-id="5cc74-213">String</span><span class="sxs-lookup"><span data-stu-id="5cc74-213">String</span></span>|<span data-ttu-id="5cc74-214">iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="5cc74-214">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="5cc74-215">buildNumber</span><span class="sxs-lookup"><span data-stu-id="5cc74-215">buildNumber</span></span>|<span data-ttu-id="5cc74-216">String</span><span class="sxs-lookup"><span data-stu-id="5cc74-216">String</span></span>|<span data-ttu-id="5cc74-217">iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="5cc74-217">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="5cc74-218">响应</span><span class="sxs-lookup"><span data-stu-id="5cc74-218">Response</span></span>
<span data-ttu-id="5cc74-219">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5cc74-219">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cc74-220">示例</span><span class="sxs-lookup"><span data-stu-id="5cc74-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cc74-221">请求</span><span class="sxs-lookup"><span data-stu-id="5cc74-221">Request</span></span>
<span data-ttu-id="5cc74-222">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5cc74-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1229

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="5cc74-223">响应</span><span class="sxs-lookup"><span data-stu-id="5cc74-223">Response</span></span>
<span data-ttu-id="5cc74-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5cc74-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1401

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



