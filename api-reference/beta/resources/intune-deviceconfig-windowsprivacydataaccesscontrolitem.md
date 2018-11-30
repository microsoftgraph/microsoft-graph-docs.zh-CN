---
title: windowsPrivacyDataAccessControlItem 资源类型
description: 指定每个隐私数据类别的访问控制级别
ms.openlocfilehash: b72571602b96f7b228361db4bf2526fda8def70f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049277"
---
# <a name="windowsprivacydataaccesscontrolitem-resource-type"></a><span data-ttu-id="437dc-103">windowsPrivacyDataAccessControlItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="437dc-103">windowsPrivacyDataAccessControlItem resource type</span></span>

> <span data-ttu-id="437dc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="437dc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="437dc-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="437dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="437dc-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="437dc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="437dc-107">指定每个隐私数据类别的访问控制级别</span><span class="sxs-lookup"><span data-stu-id="437dc-107">Specify access control level per privacy data category</span></span>
## <a name="methods"></a><span data-ttu-id="437dc-108">方法</span><span class="sxs-lookup"><span data-stu-id="437dc-108">Methods</span></span>
|<span data-ttu-id="437dc-109">方法</span><span class="sxs-lookup"><span data-stu-id="437dc-109">Method</span></span>|<span data-ttu-id="437dc-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="437dc-110">Return Type</span></span>|<span data-ttu-id="437dc-111">说明</span><span class="sxs-lookup"><span data-stu-id="437dc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="437dc-112">列表 windowsPrivacyDataAccessControlItems</span><span class="sxs-lookup"><span data-stu-id="437dc-112">List windowsPrivacyDataAccessControlItems</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-list.md)|<span data-ttu-id="437dc-113">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="437dc-113">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="437dc-114">列出属性和[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="437dc-114">List properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) objects.</span></span>|
|[<span data-ttu-id="437dc-115">获取 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="437dc-115">Get windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-get.md)|[<span data-ttu-id="437dc-116">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="437dc-116">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="437dc-117">读取属性和[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="437dc-117">Read properties and relationships of the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="437dc-118">创建 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="437dc-118">Create windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-create.md)|[<span data-ttu-id="437dc-119">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="437dc-119">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="437dc-120">创建新的[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="437dc-120">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|
|[<span data-ttu-id="437dc-121">删除 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="437dc-121">Delete windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-delete.md)|<span data-ttu-id="437dc-122">无</span><span class="sxs-lookup"><span data-stu-id="437dc-122">None</span></span>|<span data-ttu-id="437dc-123">删除[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)。</span><span class="sxs-lookup"><span data-stu-id="437dc-123">Deletes a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>|
|[<span data-ttu-id="437dc-124">更新 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="437dc-124">Update windowsPrivacyDataAccessControlItem</span></span>](../api/intune-deviceconfig-windowsprivacydataaccesscontrolitem-update.md)|[<span data-ttu-id="437dc-125">windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="437dc-125">windowsPrivacyDataAccessControlItem</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)|<span data-ttu-id="437dc-126">更新[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="437dc-126">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="437dc-127">属性</span><span class="sxs-lookup"><span data-stu-id="437dc-127">Properties</span></span>
|<span data-ttu-id="437dc-128">属性</span><span class="sxs-lookup"><span data-stu-id="437dc-128">Property</span></span>|<span data-ttu-id="437dc-129">类型</span><span class="sxs-lookup"><span data-stu-id="437dc-129">Type</span></span>|<span data-ttu-id="437dc-130">说明</span><span class="sxs-lookup"><span data-stu-id="437dc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="437dc-131">id</span><span class="sxs-lookup"><span data-stu-id="437dc-131">id</span></span>|<span data-ttu-id="437dc-132">字符串</span><span class="sxs-lookup"><span data-stu-id="437dc-132">String</span></span>|<span data-ttu-id="437dc-133">WindowsPrivacyDataAccessControlItem 键。</span><span class="sxs-lookup"><span data-stu-id="437dc-133">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="437dc-134">accessLevel</span><span class="sxs-lookup"><span data-stu-id="437dc-134">accessLevel</span></span>|[<span data-ttu-id="437dc-135">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="437dc-135">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="437dc-136">这指示到指定的应用程序会授予对隐私数据类别的访问级别。</span><span class="sxs-lookup"><span data-stu-id="437dc-136">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="437dc-137">可取值为：`notConfigured`、`forceAllow`、`forceDeny`、`userInControl`。</span><span class="sxs-lookup"><span data-stu-id="437dc-137">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="437dc-138">dataCategory</span><span class="sxs-lookup"><span data-stu-id="437dc-138">dataCategory</span></span>|[<span data-ttu-id="437dc-139">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="437dc-139">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="437dc-140">这指示特定的访问控制将应用于哪个隐私数据类别。</span><span class="sxs-lookup"><span data-stu-id="437dc-140">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="437dc-141">可能的值为： `notConfigured`， `accountInfo`， `appsRunInBackground`， `calendar`， `callHistory`， `camera`， `contacts`， `diagnosticsInfo`， `email`， `location`， `messaging`， `microphone`， `motion`， `notifications`， `phone`， `radios`， `tasks`， `syncWithDevices`， `trustedDevices`.</span><span class="sxs-lookup"><span data-stu-id="437dc-141">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="437dc-142">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="437dc-142">appPackageFamilyName</span></span>|<span data-ttu-id="437dc-143">字符串</span><span class="sxs-lookup"><span data-stu-id="437dc-143">String</span></span>|<span data-ttu-id="437dc-144">包系列 Windows 应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="437dc-144">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="437dc-145">设置时，访问级别应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="437dc-145">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="437dc-146">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="437dc-146">appDisplayName</span></span>|<span data-ttu-id="437dc-147">字符串</span><span class="sxs-lookup"><span data-stu-id="437dc-147">String</span></span>|<span data-ttu-id="437dc-148">包系列 Windows 应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="437dc-148">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="437dc-149">设置时，访问级别应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="437dc-149">When set, the access level applies to the specified application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="437dc-150">Relationships</span><span class="sxs-lookup"><span data-stu-id="437dc-150">Relationships</span></span>
<span data-ttu-id="437dc-151">无</span><span class="sxs-lookup"><span data-stu-id="437dc-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="437dc-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="437dc-152">JSON Representation</span></span>
<span data-ttu-id="437dc-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="437dc-153">Here is a JSON representation of the resource.</span></span>
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





