---
title: educationTeacher 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a2eae690076553090dbd32f46f0b777a998b615d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979537"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="90d7d-103">educationTeacher 资源类型</span><span class="sxs-lookup"><span data-stu-id="90d7d-103">educationTeacher resource type</span></span>

<span data-ttu-id="90d7d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90d7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90d7d-105">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `teacher` 时显示。</span><span class="sxs-lookup"><span data-stu-id="90d7d-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="90d7d-106">使用委派权限作用域时，Graph 将仅返回 `externalId` 属性。</span><span class="sxs-lookup"><span data-stu-id="90d7d-106">When using Delegated permission scopes, Graph will only return the `externalId` properties.</span></span> <span data-ttu-id="90d7d-107">所有其他属性都需要应用程序范围。</span><span class="sxs-lookup"><span data-stu-id="90d7d-107">All other properties require Application scopes.</span></span>

## <a name="properties"></a><span data-ttu-id="90d7d-108">属性</span><span class="sxs-lookup"><span data-stu-id="90d7d-108">Properties</span></span>

| <span data-ttu-id="90d7d-109">属性</span><span class="sxs-lookup"><span data-stu-id="90d7d-109">Property</span></span>      | <span data-ttu-id="90d7d-110">类型</span><span class="sxs-lookup"><span data-stu-id="90d7d-110">Type</span></span>   | <span data-ttu-id="90d7d-111">说明</span><span class="sxs-lookup"><span data-stu-id="90d7d-111">Description</span></span>                                  |
| :------------ | :----- | :------------------------------------------- |
| <span data-ttu-id="90d7d-112">externalId</span><span class="sxs-lookup"><span data-stu-id="90d7d-112">externalId</span></span>    | <span data-ttu-id="90d7d-113">String</span><span class="sxs-lookup"><span data-stu-id="90d7d-113">String</span></span> | <span data-ttu-id="90d7d-114">外部源系统中的教师 Id。</span><span class="sxs-lookup"><span data-stu-id="90d7d-114">Id of the Teacher in external source system.</span></span> |
| <span data-ttu-id="90d7d-115">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="90d7d-115">teacherNumber</span></span> | <span data-ttu-id="90d7d-116">String</span><span class="sxs-lookup"><span data-stu-id="90d7d-116">String</span></span> | <span data-ttu-id="90d7d-117">教师编号。</span><span class="sxs-lookup"><span data-stu-id="90d7d-117">Teacher number.</span></span>                              |

## <a name="json-representation"></a><span data-ttu-id="90d7d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90d7d-118">JSON representation</span></span>

<span data-ttu-id="90d7d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90d7d-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


