---
title: 创建 iosLobApp
description: 创建新的 iosLobApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c075c46e186e68bf2f55eee2325b1d908e700e42
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446545"
---
# <a name="create-ioslobapp"></a><span data-ttu-id="3bd59-103">创建 iosLobApp</span><span class="sxs-lookup"><span data-stu-id="3bd59-103">Create iosLobApp</span></span>

<span data-ttu-id="3bd59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bd59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3bd59-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3bd59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bd59-106">创建新的 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3bd59-106">Create a new [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bd59-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3bd59-107">Prerequisites</span></span>
<span data-ttu-id="3bd59-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3bd59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3bd59-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3bd59-110">Permission type</span></span>|<span data-ttu-id="3bd59-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3bd59-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bd59-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3bd59-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3bd59-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bd59-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3bd59-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3bd59-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bd59-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3bd59-115">Not supported.</span></span>|
|<span data-ttu-id="3bd59-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3bd59-116">Application</span></span>|<span data-ttu-id="3bd59-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bd59-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bd59-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3bd59-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3bd59-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3bd59-119">Request headers</span></span>
|<span data-ttu-id="3bd59-120">标头</span><span class="sxs-lookup"><span data-stu-id="3bd59-120">Header</span></span>|<span data-ttu-id="3bd59-121">值</span><span class="sxs-lookup"><span data-stu-id="3bd59-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bd59-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bd59-122">Authorization</span></span>|<span data-ttu-id="3bd59-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3bd59-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bd59-124">接受</span><span class="sxs-lookup"><span data-stu-id="3bd59-124">Accept</span></span>|<span data-ttu-id="3bd59-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3bd59-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bd59-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3bd59-126">Request body</span></span>
<span data-ttu-id="3bd59-127">在请求正文中，提供 iosLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3bd59-127">In the request body, supply a JSON representation for the iosLobApp object.</span></span>

<span data-ttu-id="3bd59-128">下表显示了创建 iosLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3bd59-128">The following table shows the properties that are required when you create the iosLobApp.</span></span>

