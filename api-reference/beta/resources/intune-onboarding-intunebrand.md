---
title: intuneBrand 资源类型
description: intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4550fa46df5db366342495491f1e4207f1a1bffc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029489"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="5e0fa-103">intuneBrand 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e0fa-103">intuneBrand resource type</span></span>

<span data-ttu-id="5e0fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e0fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e0fa-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e0fa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e0fa-107">intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="5e0fa-108">属性</span><span class="sxs-lookup"><span data-stu-id="5e0fa-108">Properties</span></span>
|<span data-ttu-id="5e0fa-109">属性</span><span class="sxs-lookup"><span data-stu-id="5e0fa-109">Property</span></span>|<span data-ttu-id="5e0fa-110">类型</span><span class="sxs-lookup"><span data-stu-id="5e0fa-110">Type</span></span>|<span data-ttu-id="5e0fa-111">说明</span><span class="sxs-lookup"><span data-stu-id="5e0fa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e0fa-112">displayName</span><span class="sxs-lookup"><span data-stu-id="5e0fa-112">displayName</span></span>|<span data-ttu-id="5e0fa-113">String</span><span class="sxs-lookup"><span data-stu-id="5e0fa-113">String</span></span>|<span data-ttu-id="5e0fa-114">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="5e0fa-115">themeColor</span><span class="sxs-lookup"><span data-stu-id="5e0fa-115">themeColor</span></span>|[<span data-ttu-id="5e0fa-116">rgbColor</span><span class="sxs-lookup"><span data-stu-id="5e0fa-116">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="5e0fa-117">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-117">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="5e0fa-118">showLogo</span><span class="sxs-lookup"><span data-stu-id="5e0fa-118">showLogo</span></span>|<span data-ttu-id="5e0fa-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="5e0fa-119">Boolean</span></span>|<span data-ttu-id="5e0fa-120">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-120">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="5e0fa-121">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="5e0fa-121">lightBackgroundLogo</span></span>|[<span data-ttu-id="5e0fa-122">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5e0fa-122">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5e0fa-123">在公司门户应用中显示的徽标图像，徽标后有浅色背景。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-123">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="5e0fa-124">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="5e0fa-124">darkBackgroundLogo</span></span>|[<span data-ttu-id="5e0fa-125">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5e0fa-125">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5e0fa-126">在公司门户应用中显示的徽标图像，徽标后有深色背景。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-126">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="5e0fa-127">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="5e0fa-127">showNameNextToLogo</span></span>|<span data-ttu-id="5e0fa-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="5e0fa-128">Boolean</span></span>|<span data-ttu-id="5e0fa-129">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-129">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="5e0fa-130">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="5e0fa-130">landingPageCustomizedImage</span></span>|[<span data-ttu-id="5e0fa-131">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5e0fa-131">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5e0fa-132">在公司门户应用登录页中显示的自定义图像</span><span class="sxs-lookup"><span data-stu-id="5e0fa-132">Customized image displayed in Company Portal app landing page</span></span>|
|<span data-ttu-id="5e0fa-133">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="5e0fa-133">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="5e0fa-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="5e0fa-134">Boolean</span></span>|<span data-ttu-id="5e0fa-135">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-135">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="5e0fa-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5e0fa-136">roleScopeTagIds</span></span>|<span data-ttu-id="5e0fa-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="5e0fa-137">String collection</span></span>|<span data-ttu-id="5e0fa-138">分配给默认品牌配置文件的作用域标记列表</span><span class="sxs-lookup"><span data-stu-id="5e0fa-138">List of scope tags assigned to the default branding profile</span></span>|
|<span data-ttu-id="5e0fa-139">contactITName</span><span class="sxs-lookup"><span data-stu-id="5e0fa-139">contactITName</span></span>|<span data-ttu-id="5e0fa-140">String</span><span class="sxs-lookup"><span data-stu-id="5e0fa-140">String</span></span>|<span data-ttu-id="5e0fa-141">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-141">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="5e0fa-142">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="5e0fa-142">contactITPhoneNumber</span></span>|<span data-ttu-id="5e0fa-143">String</span><span class="sxs-lookup"><span data-stu-id="5e0fa-143">String</span></span>|<span data-ttu-id="5e0fa-144">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-144">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="5e0fa-145">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="5e0fa-145">contactITEmailAddress</span></span>|<span data-ttu-id="5e0fa-146">String</span><span class="sxs-lookup"><span data-stu-id="5e0fa-146">String</span></span>|<span data-ttu-id="5e0fa-147">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-147">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="5e0fa-148">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="5e0fa-148">contactITNotes</span></span>|<span data-ttu-id="5e0fa-149">String</span><span class="sxs-lookup"><span data-stu-id="5e0fa-149">String</span></span>|<span data-ttu-id="5e0fa-150">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-150">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="5e0fa-151">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="5e0fa-151">onlineSupportSiteUrl</span></span>|<span data-ttu-id="5e0fa-152">String</span><span class="sxs-lookup"><span data-stu-id="5e0fa-152">String</span></span>|<span data-ttu-id="5e0fa-153">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-153">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="5e0fa-154">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="5e0fa-154">onlineSupportSiteName</span></span>|<span data-ttu-id="5e0fa-155">String</span><span class="sxs-lookup"><span data-stu-id="5e0fa-155">String</span></span>|<span data-ttu-id="5e0fa-156">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-156">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="5e0fa-157">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="5e0fa-157">privacyUrl</span></span>|<span data-ttu-id="5e0fa-158">String</span><span class="sxs-lookup"><span data-stu-id="5e0fa-158">String</span></span>|<span data-ttu-id="5e0fa-159">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-159">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="5e0fa-160">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="5e0fa-160">customPrivacyMessage</span></span>|<span data-ttu-id="5e0fa-161">String</span><span class="sxs-lookup"><span data-stu-id="5e0fa-161">String</span></span>|<span data-ttu-id="5e0fa-162">用于解释组织无法在托管设备上看到或执行的操作的自定义隐私邮件。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-162">The custom privacy message used to explain what the organization can’t see or do on managed devices.</span></span>|
|<span data-ttu-id="5e0fa-163">customCantSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="5e0fa-163">customCantSeePrivacyMessage</span></span>|<span data-ttu-id="5e0fa-164">String</span><span class="sxs-lookup"><span data-stu-id="5e0fa-164">String</span></span>|<span data-ttu-id="5e0fa-165">用于解释组织无法在托管设备上看到或执行的操作的自定义隐私邮件。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-165">The custom privacy message used to explain what the organization can’t see or do on managed devices.</span></span>|
|<span data-ttu-id="5e0fa-166">customCanSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="5e0fa-166">customCanSeePrivacyMessage</span></span>|<span data-ttu-id="5e0fa-167">String</span><span class="sxs-lookup"><span data-stu-id="5e0fa-167">String</span></span>|<span data-ttu-id="5e0fa-168">自定义隐私邮件，用于解释组织可以在托管设备上看到和执行的操作。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-168">The custom privacy message used to explain what the organization can see and do on managed devices.</span></span>|
|<span data-ttu-id="5e0fa-169">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="5e0fa-169">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="5e0fa-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e0fa-170">Boolean</span></span>|<span data-ttu-id="5e0fa-171">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "删除设备" 操作。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-171">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="5e0fa-172">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="5e0fa-172">isFactoryResetDisabled</span></span>|<span data-ttu-id="5e0fa-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e0fa-173">Boolean</span></span>|<span data-ttu-id="5e0fa-174">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "Factory 重置" 操作。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-174">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="5e0fa-175">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="5e0fa-175">companyPortalBlockedActions</span></span>|<span data-ttu-id="5e0fa-176">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5e0fa-176">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="5e0fa-177">按平台和设备所有权类型对公司门户的阻止操作的集合。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-177">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="5e0fa-178">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="5e0fa-178">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="5e0fa-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e0fa-179">Boolean</span></span>|<span data-ttu-id="5e0fa-180">指示是否将在公司门户中显示 AzureAD 企业应用程序的布尔值</span><span class="sxs-lookup"><span data-stu-id="5e0fa-180">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="5e0fa-181">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="5e0fa-181">showOfficeWebApps</span></span>|<span data-ttu-id="5e0fa-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e0fa-182">Boolean</span></span>|<span data-ttu-id="5e0fa-183">指示 Office WebApps 是否将显示在公司门户中的布尔值</span><span class="sxs-lookup"><span data-stu-id="5e0fa-183">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="5e0fa-184">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="5e0fa-184">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="5e0fa-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e0fa-185">Boolean</span></span>|<span data-ttu-id="5e0fa-186">一个 Boolean 类型的值，该值指示当用户的设备所有权类型从个人更改为公司时是否向用户发送推送通知</span><span class="sxs-lookup"><span data-stu-id="5e0fa-186">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="5e0fa-187">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="5e0fa-187">enrollmentAvailability</span></span>|[<span data-ttu-id="5e0fa-188">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="5e0fa-188">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="5e0fa-189">向最终用户显示的自定义设备注册流。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-189">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="5e0fa-190">可取值为：`availableWithPrompts`、`availableWithoutPrompts`、`unavailable`。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-190">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="5e0fa-191">disableClientTelemetry</span><span class="sxs-lookup"><span data-stu-id="5e0fa-191">disableClientTelemetry</span></span>|<span data-ttu-id="5e0fa-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e0fa-192">Boolean</span></span>|<span data-ttu-id="5e0fa-193">适用于从所有客户端发送到 Intune 服务的遥测。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-193">Applies to telemetry sent from all clients to the Intune service.</span></span> <span data-ttu-id="5e0fa-194">如果禁用此设置，则会关闭客户端中的所有主动故障排除和问题警告，并且遥测设置将显示为非活动或对设备用户隐藏。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-194">When disabled, all proactive troubleshooting and issue warnings within the client are turned off, and telemetry settings appear inactive or hidden to the device user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e0fa-195">关系</span><span class="sxs-lookup"><span data-stu-id="5e0fa-195">Relationships</span></span>
<span data-ttu-id="5e0fa-196">无</span><span class="sxs-lookup"><span data-stu-id="5e0fa-196">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e0fa-197">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e0fa-197">JSON Representation</span></span>
<span data-ttu-id="5e0fa-198">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e0fa-198">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showNameNextToLogo": true,
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showDisplayNameNextToLogo": true,
  "roleScopeTagIds": [
    "String"
  ],
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "privacyUrl": "String",
  "customPrivacyMessage": "String",
  "customCantSeePrivacyMessage": "String",
  "customCanSeePrivacyMessage": "String",
  "isRemoveDeviceDisabled": true,
  "isFactoryResetDisabled": true,
  "companyPortalBlockedActions": [
    {
      "@odata.type": "microsoft.graph.companyPortalBlockedAction",
      "platform": "String",
      "ownerType": "String",
      "action": "String"
    }
  ],
  "showAzureADEnterpriseApps": true,
  "showOfficeWebApps": true,
  "sendDeviceOwnershipChangePushNotification": true,
  "enrollmentAvailability": "String",
  "disableClientTelemetry": true
}
```






