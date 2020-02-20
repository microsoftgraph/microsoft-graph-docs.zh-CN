---
title: intuneBrand 资源类型
description: intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1b6b913f115ee73566a688a90355377a7ff495eb
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160345"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="10134-103">intuneBrand 资源类型</span><span class="sxs-lookup"><span data-stu-id="10134-103">intuneBrand resource type</span></span>

> <span data-ttu-id="10134-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="10134-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10134-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10134-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10134-106">intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="10134-106">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="10134-107">属性</span><span class="sxs-lookup"><span data-stu-id="10134-107">Properties</span></span>
|<span data-ttu-id="10134-108">属性</span><span class="sxs-lookup"><span data-stu-id="10134-108">Property</span></span>|<span data-ttu-id="10134-109">类型</span><span class="sxs-lookup"><span data-stu-id="10134-109">Type</span></span>|<span data-ttu-id="10134-110">说明</span><span class="sxs-lookup"><span data-stu-id="10134-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10134-111">displayName</span><span class="sxs-lookup"><span data-stu-id="10134-111">displayName</span></span>|<span data-ttu-id="10134-112">String</span><span class="sxs-lookup"><span data-stu-id="10134-112">String</span></span>|<span data-ttu-id="10134-113">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="10134-113">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="10134-114">themeColor</span><span class="sxs-lookup"><span data-stu-id="10134-114">themeColor</span></span>|[<span data-ttu-id="10134-115">rgbColor</span><span class="sxs-lookup"><span data-stu-id="10134-115">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="10134-116">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="10134-116">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="10134-117">showLogo</span><span class="sxs-lookup"><span data-stu-id="10134-117">showLogo</span></span>|<span data-ttu-id="10134-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="10134-118">Boolean</span></span>|<span data-ttu-id="10134-119">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="10134-119">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="10134-120">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="10134-120">lightBackgroundLogo</span></span>|[<span data-ttu-id="10134-121">mimeContent</span><span class="sxs-lookup"><span data-stu-id="10134-121">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="10134-122">在公司门户应用中显示的徽标图像，徽标后有浅色背景。</span><span class="sxs-lookup"><span data-stu-id="10134-122">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="10134-123">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="10134-123">darkBackgroundLogo</span></span>|[<span data-ttu-id="10134-124">mimeContent</span><span class="sxs-lookup"><span data-stu-id="10134-124">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="10134-125">在公司门户应用中显示的徽标图像，徽标后有深色背景。</span><span class="sxs-lookup"><span data-stu-id="10134-125">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="10134-126">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="10134-126">showNameNextToLogo</span></span>|<span data-ttu-id="10134-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="10134-127">Boolean</span></span>|<span data-ttu-id="10134-128">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="10134-128">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="10134-129">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="10134-129">landingPageCustomizedImage</span></span>|[<span data-ttu-id="10134-130">mimeContent</span><span class="sxs-lookup"><span data-stu-id="10134-130">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="10134-131">在公司门户应用登录页中显示的自定义图像</span><span class="sxs-lookup"><span data-stu-id="10134-131">Customized image displayed in Company Portal app landing page</span></span>|
|<span data-ttu-id="10134-132">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="10134-132">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="10134-133">布尔值</span><span class="sxs-lookup"><span data-stu-id="10134-133">Boolean</span></span>|<span data-ttu-id="10134-134">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="10134-134">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="10134-135">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="10134-135">roleScopeTagIds</span></span>|<span data-ttu-id="10134-136">String collection</span><span class="sxs-lookup"><span data-stu-id="10134-136">String collection</span></span>|<span data-ttu-id="10134-137">分配给默认品牌配置文件的作用域标记列表</span><span class="sxs-lookup"><span data-stu-id="10134-137">List of scope tags assigned to the default branding profile</span></span>|
|<span data-ttu-id="10134-138">contactITName</span><span class="sxs-lookup"><span data-stu-id="10134-138">contactITName</span></span>|<span data-ttu-id="10134-139">String</span><span class="sxs-lookup"><span data-stu-id="10134-139">String</span></span>|<span data-ttu-id="10134-140">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="10134-140">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="10134-141">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="10134-141">contactITPhoneNumber</span></span>|<span data-ttu-id="10134-142">String</span><span class="sxs-lookup"><span data-stu-id="10134-142">String</span></span>|<span data-ttu-id="10134-143">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="10134-143">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="10134-144">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="10134-144">contactITEmailAddress</span></span>|<span data-ttu-id="10134-145">String</span><span class="sxs-lookup"><span data-stu-id="10134-145">String</span></span>|<span data-ttu-id="10134-146">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="10134-146">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="10134-147">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="10134-147">contactITNotes</span></span>|<span data-ttu-id="10134-148">String</span><span class="sxs-lookup"><span data-stu-id="10134-148">String</span></span>|<span data-ttu-id="10134-149">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="10134-149">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="10134-150">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="10134-150">onlineSupportSiteUrl</span></span>|<span data-ttu-id="10134-151">String</span><span class="sxs-lookup"><span data-stu-id="10134-151">String</span></span>|<span data-ttu-id="10134-152">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="10134-152">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="10134-153">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="10134-153">onlineSupportSiteName</span></span>|<span data-ttu-id="10134-154">String</span><span class="sxs-lookup"><span data-stu-id="10134-154">String</span></span>|<span data-ttu-id="10134-155">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="10134-155">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="10134-156">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="10134-156">privacyUrl</span></span>|<span data-ttu-id="10134-157">String</span><span class="sxs-lookup"><span data-stu-id="10134-157">String</span></span>|<span data-ttu-id="10134-158">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="10134-158">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="10134-159">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="10134-159">customPrivacyMessage</span></span>|<span data-ttu-id="10134-160">String</span><span class="sxs-lookup"><span data-stu-id="10134-160">String</span></span>|<span data-ttu-id="10134-161">自定义隐私邮件。</span><span class="sxs-lookup"><span data-stu-id="10134-161">Custom privacy message.</span></span>|
|<span data-ttu-id="10134-162">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="10134-162">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="10134-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="10134-163">Boolean</span></span>|<span data-ttu-id="10134-164">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "删除设备" 操作。</span><span class="sxs-lookup"><span data-stu-id="10134-164">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="10134-165">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="10134-165">isFactoryResetDisabled</span></span>|<span data-ttu-id="10134-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="10134-166">Boolean</span></span>|<span data-ttu-id="10134-167">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "Factory 重置" 操作。</span><span class="sxs-lookup"><span data-stu-id="10134-167">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="10134-168">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="10134-168">companyPortalBlockedActions</span></span>|<span data-ttu-id="10134-169">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="10134-169">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="10134-170">按平台和设备所有权类型对公司门户的阻止操作的集合。</span><span class="sxs-lookup"><span data-stu-id="10134-170">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="10134-171">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="10134-171">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="10134-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="10134-172">Boolean</span></span>|<span data-ttu-id="10134-173">指示是否将在公司门户中显示 AzureAD 企业应用程序的布尔值</span><span class="sxs-lookup"><span data-stu-id="10134-173">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="10134-174">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="10134-174">showOfficeWebApps</span></span>|<span data-ttu-id="10134-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="10134-175">Boolean</span></span>|<span data-ttu-id="10134-176">指示 Office WebApps 是否将显示在公司门户中的布尔值</span><span class="sxs-lookup"><span data-stu-id="10134-176">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="10134-177">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="10134-177">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="10134-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="10134-178">Boolean</span></span>|<span data-ttu-id="10134-179">一个 Boolean 类型的值，该值指示当用户的设备所有权类型从个人更改为公司时是否向用户发送推送通知</span><span class="sxs-lookup"><span data-stu-id="10134-179">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="10134-180">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="10134-180">enrollmentAvailability</span></span>|[<span data-ttu-id="10134-181">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="10134-181">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="10134-182">向最终用户显示的自定义设备注册流。</span><span class="sxs-lookup"><span data-stu-id="10134-182">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="10134-183">可取值为：`availableWithPrompts`、`availableWithoutPrompts`、`unavailable`。</span><span class="sxs-lookup"><span data-stu-id="10134-183">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10134-184">关系</span><span class="sxs-lookup"><span data-stu-id="10134-184">Relationships</span></span>
<span data-ttu-id="10134-185">无</span><span class="sxs-lookup"><span data-stu-id="10134-185">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10134-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10134-186">JSON Representation</span></span>
<span data-ttu-id="10134-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10134-187">Here is a JSON representation of the resource.</span></span>
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
  "enrollmentAvailability": "String"
}
```



