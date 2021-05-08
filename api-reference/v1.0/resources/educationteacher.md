---
title: educationTeacher 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6e5e60f04af74cd09f893823e9544ba455b60113
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231841"
---
# <a name="teacher-resource-type"></a><span data-ttu-id="03c46-103">教师资源类型</span><span class="sxs-lookup"><span data-stu-id="03c46-103">Teacher resource type</span></span>

<span data-ttu-id="03c46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03c46-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="03c46-105">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。</span><span class="sxs-lookup"><span data-stu-id="03c46-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>

## <a name="properties"></a><span data-ttu-id="03c46-106">属性</span><span class="sxs-lookup"><span data-stu-id="03c46-106">Properties</span></span>

| <span data-ttu-id="03c46-107">属性</span><span class="sxs-lookup"><span data-stu-id="03c46-107">Property</span></span>      | <span data-ttu-id="03c46-108">类型</span><span class="sxs-lookup"><span data-stu-id="03c46-108">Type</span></span>   | <span data-ttu-id="03c46-109">说明</span><span class="sxs-lookup"><span data-stu-id="03c46-109">Description</span></span>                             |
| :------------ | :----- | :-------------------------------------- |
| <span data-ttu-id="03c46-110">externalId</span><span class="sxs-lookup"><span data-stu-id="03c46-110">externalId</span></span>    | <span data-ttu-id="03c46-111">String</span><span class="sxs-lookup"><span data-stu-id="03c46-111">String</span></span> | <span data-ttu-id="03c46-112">源系统中教师的 ID。</span><span class="sxs-lookup"><span data-stu-id="03c46-112">ID of the teacher in the source system.</span></span> |
| <span data-ttu-id="03c46-113">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="03c46-113">teacherNumber</span></span> | <span data-ttu-id="03c46-114">String</span><span class="sxs-lookup"><span data-stu-id="03c46-114">String</span></span> | <span data-ttu-id="03c46-115">教师编号。</span><span class="sxs-lookup"><span data-stu-id="03c46-115">Teacher number.</span></span>                         |

## <a name="relationships"></a><span data-ttu-id="03c46-116">关系</span><span class="sxs-lookup"><span data-stu-id="03c46-116">Relationships</span></span>

<span data-ttu-id="03c46-117">无。</span><span class="sxs-lookup"><span data-stu-id="03c46-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="03c46-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03c46-118">JSON representation</span></span>

<span data-ttu-id="03c46-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03c46-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationTeacher"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationTeacher",
  "teacherNumber": "String",
  "externalId": "String"
}
```
