---
title: managedEBookAssignment 资源类型
description: 包含用于为组分配电子书的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1277ad52a308601ba5712423b70a9ee0dd11a0ca
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44175355"
---
# <a name="managedebookassignment-resource-type"></a><span data-ttu-id="5be16-103">managedEBookAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="5be16-103">managedEBookAssignment resource type</span></span>

<span data-ttu-id="5be16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5be16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5be16-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5be16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5be16-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5be16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5be16-107">包含用于为组分配电子书的属性。</span><span class="sxs-lookup"><span data-stu-id="5be16-107">Contains properties used to assign a eBook to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="5be16-108">方法</span><span class="sxs-lookup"><span data-stu-id="5be16-108">Methods</span></span>
|<span data-ttu-id="5be16-109">方法</span><span class="sxs-lookup"><span data-stu-id="5be16-109">Method</span></span>|<span data-ttu-id="5be16-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5be16-110">Return Type</span></span>|<span data-ttu-id="5be16-111">说明</span><span class="sxs-lookup"><span data-stu-id="5be16-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5be16-112">列出 managedEBookAssignments</span><span class="sxs-lookup"><span data-stu-id="5be16-112">List managedEBookAssignments</span></span>](../api/intune-books-managedebookassignment-list.md)|<span data-ttu-id="5be16-113">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5be16-113">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="5be16-114">列出 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5be16-114">List properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) objects.</span></span>|
|[<span data-ttu-id="5be16-115">获取 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="5be16-115">Get managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-get.md)|[<span data-ttu-id="5be16-116">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="5be16-116">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="5be16-117">读取 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5be16-117">Read properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="5be16-118">创建 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="5be16-118">Create managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-create.md)|[<span data-ttu-id="5be16-119">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="5be16-119">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="5be16-120">创建新的 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5be16-120">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="5be16-121">删除 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="5be16-121">Delete managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-delete.md)|<span data-ttu-id="5be16-122">无</span><span class="sxs-lookup"><span data-stu-id="5be16-122">None</span></span>|<span data-ttu-id="5be16-123">删除 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="5be16-123">Deletes a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>|
|[<span data-ttu-id="5be16-124">更新 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="5be16-124">Update managedEBookAssignment</span></span>](../api/intune-books-managedebookassignment-update.md)|[<span data-ttu-id="5be16-125">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="5be16-125">managedEBookAssignment</span></span>](../resources/intune-books-managedebookassignment.md)|<span data-ttu-id="5be16-126">更新 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5be16-126">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5be16-127">属性</span><span class="sxs-lookup"><span data-stu-id="5be16-127">Properties</span></span>
|<span data-ttu-id="5be16-128">属性</span><span class="sxs-lookup"><span data-stu-id="5be16-128">Property</span></span>|<span data-ttu-id="5be16-129">类型</span><span class="sxs-lookup"><span data-stu-id="5be16-129">Type</span></span>|<span data-ttu-id="5be16-130">说明</span><span class="sxs-lookup"><span data-stu-id="5be16-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5be16-131">id</span><span class="sxs-lookup"><span data-stu-id="5be16-131">id</span></span>|<span data-ttu-id="5be16-132">字符串</span><span class="sxs-lookup"><span data-stu-id="5be16-132">String</span></span>|<span data-ttu-id="5be16-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5be16-133">Key of the entity.</span></span>|
|<span data-ttu-id="5be16-134">target</span><span class="sxs-lookup"><span data-stu-id="5be16-134">target</span></span>|[<span data-ttu-id="5be16-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5be16-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5be16-136">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="5be16-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="5be16-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="5be16-137">installIntent</span></span>|[<span data-ttu-id="5be16-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="5be16-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="5be16-139">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="5be16-139">The install intent for eBook.</span></span> <span data-ttu-id="5be16-140">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="5be16-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5be16-141">关系</span><span class="sxs-lookup"><span data-stu-id="5be16-141">Relationships</span></span>
<span data-ttu-id="5be16-142">无</span><span class="sxs-lookup"><span data-stu-id="5be16-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5be16-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5be16-143">JSON Representation</span></span>
<span data-ttu-id="5be16-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5be16-144">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "installIntent": "String"
}
```



