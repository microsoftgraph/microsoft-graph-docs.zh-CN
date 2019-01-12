---
title: windowsAssignedAccessProfile 资源类型
description: 用于 Windows 的分配的访问配置文件。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 893e81e544286c6877b9443d96f610acb939e934
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972850"
---
# <a name="windowsassignedaccessprofile-resource-type"></a><span data-ttu-id="265cd-103">windowsAssignedAccessProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="265cd-103">windowsAssignedAccessProfile resource type</span></span>

> <span data-ttu-id="265cd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="265cd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="265cd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="265cd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="265cd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="265cd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="265cd-107">用于 Windows 的分配的访问配置文件。</span><span class="sxs-lookup"><span data-stu-id="265cd-107">Assigned Access profile for Windows.</span></span>
## <a name="methods"></a><span data-ttu-id="265cd-108">方法</span><span class="sxs-lookup"><span data-stu-id="265cd-108">Methods</span></span>
|<span data-ttu-id="265cd-109">方法</span><span class="sxs-lookup"><span data-stu-id="265cd-109">Method</span></span>|<span data-ttu-id="265cd-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="265cd-110">Return Type</span></span>|<span data-ttu-id="265cd-111">说明</span><span class="sxs-lookup"><span data-stu-id="265cd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="265cd-112">列表 windowsAssignedAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="265cd-112">List windowsAssignedAccessProfiles</span></span>](../api/intune-deviceconfig-windowsassignedaccessprofile-list.md)|<span data-ttu-id="265cd-113">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="265cd-113">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) collection</span></span>|<span data-ttu-id="265cd-114">列出属性和[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="265cd-114">List properties and relationships of the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) objects.</span></span>|
|[<span data-ttu-id="265cd-115">获取 windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="265cd-115">Get windowsAssignedAccessProfile</span></span>](../api/intune-deviceconfig-windowsassignedaccessprofile-get.md)|[<span data-ttu-id="265cd-116">windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="265cd-116">windowsAssignedAccessProfile</span></span>](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|<span data-ttu-id="265cd-117">读取属性和[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="265cd-117">Read properties and relationships of the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>|
|[<span data-ttu-id="265cd-118">创建 windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="265cd-118">Create windowsAssignedAccessProfile</span></span>](../api/intune-deviceconfig-windowsassignedaccessprofile-create.md)|[<span data-ttu-id="265cd-119">windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="265cd-119">windowsAssignedAccessProfile</span></span>](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|<span data-ttu-id="265cd-120">创建新的[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="265cd-120">Create a new [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>|
|[<span data-ttu-id="265cd-121">删除 windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="265cd-121">Delete windowsAssignedAccessProfile</span></span>](../api/intune-deviceconfig-windowsassignedaccessprofile-delete.md)|<span data-ttu-id="265cd-122">无</span><span class="sxs-lookup"><span data-stu-id="265cd-122">None</span></span>|<span data-ttu-id="265cd-123">删除[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="265cd-123">Deletes a [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md).</span></span>|
|[<span data-ttu-id="265cd-124">更新 windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="265cd-124">Update windowsAssignedAccessProfile</span></span>](../api/intune-deviceconfig-windowsassignedaccessprofile-update.md)|[<span data-ttu-id="265cd-125">windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="265cd-125">windowsAssignedAccessProfile</span></span>](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|<span data-ttu-id="265cd-126">更新[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="265cd-126">Update the properties of a [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="265cd-127">属性</span><span class="sxs-lookup"><span data-stu-id="265cd-127">Properties</span></span>
|<span data-ttu-id="265cd-128">属性</span><span class="sxs-lookup"><span data-stu-id="265cd-128">Property</span></span>|<span data-ttu-id="265cd-129">类型</span><span class="sxs-lookup"><span data-stu-id="265cd-129">Type</span></span>|<span data-ttu-id="265cd-130">说明</span><span class="sxs-lookup"><span data-stu-id="265cd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="265cd-131">id</span><span class="sxs-lookup"><span data-stu-id="265cd-131">id</span></span>|<span data-ttu-id="265cd-132">String</span><span class="sxs-lookup"><span data-stu-id="265cd-132">String</span></span>|<span data-ttu-id="265cd-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="265cd-133">Key of the entity.</span></span>|
|<span data-ttu-id="265cd-134">profileName</span><span class="sxs-lookup"><span data-stu-id="265cd-134">profileName</span></span>|<span data-ttu-id="265cd-135">字符串</span><span class="sxs-lookup"><span data-stu-id="265cd-135">String</span></span>|<span data-ttu-id="265cd-136">这是用于标识一组应用程序，在开始菜单和用户为其分配此网亭配置这些应用程序的布局的友好名称。</span><span class="sxs-lookup"><span data-stu-id="265cd-136">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="265cd-137">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="265cd-137">showTaskBar</span></span>|<span data-ttu-id="265cd-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="265cd-138">Boolean</span></span>|<span data-ttu-id="265cd-139">此设置，管理员可以指定任务条形图或不所示。</span><span class="sxs-lookup"><span data-stu-id="265cd-139">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="265cd-140">appUserModelIds</span><span class="sxs-lookup"><span data-stu-id="265cd-140">appUserModelIds</span></span>|<span data-ttu-id="265cd-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="265cd-141">String collection</span></span>|<span data-ttu-id="265cd-142">这些是唯一的 Windows 应用商店应用程序将可以从开始菜单启动。</span><span class="sxs-lookup"><span data-stu-id="265cd-142">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="265cd-143">desktopAppPaths</span><span class="sxs-lookup"><span data-stu-id="265cd-143">desktopAppPaths</span></span>|<span data-ttu-id="265cd-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="265cd-144">String collection</span></span>|<span data-ttu-id="265cd-145">在开始菜单可用桌面应用程序的路径和仅应用程序用户都将能够启动。</span><span class="sxs-lookup"><span data-stu-id="265cd-145">These are the paths of the Desktop Apps that will be available on the Start menu and the only apps the user will be able to launch.</span></span>|
|<span data-ttu-id="265cd-146">用户帐户</span><span class="sxs-lookup"><span data-stu-id="265cd-146">userAccounts</span></span>|<span data-ttu-id="265cd-147">String 集合</span><span class="sxs-lookup"><span data-stu-id="265cd-147">String collection</span></span>|<span data-ttu-id="265cd-148">将锁定到此网亭配置用户帐户。</span><span class="sxs-lookup"><span data-stu-id="265cd-148">The user accounts that will be locked to this kiosk configuration.</span></span>|
|<span data-ttu-id="265cd-149">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="265cd-149">startMenuLayoutXml</span></span>|<span data-ttu-id="265cd-150">Binary</span><span class="sxs-lookup"><span data-stu-id="265cd-150">Binary</span></span>|<span data-ttu-id="265cd-151">允许管理员可以重写默认开始布局，并禁止用户更改它。</span><span class="sxs-lookup"><span data-stu-id="265cd-151">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="265cd-152">通过基于布局修改模式指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="265cd-152"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="265cd-153">XML 需要以二进制格式。</span><span class="sxs-lookup"><span data-stu-id="265cd-153">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="265cd-154">Relationships</span><span class="sxs-lookup"><span data-stu-id="265cd-154">Relationships</span></span>
<span data-ttu-id="265cd-155">无</span><span class="sxs-lookup"><span data-stu-id="265cd-155">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="265cd-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="265cd-156">JSON Representation</span></span>
<span data-ttu-id="265cd-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="265cd-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAssignedAccessProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "id": "String (identifier)",
  "profileName": "String",
  "showTaskBar": true,
  "appUserModelIds": [
    "String"
  ],
  "desktopAppPaths": [
    "String"
  ],
  "userAccounts": [
    "String"
  ],
  "startMenuLayoutXml": "binary"
}
```





