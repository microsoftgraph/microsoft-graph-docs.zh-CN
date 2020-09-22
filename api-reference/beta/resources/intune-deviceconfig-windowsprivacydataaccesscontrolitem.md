---
title: windowsPrivacyDataAccessControlItem 资源类型
description: 指定每个隐私数据类别的访问控制级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8f4853d9c7778164ff77295a24daff65bb61bf9b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039753"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a><span data-ttu-id="afc1f-103">windowsPrivacyDataAccessControlItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="afc1f-103">windowsPrivacyDataAccessControlItem resource type</span></span>

<span data-ttu-id="afc1f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afc1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afc1f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="afc1f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afc1f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="afc1f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afc1f-107">指定每个隐私数据类别的访问控制级别</span><span class="sxs-lookup"><span data-stu-id="afc1f-107">Specify access control level per privacy data category</span></span>

## <a name="methods"></a><span data-ttu-id="afc1f-108">方法</span><span class="sxs-lookup"><span data-stu-id="afc1f-108">Methods</span></span>
|<span data-ttu-id="afc1f-109">方法</span><span class="sxs-lookup"><span data-stu-id="afc1f-109">Method</span></span>|<span data-ttu-id="afc1f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="afc1f-110">Return Type</span></span>|<span data-ttu-id="afc1f-111">说明</span><span class="sxs-lookup"><span data-stu-id="afc1f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="afc1f-112">列出 windowsPrivacyDataAccessControlItems</span><span class="sxs-lookup"><span data-stu-id="afc1f-112">List windowsPrivacyDataAccessControlItems</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|<span data-ttu-id="afc1f-113">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="afc1f-113">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="afc1f-114">列出 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="afc1f-114">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>|
|[<span data-ttu-id="afc1f-115">获取 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="afc1f-115">Get windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[<span data-ttu-id="afc1f-116">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="afc1f-116">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="afc1f-117">读取 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="afc1f-117">Read properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="afc1f-118">创建 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="afc1f-118">Create windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[<span data-ttu-id="afc1f-119">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="afc1f-119">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="afc1f-120">创建新的 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="afc1f-120">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="afc1f-121">删除 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="afc1f-121">Delete windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|<span data-ttu-id="afc1f-122">无</span><span class="sxs-lookup"><span data-stu-id="afc1f-122">None</span></span>|<span data-ttu-id="afc1f-123">删除 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)。</span><span class="sxs-lookup"><span data-stu-id="afc1f-123">Deletes a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>|
|[<span data-ttu-id="afc1f-124">更新 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="afc1f-124">Update windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[<span data-ttu-id="afc1f-125">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="afc1f-125">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="afc1f-126">更新 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="afc1f-126">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="afc1f-127">属性</span><span class="sxs-lookup"><span data-stu-id="afc1f-127">Properties</span></span>
|<span data-ttu-id="afc1f-128">属性</span><span class="sxs-lookup"><span data-stu-id="afc1f-128">Property</span></span>|<span data-ttu-id="afc1f-129">类型</span><span class="sxs-lookup"><span data-stu-id="afc1f-129">Type</span></span>|<span data-ttu-id="afc1f-130">说明</span><span class="sxs-lookup"><span data-stu-id="afc1f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afc1f-131">id</span><span class="sxs-lookup"><span data-stu-id="afc1f-131">id</span></span>|<span data-ttu-id="afc1f-132">String</span><span class="sxs-lookup"><span data-stu-id="afc1f-132">String</span></span>|<span data-ttu-id="afc1f-133">WindowsPrivacyDataAccessControlItem 的键。</span><span class="sxs-lookup"><span data-stu-id="afc1f-133">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="afc1f-134">accessLevel</span><span class="sxs-lookup"><span data-stu-id="afc1f-134">accessLevel</span></span>|[<span data-ttu-id="afc1f-135">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="afc1f-135">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="afc1f-136">这表示将向其授予指定应用程序的隐私数据类别的访问级别。</span><span class="sxs-lookup"><span data-stu-id="afc1f-136">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="afc1f-137">可取值为：`notConfigured`、`forceAllow`、`forceDeny`、`userInControl`。</span><span class="sxs-lookup"><span data-stu-id="afc1f-137">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="afc1f-138">dataCategory</span><span class="sxs-lookup"><span data-stu-id="afc1f-138">dataCategory</span></span>|[<span data-ttu-id="afc1f-139">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="afc1f-139">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="afc1f-140">这表示将应用特定访问控制的隐私数据类别。</span><span class="sxs-lookup"><span data-stu-id="afc1f-140">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="afc1f-141">可能的值为：、、、、、、、、、、、、、、、、、、、 `notConfigured` `accountInfo` `appsRunInBackground` `calendar` `callHistory` `camera` `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone` `motion` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices` 。</span><span class="sxs-lookup"><span data-stu-id="afc1f-141">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="afc1f-142">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="afc1f-142">appPackageFamilyName</span></span>|<span data-ttu-id="afc1f-143">String</span><span class="sxs-lookup"><span data-stu-id="afc1f-143">String</span></span>|<span data-ttu-id="afc1f-144">Windows 应用的程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="afc1f-144">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="afc1f-145">设置后，该访问级别将应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="afc1f-145">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="afc1f-146">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="afc1f-146">appDisplayName</span></span>|<span data-ttu-id="afc1f-147">String</span><span class="sxs-lookup"><span data-stu-id="afc1f-147">String</span></span>|<span data-ttu-id="afc1f-148">Windows 应用的程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="afc1f-148">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="afc1f-149">设置后，该访问级别将应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="afc1f-149">When set, the access level applies to the specified application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="afc1f-150">关系</span><span class="sxs-lookup"><span data-stu-id="afc1f-150">Relationships</span></span>
<span data-ttu-id="afc1f-151">无</span><span class="sxs-lookup"><span data-stu-id="afc1f-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="afc1f-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="afc1f-152">JSON Representation</span></span>
<span data-ttu-id="afc1f-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="afc1f-153">Here is a JSON representation of the resource.</span></span>
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






