---
title: intuneBrand 资源类型
description: intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 92b706fee0e1b0a6af0d877d040339416d9b78c4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455572"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="806c2-103">intuneBrand 资源类型</span><span class="sxs-lookup"><span data-stu-id="806c2-103">intuneBrand resource type</span></span>

<span data-ttu-id="806c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="806c2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="806c2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="806c2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="806c2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="806c2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="806c2-107">intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="806c2-107">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="806c2-108">属性</span><span class="sxs-lookup"><span data-stu-id="806c2-108">Properties</span></span>
|<span data-ttu-id="806c2-109">属性</span><span class="sxs-lookup"><span data-stu-id="806c2-109">Property</span></span>|<span data-ttu-id="806c2-110">类型</span><span class="sxs-lookup"><span data-stu-id="806c2-110">Type</span></span>|<span data-ttu-id="806c2-111">说明</span><span class="sxs-lookup"><span data-stu-id="806c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="806c2-112">displayName</span><span class="sxs-lookup"><span data-stu-id="806c2-112">displayName</span></span>|<span data-ttu-id="806c2-113">String</span><span class="sxs-lookup"><span data-stu-id="806c2-113">String</span></span>|<span data-ttu-id="806c2-114">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="806c2-114">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="806c2-115">themeColor</span><span class="sxs-lookup"><span data-stu-id="806c2-115">themeColor</span></span>|[<span data-ttu-id="806c2-116">rgbColor</span><span class="sxs-lookup"><span data-stu-id="806c2-116">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="806c2-117">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="806c2-117">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="806c2-118">showLogo</span><span class="sxs-lookup"><span data-stu-id="806c2-118">showLogo</span></span>|<span data-ttu-id="806c2-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="806c2-119">Boolean</span></span>|<span data-ttu-id="806c2-120">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="806c2-120">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="806c2-121">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="806c2-121">lightBackgroundLogo</span></span>|[<span data-ttu-id="806c2-122">mimeContent</span><span class="sxs-lookup"><span data-stu-id="806c2-122">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="806c2-123">在公司门户应用中显示的徽标图像，徽标后有浅色背景。</span><span class="sxs-lookup"><span data-stu-id="806c2-123">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="806c2-124">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="806c2-124">darkBackgroundLogo</span></span>|[<span data-ttu-id="806c2-125">mimeContent</span><span class="sxs-lookup"><span data-stu-id="806c2-125">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="806c2-126">在公司门户应用中显示的徽标图像，徽标后有深色背景。</span><span class="sxs-lookup"><span data-stu-id="806c2-126">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="806c2-127">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="806c2-127">showNameNextToLogo</span></span>|<span data-ttu-id="806c2-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="806c2-128">Boolean</span></span>|<span data-ttu-id="806c2-129">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="806c2-129">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="806c2-130">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="806c2-130">landingPageCustomizedImage</span></span>|[<span data-ttu-id="806c2-131">mimeContent</span><span class="sxs-lookup"><span data-stu-id="806c2-131">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="806c2-132">在公司门户应用登录页中显示的自定义图像</span><span class="sxs-lookup"><span data-stu-id="806c2-132">Customized image displayed in Company Portal app landing page</span></span>|
|<span data-ttu-id="806c2-133">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="806c2-133">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="806c2-134">布尔值</span><span class="sxs-lookup"><span data-stu-id="806c2-134">Boolean</span></span>|<span data-ttu-id="806c2-135">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="806c2-135">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="806c2-136">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="806c2-136">roleScopeTagIds</span></span>|<span data-ttu-id="806c2-137">String 集合</span><span class="sxs-lookup"><span data-stu-id="806c2-137">String collection</span></span>|<span data-ttu-id="806c2-138">分配给默认品牌配置文件的作用域标记列表</span><span class="sxs-lookup"><span data-stu-id="806c2-138">List of scope tags assigned to the default branding profile</span></span>|
|<span data-ttu-id="806c2-139">contactITName</span><span class="sxs-lookup"><span data-stu-id="806c2-139">contactITName</span></span>|<span data-ttu-id="806c2-140">String</span><span class="sxs-lookup"><span data-stu-id="806c2-140">String</span></span>|<span data-ttu-id="806c2-141">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="806c2-141">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="806c2-142">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="806c2-142">contactITPhoneNumber</span></span>|<span data-ttu-id="806c2-143">String</span><span class="sxs-lookup"><span data-stu-id="806c2-143">String</span></span>|<span data-ttu-id="806c2-144">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="806c2-144">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="806c2-145">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="806c2-145">contactITEmailAddress</span></span>|<span data-ttu-id="806c2-146">String</span><span class="sxs-lookup"><span data-stu-id="806c2-146">String</span></span>|<span data-ttu-id="806c2-147">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="806c2-147">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="806c2-148">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="806c2-148">contactITNotes</span></span>|<span data-ttu-id="806c2-149">String</span><span class="sxs-lookup"><span data-stu-id="806c2-149">String</span></span>|<span data-ttu-id="806c2-150">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="806c2-150">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="806c2-151">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="806c2-151">onlineSupportSiteUrl</span></span>|<span data-ttu-id="806c2-152">String</span><span class="sxs-lookup"><span data-stu-id="806c2-152">String</span></span>|<span data-ttu-id="806c2-153">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="806c2-153">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="806c2-154">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="806c2-154">onlineSupportSiteName</span></span>|<span data-ttu-id="806c2-155">String</span><span class="sxs-lookup"><span data-stu-id="806c2-155">String</span></span>|<span data-ttu-id="806c2-156">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="806c2-156">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="806c2-157">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="806c2-157">privacyUrl</span></span>|<span data-ttu-id="806c2-158">String</span><span class="sxs-lookup"><span data-stu-id="806c2-158">String</span></span>|<span data-ttu-id="806c2-159">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="806c2-159">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="806c2-160">customPrivacyMessage</span><span class="sxs-lookup"><span data-stu-id="806c2-160">customPrivacyMessage</span></span>|<span data-ttu-id="806c2-161">String</span><span class="sxs-lookup"><span data-stu-id="806c2-161">String</span></span>|<span data-ttu-id="806c2-162">自定义隐私邮件。</span><span class="sxs-lookup"><span data-stu-id="806c2-162">Custom privacy message.</span></span>|
|<span data-ttu-id="806c2-163">isRemoveDeviceDisabled</span><span class="sxs-lookup"><span data-stu-id="806c2-163">isRemoveDeviceDisabled</span></span>|<span data-ttu-id="806c2-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="806c2-164">Boolean</span></span>|<span data-ttu-id="806c2-165">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "删除设备" 操作。</span><span class="sxs-lookup"><span data-stu-id="806c2-165">Boolean that represents whether the adminsistrator has disabled the 'Remove Device' action on corporate owned devices.</span></span>|
|<span data-ttu-id="806c2-166">isFactoryResetDisabled</span><span class="sxs-lookup"><span data-stu-id="806c2-166">isFactoryResetDisabled</span></span>|<span data-ttu-id="806c2-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="806c2-167">Boolean</span></span>|<span data-ttu-id="806c2-168">一个 Boolean 类型的值，该值表示 adminsistrator 是否已在企业拥有的设备上禁用了 "Factory 重置" 操作。</span><span class="sxs-lookup"><span data-stu-id="806c2-168">Boolean that represents whether the adminsistrator has disabled the 'Factory Reset' action on corporate owned devices.</span></span>|
|<span data-ttu-id="806c2-169">companyPortalBlockedActions</span><span class="sxs-lookup"><span data-stu-id="806c2-169">companyPortalBlockedActions</span></span>|<span data-ttu-id="806c2-170">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md)集合</span><span class="sxs-lookup"><span data-stu-id="806c2-170">[companyPortalBlockedAction](../resources/intune-shared-companyportalblockedaction.md) collection</span></span>|<span data-ttu-id="806c2-171">按平台和设备所有权类型对公司门户的阻止操作的集合。</span><span class="sxs-lookup"><span data-stu-id="806c2-171">Collection of blocked actions on the company portal as per platform and device ownership types.</span></span>|
|<span data-ttu-id="806c2-172">showAzureADEnterpriseApps</span><span class="sxs-lookup"><span data-stu-id="806c2-172">showAzureADEnterpriseApps</span></span>|<span data-ttu-id="806c2-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="806c2-173">Boolean</span></span>|<span data-ttu-id="806c2-174">指示是否将在公司门户中显示 AzureAD 企业应用程序的布尔值</span><span class="sxs-lookup"><span data-stu-id="806c2-174">Boolean that indicates if AzureAD Enterprise Apps will be shown in Company Portal</span></span>|
|<span data-ttu-id="806c2-175">showOfficeWebApps</span><span class="sxs-lookup"><span data-stu-id="806c2-175">showOfficeWebApps</span></span>|<span data-ttu-id="806c2-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="806c2-176">Boolean</span></span>|<span data-ttu-id="806c2-177">指示 Office WebApps 是否将显示在公司门户中的布尔值</span><span class="sxs-lookup"><span data-stu-id="806c2-177">Boolean that indicates if Office WebApps will be shown in Company Portal</span></span>|
|<span data-ttu-id="806c2-178">sendDeviceOwnershipChangePushNotification</span><span class="sxs-lookup"><span data-stu-id="806c2-178">sendDeviceOwnershipChangePushNotification</span></span>|<span data-ttu-id="806c2-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="806c2-179">Boolean</span></span>|<span data-ttu-id="806c2-180">一个 Boolean 类型的值，该值指示当用户的设备所有权类型从个人更改为公司时是否向用户发送推送通知</span><span class="sxs-lookup"><span data-stu-id="806c2-180">Boolean that indicates if a push notification is sent to users when their device ownership type changes from personal to corporate</span></span>|
|<span data-ttu-id="806c2-181">enrollmentAvailability</span><span class="sxs-lookup"><span data-stu-id="806c2-181">enrollmentAvailability</span></span>|[<span data-ttu-id="806c2-182">enrollmentAvailabilityOptions</span><span class="sxs-lookup"><span data-stu-id="806c2-182">enrollmentAvailabilityOptions</span></span>](../resources/intune-shared-enrollmentavailabilityoptions.md)|<span data-ttu-id="806c2-183">向最终用户显示的自定义设备注册流。</span><span class="sxs-lookup"><span data-stu-id="806c2-183">Customized device enrollment flow displayed to the end user .</span></span> <span data-ttu-id="806c2-184">可取值为：`availableWithPrompts`、`availableWithoutPrompts`、`unavailable`。</span><span class="sxs-lookup"><span data-stu-id="806c2-184">Possible values are: `availableWithPrompts`, `availableWithoutPrompts`, `unavailable`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="806c2-185">关系</span><span class="sxs-lookup"><span data-stu-id="806c2-185">Relationships</span></span>
<span data-ttu-id="806c2-186">无</span><span class="sxs-lookup"><span data-stu-id="806c2-186">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="806c2-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="806c2-187">JSON Representation</span></span>
<span data-ttu-id="806c2-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="806c2-188">Here is a JSON representation of the resource.</span></span>
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



