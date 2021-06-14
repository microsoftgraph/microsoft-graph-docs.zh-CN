---
title: educationAssignmentDefaults 资源类型
description: 指定在类中创建的新作业所遵守的类级别默认值
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e990e7fe940fface9ecc33d066ce86b6cc331e4f
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912256"
---
# <a name="educationassignmentdefaults-resource-type"></a><span data-ttu-id="cbc08-103">educationAssignmentDefaults 资源类型</span><span class="sxs-lookup"><span data-stu-id="cbc08-103">educationAssignmentDefaults resource type</span></span>

<span data-ttu-id="cbc08-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cbc08-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cbc08-105">指定在类中创建的新工作分配所遵守的类级别默认值。</span><span class="sxs-lookup"><span data-stu-id="cbc08-105">Specifies class-level defaults respected by new assignments created in the class.</span></span> 

<span data-ttu-id="cbc08-106">如果调用方不希望使用默认行为，可以继续为每个工作分配创建指定自定义值。</span><span class="sxs-lookup"><span data-stu-id="cbc08-106">Callers can continue to specify custom values on each assignment creation if they Don't want the default behaviors.</span></span>

## <a name="methods"></a><span data-ttu-id="cbc08-107">方法</span><span class="sxs-lookup"><span data-stu-id="cbc08-107">Methods</span></span>
|<span data-ttu-id="cbc08-108">方法</span><span class="sxs-lookup"><span data-stu-id="cbc08-108">Method</span></span>|<span data-ttu-id="cbc08-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cbc08-109">Return type</span></span>|<span data-ttu-id="cbc08-110">说明</span><span class="sxs-lookup"><span data-stu-id="cbc08-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cbc08-111">获取 educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="cbc08-111">Get educationAssignmentDefaults</span></span>](../api/educationassignmentdefaults-get.md)|[<span data-ttu-id="cbc08-112">educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="cbc08-112">educationAssignmentDefaults</span></span>](../resources/educationassignmentdefaults.md)|<span data-ttu-id="cbc08-113">读取 [educationAssignmentDefaults 对象的属性和](../resources/educationassignmentdefaults.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="cbc08-113">Read the properties and relationships of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span>|
|[<span data-ttu-id="cbc08-114">更新 educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="cbc08-114">Update educationAssignmentDefaults</span></span>](../api/educationassignmentdefaults-update.md)|[<span data-ttu-id="cbc08-115">educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="cbc08-115">educationAssignmentDefaults</span></span>](../resources/educationassignmentdefaults.md)|<span data-ttu-id="cbc08-116">更新 [educationAssignmentDefaults 对象](../resources/educationassignmentdefaults.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="cbc08-116">Update the properties of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cbc08-117">属性</span><span class="sxs-lookup"><span data-stu-id="cbc08-117">Properties</span></span>
|<span data-ttu-id="cbc08-118">属性</span><span class="sxs-lookup"><span data-stu-id="cbc08-118">Property</span></span>|<span data-ttu-id="cbc08-119">类型</span><span class="sxs-lookup"><span data-stu-id="cbc08-119">Type</span></span>|<span data-ttu-id="cbc08-120">说明</span><span class="sxs-lookup"><span data-stu-id="cbc08-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbc08-121">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="cbc08-121">addedStudentAction</span></span>|<span data-ttu-id="cbc08-122">educationAddedStudentAction</span><span class="sxs-lookup"><span data-stu-id="cbc08-122">educationAddedStudentAction</span></span>|<span data-ttu-id="cbc08-123">用于处理作业发布后添加的学生的课堂级别默认行为。</span><span class="sxs-lookup"><span data-stu-id="cbc08-123">Class-level default behavior for handling students who are added after the assignment is published.</span></span> <span data-ttu-id="cbc08-124">可取值为：`none`、`assignIfOpen`。</span><span class="sxs-lookup"><span data-stu-id="cbc08-124">Possible values are: `none`, `assignIfOpen`.</span></span>|
|<span data-ttu-id="cbc08-125">dueTime</span><span class="sxs-lookup"><span data-stu-id="cbc08-125">dueTime</span></span>|<span data-ttu-id="cbc08-126">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="cbc08-126">TimeOfDay</span></span>|<span data-ttu-id="cbc08-127">"到期时间"字段的类级别默认值。</span><span class="sxs-lookup"><span data-stu-id="cbc08-127">Class-level default value for due time field.</span></span> <span data-ttu-id="cbc08-128">默认值为 `23:59:00`。</span><span class="sxs-lookup"><span data-stu-id="cbc08-128">Default value is `23:59:00`.</span></span>|
|<span data-ttu-id="cbc08-129">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="cbc08-129">notificationChannelUrl</span></span>|<span data-ttu-id="cbc08-130">String</span><span class="sxs-lookup"><span data-stu-id="cbc08-130">String</span></span>|<span data-ttu-id="cbc08-131">默认Teams通知将发送到的频道。</span><span class="sxs-lookup"><span data-stu-id="cbc08-131">Default Teams channel to which notifications will be sent.</span></span> <span data-ttu-id="cbc08-132">默认值为 `null`。</span><span class="sxs-lookup"><span data-stu-id="cbc08-132">Default value is `null`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbc08-133">关系</span><span class="sxs-lookup"><span data-stu-id="cbc08-133">Relationships</span></span>
<span data-ttu-id="cbc08-134">无。</span><span class="sxs-lookup"><span data-stu-id="cbc08-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbc08-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cbc08-135">JSON representation</span></span>
<span data-ttu-id="cbc08-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbc08-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentDefaults",
  "openType": false
}
-->
``` json
{
  "addedStudentAction": "String",
  "dueTime": "String (timestamp)",
  "notificationChannelUrl": "String"
}
```

