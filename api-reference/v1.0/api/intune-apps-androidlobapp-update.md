---
title: 更新 androidLobApp
description: 更新 androidLobApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df75bcedcdad698bb48a607c2833cf5149e9af6f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757701"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="c3a7c-103">更新 androidLobApp</span><span class="sxs-lookup"><span data-stu-id="c3a7c-103">Update androidLobApp</span></span>

<span data-ttu-id="c3a7c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3a7c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3a7c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3a7c-106">更新 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-106">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3a7c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c3a7c-107">Prerequisites</span></span>
<span data-ttu-id="c3a7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3a7c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3a7c-110">Permission type</span></span>|<span data-ttu-id="c3a7c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c3a7c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3a7c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3a7c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3a7c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a7c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3a7c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3a7c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3a7c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-115">Not supported.</span></span>|
|<span data-ttu-id="c3a7c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3a7c-116">Application</span></span>|<span data-ttu-id="c3a7c-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a7c-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3a7c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3a7c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="c3a7c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3a7c-119">Request headers</span></span>
|<span data-ttu-id="c3a7c-120">标头</span><span class="sxs-lookup"><span data-stu-id="c3a7c-120">Header</span></span>|<span data-ttu-id="c3a7c-121">值</span><span class="sxs-lookup"><span data-stu-id="c3a7c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3a7c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3a7c-122">Authorization</span></span>|<span data-ttu-id="c3a7c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3a7c-124">接受</span><span class="sxs-lookup"><span data-stu-id="c3a7c-124">Accept</span></span>|<span data-ttu-id="c3a7c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3a7c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3a7c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3a7c-126">Request body</span></span>
<span data-ttu-id="c3a7c-127">在请求正文中，提供 [androidLobApp](../resources/intune-apps-androidlobapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-127">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="c3a7c-128">下表显示了创建 [androidLobApp](../resources/intune-apps-androidlobapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-128">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="c3a7c-129">属性</span><span class="sxs-lookup"><span data-stu-id="c3a7c-129">Property</span></span>|<span data-ttu-id="c3a7c-130">类型</span><span class="sxs-lookup"><span data-stu-id="c3a7c-130">Type</span></span>|<span data-ttu-id="c3a7c-131">说明</span><span class="sxs-lookup"><span data-stu-id="c3a7c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3a7c-132">id</span><span class="sxs-lookup"><span data-stu-id="c3a7c-132">id</span></span>|<span data-ttu-id="c3a7c-133">String</span><span class="sxs-lookup"><span data-stu-id="c3a7c-133">String</span></span>|<span data-ttu-id="c3a7c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-134">Key of the entity.</span></span> <span data-ttu-id="c3a7c-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3a7c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c3a7c-136">displayName</span></span>|<span data-ttu-id="c3a7c-137">String</span><span class="sxs-lookup"><span data-stu-id="c3a7c-137">String</span></span>|<span data-ttu-id="c3a7c-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c3a7c-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3a7c-140">description</span><span class="sxs-lookup"><span data-stu-id="c3a7c-140">description</span></span>|<span data-ttu-id="c3a7c-141">String</span><span class="sxs-lookup"><span data-stu-id="c3a7c-141">String</span></span>|<span data-ttu-id="c3a7c-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-142">The description of the app.</span></span> <span data-ttu-id="c3a7c-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3a7c-144">publisher</span><span class="sxs-lookup"><span data-stu-id="c3a7c-144">publisher</span></span>|<span data-ttu-id="c3a7c-145">String</span><span class="sxs-lookup"><span data-stu-id="c3a7c-145">String</span></span>|<span data-ttu-id="c3a7c-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-146">The publisher of the app.</span></span> <span data-ttu-id="c3a7c-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3a7c-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c3a7c-148">largeIcon</span></span>|[<span data-ttu-id="c3a7c-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c3a7c-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c3a7c-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c3a7c-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3a7c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3a7c-152">createdDateTime</span></span>|<span data-ttu-id="c3a7c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3a7c-153">DateTimeOffset</span></span>|<span data-ttu-id="c3a7c-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-154">The date and time the app was created.</span></span> <span data-ttu-id="c3a7c-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3a7c-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3a7c-156">lastModifiedDateTime</span></span>|<span data-ttu-id="c3a7c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3a7c-157">DateTimeOffset</span></span>|<span data-ttu-id="c3a7c-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-158">The date and time the app was last modified.</span></span> <span data-ttu-id="c3a7c-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3a7c-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c3a7c-160">isFeatured</span></span>|<span data-ttu-id="c3a7c-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3a7c-161">Boolean</span></span>|<span data-ttu-id="c3a7c-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3a7c-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c3a7c-163">privacyInformationUrl</span></span>|<span data-ttu-id="c3a7c-164">String</span><span class="sxs-lookup"><span data-stu-id="c3a7c-164">String</span></span>|<span data-ttu-id="c3a7c-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-165">The privacy statement Url.</span></span> <span data-ttu-id="c3a7c-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3a7c-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c3a7c-167">informationUrl</span></span>|<span data-ttu-id="c3a7c-168">String</span><span class="sxs-lookup"><span data-stu-id="c3a7c-168">String</span></span>|<span data-ttu-id="c3a7c-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-169">The more information Url.</span></span> <span data-ttu-id="c3a7c-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3a7c-171">所有者</span><span class="sxs-lookup"><span data-stu-id="c3a7c-171">owner</span></span>|<span data-ttu-id="c3a7c-172">String</span><span class="sxs-lookup"><span data-stu-id="c3a7c-172">String</span></span>|<span data-ttu-id="c3a7c-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-173">The owner of the app.</span></span> <span data-ttu-id="c3a7c-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3a7c-175">developer</span><span class="sxs-lookup"><span data-stu-id="c3a7c-175">developer</span></span>|<span data-ttu-id="c3a7c-176">String</span><span class="sxs-lookup"><span data-stu-id="c3a7c-176">String</span></span>|<span data-ttu-id="c3a7c-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-177">The developer of the app.</span></span> <span data-ttu-id="c3a7c-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3a7c-179">notes</span><span class="sxs-lookup"><span data-stu-id="c3a7c-179">notes</span></span>|<span data-ttu-id="c3a7c-180">String</span><span class="sxs-lookup"><span data-stu-id="c3a7c-180">String</span></span>|<span data-ttu-id="c3a7c-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-181">Notes for the app.</span></span> <span data-ttu-id="c3a7c-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c3a7c-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="c3a7c-183">publishingState</span></span>|[<span data-ttu-id="c3a7c-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c3a7c-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c3a7c-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-185">The publishing state for the app.</span></span> <span data-ttu-id="c3a7c-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c3a7c-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c3a7c-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c3a7c-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="c3a7c-189">committedContentVersion</span></span>|<span data-ttu-id="c3a7c-190">String</span><span class="sxs-lookup"><span data-stu-id="c3a7c-190">String</span></span>|<span data-ttu-id="c3a7c-191">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-191">The internal committed content version.</span></span> <span data-ttu-id="c3a7c-192">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c3a7c-193">fileName</span><span class="sxs-lookup"><span data-stu-id="c3a7c-193">fileName</span></span>|<span data-ttu-id="c3a7c-194">String</span><span class="sxs-lookup"><span data-stu-id="c3a7c-194">String</span></span>|<span data-ttu-id="c3a7c-195">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-195">The name of the main Lob application file.</span></span> <span data-ttu-id="c3a7c-196">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c3a7c-197">size</span><span class="sxs-lookup"><span data-stu-id="c3a7c-197">size</span></span>|<span data-ttu-id="c3a7c-198">Int64</span><span class="sxs-lookup"><span data-stu-id="c3a7c-198">Int64</span></span>|<span data-ttu-id="c3a7c-199">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="c3a7c-200">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="c3a7c-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="c3a7c-201">packageId</span><span class="sxs-lookup"><span data-stu-id="c3a7c-201">packageId</span></span>|<span data-ttu-id="c3a7c-202">String</span><span class="sxs-lookup"><span data-stu-id="c3a7c-202">String</span></span>|<span data-ttu-id="c3a7c-203">包标识符。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-203">The package identifier.</span></span>|
|<span data-ttu-id="c3a7c-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c3a7c-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c3a7c-205">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c3a7c-205">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="c3a7c-206">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-206">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="c3a7c-207">versionName</span><span class="sxs-lookup"><span data-stu-id="c3a7c-207">versionName</span></span>|<span data-ttu-id="c3a7c-208">String</span><span class="sxs-lookup"><span data-stu-id="c3a7c-208">String</span></span>|<span data-ttu-id="c3a7c-209">Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-209">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c3a7c-210">versionCode</span><span class="sxs-lookup"><span data-stu-id="c3a7c-210">versionCode</span></span>|<span data-ttu-id="c3a7c-211">String</span><span class="sxs-lookup"><span data-stu-id="c3a7c-211">String</span></span>|<span data-ttu-id="c3a7c-212">Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-212">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="c3a7c-213">响应</span><span class="sxs-lookup"><span data-stu-id="c3a7c-213">Response</span></span>
<span data-ttu-id="c3a7c-214">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [androidLobApp](../resources/intune-apps-androidlobapp.md)  对象。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-214">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3a7c-215">示例</span><span class="sxs-lookup"><span data-stu-id="c3a7c-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3a7c-216">请求</span><span class="sxs-lookup"><span data-stu-id="c3a7c-216">Request</span></span>
<span data-ttu-id="c3a7c-217">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1115

{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="c3a7c-218">响应</span><span class="sxs-lookup"><span data-stu-id="c3a7c-218">Response</span></span>
<span data-ttu-id="c3a7c-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c3a7c-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1287

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```




