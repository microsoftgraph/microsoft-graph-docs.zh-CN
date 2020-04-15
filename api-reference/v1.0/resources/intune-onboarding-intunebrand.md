---
title: intuneBrand 资源类型
description: intuneBrand 包含在自定义公司门户应用程序以及最终用户 Web 门户的外观时使用的数据。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6048e295ba0ca06fe02872aca52fdc32ae686a54
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459408"
---
# <a name="intunebrand-resource-type"></a><span data-ttu-id="834a9-103">intuneBrand 资源类型</span><span class="sxs-lookup"><span data-stu-id="834a9-103">intuneBrand resource type</span></span>

<span data-ttu-id="834a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="834a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="834a9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="834a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="834a9-106">intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="834a9-106">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>

## <a name="properties"></a><span data-ttu-id="834a9-107">属性</span><span class="sxs-lookup"><span data-stu-id="834a9-107">Properties</span></span>
|<span data-ttu-id="834a9-108">属性</span><span class="sxs-lookup"><span data-stu-id="834a9-108">Property</span></span>|<span data-ttu-id="834a9-109">类型</span><span class="sxs-lookup"><span data-stu-id="834a9-109">Type</span></span>|<span data-ttu-id="834a9-110">说明</span><span class="sxs-lookup"><span data-stu-id="834a9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="834a9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="834a9-111">displayName</span></span>|<span data-ttu-id="834a9-112">String</span><span class="sxs-lookup"><span data-stu-id="834a9-112">String</span></span>|<span data-ttu-id="834a9-113">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="834a9-113">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="834a9-114">contactITName</span><span class="sxs-lookup"><span data-stu-id="834a9-114">contactITName</span></span>|<span data-ttu-id="834a9-115">String</span><span class="sxs-lookup"><span data-stu-id="834a9-115">String</span></span>|<span data-ttu-id="834a9-116">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="834a9-116">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="834a9-117">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="834a9-117">contactITPhoneNumber</span></span>|<span data-ttu-id="834a9-118">String</span><span class="sxs-lookup"><span data-stu-id="834a9-118">String</span></span>|<span data-ttu-id="834a9-119">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="834a9-119">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="834a9-120">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="834a9-120">contactITEmailAddress</span></span>|<span data-ttu-id="834a9-121">String</span><span class="sxs-lookup"><span data-stu-id="834a9-121">String</span></span>|<span data-ttu-id="834a9-122">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="834a9-122">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="834a9-123">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="834a9-123">contactITNotes</span></span>|<span data-ttu-id="834a9-124">String</span><span class="sxs-lookup"><span data-stu-id="834a9-124">String</span></span>|<span data-ttu-id="834a9-125">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="834a9-125">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="834a9-126">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="834a9-126">privacyUrl</span></span>|<span data-ttu-id="834a9-127">String</span><span class="sxs-lookup"><span data-stu-id="834a9-127">String</span></span>|<span data-ttu-id="834a9-128">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="834a9-128">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="834a9-129">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="834a9-129">onlineSupportSiteUrl</span></span>|<span data-ttu-id="834a9-130">String</span><span class="sxs-lookup"><span data-stu-id="834a9-130">String</span></span>|<span data-ttu-id="834a9-131">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="834a9-131">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="834a9-132">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="834a9-132">onlineSupportSiteName</span></span>|<span data-ttu-id="834a9-133">String</span><span class="sxs-lookup"><span data-stu-id="834a9-133">String</span></span>|<span data-ttu-id="834a9-134">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="834a9-134">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="834a9-135">themeColor</span><span class="sxs-lookup"><span data-stu-id="834a9-135">themeColor</span></span>|[<span data-ttu-id="834a9-136">rgbColor</span><span class="sxs-lookup"><span data-stu-id="834a9-136">rgbColor</span></span>](../resources/intune-onboarding-rgbcolor.md)|<span data-ttu-id="834a9-137">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="834a9-137">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="834a9-138">showLogo</span><span class="sxs-lookup"><span data-stu-id="834a9-138">showLogo</span></span>|<span data-ttu-id="834a9-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="834a9-139">Boolean</span></span>|<span data-ttu-id="834a9-140">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="834a9-140">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="834a9-141">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="834a9-141">lightBackgroundLogo</span></span>|[<span data-ttu-id="834a9-142">mimeContent</span><span class="sxs-lookup"><span data-stu-id="834a9-142">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="834a9-143">在公司门户应用中显示的徽标图像，徽标后有浅色背景。</span><span class="sxs-lookup"><span data-stu-id="834a9-143">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="834a9-144">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="834a9-144">darkBackgroundLogo</span></span>|[<span data-ttu-id="834a9-145">mimeContent</span><span class="sxs-lookup"><span data-stu-id="834a9-145">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="834a9-146">在公司门户应用中显示的徽标图像，徽标后有深色背景。</span><span class="sxs-lookup"><span data-stu-id="834a9-146">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="834a9-147">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="834a9-147">showNameNextToLogo</span></span>|<span data-ttu-id="834a9-148">布尔值</span><span class="sxs-lookup"><span data-stu-id="834a9-148">Boolean</span></span>|<span data-ttu-id="834a9-149">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="834a9-149">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="834a9-150">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="834a9-150">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="834a9-151">布尔值</span><span class="sxs-lookup"><span data-stu-id="834a9-151">Boolean</span></span>|<span data-ttu-id="834a9-152">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="834a9-152">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="834a9-153">关系</span><span class="sxs-lookup"><span data-stu-id="834a9-153">Relationships</span></span>
<span data-ttu-id="834a9-154">无</span><span class="sxs-lookup"><span data-stu-id="834a9-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="834a9-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="834a9-155">JSON Representation</span></span>
<span data-ttu-id="834a9-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="834a9-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
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
  "showDisplayNameNextToLogo": true
}
```







