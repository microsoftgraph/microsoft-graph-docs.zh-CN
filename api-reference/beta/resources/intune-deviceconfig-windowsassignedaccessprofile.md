---
title: windowsAssignedAccessProfile 资源类型
description: 用于 Windows 的分配的访问配置文件。
ms.openlocfilehash: 2fc23bfed54ef850050b177589d5b4c0c79c22cc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042744"
---
# <a name="windowsassignedaccessprofile-resource-type"></a><span data-ttu-id="01003-103">windowsAssignedAccessProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="01003-103">windowsAssignedAccessProfile resource type</span></span>

> <span data-ttu-id="01003-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="01003-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01003-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="01003-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01003-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="01003-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01003-107">用于 Windows 的分配的访问配置文件。</span><span class="sxs-lookup"><span data-stu-id="01003-107">Assigned Access profile for Windows.</span></span>
## <a name="methods"></a><span data-ttu-id="01003-108">方法</span><span class="sxs-lookup"><span data-stu-id="01003-108">Methods</span></span>
|<span data-ttu-id="01003-109">方法</span><span class="sxs-lookup"><span data-stu-id="01003-109">Method</span></span>|<span data-ttu-id="01003-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="01003-110">Return Type</span></span>|<span data-ttu-id="01003-111">说明</span><span class="sxs-lookup"><span data-stu-id="01003-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="01003-112">列表 windowsAssignedAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="01003-112">List windowsAssignedAccessProfiles</span></span>](../api/intune-deviceconfig-windowsassignedaccessprofile-list.md)|<span data-ttu-id="01003-113">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="01003-113">[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) collection</span></span>|<span data-ttu-id="01003-114">列出属性和[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="01003-114">List properties and relationships of the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) objects.</span></span>|
|[<span data-ttu-id="01003-115">获取 windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="01003-115">Get windowsAssignedAccessProfile</span></span>](../api/intune-deviceconfig-windowsassignedaccessprofile-get.md)|[<span data-ttu-id="01003-116">windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="01003-116">windowsAssignedAccessProfile</span></span>](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|<span data-ttu-id="01003-117">读取属性和[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="01003-117">Read properties and relationships of the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>|
|[<span data-ttu-id="01003-118">创建 windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="01003-118">Create windowsAssignedAccessProfile</span></span>](../api/intune-deviceconfig-windowsassignedaccessprofile-create.md)|[<span data-ttu-id="01003-119">windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="01003-119">windowsAssignedAccessProfile</span></span>](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|<span data-ttu-id="01003-120">创建新的[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="01003-120">Create a new [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>|
|[<span data-ttu-id="01003-121">删除 windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="01003-121">Delete windowsAssignedAccessProfile</span></span>](../api/intune-deviceconfig-windowsassignedaccessprofile-delete.md)|<span data-ttu-id="01003-122">无</span><span class="sxs-lookup"><span data-stu-id="01003-122">None</span></span>|<span data-ttu-id="01003-123">删除[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="01003-123">Deletes a [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md).</span></span>|
|[<span data-ttu-id="01003-124">更新 windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="01003-124">Update windowsAssignedAccessProfile</span></span>](../api/intune-deviceconfig-windowsassignedaccessprofile-update.md)|[<span data-ttu-id="01003-125">windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="01003-125">windowsAssignedAccessProfile</span></span>](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)|<span data-ttu-id="01003-126">更新[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="01003-126">Update the properties of a [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="01003-127">属性</span><span class="sxs-lookup"><span data-stu-id="01003-127">Properties</span></span>
|<span data-ttu-id="01003-128">属性</span><span class="sxs-lookup"><span data-stu-id="01003-128">Property</span></span>|<span data-ttu-id="01003-129">类型</span><span class="sxs-lookup"><span data-stu-id="01003-129">Type</span></span>|<span data-ttu-id="01003-130">说明</span><span class="sxs-lookup"><span data-stu-id="01003-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01003-131">id</span><span class="sxs-lookup"><span data-stu-id="01003-131">id</span></span>|<span data-ttu-id="01003-132">String</span><span class="sxs-lookup"><span data-stu-id="01003-132">String</span></span>|<span data-ttu-id="01003-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="01003-133">Key of the entity.</span></span>|
|<span data-ttu-id="01003-134">profileName</span><span class="sxs-lookup"><span data-stu-id="01003-134">profileName</span></span>|<span data-ttu-id="01003-135">字符串</span><span class="sxs-lookup"><span data-stu-id="01003-135">String</span></span>|<span data-ttu-id="01003-136">这是用于标识一组应用程序，在开始菜单和用户为其分配此网亭配置这些应用程序的布局的友好名称。</span><span class="sxs-lookup"><span data-stu-id="01003-136">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="01003-137">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="01003-137">showTaskBar</span></span>|<span data-ttu-id="01003-138">布尔</span><span class="sxs-lookup"><span data-stu-id="01003-138">Boolean</span></span>|<span data-ttu-id="01003-139">此设置，管理员可以指定任务条形图或不所示。</span><span class="sxs-lookup"><span data-stu-id="01003-139">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="01003-140">appUserModelIds</span><span class="sxs-lookup"><span data-stu-id="01003-140">appUserModelIds</span></span>|<span data-ttu-id="01003-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="01003-141">String collection</span></span>|<span data-ttu-id="01003-142">这些是唯一的 Windows 应用商店应用程序将可以从开始菜单启动。</span><span class="sxs-lookup"><span data-stu-id="01003-142">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="01003-143">desktopAppPaths</span><span class="sxs-lookup"><span data-stu-id="01003-143">desktopAppPaths</span></span>|<span data-ttu-id="01003-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="01003-144">String collection</span></span>|<span data-ttu-id="01003-145">在开始菜单可用桌面应用程序的路径和仅应用程序用户都将能够启动。</span><span class="sxs-lookup"><span data-stu-id="01003-145">These are the paths of the Desktop Apps that will be available on the Start menu and the only apps the user will be able to launch.</span></span>|
|<span data-ttu-id="01003-146">用户帐户</span><span class="sxs-lookup"><span data-stu-id="01003-146">userAccounts</span></span>|<span data-ttu-id="01003-147">String 集合</span><span class="sxs-lookup"><span data-stu-id="01003-147">String collection</span></span>|<span data-ttu-id="01003-148">将锁定到此网亭配置用户帐户。</span><span class="sxs-lookup"><span data-stu-id="01003-148">The user accounts that will be locked to this kiosk configuration.</span></span>|
|<span data-ttu-id="01003-149">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="01003-149">startMenuLayoutXml</span></span>|<span data-ttu-id="01003-150">Binary</span><span class="sxs-lookup"><span data-stu-id="01003-150">Binary</span></span>|<span data-ttu-id="01003-151">允许管理员可以重写默认开始布局，并禁止用户更改它。</span><span class="sxs-lookup"><span data-stu-id="01003-151">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="01003-152">通过基于布局修改模式指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="01003-152"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="01003-153">XML 需要以二进制格式。</span><span class="sxs-lookup"><span data-stu-id="01003-153">XML needs to be in Binary format.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01003-154">Relationships</span><span class="sxs-lookup"><span data-stu-id="01003-154">Relationships</span></span>
<span data-ttu-id="01003-155">无</span><span class="sxs-lookup"><span data-stu-id="01003-155">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="01003-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01003-156">JSON Representation</span></span>
<span data-ttu-id="01003-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01003-157">Here is a JSON representation of the resource.</span></span>
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





