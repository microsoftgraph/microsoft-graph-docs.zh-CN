---
title: windowsPrivacyDataAccessControlItem 资源类型
description: 指定每个隐私数据类别的访问控制级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a040a24aaf4f51d5aec5b970cb2f9e4026732a7b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684881"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a><span data-ttu-id="dfdd4-103">windowsPrivacyDataAccessControlItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="dfdd4-103">windowsPrivacyDataAccessControlItem resource type</span></span>

<span data-ttu-id="dfdd4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfdd4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dfdd4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfdd4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfdd4-107">指定每个隐私数据类别的访问控制级别</span><span class="sxs-lookup"><span data-stu-id="dfdd4-107">Specify access control level per privacy data category</span></span>

## <a name="methods"></a><span data-ttu-id="dfdd4-108">Methods</span><span class="sxs-lookup"><span data-stu-id="dfdd4-108">Methods</span></span>
|<span data-ttu-id="dfdd4-109">方法</span><span class="sxs-lookup"><span data-stu-id="dfdd4-109">Method</span></span>|<span data-ttu-id="dfdd4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="dfdd4-110">Return Type</span></span>|<span data-ttu-id="dfdd4-111">说明</span><span class="sxs-lookup"><span data-stu-id="dfdd4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dfdd4-112">列出 windowsPrivacyDataAccessControlItems</span><span class="sxs-lookup"><span data-stu-id="dfdd4-112">List windowsPrivacyDataAccessControlItems</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|<span data-ttu-id="dfdd4-113">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dfdd4-113">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="dfdd4-114">列出 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-114">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>|
|[<span data-ttu-id="dfdd4-115">获取 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="dfdd4-115">Get windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[<span data-ttu-id="dfdd4-116">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="dfdd4-116">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="dfdd4-117">读取 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-117">Read properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="dfdd4-118">创建 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="dfdd4-118">Create windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[<span data-ttu-id="dfdd4-119">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="dfdd4-119">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="dfdd4-120">创建新的 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-120">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="dfdd4-121">删除 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="dfdd4-121">Delete windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|<span data-ttu-id="dfdd4-122">无</span><span class="sxs-lookup"><span data-stu-id="dfdd4-122">None</span></span>|<span data-ttu-id="dfdd4-123">删除 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-123">Deletes a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>|
|[<span data-ttu-id="dfdd4-124">更新 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="dfdd4-124">Update windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[<span data-ttu-id="dfdd4-125">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="dfdd4-125">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="dfdd4-126">更新 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-126">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dfdd4-127">属性</span><span class="sxs-lookup"><span data-stu-id="dfdd4-127">Properties</span></span>
|<span data-ttu-id="dfdd4-128">属性</span><span class="sxs-lookup"><span data-stu-id="dfdd4-128">Property</span></span>|<span data-ttu-id="dfdd4-129">类型</span><span class="sxs-lookup"><span data-stu-id="dfdd4-129">Type</span></span>|<span data-ttu-id="dfdd4-130">说明</span><span class="sxs-lookup"><span data-stu-id="dfdd4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfdd4-131">id</span><span class="sxs-lookup"><span data-stu-id="dfdd4-131">id</span></span>|<span data-ttu-id="dfdd4-132">String</span><span class="sxs-lookup"><span data-stu-id="dfdd4-132">String</span></span>|<span data-ttu-id="dfdd4-133">WindowsPrivacyDataAccessControlItem 的键。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-133">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="dfdd4-134">accessLevel</span><span class="sxs-lookup"><span data-stu-id="dfdd4-134">accessLevel</span></span>|[<span data-ttu-id="dfdd4-135">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="dfdd4-135">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="dfdd4-136">这表示将向其授予指定应用程序的隐私数据类别的访问级别。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-136">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="dfdd4-137">可取值为：`notConfigured`、`forceAllow`、`forceDeny`、`userInControl`。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-137">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="dfdd4-138">dataCategory</span><span class="sxs-lookup"><span data-stu-id="dfdd4-138">dataCategory</span></span>|[<span data-ttu-id="dfdd4-139">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="dfdd4-139">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="dfdd4-140">这表示将应用特定访问控制的隐私数据类别。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-140">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="dfdd4-141">可能的值为：、、、、、、、、、、、、、、、、、、、 `notConfigured` `accountInfo` `appsRunInBackground` `calendar` `callHistory` `camera` `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone` `motion` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices` 。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-141">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="dfdd4-142">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="dfdd4-142">appPackageFamilyName</span></span>|<span data-ttu-id="dfdd4-143">String</span><span class="sxs-lookup"><span data-stu-id="dfdd4-143">String</span></span>|<span data-ttu-id="dfdd4-144">Windows 应用的程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-144">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="dfdd4-145">设置后，该访问级别将应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-145">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="dfdd4-146">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="dfdd4-146">appDisplayName</span></span>|<span data-ttu-id="dfdd4-147">String</span><span class="sxs-lookup"><span data-stu-id="dfdd4-147">String</span></span>|<span data-ttu-id="dfdd4-148">Windows 应用的程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-148">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="dfdd4-149">设置后，该访问级别将应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-149">When set, the access level applies to the specified application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfdd4-150">关系</span><span class="sxs-lookup"><span data-stu-id="dfdd4-150">Relationships</span></span>
<span data-ttu-id="dfdd4-151">无</span><span class="sxs-lookup"><span data-stu-id="dfdd4-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfdd4-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dfdd4-152">JSON Representation</span></span>
<span data-ttu-id="dfdd4-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfdd4-153">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsPrivacyDataAccessControlItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "String (identifier)",
  "accessLevel": "String",
  "dataCategory": "String",
  "appPackageFamilyName": "String",
  "appDisplayName": "String"
}
```





