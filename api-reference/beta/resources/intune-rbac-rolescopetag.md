---
title: roleScopeTag 资源类型
description: 角色作用域标记
ms.openlocfilehash: 9be1f1307243c18e10f8e6dfc3f302502cdb54a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044758"
---
# <a name="rolescopetag-resource-type"></a><span data-ttu-id="0045e-103">roleScopeTag 资源类型</span><span class="sxs-lookup"><span data-stu-id="0045e-103">roleScopeTag resource type</span></span>

> <span data-ttu-id="0045e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0045e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0045e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0045e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0045e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0045e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0045e-107">角色作用域标记</span><span class="sxs-lookup"><span data-stu-id="0045e-107">Role Scope Tag</span></span>
## <a name="methods"></a><span data-ttu-id="0045e-108">方法</span><span class="sxs-lookup"><span data-stu-id="0045e-108">Methods</span></span>
|<span data-ttu-id="0045e-109">方法</span><span class="sxs-lookup"><span data-stu-id="0045e-109">Method</span></span>|<span data-ttu-id="0045e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="0045e-110">Return Type</span></span>|<span data-ttu-id="0045e-111">说明</span><span class="sxs-lookup"><span data-stu-id="0045e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0045e-112">列表 roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="0045e-112">List roleScopeTags</span></span>](../api/intune-rbac-rolescopetag-list.md)|<span data-ttu-id="0045e-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md)集合</span><span class="sxs-lookup"><span data-stu-id="0045e-113">[roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection</span></span>|<span data-ttu-id="0045e-114">列出属性和[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="0045e-114">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>|
|[<span data-ttu-id="0045e-115">获取 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0045e-115">Get roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-get.md)|[<span data-ttu-id="0045e-116">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0045e-116">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="0045e-117">读取属性和[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="0045e-117">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="0045e-118">创建 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0045e-118">Create roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-create.md)|[<span data-ttu-id="0045e-119">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0045e-119">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="0045e-120">创建新的[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0045e-120">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|
|[<span data-ttu-id="0045e-121">删除 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0045e-121">Delete roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-delete.md)|<span data-ttu-id="0045e-122">无</span><span class="sxs-lookup"><span data-stu-id="0045e-122">None</span></span>|<span data-ttu-id="0045e-123">删除[roleScopeTag](../resources/intune-rbac-rolescopetag.md)。</span><span class="sxs-lookup"><span data-stu-id="0045e-123">Deletes a [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>|
|[<span data-ttu-id="0045e-124">更新 roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0045e-124">Update roleScopeTag</span></span>](../api/intune-rbac-rolescopetag-update.md)|[<span data-ttu-id="0045e-125">roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="0045e-125">roleScopeTag</span></span>](../resources/intune-rbac-rolescopetag.md)|<span data-ttu-id="0045e-126">更新[roleScopeTag](../resources/intune-rbac-rolescopetag.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0045e-126">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0045e-127">属性</span><span class="sxs-lookup"><span data-stu-id="0045e-127">Properties</span></span>
|<span data-ttu-id="0045e-128">属性</span><span class="sxs-lookup"><span data-stu-id="0045e-128">Property</span></span>|<span data-ttu-id="0045e-129">类型</span><span class="sxs-lookup"><span data-stu-id="0045e-129">Type</span></span>|<span data-ttu-id="0045e-130">说明</span><span class="sxs-lookup"><span data-stu-id="0045e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0045e-131">id</span><span class="sxs-lookup"><span data-stu-id="0045e-131">id</span></span>|<span data-ttu-id="0045e-132">String</span><span class="sxs-lookup"><span data-stu-id="0045e-132">String</span></span>|<span data-ttu-id="0045e-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0045e-133">Key of the entity.</span></span> <span data-ttu-id="0045e-134">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="0045e-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="0045e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0045e-135">displayName</span></span>|<span data-ttu-id="0045e-136">字符串</span><span class="sxs-lookup"><span data-stu-id="0045e-136">String</span></span>|<span data-ttu-id="0045e-137">显示或角色作用域标记的友好名称。</span><span class="sxs-lookup"><span data-stu-id="0045e-137">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="0045e-138">说明</span><span class="sxs-lookup"><span data-stu-id="0045e-138">description</span></span>|<span data-ttu-id="0045e-139">字符串</span><span class="sxs-lookup"><span data-stu-id="0045e-139">String</span></span>|<span data-ttu-id="0045e-140">角色作用域标记的说明。</span><span class="sxs-lookup"><span data-stu-id="0045e-140">Description of the Role Scope Tag.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0045e-141">Relationships</span><span class="sxs-lookup"><span data-stu-id="0045e-141">Relationships</span></span>
<span data-ttu-id="0045e-142">无</span><span class="sxs-lookup"><span data-stu-id="0045e-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0045e-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0045e-143">JSON Representation</span></span>
<span data-ttu-id="0045e-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0045e-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTag"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```





