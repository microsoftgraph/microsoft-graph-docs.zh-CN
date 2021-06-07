---
title: educationAssignmentDefaults 资源类型
description: 指定在类中创建的新作业所遵守的类级别默认值
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: cdd4cb3814900f41f7cb7ee5ede407af61e9c4d7
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781063"
---
# <a name="educationassignmentdefaults-resource-type"></a><span data-ttu-id="d2139-103">educationAssignmentDefaults 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2139-103">educationAssignmentDefaults resource type</span></span>

<span data-ttu-id="d2139-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2139-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2139-105">指定在类中创建的新工作分配所遵守的类级别默认值。</span><span class="sxs-lookup"><span data-stu-id="d2139-105">Specifies class-level defaults respected by new assignments created in the class.</span></span> <span data-ttu-id="d2139-106">如果调用方不需要默认行为，可以继续为每个工作分配创建指定自定义值。</span><span class="sxs-lookup"><span data-stu-id="d2139-106">Callers can continue to specify custom values on each assignment creation if they do not want the default behaviors.</span></span>

## <a name="methods"></a><span data-ttu-id="d2139-107">方法</span><span class="sxs-lookup"><span data-stu-id="d2139-107">Methods</span></span>
|<span data-ttu-id="d2139-108">方法</span><span class="sxs-lookup"><span data-stu-id="d2139-108">Method</span></span>|<span data-ttu-id="d2139-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2139-109">Return type</span></span>|<span data-ttu-id="d2139-110">说明</span><span class="sxs-lookup"><span data-stu-id="d2139-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2139-111">获取 educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="d2139-111">Get educationAssignmentDefaults</span></span>](../api/educationassignmentdefaults-get.md)|[<span data-ttu-id="d2139-112">educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="d2139-112">educationAssignmentDefaults</span></span>](../resources/educationassignmentdefaults.md)|<span data-ttu-id="d2139-113">读取 [educationAssignmentDefaults 对象的属性和](../resources/educationassignmentdefaults.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="d2139-113">Read the properties and relationships of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span>|
|[<span data-ttu-id="d2139-114">更新 educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="d2139-114">Update educationAssignmentDefaults</span></span>](../api/educationassignmentdefaults-update.md)|[<span data-ttu-id="d2139-115">educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="d2139-115">educationAssignmentDefaults</span></span>](../resources/educationassignmentdefaults.md)|<span data-ttu-id="d2139-116">更新 [educationAssignmentDefaults 对象](../resources/educationassignmentdefaults.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="d2139-116">Update the properties of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2139-117">属性</span><span class="sxs-lookup"><span data-stu-id="d2139-117">Properties</span></span>
|<span data-ttu-id="d2139-118">属性</span><span class="sxs-lookup"><span data-stu-id="d2139-118">Property</span></span>|<span data-ttu-id="d2139-119">类型</span><span class="sxs-lookup"><span data-stu-id="d2139-119">Type</span></span>|<span data-ttu-id="d2139-120">说明</span><span class="sxs-lookup"><span data-stu-id="d2139-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2139-121">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="d2139-121">addedStudentAction</span></span>|<span data-ttu-id="d2139-122">educationAddedStudentAction</span><span class="sxs-lookup"><span data-stu-id="d2139-122">educationAddedStudentAction</span></span>|<span data-ttu-id="d2139-123">用于处理作业发布后添加的学生的课堂级别默认行为。</span><span class="sxs-lookup"><span data-stu-id="d2139-123">Class-level default behavior for handling students who are added after the assignment is published.</span></span> <span data-ttu-id="d2139-124">可取值为：`none`、`assignIfOpen`。</span><span class="sxs-lookup"><span data-stu-id="d2139-124">Possible values are: `none`, `assignIfOpen`.</span></span>|
|<span data-ttu-id="d2139-125">addToCalendarAction</span><span class="sxs-lookup"><span data-stu-id="d2139-125">addToCalendarAction</span></span>| <span data-ttu-id="d2139-126">educationAddToCalendarOptions</span><span class="sxs-lookup"><span data-stu-id="d2139-126">educationAddToCalendarOptions</span></span>|<span data-ttu-id="d2139-127">可选字段，用于控制在作业发布时将作业添加到学生和教师的日历中。</span><span class="sxs-lookup"><span data-stu-id="d2139-127">Optional field to control the asfor adding assignments to students' and teachers' calendars when the assignment is published.</span></span> <span data-ttu-id="d2139-128">可取值为：`studentsAndPublisher`、`studentsAndTeamOwners`、`none`。</span><span class="sxs-lookup"><span data-stu-id="d2139-128">Possible values are: `studentsAndPublisher`, `studentsAndTeamOwners`, `none`.</span></span> <span data-ttu-id="d2139-129">默认值为 `none`。</span><span class="sxs-lookup"><span data-stu-id="d2139-129">Default value is `none`.</span></span>|
|<span data-ttu-id="d2139-130">dueTime</span><span class="sxs-lookup"><span data-stu-id="d2139-130">dueTime</span></span>|<span data-ttu-id="d2139-131">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d2139-131">TimeOfDay</span></span>|<span data-ttu-id="d2139-132">"到期时间"字段的类级别默认值。</span><span class="sxs-lookup"><span data-stu-id="d2139-132">Class-level default value for due time field.</span></span> <span data-ttu-id="d2139-133">默认值为 `23:59:00`。</span><span class="sxs-lookup"><span data-stu-id="d2139-133">Default value is `23:59:00`.</span></span>|
|<span data-ttu-id="d2139-134">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="d2139-134">notificationChannelUrl</span></span>|<span data-ttu-id="d2139-135">String</span><span class="sxs-lookup"><span data-stu-id="d2139-135">String</span></span>|<span data-ttu-id="d2139-136">默认Teams通知将发送到的频道。</span><span class="sxs-lookup"><span data-stu-id="d2139-136">Default Teams channel to which notifications will be sent.</span></span> <span data-ttu-id="d2139-137">默认值为 `null`。</span><span class="sxs-lookup"><span data-stu-id="d2139-137">Default value is `null`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2139-138">关系</span><span class="sxs-lookup"><span data-stu-id="d2139-138">Relationships</span></span>
<span data-ttu-id="d2139-139">无。</span><span class="sxs-lookup"><span data-stu-id="d2139-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2139-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2139-140">JSON representation</span></span>
<span data-ttu-id="d2139-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2139-141">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentDefaults",
  "openType": false
}
-->
``` json
{
  "addedStudentAction": "none",
  "addToCalendarAction": "none",
  "dueTime": "23:59:00",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
}
```

