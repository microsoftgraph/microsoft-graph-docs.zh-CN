---
title: managedEBookAssignment 资源类型
description: 包含用于为组分配电子书的属性。
author: tfitzmac
ms.openlocfilehash: 26694093b320be1518f92e97877a7331f3f78866
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308461"
---
# <a name="managedebookassignment-resource-type"></a><span data-ttu-id="47ff4-103">managedEBookAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="47ff4-103">managedEBookAssignment resource type</span></span>

> <span data-ttu-id="47ff4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="47ff4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47ff4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="47ff4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47ff4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="47ff4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47ff4-107">包含用于为组分配电子书的属性。</span><span class="sxs-lookup"><span data-stu-id="47ff4-107">Contains properties used to assign a eBook to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="47ff4-108">方法</span><span class="sxs-lookup"><span data-stu-id="47ff4-108">Methods</span></span>
|<span data-ttu-id="47ff4-109">方法</span><span class="sxs-lookup"><span data-stu-id="47ff4-109">Method</span></span>|<span data-ttu-id="47ff4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="47ff4-110">Return Type</span></span>|<span data-ttu-id="47ff4-111">说明</span><span class="sxs-lookup"><span data-stu-id="47ff4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="47ff4-112">列出 managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="47ff4-112">List managedEBookAssignments</span></span>](../api/intune-books-managedebookassignment-list.md)|<span data-ttu-id="47ff4-113">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="47ff4-113">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="47ff4-114">列出 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="47ff4-114">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>|
|[<span data-ttu-id="47ff4-115">获取 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="47ff4-115">Get managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-get.md)|[<span data-ttu-id="47ff4-116">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="47ff4-116">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="47ff4-117">读取 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="47ff4-117">Read properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="47ff4-118">创建 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="47ff4-118">Create managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-create.md)|[<span data-ttu-id="47ff4-119">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="47ff4-119">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="47ff4-120">创建新的 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="47ff4-120">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="47ff4-121">删除 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="47ff4-121">Delete managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-delete.md)|<span data-ttu-id="47ff4-122">无</span><span class="sxs-lookup"><span data-stu-id="47ff4-122">None</span></span>|<span data-ttu-id="47ff4-123">删除 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="47ff4-123">Deletes a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>|
|[<span data-ttu-id="47ff4-124">更新 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="47ff4-124">Update managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-update.md)|[<span data-ttu-id="47ff4-125">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="47ff4-125">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="47ff4-126">更新 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="47ff4-126">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="47ff4-127">属性</span><span class="sxs-lookup"><span data-stu-id="47ff4-127">Properties</span></span>
|<span data-ttu-id="47ff4-128">属性</span><span class="sxs-lookup"><span data-stu-id="47ff4-128">Property</span></span>|<span data-ttu-id="47ff4-129">类型</span><span class="sxs-lookup"><span data-stu-id="47ff4-129">Type</span></span>|<span data-ttu-id="47ff4-130">说明</span><span class="sxs-lookup"><span data-stu-id="47ff4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47ff4-131">id</span><span class="sxs-lookup"><span data-stu-id="47ff4-131">id</span></span>|<span data-ttu-id="47ff4-132">String</span><span class="sxs-lookup"><span data-stu-id="47ff4-132">String</span></span>|<span data-ttu-id="47ff4-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="47ff4-133">Key of the entity.</span></span>|
|<span data-ttu-id="47ff4-134">target</span><span class="sxs-lookup"><span data-stu-id="47ff4-134">target</span></span>|[<span data-ttu-id="47ff4-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="47ff4-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="47ff4-136">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="47ff4-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="47ff4-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="47ff4-137">installIntent</span></span>|[<span data-ttu-id="47ff4-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="47ff4-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="47ff4-139">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="47ff4-139">The install intent for eBook.</span></span> <span data-ttu-id="47ff4-140">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="47ff4-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47ff4-141">Relationships</span><span class="sxs-lookup"><span data-stu-id="47ff4-141">Relationships</span></span>
<span data-ttu-id="47ff4-142">无</span><span class="sxs-lookup"><span data-stu-id="47ff4-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="47ff4-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47ff4-143">JSON Representation</span></span>
<span data-ttu-id="47ff4-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47ff4-144">Here is a JSON representation of the resource.</span></span>
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





