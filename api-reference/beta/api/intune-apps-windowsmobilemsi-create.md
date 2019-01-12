---
title: 创建 windowsMobileMSI
description: 创建新的 windowsMobileMSI 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1244b3e4720646bf89a61b8ec27e3d2aee5db5a5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914395"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="d7fe4-103">创建 windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="d7fe4-103">Create windowsMobileMSI</span></span>

> <span data-ttu-id="d7fe4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7fe4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7fe4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7fe4-107">创建新的 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-107">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d7fe4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d7fe4-108">Prerequisites</span></span>
<span data-ttu-id="d7fe4-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d7fe4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7fe4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7fe4-111">Permission type</span></span>|<span data-ttu-id="d7fe4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d7fe4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7fe4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7fe4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7fe4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7fe4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d7fe4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7fe4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7fe4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-116">Not supported.</span></span>|
|<span data-ttu-id="d7fe4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7fe4-117">Application</span></span>|<span data-ttu-id="d7fe4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7fe4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7fe4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="d7fe4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7fe4-120">Request headers</span></span>
|<span data-ttu-id="d7fe4-121">标头</span><span class="sxs-lookup"><span data-stu-id="d7fe4-121">Header</span></span>|<span data-ttu-id="d7fe4-122">值</span><span class="sxs-lookup"><span data-stu-id="d7fe4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7fe4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7fe4-123">Authorization</span></span>|<span data-ttu-id="d7fe4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7fe4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d7fe4-125">Accept</span></span>|<span data-ttu-id="d7fe4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7fe4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7fe4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7fe4-127">Request body</span></span>
<span data-ttu-id="d7fe4-128">在请求正文中，提供 windowsMobileMSI 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-128">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="d7fe4-129">下表显示创建 windowsMobileMSI 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-129">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="d7fe4-130">属性</span><span class="sxs-lookup"><span data-stu-id="d7fe4-130">Property</span></span>|<span data-ttu-id="d7fe4-131">类型</span><span class="sxs-lookup"><span data-stu-id="d7fe4-131">Type</span></span>|<span data-ttu-id="d7fe4-132">说明</span><span class="sxs-lookup"><span data-stu-id="d7fe4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7fe4-133">id</span><span class="sxs-lookup"><span data-stu-id="d7fe4-133">id</span></span>|<span data-ttu-id="d7fe4-134">String</span><span class="sxs-lookup"><span data-stu-id="d7fe4-134">String</span></span>|<span data-ttu-id="d7fe4-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-135">Key of the entity.</span></span> <span data-ttu-id="d7fe4-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7fe4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d7fe4-137">displayName</span></span>|<span data-ttu-id="d7fe4-138">String</span><span class="sxs-lookup"><span data-stu-id="d7fe4-138">String</span></span>|<span data-ttu-id="d7fe4-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d7fe4-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7fe4-141">description</span><span class="sxs-lookup"><span data-stu-id="d7fe4-141">description</span></span>|<span data-ttu-id="d7fe4-142">String</span><span class="sxs-lookup"><span data-stu-id="d7fe4-142">String</span></span>|<span data-ttu-id="d7fe4-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-143">The description of the app.</span></span> <span data-ttu-id="d7fe4-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7fe4-145">publisher</span><span class="sxs-lookup"><span data-stu-id="d7fe4-145">publisher</span></span>|<span data-ttu-id="d7fe4-146">String</span><span class="sxs-lookup"><span data-stu-id="d7fe4-146">String</span></span>|<span data-ttu-id="d7fe4-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-147">The publisher of the app.</span></span> <span data-ttu-id="d7fe4-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7fe4-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d7fe4-149">largeIcon</span></span>|[<span data-ttu-id="d7fe4-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d7fe4-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d7fe4-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d7fe4-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7fe4-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7fe4-153">createdDateTime</span></span>|<span data-ttu-id="d7fe4-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7fe4-154">DateTimeOffset</span></span>|<span data-ttu-id="d7fe4-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-155">The date and time the app was created.</span></span> <span data-ttu-id="d7fe4-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7fe4-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7fe4-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d7fe4-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7fe4-158">DateTimeOffset</span></span>|<span data-ttu-id="d7fe4-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d7fe4-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7fe4-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d7fe4-161">isFeatured</span></span>|<span data-ttu-id="d7fe4-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7fe4-162">Boolean</span></span>|<span data-ttu-id="d7fe4-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7fe4-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d7fe4-164">privacyInformationUrl</span></span>|<span data-ttu-id="d7fe4-165">String</span><span class="sxs-lookup"><span data-stu-id="d7fe4-165">String</span></span>|<span data-ttu-id="d7fe4-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-166">The privacy statement Url.</span></span> <span data-ttu-id="d7fe4-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7fe4-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d7fe4-168">informationUrl</span></span>|<span data-ttu-id="d7fe4-169">String</span><span class="sxs-lookup"><span data-stu-id="d7fe4-169">String</span></span>|<span data-ttu-id="d7fe4-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-170">The more information Url.</span></span> <span data-ttu-id="d7fe4-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7fe4-172">owner</span><span class="sxs-lookup"><span data-stu-id="d7fe4-172">owner</span></span>|<span data-ttu-id="d7fe4-173">String</span><span class="sxs-lookup"><span data-stu-id="d7fe4-173">String</span></span>|<span data-ttu-id="d7fe4-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-174">The owner of the app.</span></span> <span data-ttu-id="d7fe4-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7fe4-176">developer</span><span class="sxs-lookup"><span data-stu-id="d7fe4-176">developer</span></span>|<span data-ttu-id="d7fe4-177">String</span><span class="sxs-lookup"><span data-stu-id="d7fe4-177">String</span></span>|<span data-ttu-id="d7fe4-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-178">The developer of the app.</span></span> <span data-ttu-id="d7fe4-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7fe4-180">notes</span><span class="sxs-lookup"><span data-stu-id="d7fe4-180">notes</span></span>|<span data-ttu-id="d7fe4-181">String</span><span class="sxs-lookup"><span data-stu-id="d7fe4-181">String</span></span>|<span data-ttu-id="d7fe4-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-182">Notes for the app.</span></span> <span data-ttu-id="d7fe4-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7fe4-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d7fe4-184">uploadState</span></span>|<span data-ttu-id="d7fe4-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d7fe4-185">Int32</span></span>|<span data-ttu-id="d7fe4-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-186">The upload state.</span></span> <span data-ttu-id="d7fe4-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7fe4-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="d7fe4-188">publishingState</span></span>|[<span data-ttu-id="d7fe4-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d7fe4-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d7fe4-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-190">The publishing state for the app.</span></span> <span data-ttu-id="d7fe4-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d7fe4-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d7fe4-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d7fe4-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d7fe4-194">committedContentVersion</span></span>|<span data-ttu-id="d7fe4-195">String</span><span class="sxs-lookup"><span data-stu-id="d7fe4-195">String</span></span>|<span data-ttu-id="d7fe4-196">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-196">The internal committed content version.</span></span> <span data-ttu-id="d7fe4-197">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d7fe4-198">fileName</span><span class="sxs-lookup"><span data-stu-id="d7fe4-198">fileName</span></span>|<span data-ttu-id="d7fe4-199">String</span><span class="sxs-lookup"><span data-stu-id="d7fe4-199">String</span></span>|<span data-ttu-id="d7fe4-200">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-200">The name of the main Lob application file.</span></span> <span data-ttu-id="d7fe4-201">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d7fe4-202">size</span><span class="sxs-lookup"><span data-stu-id="d7fe4-202">size</span></span>|<span data-ttu-id="d7fe4-203">Int64</span><span class="sxs-lookup"><span data-stu-id="d7fe4-203">Int64</span></span>|<span data-ttu-id="d7fe4-204">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="d7fe4-205">继承自 [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="d7fe4-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d7fe4-206">commandLine</span><span class="sxs-lookup"><span data-stu-id="d7fe4-206">commandLine</span></span>|<span data-ttu-id="d7fe4-207">String</span><span class="sxs-lookup"><span data-stu-id="d7fe4-207">String</span></span>|<span data-ttu-id="d7fe4-208">命令行。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-208">The command line.</span></span>|
|<span data-ttu-id="d7fe4-209">productCode</span><span class="sxs-lookup"><span data-stu-id="d7fe4-209">productCode</span></span>|<span data-ttu-id="d7fe4-210">String</span><span class="sxs-lookup"><span data-stu-id="d7fe4-210">String</span></span>|<span data-ttu-id="d7fe4-211">产品代码。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-211">The product code.</span></span>|
|<span data-ttu-id="d7fe4-212">productVersion</span><span class="sxs-lookup"><span data-stu-id="d7fe4-212">productVersion</span></span>|<span data-ttu-id="d7fe4-213">String</span><span class="sxs-lookup"><span data-stu-id="d7fe4-213">String</span></span>|<span data-ttu-id="d7fe4-214">Windows Mobile MSI 业务线 (LoB) 应用的产品版本。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-214">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d7fe4-215">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="d7fe4-215">ignoreVersionDetection</span></span>|<span data-ttu-id="d7fe4-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7fe4-216">Boolean</span></span>|<span data-ttu-id="d7fe4-217">控制应用的版本是否将用于检测安装在设备上的应用的布尔值。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-217">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="d7fe4-218">对于使用自更新功能的 Windows Mobile MSI 业务线 (LoB) 应用，将此值设置为 true。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-218">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="d7fe4-219">identityVersion</span><span class="sxs-lookup"><span data-stu-id="d7fe4-219">identityVersion</span></span>|<span data-ttu-id="d7fe4-220">String</span><span class="sxs-lookup"><span data-stu-id="d7fe4-220">String</span></span>|<span data-ttu-id="d7fe4-221">标识版本。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-221">The identity version.</span></span>|
|<span data-ttu-id="d7fe4-222">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="d7fe4-222">useDeviceContext</span></span>|<span data-ttu-id="d7fe4-223">布尔值</span><span class="sxs-lookup"><span data-stu-id="d7fe4-223">Boolean</span></span>|<span data-ttu-id="d7fe4-224">指示是否双模式 MSI 安装设备上下文中。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-224">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="d7fe4-225">如果为 true，则将为所有用户安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-225">If true, app will be installed for all users.</span></span> <span data-ttu-id="d7fe4-226">如果为 false，应用程序将安装的每个用户。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-226">If false, app will be installed per-user.</span></span> <span data-ttu-id="d7fe4-227">如果为空，服务将使用 MSI 数据包的默认安装上下文。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-227">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="d7fe4-228">双模式 MSI 时此默认值将为每个用户。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-228">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="d7fe4-229">不能设置为非双协议模式应用程序。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-229">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="d7fe4-230">不能更改首次创建的应用程序后。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-230">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="d7fe4-231">响应</span><span class="sxs-lookup"><span data-stu-id="d7fe4-231">Response</span></span>
<span data-ttu-id="d7fe4-232">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-232">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7fe4-233">示例</span><span class="sxs-lookup"><span data-stu-id="d7fe4-233">Example</span></span>
### <a name="request"></a><span data-ttu-id="d7fe4-234">请求</span><span class="sxs-lookup"><span data-stu-id="d7fe4-234">Request</span></span>
<span data-ttu-id="d7fe4-235">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1018

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
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
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

### <a name="response"></a><span data-ttu-id="d7fe4-236">响应</span><span class="sxs-lookup"><span data-stu-id="d7fe4-236">Response</span></span>
<span data-ttu-id="d7fe4-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d7fe4-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1126

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





