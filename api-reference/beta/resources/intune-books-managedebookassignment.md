---
title: managedEBookAssignment 资源类型
description: 包含用于为组分配电子书的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f7f5eb73b8867bcbcf5547b0900e0196d70cd0a8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937876"
---
# <a name="managedebookassignment-resource-type"></a><span data-ttu-id="48919-103">managedEBookAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="48919-103">managedEBookAssignment resource type</span></span>

> <span data-ttu-id="48919-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="48919-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="48919-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="48919-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48919-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="48919-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48919-107">包含用于为组分配电子书的属性。</span><span class="sxs-lookup"><span data-stu-id="48919-107">Contains properties used to assign a eBook to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="48919-108">方法</span><span class="sxs-lookup"><span data-stu-id="48919-108">Methods</span></span>
|<span data-ttu-id="48919-109">方法</span><span class="sxs-lookup"><span data-stu-id="48919-109">Method</span></span>|<span data-ttu-id="48919-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="48919-110">Return Type</span></span>|<span data-ttu-id="48919-111">说明</span><span class="sxs-lookup"><span data-stu-id="48919-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="48919-112">列出 managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="48919-112">List managedEBookAssignments</span></span>](../api/intune-books-managedebookassignment-list.md)|<span data-ttu-id="48919-113">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="48919-113">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="48919-114">列出 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="48919-114">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>|
|[<span data-ttu-id="48919-115">获取 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="48919-115">Get managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-get.md)|[<span data-ttu-id="48919-116">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="48919-116">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="48919-117">读取 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="48919-117">Read properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="48919-118">创建 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="48919-118">Create managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-create.md)|[<span data-ttu-id="48919-119">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="48919-119">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="48919-120">创建新的 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="48919-120">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="48919-121">删除 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="48919-121">Delete managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-delete.md)|<span data-ttu-id="48919-122">无</span><span class="sxs-lookup"><span data-stu-id="48919-122">None</span></span>|<span data-ttu-id="48919-123">删除 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="48919-123">Deletes a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>|
|[<span data-ttu-id="48919-124">更新 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="48919-124">Update managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-update.md)|[<span data-ttu-id="48919-125">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="48919-125">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="48919-126">更新 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="48919-126">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="48919-127">属性</span><span class="sxs-lookup"><span data-stu-id="48919-127">Properties</span></span>
|<span data-ttu-id="48919-128">属性</span><span class="sxs-lookup"><span data-stu-id="48919-128">Property</span></span>|<span data-ttu-id="48919-129">类型</span><span class="sxs-lookup"><span data-stu-id="48919-129">Type</span></span>|<span data-ttu-id="48919-130">说明</span><span class="sxs-lookup"><span data-stu-id="48919-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48919-131">id</span><span class="sxs-lookup"><span data-stu-id="48919-131">id</span></span>|<span data-ttu-id="48919-132">String</span><span class="sxs-lookup"><span data-stu-id="48919-132">String</span></span>|<span data-ttu-id="48919-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="48919-133">Key of the entity.</span></span>|
|<span data-ttu-id="48919-134">target</span><span class="sxs-lookup"><span data-stu-id="48919-134">target</span></span>|[<span data-ttu-id="48919-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="48919-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="48919-136">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="48919-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="48919-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="48919-137">installIntent</span></span>|[<span data-ttu-id="48919-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="48919-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="48919-139">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="48919-139">The install intent for eBook.</span></span> <span data-ttu-id="48919-140">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="48919-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48919-141">Relationships</span><span class="sxs-lookup"><span data-stu-id="48919-141">Relationships</span></span>
<span data-ttu-id="48919-142">无</span><span class="sxs-lookup"><span data-stu-id="48919-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="48919-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48919-143">JSON Representation</span></span>
<span data-ttu-id="48919-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48919-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```





