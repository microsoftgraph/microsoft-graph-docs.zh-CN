---
title: 更新 officeSuiteApp
description: 更新 officeSuiteApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 24d5a8031580fa1d7cfe74415d84de32f49fa398
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979325"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="03bfc-103">更新 officeSuiteApp</span><span class="sxs-lookup"><span data-stu-id="03bfc-103">Update officeSuiteApp</span></span>

> <span data-ttu-id="03bfc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="03bfc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03bfc-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="03bfc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03bfc-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="03bfc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03bfc-107">更新[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="03bfc-107">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="03bfc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="03bfc-108">Prerequisites</span></span>
<span data-ttu-id="03bfc-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="03bfc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03bfc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="03bfc-111">Permission type</span></span>|<span data-ttu-id="03bfc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="03bfc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03bfc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03bfc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03bfc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03bfc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="03bfc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03bfc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03bfc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="03bfc-116">Not supported.</span></span>|
|<span data-ttu-id="03bfc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="03bfc-117">Application</span></span>|<span data-ttu-id="03bfc-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="03bfc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03bfc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03bfc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="03bfc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="03bfc-120">Request headers</span></span>
|<span data-ttu-id="03bfc-121">标头</span><span class="sxs-lookup"><span data-stu-id="03bfc-121">Header</span></span>|<span data-ttu-id="03bfc-122">值</span><span class="sxs-lookup"><span data-stu-id="03bfc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03bfc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03bfc-123">Authorization</span></span>|<span data-ttu-id="03bfc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="03bfc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03bfc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="03bfc-125">Accept</span></span>|<span data-ttu-id="03bfc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03bfc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03bfc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="03bfc-127">Request body</span></span>
<span data-ttu-id="03bfc-128">在请求正文中，提供[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03bfc-128">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="03bfc-129">下表显示时创建[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="03bfc-129">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="03bfc-130">属性</span><span class="sxs-lookup"><span data-stu-id="03bfc-130">Property</span></span>|<span data-ttu-id="03bfc-131">类型</span><span class="sxs-lookup"><span data-stu-id="03bfc-131">Type</span></span>|<span data-ttu-id="03bfc-132">说明</span><span class="sxs-lookup"><span data-stu-id="03bfc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03bfc-133">id</span><span class="sxs-lookup"><span data-stu-id="03bfc-133">id</span></span>|<span data-ttu-id="03bfc-134">String</span><span class="sxs-lookup"><span data-stu-id="03bfc-134">String</span></span>|<span data-ttu-id="03bfc-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="03bfc-135">Key of the entity.</span></span> <span data-ttu-id="03bfc-136">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03bfc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="03bfc-137">displayName</span></span>|<span data-ttu-id="03bfc-138">String</span><span class="sxs-lookup"><span data-stu-id="03bfc-138">String</span></span>|<span data-ttu-id="03bfc-139">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="03bfc-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="03bfc-140">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03bfc-141">description</span><span class="sxs-lookup"><span data-stu-id="03bfc-141">description</span></span>|<span data-ttu-id="03bfc-142">String</span><span class="sxs-lookup"><span data-stu-id="03bfc-142">String</span></span>|<span data-ttu-id="03bfc-143">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="03bfc-143">The description of the app.</span></span> <span data-ttu-id="03bfc-144">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03bfc-145">publisher</span><span class="sxs-lookup"><span data-stu-id="03bfc-145">publisher</span></span>|<span data-ttu-id="03bfc-146">String</span><span class="sxs-lookup"><span data-stu-id="03bfc-146">String</span></span>|<span data-ttu-id="03bfc-147">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="03bfc-147">The publisher of the app.</span></span> <span data-ttu-id="03bfc-148">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03bfc-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="03bfc-149">largeIcon</span></span>|[<span data-ttu-id="03bfc-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="03bfc-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="03bfc-151">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="03bfc-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="03bfc-152">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03bfc-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03bfc-153">createdDateTime</span></span>|<span data-ttu-id="03bfc-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03bfc-154">DateTimeOffset</span></span>|<span data-ttu-id="03bfc-155">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="03bfc-155">The date and time the app was created.</span></span> <span data-ttu-id="03bfc-156">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03bfc-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03bfc-157">lastModifiedDateTime</span></span>|<span data-ttu-id="03bfc-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03bfc-158">DateTimeOffset</span></span>|<span data-ttu-id="03bfc-159">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="03bfc-159">The date and time the app was last modified.</span></span> <span data-ttu-id="03bfc-160">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03bfc-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="03bfc-161">isFeatured</span></span>|<span data-ttu-id="03bfc-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="03bfc-162">Boolean</span></span>|<span data-ttu-id="03bfc-163">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03bfc-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="03bfc-164">privacyInformationUrl</span></span>|<span data-ttu-id="03bfc-165">String</span><span class="sxs-lookup"><span data-stu-id="03bfc-165">String</span></span>|<span data-ttu-id="03bfc-166">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="03bfc-166">The privacy statement Url.</span></span> <span data-ttu-id="03bfc-167">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03bfc-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="03bfc-168">informationUrl</span></span>|<span data-ttu-id="03bfc-169">String</span><span class="sxs-lookup"><span data-stu-id="03bfc-169">String</span></span>|<span data-ttu-id="03bfc-170">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="03bfc-170">The more information Url.</span></span> <span data-ttu-id="03bfc-171">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03bfc-172">owner</span><span class="sxs-lookup"><span data-stu-id="03bfc-172">owner</span></span>|<span data-ttu-id="03bfc-173">String</span><span class="sxs-lookup"><span data-stu-id="03bfc-173">String</span></span>|<span data-ttu-id="03bfc-174">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="03bfc-174">The owner of the app.</span></span> <span data-ttu-id="03bfc-175">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03bfc-176">developer</span><span class="sxs-lookup"><span data-stu-id="03bfc-176">developer</span></span>|<span data-ttu-id="03bfc-177">String</span><span class="sxs-lookup"><span data-stu-id="03bfc-177">String</span></span>|<span data-ttu-id="03bfc-178">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="03bfc-178">The developer of the app.</span></span> <span data-ttu-id="03bfc-179">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03bfc-180">notes</span><span class="sxs-lookup"><span data-stu-id="03bfc-180">notes</span></span>|<span data-ttu-id="03bfc-181">String</span><span class="sxs-lookup"><span data-stu-id="03bfc-181">String</span></span>|<span data-ttu-id="03bfc-182">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="03bfc-182">Notes for the app.</span></span> <span data-ttu-id="03bfc-183">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03bfc-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="03bfc-184">uploadState</span></span>|<span data-ttu-id="03bfc-185">Int32</span><span class="sxs-lookup"><span data-stu-id="03bfc-185">Int32</span></span>|<span data-ttu-id="03bfc-186">上载状态。</span><span class="sxs-lookup"><span data-stu-id="03bfc-186">The upload state.</span></span> <span data-ttu-id="03bfc-187">继承自 [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="03bfc-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="03bfc-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="03bfc-188">publishingState</span></span>|[<span data-ttu-id="03bfc-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="03bfc-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="03bfc-190">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="03bfc-190">The publishing state for the app.</span></span> <span data-ttu-id="03bfc-191">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="03bfc-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="03bfc-192">继承自[mobileApp](../resources/intune-apps-mobileapp.md)。</span><span class="sxs-lookup"><span data-stu-id="03bfc-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="03bfc-193">可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="03bfc-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="03bfc-194">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="03bfc-194">autoAcceptEula</span></span>|<span data-ttu-id="03bfc-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="03bfc-195">Boolean</span></span>|<span data-ttu-id="03bfc-196">要接受 EULA 自动在最终用户的设备上的值。</span><span class="sxs-lookup"><span data-stu-id="03bfc-196">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="03bfc-197">productIds</span><span class="sxs-lookup"><span data-stu-id="03bfc-197">productIds</span></span>|<span data-ttu-id="03bfc-198">[officeProductId](../resources/intune-apps-officeproductid.md)集合</span><span class="sxs-lookup"><span data-stu-id="03bfc-198">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="03bfc-199">表示 Office365 套件 SKU 产品 Id。</span><span class="sxs-lookup"><span data-stu-id="03bfc-199">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="03bfc-200">可取值为：`o365ProPlusRetail`、`o365BusinessRetail`、`visioProRetail`、`projectProRetail`。</span><span class="sxs-lookup"><span data-stu-id="03bfc-200">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="03bfc-201">excludedApps</span><span class="sxs-lookup"><span data-stu-id="03bfc-201">excludedApps</span></span>|[<span data-ttu-id="03bfc-202">excludedApps</span><span class="sxs-lookup"><span data-stu-id="03bfc-202">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="03bfc-203">该属性表示的应用程序即排除从所选 Office365 产品 id。</span><span class="sxs-lookup"><span data-stu-id="03bfc-203">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="03bfc-204">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="03bfc-204">useSharedComputerActivation</span></span>|<span data-ttu-id="03bfc-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="03bfc-205">Boolean</span></span>|<span data-ttu-id="03bfc-206">是否在共享的计算机激活不用于 Office365 应用程序套件表示的属性。</span><span class="sxs-lookup"><span data-stu-id="03bfc-206">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="03bfc-207">updateChannel</span><span class="sxs-lookup"><span data-stu-id="03bfc-207">updateChannel</span></span>|[<span data-ttu-id="03bfc-208">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="03bfc-208">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="03bfc-209">表示 Office365 更新频道属性。</span><span class="sxs-lookup"><span data-stu-id="03bfc-209">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="03bfc-210">可取值为：`none`、`current`、`deferred`、`firstReleaseCurrent`、`firstReleaseDeferred`。</span><span class="sxs-lookup"><span data-stu-id="03bfc-210">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="03bfc-211">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="03bfc-211">officePlatformArchitecture</span></span>|[<span data-ttu-id="03bfc-212">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="03bfc-212">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="03bfc-213">要代表 Office365 应用程序套件版本的属性。</span><span class="sxs-lookup"><span data-stu-id="03bfc-213">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="03bfc-214">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。</span><span class="sxs-lookup"><span data-stu-id="03bfc-214">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="03bfc-215">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="03bfc-215">localesToInstall</span></span>|<span data-ttu-id="03bfc-216">String 集合</span><span class="sxs-lookup"><span data-stu-id="03bfc-216">String collection</span></span>|<span data-ttu-id="03bfc-217">表示安装的区域设置的属性中 Office365 应用程序在安装时。</span><span class="sxs-lookup"><span data-stu-id="03bfc-217">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="03bfc-218">它使用标准 RFC 6033。</span><span class="sxs-lookup"><span data-stu-id="03bfc-218">It uses standard RFC 6033.</span></span> <span data-ttu-id="03bfc-219">参考：https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="03bfc-219">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="03bfc-220">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="03bfc-220">installProgressDisplayLevel</span></span>|[<span data-ttu-id="03bfc-221">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="03bfc-221">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="03bfc-222">若要指定在设备上显示安装进度安装程序 UI 的级别。</span><span class="sxs-lookup"><span data-stu-id="03bfc-222">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="03bfc-223">可取值为：`none`、`full`。</span><span class="sxs-lookup"><span data-stu-id="03bfc-223">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="03bfc-224">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="03bfc-224">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="03bfc-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="03bfc-225">Boolean</span></span>|<span data-ttu-id="03bfc-226">要确定是否如果 Office365 应用程序套件部署到设备，或不卸载现有 Office MSI 的属性。</span><span class="sxs-lookup"><span data-stu-id="03bfc-226">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="03bfc-227">targetVersion</span><span class="sxs-lookup"><span data-stu-id="03bfc-227">targetVersion</span></span>|<span data-ttu-id="03bfc-228">字符串</span><span class="sxs-lookup"><span data-stu-id="03bfc-228">String</span></span>|<span data-ttu-id="03bfc-229">要代表应保持在设备上部署的 Office365 应用程序套件的特定目标版本的属性。</span><span class="sxs-lookup"><span data-stu-id="03bfc-229">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="03bfc-230">updateVersion</span><span class="sxs-lookup"><span data-stu-id="03bfc-230">updateVersion</span></span>|<span data-ttu-id="03bfc-231">字符串</span><span class="sxs-lookup"><span data-stu-id="03bfc-231">String</span></span>|<span data-ttu-id="03bfc-232">要代表特定目标版本处于可供 Office365 应用程序套件的更新版本的属性。</span><span class="sxs-lookup"><span data-stu-id="03bfc-232">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|



## <a name="response"></a><span data-ttu-id="03bfc-233">响应</span><span class="sxs-lookup"><span data-stu-id="03bfc-233">Response</span></span>
<span data-ttu-id="03bfc-234">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="03bfc-234">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03bfc-235">示例</span><span class="sxs-lookup"><span data-stu-id="03bfc-235">Example</span></span>
### <a name="request"></a><span data-ttu-id="03bfc-236">请求</span><span class="sxs-lookup"><span data-stu-id="03bfc-236">Request</span></span>
<span data-ttu-id="03bfc-237">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03bfc-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1413

{
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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value"
}
```

### <a name="response"></a><span data-ttu-id="03bfc-238">响应</span><span class="sxs-lookup"><span data-stu-id="03bfc-238">Response</span></span>
<span data-ttu-id="03bfc-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03bfc-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "id": "9b263b46-3b46-9b26-463b-269b463b269b",
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
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value"
}
```





