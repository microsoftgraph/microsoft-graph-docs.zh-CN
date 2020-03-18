---
title: windowsPrivacyDataAccessControlItem 资源类型
description: 指定每个隐私数据类别的访问控制级别
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 237b7f992b78d134d37ebdeb7d47b14257b0f801
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786255"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a><span data-ttu-id="f4bf6-103">windowsPrivacyDataAccessControlItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4bf6-103">windowsPrivacyDataAccessControlItem resource type</span></span>

> <span data-ttu-id="f4bf6-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f4bf6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4bf6-106">指定每个隐私数据类别的访问控制级别</span><span class="sxs-lookup"><span data-stu-id="f4bf6-106">Specify access control level per privacy data category</span></span>

## <a name="methods"></a><span data-ttu-id="f4bf6-107">方法</span><span class="sxs-lookup"><span data-stu-id="f4bf6-107">Methods</span></span>
|<span data-ttu-id="f4bf6-108">方法</span><span class="sxs-lookup"><span data-stu-id="f4bf6-108">Method</span></span>|<span data-ttu-id="f4bf6-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f4bf6-109">Return Type</span></span>|<span data-ttu-id="f4bf6-110">说明</span><span class="sxs-lookup"><span data-stu-id="f4bf6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f4bf6-111">列出 windowsPrivacyDataAccessControlItems</span><span class="sxs-lookup"><span data-stu-id="f4bf6-111">List windowsPrivacyDataAccessControlItems</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|<span data-ttu-id="f4bf6-112">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="f4bf6-112">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="f4bf6-113">列出[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-113">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>|
|[<span data-ttu-id="f4bf6-114">获取 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="f4bf6-114">Get windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[<span data-ttu-id="f4bf6-115">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="f4bf6-115">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="f4bf6-116">读取[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-116">Read properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="f4bf6-117">创建 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="f4bf6-117">Create windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[<span data-ttu-id="f4bf6-118">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="f4bf6-118">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="f4bf6-119">创建新的[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-119">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="f4bf6-120">删除 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="f4bf6-120">Delete windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|<span data-ttu-id="f4bf6-121">None</span><span class="sxs-lookup"><span data-stu-id="f4bf6-121">None</span></span>|<span data-ttu-id="f4bf6-122">删除[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-122">Deletes a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>|
|[<span data-ttu-id="f4bf6-123">更新 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="f4bf6-123">Update windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[<span data-ttu-id="f4bf6-124">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="f4bf6-124">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="f4bf6-125">更新[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-125">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f4bf6-126">属性</span><span class="sxs-lookup"><span data-stu-id="f4bf6-126">Properties</span></span>
|<span data-ttu-id="f4bf6-127">属性</span><span class="sxs-lookup"><span data-stu-id="f4bf6-127">Property</span></span>|<span data-ttu-id="f4bf6-128">类型</span><span class="sxs-lookup"><span data-stu-id="f4bf6-128">Type</span></span>|<span data-ttu-id="f4bf6-129">说明</span><span class="sxs-lookup"><span data-stu-id="f4bf6-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4bf6-130">id</span><span class="sxs-lookup"><span data-stu-id="f4bf6-130">id</span></span>|<span data-ttu-id="f4bf6-131">字符串</span><span class="sxs-lookup"><span data-stu-id="f4bf6-131">String</span></span>|<span data-ttu-id="f4bf6-132">WindowsPrivacyDataAccessControlItem 的键。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-132">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="f4bf6-133">accessLevel</span><span class="sxs-lookup"><span data-stu-id="f4bf6-133">accessLevel</span></span>|[<span data-ttu-id="f4bf6-134">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="f4bf6-134">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="f4bf6-135">这表示将向其授予指定应用程序的隐私数据类别的访问级别。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-135">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="f4bf6-136">可取值为：`notConfigured`、`forceAllow`、`forceDeny`、`userInControl`。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-136">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="f4bf6-137">dataCategory</span><span class="sxs-lookup"><span data-stu-id="f4bf6-137">dataCategory</span></span>|[<span data-ttu-id="f4bf6-138">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="f4bf6-138">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="f4bf6-139">这表示将应用特定访问控制的隐私数据类别。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-139">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="f4bf6-140">可能的值为`notConfigured`： `accountInfo`、 `appsRunInBackground`、 `calendar` `callHistory` `camera` `contacts` `diagnosticsInfo` `email` `location` `messaging` `trustedDevices`、、 `notifications`、、、、、、、、、、、、、、、。 `microphone` `motion` `phone` `radios` `tasks` `syncWithDevices`</span><span class="sxs-lookup"><span data-stu-id="f4bf6-140">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="f4bf6-141">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="f4bf6-141">appPackageFamilyName</span></span>|<span data-ttu-id="f4bf6-142">String</span><span class="sxs-lookup"><span data-stu-id="f4bf6-142">String</span></span>|<span data-ttu-id="f4bf6-143">Windows 应用的程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-143">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="f4bf6-144">设置后，该访问级别将应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-144">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="f4bf6-145">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="f4bf6-145">appDisplayName</span></span>|<span data-ttu-id="f4bf6-146">String</span><span class="sxs-lookup"><span data-stu-id="f4bf6-146">String</span></span>|<span data-ttu-id="f4bf6-147">Windows 应用的程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-147">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="f4bf6-148">设置后，该访问级别将应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-148">When set, the access level applies to the specified application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4bf6-149">关系</span><span class="sxs-lookup"><span data-stu-id="f4bf6-149">Relationships</span></span>
<span data-ttu-id="f4bf6-150">无</span><span class="sxs-lookup"><span data-stu-id="f4bf6-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4bf6-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4bf6-151">JSON Representation</span></span>
<span data-ttu-id="f4bf6-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4bf6-152">Here is a JSON representation of the resource.</span></span>
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



