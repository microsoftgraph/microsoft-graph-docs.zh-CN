---
title: managedEBookAssignment 资源类型
description: 包含用于为组分配电子书的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39fc5a56e4fb63a62a4fe2c15dd478efda426636
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949862"
---
# <a name="managedebookassignment-resource-type"></a><span data-ttu-id="e24a3-103">managedEBookAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="e24a3-103">managedEBookAssignment resource type</span></span>

> <span data-ttu-id="e24a3-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e24a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e24a3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e24a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e24a3-106">包含用于为组分配电子书的属性。</span><span class="sxs-lookup"><span data-stu-id="e24a3-106">Contains properties used to assign a eBook to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="e24a3-107">方法</span><span class="sxs-lookup"><span data-stu-id="e24a3-107">Methods</span></span>
|<span data-ttu-id="e24a3-108">方法</span><span class="sxs-lookup"><span data-stu-id="e24a3-108">Method</span></span>|<span data-ttu-id="e24a3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e24a3-109">Return Type</span></span>|<span data-ttu-id="e24a3-110">说明</span><span class="sxs-lookup"><span data-stu-id="e24a3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e24a3-111">列出 managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="e24a3-111">List managedEBookAssignments</span></span>](../api/intune-books-managedebookassignment-list.md)|<span data-ttu-id="e24a3-112">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e24a3-112">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="e24a3-113">列出 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e24a3-113">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>|
|[<span data-ttu-id="e24a3-114">获取 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="e24a3-114">Get managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-get.md)|[<span data-ttu-id="e24a3-115">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="e24a3-115">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="e24a3-116">读取 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e24a3-116">Read properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="e24a3-117">创建 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="e24a3-117">Create managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-create.md)|[<span data-ttu-id="e24a3-118">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="e24a3-118">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="e24a3-119">创建新的 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e24a3-119">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="e24a3-120">删除 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="e24a3-120">Delete managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-delete.md)|<span data-ttu-id="e24a3-121">无</span><span class="sxs-lookup"><span data-stu-id="e24a3-121">None</span></span>|<span data-ttu-id="e24a3-122">删除 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="e24a3-122">Deletes a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>|
|[<span data-ttu-id="e24a3-123">更新 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="e24a3-123">Update managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-update.md)|[<span data-ttu-id="e24a3-124">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="e24a3-124">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="e24a3-125">更新 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e24a3-125">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e24a3-126">属性</span><span class="sxs-lookup"><span data-stu-id="e24a3-126">Properties</span></span>
|<span data-ttu-id="e24a3-127">属性</span><span class="sxs-lookup"><span data-stu-id="e24a3-127">Property</span></span>|<span data-ttu-id="e24a3-128">类型</span><span class="sxs-lookup"><span data-stu-id="e24a3-128">Type</span></span>|<span data-ttu-id="e24a3-129">说明</span><span class="sxs-lookup"><span data-stu-id="e24a3-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e24a3-130">id</span><span class="sxs-lookup"><span data-stu-id="e24a3-130">id</span></span>|<span data-ttu-id="e24a3-131">String</span><span class="sxs-lookup"><span data-stu-id="e24a3-131">String</span></span>|<span data-ttu-id="e24a3-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e24a3-132">Key of the entity.</span></span>|
|<span data-ttu-id="e24a3-133">target</span><span class="sxs-lookup"><span data-stu-id="e24a3-133">target</span></span>|[<span data-ttu-id="e24a3-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e24a3-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e24a3-135">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="e24a3-135">The assignment target for eBook.</span></span>|
|<span data-ttu-id="e24a3-136">installIntent</span><span class="sxs-lookup"><span data-stu-id="e24a3-136">installIntent</span></span>|[<span data-ttu-id="e24a3-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="e24a3-137">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="e24a3-138">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="e24a3-138">The install intent for eBook.</span></span> <span data-ttu-id="e24a3-139">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="e24a3-139">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e24a3-140">关系</span><span class="sxs-lookup"><span data-stu-id="e24a3-140">Relationships</span></span>
<span data-ttu-id="e24a3-141">无</span><span class="sxs-lookup"><span data-stu-id="e24a3-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e24a3-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e24a3-142">JSON Representation</span></span>
<span data-ttu-id="e24a3-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e24a3-143">Here is a JSON representation of the resource.</span></span>
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




