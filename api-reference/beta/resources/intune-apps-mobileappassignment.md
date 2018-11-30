---
title: mobileAppAssignment 资源类型
description: 包含用于移动应用的组分配的属性的类。
ms.openlocfilehash: f6a84e40ccbdc2192e0d5f81d20d3d598f50f913
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042617"
---
# <a name="mobileappassignment-resource-type"></a><span data-ttu-id="04d49-103">mobileAppAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="04d49-103">mobileAppAssignment resource type</span></span>

> <span data-ttu-id="04d49-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="04d49-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04d49-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="04d49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04d49-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="04d49-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04d49-107">包含用于移动应用的组分配的属性的类。</span><span class="sxs-lookup"><span data-stu-id="04d49-107">A class containing the properties used for Group Assignment of a Mobile App.</span></span>
## <a name="methods"></a><span data-ttu-id="04d49-108">方法</span><span class="sxs-lookup"><span data-stu-id="04d49-108">Methods</span></span>
|<span data-ttu-id="04d49-109">方法</span><span class="sxs-lookup"><span data-stu-id="04d49-109">Method</span></span>|<span data-ttu-id="04d49-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="04d49-110">Return Type</span></span>|<span data-ttu-id="04d49-111">说明</span><span class="sxs-lookup"><span data-stu-id="04d49-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="04d49-112">列出 mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="04d49-112">List mobileAppAssignments</span></span>](../api/intune-apps-mobileappassignment-list.md)|<span data-ttu-id="04d49-113">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span><span class="sxs-lookup"><span data-stu-id="04d49-113">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="04d49-114">列出 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="04d49-114">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>|
|[<span data-ttu-id="04d49-115">获取 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="04d49-115">Get mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-get.md)|[<span data-ttu-id="04d49-116">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="04d49-116">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="04d49-117">读取 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="04d49-117">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|
|[<span data-ttu-id="04d49-118">创建 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="04d49-118">Create mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-create.md)|[<span data-ttu-id="04d49-119">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="04d49-119">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="04d49-120">创建新的 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="04d49-120">Create a new [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|
|[<span data-ttu-id="04d49-121">删除 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="04d49-121">Delete mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-delete.md)|<span data-ttu-id="04d49-122">无</span><span class="sxs-lookup"><span data-stu-id="04d49-122">None</span></span>|<span data-ttu-id="04d49-123">删除 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md)</span><span class="sxs-lookup"><span data-stu-id="04d49-123">Deletes a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>|
|[<span data-ttu-id="04d49-124">更新 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="04d49-124">Update mobileAppAssignment</span></span>](../api/intune-apps-mobileappassignment-update.md)|[<span data-ttu-id="04d49-125">mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="04d49-125">mobileAppAssignment</span></span>](../resources/intune-apps-mobileappassignment.md)|<span data-ttu-id="04d49-126">更新 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="04d49-126">Update the properties of a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="04d49-127">属性</span><span class="sxs-lookup"><span data-stu-id="04d49-127">Properties</span></span>
|<span data-ttu-id="04d49-128">属性</span><span class="sxs-lookup"><span data-stu-id="04d49-128">Property</span></span>|<span data-ttu-id="04d49-129">类型</span><span class="sxs-lookup"><span data-stu-id="04d49-129">Type</span></span>|<span data-ttu-id="04d49-130">说明</span><span class="sxs-lookup"><span data-stu-id="04d49-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04d49-131">id</span><span class="sxs-lookup"><span data-stu-id="04d49-131">id</span></span>|<span data-ttu-id="04d49-132">String</span><span class="sxs-lookup"><span data-stu-id="04d49-132">String</span></span>|<span data-ttu-id="04d49-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="04d49-133">Key of the entity.</span></span>|
|<span data-ttu-id="04d49-134">intent</span><span class="sxs-lookup"><span data-stu-id="04d49-134">intent</span></span>|[<span data-ttu-id="04d49-135">installIntent</span><span class="sxs-lookup"><span data-stu-id="04d49-135">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="04d49-136">由管理员定义的安装意图。可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="04d49-136">The install intent defined by the admin. Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|
|<span data-ttu-id="04d49-137">target</span><span class="sxs-lookup"><span data-stu-id="04d49-137">target</span></span>|[<span data-ttu-id="04d49-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="04d49-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="04d49-139">由管理员定义的目标组分配。</span><span class="sxs-lookup"><span data-stu-id="04d49-139">The target group assignment defined by the admin.</span></span>|
|<span data-ttu-id="04d49-140">settings</span><span class="sxs-lookup"><span data-stu-id="04d49-140">settings</span></span>|[<span data-ttu-id="04d49-141">mobileAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="04d49-141">mobileAppAssignmentSettings</span></span>](../resources/intune-apps-mobileappassignmentsettings.md)|<span data-ttu-id="04d49-142">由管理员定义的目标分配的设置。</span><span class="sxs-lookup"><span data-stu-id="04d49-142">The settings for target assignment defined by the admin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04d49-143">关系</span><span class="sxs-lookup"><span data-stu-id="04d49-143">Relationships</span></span>
<span data-ttu-id="04d49-144">无</span><span class="sxs-lookup"><span data-stu-id="04d49-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="04d49-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04d49-145">JSON Representation</span></span>
<span data-ttu-id="04d49-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04d49-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```





