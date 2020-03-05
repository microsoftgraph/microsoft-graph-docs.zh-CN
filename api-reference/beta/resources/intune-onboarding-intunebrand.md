---
title: intuneBrand 资源类型
description: intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d31b4ab9931fd0693776646161528aa73e31205e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527728"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="3a366-103">intuneBrand 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a366-103">intuneBrand resource type</span></span>

<span data-ttu-id="3a366-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3a366-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a366-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3a366-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a366-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3a366-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a366-107">intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="3a366-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="3a366-108">属性</span><span class="sxs-lookup"><span data-stu-id="3a366-108">Properties</span></span>
|<span data-ttu-id="3a366-109">属性</span><span class="sxs-lookup"><span data-stu-id="3a366-109">Property</span></span>|<span data-ttu-id="3a366-110">类型</span><span class="sxs-lookup"><span data-stu-id="3a366-110">Type</span></span>|<span data-ttu-id="3a366-111">说明</span><span class="sxs-lookup"><span data-stu-id="3a366-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a366-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3a366-112">displayName</span></span>|<span data-ttu-id="3a366-113">String</span><span class="sxs-lookup"><span data-stu-id="3a366-113">String</span></span>|<span data-ttu-id="3a366-114">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="3a366-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="3a366-115">themeColor</span><span class="sxs-lookup"><span data-stu-id="3a366-115">themeColor</span></span>|[<span data-ttu-id="3a366-116">rgbColor</span><span class="sxs-lookup"><span data-stu-id="3a366-116">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="3a366-117">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="3a366-117">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="3a366-118">showLogo</span><span class="sxs-lookup"><span data-stu-id="3a366-118">showLogo</span></span>|<span data-ttu-id="3a366-119">布尔</span><span class="sxs-lookup"><span data-stu-id="3a366-119">Boolean</span></span>|<span data-ttu-id="3a366-120">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="3a366-120">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="3a366-121">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="3a366-121">lightBackgroundLogo</span></span>|[<span data-ttu-id="3a366-122">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3a366-122">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3a366-123">在公司门户应用中显示的徽标图像，徽标后有浅色背景。</span><span class="sxs-lookup"><span data-stu-id="3a366-123">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="3a366-124">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="3a366-124">darkBackgroundLogo</span></span>|[<span data-ttu-id="3a366-125">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3a366-125">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3a366-126">在公司门户应用中显示的徽标图像，徽标后有深色背景。</span><span class="sxs-lookup"><span data-stu-id="3a366-126">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="3a366-127">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="3a366-127">showNameNextToLogo</span></span>|<span data-ttu-id="3a366-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="3a366-128">Boolean</span></span>|<span data-ttu-id="3a366-129">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="3a366-129">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="3a366-130">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="3a366-130">landingPageCustomizedImage</span></span>|[<span data-ttu-id="3a366-131">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3a366-131">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3a366-132">在公司门户应用登录页中显示的自定义图像</span><span class="sxs-lookup"><span data-stu-id="3a366-132">Customized image displayed in Company Portal app landing page</span></span>|
|<span data-ttu-id="3a366-133">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="3a366-133">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="3a366-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="3a366-134">Boolean</span></span>|<span data-ttu-id="3a366-135">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="3a366-135">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="3a366-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3a366-136">roleScopeTagIds</span></span>|<span data-ttu-id="3a366-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="3a366-137">String collection</span></span>|<span data-ttu-id="3a366-138">分配给默认品牌配置文件的作用域标记列表</span><span class="sxs-lookup"><span data-stu-id="3a366-138">List of scope tags assigned to the default branding profile</span></span>|
|<span data-ttu-id="3a366-139">contactITName</span><span class="sxs-lookup"><span data-stu-id="3a366-139">contactITName</span></span>|<span data-ttu-id="3a366-140">String</span><span class="sxs-lookup"><span data-stu-id="3a366-140">String</span></span>|<span data-ttu-id="3a366-141">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="3a366-141">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="3a366-142">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="3a366-142">contactITPhoneNumber</span></span>|<span data-ttu-id="3a366-143">String</span><span class="sxs-lookup"><span data-stu-id="3a366-143">String</span></span>|<span data-ttu-id="3a366-144">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="3a366-144">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="3a366-145">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="3a366-145">contactITEmailAddress</span></span>|<span data-ttu-id="3a366-146">String</span><span class="sxs-lookup"><span data-stu-id="3a366-146">String</span></span>|<span data-ttu-id="3a366-147">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="3a366-147">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="3a366-148">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="3a366-148">contactITNotes</span></span>|<span data-ttu-id="3a366-149">String</span><span class="sxs-lookup"><span data-stu-id="3a366-149">String</span></span>|<span data-ttu-id="3a366-150">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="3a366-150">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="3a366-151">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="3a366-151">onlineSupportSiteUrl</span></span>|<span data-ttu-id="3a366-152">String</span><span class="sxs-lookup"><span data-stu-id="3a366-152">String</span></span>|<span data-ttu-id="3a366-153">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="3a366-153">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="3a366-154">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="3a366-154">onlineSupportSiteName</span></span>|<span data-ttu-id="3a366-155">String</span><span class="sxs-lookup"><span data-stu-id="3a366-155">String</span></span>|<span data-ttu-id="3a366-156">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="3a366-156">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="3a366-157">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="3a366-157">privacyUrl</span></span>|<span data-ttu-id="3a366-158">String</span><span class="sxs-lookup"><span data-stu-id="3a366-158">String</span></span>|<span data-ttu-id="3a366-159">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="3a366-159">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="3a366-160">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="3a366-160">customPrivacyMessage</span></span>|<span data-ttu-id="3a366-161">String</span><span class="sxs-lookup"><span data-stu-id="3a366-161">String</span></span>|<span data-ttu-id="3a366-162">自定义隐私邮件。</span><span class="sxs-lookup"><span data-stu-id="3a366-162">Custom privacy message.</span></span>|
|<span data-ttu-id="3a366-163">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="3a366-163">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="3a366-164">布尔</span><span class="sxs-lookup"><span data-stu-id="3a366-164">Boolean</span></span>|<span data-ttu-id="3a366-165">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "删除设备" 操作。</span><span class="sxs-lookup"><span data-stu-id="3a366-165">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="3a366-166">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="3a366-166">isFactoryResetDisabled</span></span>|<span data-ttu-id="3a366-167">布尔</span><span class="sxs-lookup"><span data-stu-id="3a366-167">Boolean</span></span>|<span data-ttu-id="3a366-168">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "Factory 重置" 操作。</span><span class="sxs-lookup"><span data-stu-id="3a366-168">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="3a366-169">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="3a366-169">companyPortalBlockedActions</span></span>|<span data-ttu-id="3a366-170">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="3a366-170">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="3a366-171">按平台和设备所有权类型对公司门户的阻止操作的集合。</span><span class="sxs-lookup"><span data-stu-id="3a366-171">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="3a366-172">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="3a366-172">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="3a366-173">布尔</span><span class="sxs-lookup"><span data-stu-id="3a366-173">Boolean</span></span>|<span data-ttu-id="3a366-174">指示是否将在公司门户中显示 AzureAD 企业应用程序的布尔值</span><span class="sxs-lookup"><span data-stu-id="3a366-174">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="3a366-175">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="3a366-175">showOfficeWebApps</span></span>|<span data-ttu-id="3a366-176">布尔</span><span class="sxs-lookup"><span data-stu-id="3a366-176">Boolean</span></span>|<span data-ttu-id="3a366-177">指示 Office WebApps 是否将显示在公司门户中的布尔值</span><span class="sxs-lookup"><span data-stu-id="3a366-177">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="3a366-178">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="3a366-178">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="3a366-179">布尔</span><span class="sxs-lookup"><span data-stu-id="3a366-179">Boolean</span></span>|<span data-ttu-id="3a366-180">一个 Boolean 类型的值，该值指示当用户的设备所有权类型从个人更改为公司时是否向用户发送推送通知</span><span class="sxs-lookup"><span data-stu-id="3a366-180">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="3a366-181">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="3a366-181">enrollmentAvailability</span></span>|[<span data-ttu-id="3a366-182">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="3a366-182">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="3a366-183">向最终用户显示的自定义设备注册流。</span><span class="sxs-lookup"><span data-stu-id="3a366-183">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="3a366-184">可取值为：`availableWithPrompts`、`availableWithoutPrompts`、`unavailable`。</span><span class="sxs-lookup"><span data-stu-id="3a366-184">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a366-185">关系</span><span class="sxs-lookup"><span data-stu-id="3a366-185">Relationships</span></span>
<span data-ttu-id="3a366-186">无</span><span class="sxs-lookup"><span data-stu-id="3a366-186">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a366-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a366-187">JSON Representation</span></span>
<span data-ttu-id="3a366-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a366-188">Here is a JSON representation of the resource.</span></span>
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