|<span data-ttu-id="3bd59-129">属性</span><span class="sxs-lookup"><span data-stu-id="3bd59-129">Property</span></span>|<span data-ttu-id="3bd59-130">类型</span><span class="sxs-lookup"><span data-stu-id="3bd59-130">Type</span></span>|<span data-ttu-id="3bd59-131">说明</span><span class="sxs-lookup"><span data-stu-id="3bd59-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bd59-132">id</span><span class="sxs-lookup"><span data-stu-id="3bd59-132">id</span></span>|<span data-ttu-id="3bd59-133">字符串</span><span class="sxs-lookup"><span data-stu-id="3bd59-133">String</span></span>|<span data-ttu-id="3bd59-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3bd59-134">Key of the entity.</span></span> <span data-ttu-id="3bd59-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3bd59-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3bd59-136">displayName</span></span>|<span data-ttu-id="3bd59-137">String</span><span class="sxs-lookup"><span data-stu-id="3bd59-137">String</span></span>|<span data-ttu-id="3bd59-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="3bd59-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3bd59-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3bd59-140">description</span><span class="sxs-lookup"><span data-stu-id="3bd59-140">description</span></span>|<span data-ttu-id="3bd59-141">字符串</span><span class="sxs-lookup"><span data-stu-id="3bd59-141">String</span></span>|<span data-ttu-id="3bd59-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="3bd59-142">The description of the app.</span></span> <span data-ttu-id="3bd59-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3bd59-144">publisher</span><span class="sxs-lookup"><span data-stu-id="3bd59-144">publisher</span></span>|<span data-ttu-id="3bd59-145">String</span><span class="sxs-lookup"><span data-stu-id="3bd59-145">String</span></span>|<span data-ttu-id="3bd59-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="3bd59-146">The publisher of the app.</span></span> <span data-ttu-id="3bd59-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3bd59-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3bd59-148">largeIcon</span></span>|[<span data-ttu-id="3bd59-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3bd59-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3bd59-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="3bd59-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3bd59-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3bd59-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3bd59-152">createdDateTime</span></span>|<span data-ttu-id="3bd59-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bd59-153">DateTimeOffset</span></span>|<span data-ttu-id="3bd59-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3bd59-154">The date and time the app was created.</span></span> <span data-ttu-id="3bd59-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3bd59-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3bd59-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3bd59-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bd59-157">DateTimeOffset</span></span>|<span data-ttu-id="3bd59-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3bd59-158">The date and time the app was last modified.</span></span> <span data-ttu-id="3bd59-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3bd59-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3bd59-160">isFeatured</span></span>|<span data-ttu-id="3bd59-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="3bd59-161">Boolean</span></span>|<span data-ttu-id="3bd59-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3bd59-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3bd59-163">privacyInformationUrl</span></span>|<span data-ttu-id="3bd59-164">String</span><span class="sxs-lookup"><span data-stu-id="3bd59-164">String</span></span>|<span data-ttu-id="3bd59-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="3bd59-165">The privacy statement Url.</span></span> <span data-ttu-id="3bd59-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3bd59-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3bd59-167">informationUrl</span></span>|<span data-ttu-id="3bd59-168">String</span><span class="sxs-lookup"><span data-stu-id="3bd59-168">String</span></span>|<span data-ttu-id="3bd59-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="3bd59-169">The more information Url.</span></span> <span data-ttu-id="3bd59-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3bd59-171">owner</span><span class="sxs-lookup"><span data-stu-id="3bd59-171">owner</span></span>|<span data-ttu-id="3bd59-172">String</span><span class="sxs-lookup"><span data-stu-id="3bd59-172">String</span></span>|<span data-ttu-id="3bd59-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="3bd59-173">The owner of the app.</span></span> <span data-ttu-id="3bd59-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3bd59-175">developer</span><span class="sxs-lookup"><span data-stu-id="3bd59-175">developer</span></span>|<span data-ttu-id="3bd59-176">String</span><span class="sxs-lookup"><span data-stu-id="3bd59-176">String</span></span>|<span data-ttu-id="3bd59-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="3bd59-177">The developer of the app.</span></span> <span data-ttu-id="3bd59-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3bd59-179">notes</span><span class="sxs-lookup"><span data-stu-id="3bd59-179">notes</span></span>|<span data-ttu-id="3bd59-180">String</span><span class="sxs-lookup"><span data-stu-id="3bd59-180">String</span></span>|<span data-ttu-id="3bd59-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="3bd59-181">Notes for the app.</span></span> <span data-ttu-id="3bd59-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3bd59-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="3bd59-183">publishingState</span></span>|[<span data-ttu-id="3bd59-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3bd59-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3bd59-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="3bd59-185">The publishing state for the app.</span></span> <span data-ttu-id="3bd59-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="3bd59-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3bd59-187">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="3bd59-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3bd59-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="3bd59-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3bd59-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="3bd59-189">committedContentVersion</span></span>|<span data-ttu-id="3bd59-190">String</span><span class="sxs-lookup"><span data-stu-id="3bd59-190">String</span></span>|<span data-ttu-id="3bd59-191">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="3bd59-191">The internal committed content version.</span></span> <span data-ttu-id="3bd59-192">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3bd59-193">fileName</span><span class="sxs-lookup"><span data-stu-id="3bd59-193">fileName</span></span>|<span data-ttu-id="3bd59-194">String</span><span class="sxs-lookup"><span data-stu-id="3bd59-194">String</span></span>|<span data-ttu-id="3bd59-195">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="3bd59-195">The name of the main Lob application file.</span></span> <span data-ttu-id="3bd59-196">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3bd59-197">size</span><span class="sxs-lookup"><span data-stu-id="3bd59-197">size</span></span>|<span data-ttu-id="3bd59-198">Int64</span><span class="sxs-lookup"><span data-stu-id="3bd59-198">Int64</span></span>|<span data-ttu-id="3bd59-199">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="3bd59-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="3bd59-200">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3bd59-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3bd59-201">bundleId</span><span class="sxs-lookup"><span data-stu-id="3bd59-201">bundleId</span></span>|<span data-ttu-id="3bd59-202">String</span><span class="sxs-lookup"><span data-stu-id="3bd59-202">String</span></span>|<span data-ttu-id="3bd59-203">标识名称。</span><span class="sxs-lookup"><span data-stu-id="3bd59-203">The Identity Name.</span></span>|
|<span data-ttu-id="3bd59-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="3bd59-204">applicableDeviceType</span></span>|[<span data-ttu-id="3bd59-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="3bd59-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="3bd59-206">可运行此应用的 iOS 体系结构。</span><span class="sxs-lookup"><span data-stu-id="3bd59-206">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="3bd59-207">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3bd59-207">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3bd59-208">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3bd59-208">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="3bd59-209">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="3bd59-209">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="3bd59-210">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3bd59-210">expirationDateTime</span></span>|<span data-ttu-id="3bd59-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bd59-211">DateTimeOffset</span></span>|<span data-ttu-id="3bd59-212">过期时间。</span><span class="sxs-lookup"><span data-stu-id="3bd59-212">The expiration time.</span></span>|
|<span data-ttu-id="3bd59-213">versionNumber</span><span class="sxs-lookup"><span data-stu-id="3bd59-213">versionNumber</span></span>|<span data-ttu-id="3bd59-214">String</span><span class="sxs-lookup"><span data-stu-id="3bd59-214">String</span></span>|<span data-ttu-id="3bd59-215">iOS 业务线 (LoB) 应用的版本号。</span><span class="sxs-lookup"><span data-stu-id="3bd59-215">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3bd59-216">buildNumber</span><span class="sxs-lookup"><span data-stu-id="3bd59-216">buildNumber</span></span>|<span data-ttu-id="3bd59-217">String</span><span class="sxs-lookup"><span data-stu-id="3bd59-217">String</span></span>|<span data-ttu-id="3bd59-218">iOS 业务线 (LoB) 应用的内部版本号。</span><span class="sxs-lookup"><span data-stu-id="3bd59-218">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="3bd59-219">响应</span><span class="sxs-lookup"><span data-stu-id="3bd59-219">Response</span></span>
<span data-ttu-id="3bd59-220">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [iosLobApp](../resources/intune-apps-ioslobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3bd59-220">If successful, this method returns a `201 Created` response code and a [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bd59-221">示例</span><span class="sxs-lookup"><span data-stu-id="3bd59-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bd59-222">请求</span><span class="sxs-lookup"><span data-stu-id="3bd59-222">Request</span></span>
<span data-ttu-id="3bd59-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3bd59-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="3bd59-224">响应</span><span class="sxs-lookup"><span data-stu-id="3bd59-224">Response</span></span>
<span data-ttu-id="3bd59-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3bd59-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






