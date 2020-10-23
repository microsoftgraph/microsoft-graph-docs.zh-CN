---
title: intuneBrand 资源类型
description: intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a839029e79bb88fc134054a5732c6d1e2ab21127
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733257"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="b76f2-103">intuneBrand 资源类型</span><span class="sxs-lookup"><span data-stu-id="b76f2-103">intuneBrand resource type</span></span>

<span data-ttu-id="b76f2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b76f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b76f2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b76f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b76f2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b76f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b76f2-107">intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="b76f2-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="b76f2-108">属性</span><span class="sxs-lookup"><span data-stu-id="b76f2-108">Properties</span></span>
|<span data-ttu-id="b76f2-109">属性</span><span class="sxs-lookup"><span data-stu-id="b76f2-109">Property</span></span>|<span data-ttu-id="b76f2-110">类型</span><span class="sxs-lookup"><span data-stu-id="b76f2-110">Type</span></span>|<span data-ttu-id="b76f2-111">说明</span><span class="sxs-lookup"><span data-stu-id="b76f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b76f2-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b76f2-112">displayName</span></span>|<span data-ttu-id="b76f2-113">String</span><span class="sxs-lookup"><span data-stu-id="b76f2-113">String</span></span>|<span data-ttu-id="b76f2-114">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="b76f2-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="b76f2-115">themeColor</span><span class="sxs-lookup"><span data-stu-id="b76f2-115">themeColor</span></span>|[<span data-ttu-id="b76f2-116">rgbColor</span><span class="sxs-lookup"><span data-stu-id="b76f2-116">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="b76f2-117">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="b76f2-117">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="b76f2-118">showLogo</span><span class="sxs-lookup"><span data-stu-id="b76f2-118">showLogo</span></span>|<span data-ttu-id="b76f2-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="b76f2-119">Boolean</span></span>|<span data-ttu-id="b76f2-120">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="b76f2-120">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="b76f2-121">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="b76f2-121">lightBackgroundLogo</span></span>|[<span data-ttu-id="b76f2-122">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b76f2-122">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b76f2-123">在公司门户应用中显示的徽标图像，徽标后有浅色背景。</span><span class="sxs-lookup"><span data-stu-id="b76f2-123">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="b76f2-124">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="b76f2-124">darkBackgroundLogo</span></span>|[<span data-ttu-id="b76f2-125">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b76f2-125">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b76f2-126">在公司门户应用中显示的徽标图像，徽标后有深色背景。</span><span class="sxs-lookup"><span data-stu-id="b76f2-126">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="b76f2-127">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="b76f2-127">showNameNextToLogo</span></span>|<span data-ttu-id="b76f2-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="b76f2-128">Boolean</span></span>|<span data-ttu-id="b76f2-129">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="b76f2-129">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="b76f2-130">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="b76f2-130">landingPageCustomizedImage</span></span>|[<span data-ttu-id="b76f2-131">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b76f2-131">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b76f2-132">在公司门户应用登录页中显示的自定义图像</span><span class="sxs-lookup"><span data-stu-id="b76f2-132">Customized image displayed in Company Portal app landing page</span></span>|
|<span data-ttu-id="b76f2-133">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="b76f2-133">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="b76f2-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="b76f2-134">Boolean</span></span>|<span data-ttu-id="b76f2-135">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="b76f2-135">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="b76f2-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b76f2-136">roleScopeTagIds</span></span>|<span data-ttu-id="b76f2-137">String collection</span><span class="sxs-lookup"><span data-stu-id="b76f2-137">String collection</span></span>|<span data-ttu-id="b76f2-138">分配给默认品牌配置文件的作用域标记列表</span><span class="sxs-lookup"><span data-stu-id="b76f2-138">List of scope tags assigned to the default branding profile</span></span>|
|<span data-ttu-id="b76f2-139">contactITName</span><span class="sxs-lookup"><span data-stu-id="b76f2-139">contactITName</span></span>|<span data-ttu-id="b76f2-140">String</span><span class="sxs-lookup"><span data-stu-id="b76f2-140">String</span></span>|<span data-ttu-id="b76f2-141">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="b76f2-141">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="b76f2-142">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="b76f2-142">contactITPhoneNumber</span></span>|<span data-ttu-id="b76f2-143">String</span><span class="sxs-lookup"><span data-stu-id="b76f2-143">String</span></span>|<span data-ttu-id="b76f2-144">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="b76f2-144">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="b76f2-145">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="b76f2-145">contactITEmailAddress</span></span>|<span data-ttu-id="b76f2-146">String</span><span class="sxs-lookup"><span data-stu-id="b76f2-146">String</span></span>|<span data-ttu-id="b76f2-147">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b76f2-147">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="b76f2-148">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="b76f2-148">contactITNotes</span></span>|<span data-ttu-id="b76f2-149">String</span><span class="sxs-lookup"><span data-stu-id="b76f2-149">String</span></span>|<span data-ttu-id="b76f2-150">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="b76f2-150">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="b76f2-151">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="b76f2-151">onlineSupportSiteUrl</span></span>|<span data-ttu-id="b76f2-152">String</span><span class="sxs-lookup"><span data-stu-id="b76f2-152">String</span></span>|<span data-ttu-id="b76f2-153">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="b76f2-153">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="b76f2-154">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="b76f2-154">onlineSupportSiteName</span></span>|<span data-ttu-id="b76f2-155">String</span><span class="sxs-lookup"><span data-stu-id="b76f2-155">String</span></span>|<span data-ttu-id="b76f2-156">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="b76f2-156">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="b76f2-157">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="b76f2-157">privacyUrl</span></span>|<span data-ttu-id="b76f2-158">String</span><span class="sxs-lookup"><span data-stu-id="b76f2-158">String</span></span>|<span data-ttu-id="b76f2-159">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="b76f2-159">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="b76f2-160">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="b76f2-160">customPrivacyMessage</span></span>|<span data-ttu-id="b76f2-161">String</span><span class="sxs-lookup"><span data-stu-id="b76f2-161">String</span></span>|<span data-ttu-id="b76f2-162">用于解释组织无法在托管设备上看到或执行的操作的自定义隐私邮件。</span><span class="sxs-lookup"><span data-stu-id="b76f2-162">The custom privacy message used to explain what the organization can’t see or do on managed devices.</span></span>|
|<span data-ttu-id="b76f2-163">customCantSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="b76f2-163">customCantSeePrivacyMessage</span></span>|<span data-ttu-id="b76f2-164">String</span><span class="sxs-lookup"><span data-stu-id="b76f2-164">String</span></span>|<span data-ttu-id="b76f2-165">用于解释组织无法在托管设备上看到或执行的操作的自定义隐私邮件。</span><span class="sxs-lookup"><span data-stu-id="b76f2-165">The custom privacy message used to explain what the organization can’t see or do on managed devices.</span></span>|
|<span data-ttu-id="b76f2-166">customCanSeePrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="b76f2-166">customCanSeePrivacyMessage</span></span>|<span data-ttu-id="b76f2-167">String</span><span class="sxs-lookup"><span data-stu-id="b76f2-167">String</span></span>|<span data-ttu-id="b76f2-168">自定义隐私邮件，用于解释组织可以在托管设备上看到和执行的操作。</span><span class="sxs-lookup"><span data-stu-id="b76f2-168">The custom privacy message used to explain what the organization can see and do on managed devices.</span></span>|
|<span data-ttu-id="b76f2-169">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="b76f2-169">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="b76f2-170">布尔</span><span class="sxs-lookup"><span data-stu-id="b76f2-170">Boolean</span></span>|<span data-ttu-id="b76f2-171">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "删除设备" 操作。</span><span class="sxs-lookup"><span data-stu-id="b76f2-171">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="b76f2-172">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="b76f2-172">isFactoryResetDisabled</span></span>|<span data-ttu-id="b76f2-173">布尔</span><span class="sxs-lookup"><span data-stu-id="b76f2-173">Boolean</span></span>|<span data-ttu-id="b76f2-174">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "Factory 重置" 操作。</span><span class="sxs-lookup"><span data-stu-id="b76f2-174">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="b76f2-175">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="b76f2-175">companyPortalBlockedActions</span></span>|<span data-ttu-id="b76f2-176">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b76f2-176">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="b76f2-177">按平台和设备所有权类型对公司门户的阻止操作的集合。</span><span class="sxs-lookup"><span data-stu-id="b76f2-177">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="b76f2-178">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="b76f2-178">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="b76f2-179">布尔</span><span class="sxs-lookup"><span data-stu-id="b76f2-179">Boolean</span></span>|<span data-ttu-id="b76f2-180">指示是否将在公司门户中显示 AzureAD 企业应用程序的布尔值</span><span class="sxs-lookup"><span data-stu-id="b76f2-180">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="b76f2-181">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="b76f2-181">showOfficeWebApps</span></span>|<span data-ttu-id="b76f2-182">布尔</span><span class="sxs-lookup"><span data-stu-id="b76f2-182">Boolean</span></span>|<span data-ttu-id="b76f2-183">指示 Office WebApps 是否将显示在公司门户中的布尔值</span><span class="sxs-lookup"><span data-stu-id="b76f2-183">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="b76f2-184">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="b76f2-184">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="b76f2-185">布尔</span><span class="sxs-lookup"><span data-stu-id="b76f2-185">Boolean</span></span>|<span data-ttu-id="b76f2-186">一个 Boolean 类型的值，该值指示当用户的设备所有权类型从个人更改为公司时是否向用户发送推送通知</span><span class="sxs-lookup"><span data-stu-id="b76f2-186">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="b76f2-187">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="b76f2-187">enrollmentAvailability</span></span>|[<span data-ttu-id="b76f2-188">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="b76f2-188">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="b76f2-189">向最终用户显示的自定义设备注册流。</span><span class="sxs-lookup"><span data-stu-id="b76f2-189">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="b76f2-190">可取值为：`availableWithPrompts`、`availableWithoutPrompts`、`unavailable`。</span><span class="sxs-lookup"><span data-stu-id="b76f2-190">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|
|<span data-ttu-id="b76f2-191">disableClientTelemetry</span><span class="sxs-lookup"><span data-stu-id="b76f2-191">disableClientTelemetry</span></span>|<span data-ttu-id="b76f2-192">布尔</span><span class="sxs-lookup"><span data-stu-id="b76f2-192">Boolean</span></span>|<span data-ttu-id="b76f2-193">适用于从所有客户端发送到 Intune 服务的遥测。</span><span class="sxs-lookup"><span data-stu-id="b76f2-193">Applies to telemetry sent from all clients to the Intune service.</span></span> <span data-ttu-id="b76f2-194">如果禁用此设置，则会关闭客户端中的所有主动故障排除和问题警告，并且遥测设置将显示为非活动或对设备用户隐藏。</span><span class="sxs-lookup"><span data-stu-id="b76f2-194">When disabled, all proactive troubleshooting and issue warnings within the client are turned off, and telemetry settings appear inactive or hidden to the device user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b76f2-195">关系</span><span class="sxs-lookup"><span data-stu-id="b76f2-195">Relationships</span></span>
<span data-ttu-id="b76f2-196">无</span><span class="sxs-lookup"><span data-stu-id="b76f2-196">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b76f2-197">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b76f2-197">JSON Representation</span></span>
<span data-ttu-id="b76f2-198">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b76f2-198">Here is a JSON representation of the resource.</span></span>
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





