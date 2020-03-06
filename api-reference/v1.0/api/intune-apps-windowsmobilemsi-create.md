---
title: 创建 windowsMobileMSI
description: 创建新的 windowsMobileMSI 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a27e369110b0b426c412049848d2d36f80d9d77d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515845"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="fc3e7-103">创建 windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="fc3e7-103">Create windowsMobileMSI</span></span>

<span data-ttu-id="fc3e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc3e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc3e7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc3e7-106">创建新的 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-106">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc3e7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fc3e7-107">Prerequisites</span></span>
<span data-ttu-id="fc3e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc3e7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc3e7-110">Permission type</span></span>|<span data-ttu-id="fc3e7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fc3e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc3e7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc3e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fc3e7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc3e7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fc3e7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc3e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc3e7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-115">Not supported.</span></span>|
|<span data-ttu-id="fc3e7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc3e7-116">Application</span></span>|<span data-ttu-id="fc3e7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc3e7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc3e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fc3e7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc3e7-119">Request headers</span></span>
|<span data-ttu-id="fc3e7-120">标头</span><span class="sxs-lookup"><span data-stu-id="fc3e7-120">Header</span></span>|<span data-ttu-id="fc3e7-121">值</span><span class="sxs-lookup"><span data-stu-id="fc3e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc3e7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc3e7-122">Authorization</span></span>|<span data-ttu-id="fc3e7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc3e7-124">接受</span><span class="sxs-lookup"><span data-stu-id="fc3e7-124">Accept</span></span>|<span data-ttu-id="fc3e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fc3e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc3e7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc3e7-126">Request body</span></span>
<span data-ttu-id="fc3e7-127">在请求正文中，提供 windowsMobileMSI 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-127">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="fc3e7-128">下表显示创建 windowsMobileMSI 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-128">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="fc3e7-129">属性</span><span class="sxs-lookup"><span data-stu-id="fc3e7-129">Property</span></span>|<span data-ttu-id="fc3e7-130">类型</span><span class="sxs-lookup"><span data-stu-id="fc3e7-130">Type</span></span>|<span data-ttu-id="fc3e7-131">说明</span><span class="sxs-lookup"><span data-stu-id="fc3e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc3e7-132">id</span><span class="sxs-lookup"><span data-stu-id="fc3e7-132">id</span></span>|<span data-ttu-id="fc3e7-133">字符串</span><span class="sxs-lookup"><span data-stu-id="fc3e7-133">String</span></span>|<span data-ttu-id="fc3e7-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-134">Key of the entity.</span></span> <span data-ttu-id="fc3e7-135">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc3e7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fc3e7-136">displayName</span></span>|<span data-ttu-id="fc3e7-137">字符串</span><span class="sxs-lookup"><span data-stu-id="fc3e7-137">String</span></span>|<span data-ttu-id="fc3e7-138">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="fc3e7-139">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc3e7-140">说明</span><span class="sxs-lookup"><span data-stu-id="fc3e7-140">description</span></span>|<span data-ttu-id="fc3e7-141">字符串</span><span class="sxs-lookup"><span data-stu-id="fc3e7-141">String</span></span>|<span data-ttu-id="fc3e7-142">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-142">The description of the app.</span></span> <span data-ttu-id="fc3e7-143">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc3e7-144">publisher</span><span class="sxs-lookup"><span data-stu-id="fc3e7-144">publisher</span></span>|<span data-ttu-id="fc3e7-145">字符串</span><span class="sxs-lookup"><span data-stu-id="fc3e7-145">String</span></span>|<span data-ttu-id="fc3e7-146">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-146">The publisher of the app.</span></span> <span data-ttu-id="fc3e7-147">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc3e7-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="fc3e7-148">largeIcon</span></span>|[<span data-ttu-id="fc3e7-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="fc3e7-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="fc3e7-150">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="fc3e7-151">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc3e7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc3e7-152">createdDateTime</span></span>|<span data-ttu-id="fc3e7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc3e7-153">DateTimeOffset</span></span>|<span data-ttu-id="fc3e7-154">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-154">The date and time the app was created.</span></span> <span data-ttu-id="fc3e7-155">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc3e7-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc3e7-156">lastModifiedDateTime</span></span>|<span data-ttu-id="fc3e7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc3e7-157">DateTimeOffset</span></span>|<span data-ttu-id="fc3e7-158">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-158">The date and time the app was last modified.</span></span> <span data-ttu-id="fc3e7-159">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc3e7-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="fc3e7-160">isFeatured</span></span>|<span data-ttu-id="fc3e7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc3e7-161">Boolean</span></span>|<span data-ttu-id="fc3e7-162">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc3e7-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="fc3e7-163">privacyInformationUrl</span></span>|<span data-ttu-id="fc3e7-164">字符串</span><span class="sxs-lookup"><span data-stu-id="fc3e7-164">String</span></span>|<span data-ttu-id="fc3e7-165">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-165">The privacy statement Url.</span></span> <span data-ttu-id="fc3e7-166">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc3e7-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="fc3e7-167">informationUrl</span></span>|<span data-ttu-id="fc3e7-168">字符串</span><span class="sxs-lookup"><span data-stu-id="fc3e7-168">String</span></span>|<span data-ttu-id="fc3e7-169">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-169">The more information Url.</span></span> <span data-ttu-id="fc3e7-170">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc3e7-171">owner</span><span class="sxs-lookup"><span data-stu-id="fc3e7-171">owner</span></span>|<span data-ttu-id="fc3e7-172">String</span><span class="sxs-lookup"><span data-stu-id="fc3e7-172">String</span></span>|<span data-ttu-id="fc3e7-173">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-173">The owner of the app.</span></span> <span data-ttu-id="fc3e7-174">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc3e7-175">developer</span><span class="sxs-lookup"><span data-stu-id="fc3e7-175">developer</span></span>|<span data-ttu-id="fc3e7-176">字符串</span><span class="sxs-lookup"><span data-stu-id="fc3e7-176">String</span></span>|<span data-ttu-id="fc3e7-177">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-177">The developer of the app.</span></span> <span data-ttu-id="fc3e7-178">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc3e7-179">notes</span><span class="sxs-lookup"><span data-stu-id="fc3e7-179">notes</span></span>|<span data-ttu-id="fc3e7-180">字符串</span><span class="sxs-lookup"><span data-stu-id="fc3e7-180">String</span></span>|<span data-ttu-id="fc3e7-181">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-181">Notes for the app.</span></span> <span data-ttu-id="fc3e7-182">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="fc3e7-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="fc3e7-183">publishingState</span></span>|[<span data-ttu-id="fc3e7-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="fc3e7-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="fc3e7-185">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-185">The publishing state for the app.</span></span> <span data-ttu-id="fc3e7-186">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="fc3e7-187">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="fc3e7-188">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="fc3e7-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="fc3e7-189">committedContentVersion</span></span>|<span data-ttu-id="fc3e7-190">字符串</span><span class="sxs-lookup"><span data-stu-id="fc3e7-190">String</span></span>|<span data-ttu-id="fc3e7-191">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-191">The internal committed content version.</span></span> <span data-ttu-id="fc3e7-192">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fc3e7-193">fileName</span><span class="sxs-lookup"><span data-stu-id="fc3e7-193">fileName</span></span>|<span data-ttu-id="fc3e7-194">字符串</span><span class="sxs-lookup"><span data-stu-id="fc3e7-194">String</span></span>|<span data-ttu-id="fc3e7-195">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-195">The name of the main Lob application file.</span></span> <span data-ttu-id="fc3e7-196">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fc3e7-197">size</span><span class="sxs-lookup"><span data-stu-id="fc3e7-197">size</span></span>|<span data-ttu-id="fc3e7-198">Int64</span><span class="sxs-lookup"><span data-stu-id="fc3e7-198">Int64</span></span>|<span data-ttu-id="fc3e7-199">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="fc3e7-200">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc3e7-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="fc3e7-201">commandLine</span><span class="sxs-lookup"><span data-stu-id="fc3e7-201">commandLine</span></span>|<span data-ttu-id="fc3e7-202">字符串</span><span class="sxs-lookup"><span data-stu-id="fc3e7-202">String</span></span>|<span data-ttu-id="fc3e7-203">命令行。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-203">The command line.</span></span>|
|<span data-ttu-id="fc3e7-204">productCode</span><span class="sxs-lookup"><span data-stu-id="fc3e7-204">productCode</span></span>|<span data-ttu-id="fc3e7-205">字符串</span><span class="sxs-lookup"><span data-stu-id="fc3e7-205">String</span></span>|<span data-ttu-id="fc3e7-206">产品代码。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-206">The product code.</span></span>|
|<span data-ttu-id="fc3e7-207">productVersion</span><span class="sxs-lookup"><span data-stu-id="fc3e7-207">productVersion</span></span>|<span data-ttu-id="fc3e7-208">String</span><span class="sxs-lookup"><span data-stu-id="fc3e7-208">String</span></span>|<span data-ttu-id="fc3e7-209">Windows Mobile MSI 业务线 (LoB) 应用的产品版本。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-209">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="fc3e7-210">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="fc3e7-210">ignoreVersionDetection</span></span>|<span data-ttu-id="fc3e7-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc3e7-211">Boolean</span></span>|<span data-ttu-id="fc3e7-212">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-212">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="fc3e7-213">对于使用自更新功能的 Windows Mobile MSI 业务线 (LoB) 应用，将此值设置为 true。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-213">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="fc3e7-214">响应</span><span class="sxs-lookup"><span data-stu-id="fc3e7-214">Response</span></span>
<span data-ttu-id="fc3e7-215">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-215">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc3e7-216">示例</span><span class="sxs-lookup"><span data-stu-id="fc3e7-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc3e7-217">请求</span><span class="sxs-lookup"><span data-stu-id="fc3e7-217">Request</span></span>
<span data-ttu-id="fc3e7-218">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-218">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 855

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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="fc3e7-219">响应</span><span class="sxs-lookup"><span data-stu-id="fc3e7-219">Response</span></span>
<span data-ttu-id="fc3e7-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fc3e7-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1027

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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```




