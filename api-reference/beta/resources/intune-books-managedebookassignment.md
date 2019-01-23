---
title: managedEBookAssignment 资源类型
description: 包含用于为组分配电子书的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6d6cdc1cbe5b2eb7b734219dbb7c67152afe3a2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423543"
---
# <a name="managedebookassignment-resource-type"></a><span data-ttu-id="4f1fa-103">managedEBookAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f1fa-103">managedEBookAssignment resource type</span></span>

> <span data-ttu-id="4f1fa-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4f1fa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4f1fa-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4f1fa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f1fa-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f1fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f1fa-107">包含用于为组分配电子书的属性。</span><span class="sxs-lookup"><span data-stu-id="4f1fa-107">Contains properties used to assign a eBook to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="4f1fa-108">方法</span><span class="sxs-lookup"><span data-stu-id="4f1fa-108">Methods</span></span>
|<span data-ttu-id="4f1fa-109">方法</span><span class="sxs-lookup"><span data-stu-id="4f1fa-109">Method</span></span>|<span data-ttu-id="4f1fa-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4f1fa-110">Return Type</span></span>|<span data-ttu-id="4f1fa-111">说明</span><span class="sxs-lookup"><span data-stu-id="4f1fa-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4f1fa-112">列出 managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="4f1fa-112">List managedEBookAssignments</span></span>](../api/intune-books-managedebookassignment-list.md)|<span data-ttu-id="4f1fa-113">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f1fa-113">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="4f1fa-114">列出 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4f1fa-114">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>|
|[<span data-ttu-id="4f1fa-115">获取 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="4f1fa-115">Get managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-get.md)|[<span data-ttu-id="4f1fa-116">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="4f1fa-116">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="4f1fa-117">读取 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4f1fa-117">Read properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="4f1fa-118">创建 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="4f1fa-118">Create managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-create.md)|[<span data-ttu-id="4f1fa-119">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="4f1fa-119">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="4f1fa-120">创建新的 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f1fa-120">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="4f1fa-121">删除 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="4f1fa-121">Delete managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-delete.md)|<span data-ttu-id="4f1fa-122">无</span><span class="sxs-lookup"><span data-stu-id="4f1fa-122">None</span></span>|<span data-ttu-id="4f1fa-123">删除 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4f1fa-123">Deletes a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>|
|[<span data-ttu-id="4f1fa-124">更新 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="4f1fa-124">Update managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-update.md)|[<span data-ttu-id="4f1fa-125">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="4f1fa-125">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="4f1fa-126">更新 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4f1fa-126">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4f1fa-127">属性</span><span class="sxs-lookup"><span data-stu-id="4f1fa-127">Properties</span></span>
|<span data-ttu-id="4f1fa-128">属性</span><span class="sxs-lookup"><span data-stu-id="4f1fa-128">Property</span></span>|<span data-ttu-id="4f1fa-129">类型</span><span class="sxs-lookup"><span data-stu-id="4f1fa-129">Type</span></span>|<span data-ttu-id="4f1fa-130">说明</span><span class="sxs-lookup"><span data-stu-id="4f1fa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f1fa-131">id</span><span class="sxs-lookup"><span data-stu-id="4f1fa-131">id</span></span>|<span data-ttu-id="4f1fa-132">String</span><span class="sxs-lookup"><span data-stu-id="4f1fa-132">String</span></span>|<span data-ttu-id="4f1fa-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4f1fa-133">Key of the entity.</span></span>|
|<span data-ttu-id="4f1fa-134">target</span><span class="sxs-lookup"><span data-stu-id="4f1fa-134">target</span></span>|[<span data-ttu-id="4f1fa-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4f1fa-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4f1fa-136">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="4f1fa-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="4f1fa-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="4f1fa-137">installIntent</span></span>|[<span data-ttu-id="4f1fa-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="4f1fa-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="4f1fa-139">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="4f1fa-139">The install intent for eBook.</span></span> <span data-ttu-id="4f1fa-140">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="4f1fa-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f1fa-141">Relationships</span><span class="sxs-lookup"><span data-stu-id="4f1fa-141">Relationships</span></span>
<span data-ttu-id="4f1fa-142">无</span><span class="sxs-lookup"><span data-stu-id="4f1fa-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f1fa-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f1fa-143">JSON Representation</span></span>
<span data-ttu-id="4f1fa-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f1fa-144">Here is a JSON representation of the resource.</span></span>
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




