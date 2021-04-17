---
title: attendanceRecord 资源类型
description: 包含与与会者报告中的与会者记录关联的信息。
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 025c878d8778604bab34dda15f6ab0fa2c541151
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882646"
---
# <a name="attendancerecord-resource-type"></a><span data-ttu-id="ababb-103">attendanceRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="ababb-103">attendanceRecord resource type</span></span>

<span data-ttu-id="ababb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ababb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ababb-105">包含与与会者报告中的与会者记录关联的信息。</span><span class="sxs-lookup"><span data-stu-id="ababb-105">Contains information associated with attendance record in meeting attendance report.</span></span>

## <a name="properties"></a><span data-ttu-id="ababb-106">属性</span><span class="sxs-lookup"><span data-stu-id="ababb-106">Properties</span></span>

| <span data-ttu-id="ababb-107">属性</span><span class="sxs-lookup"><span data-stu-id="ababb-107">Property</span></span>            | <span data-ttu-id="ababb-108">类型</span><span class="sxs-lookup"><span data-stu-id="ababb-108">Type</span></span>    | <span data-ttu-id="ababb-109">说明</span><span class="sxs-lookup"><span data-stu-id="ababb-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="ababb-110">identity</span><span class="sxs-lookup"><span data-stu-id="ababb-110">identity</span></span> | [<span data-ttu-id="ababb-111">标识</span><span class="sxs-lookup"><span data-stu-id="ababb-111">Identity</span></span>](identity.md) | <span data-ttu-id="ababb-112">标识符，例如显示名称。</span><span class="sxs-lookup"><span data-stu-id="ababb-112">Identifier, such as display name.</span></span> |
| <span data-ttu-id="ababb-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ababb-113">emailAddress</span></span> | <span data-ttu-id="ababb-114">String</span><span class="sxs-lookup"><span data-stu-id="ababb-114">String</span></span> | <span data-ttu-id="ababb-115">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="ababb-115">Email address.</span></span> |
| <span data-ttu-id="ababb-116">totalAttendanceInSeconds</span><span class="sxs-lookup"><span data-stu-id="ababb-116">totalAttendanceInSeconds</span></span> | <span data-ttu-id="ababb-117">Int32</span><span class="sxs-lookup"><span data-stu-id="ababb-117">Int32</span></span> | <span data-ttu-id="ababb-118">总出席持续时间（以秒表示）。</span><span class="sxs-lookup"><span data-stu-id="ababb-118">Total duration of the attendances in seconds.</span></span> |
| <span data-ttu-id="ababb-119">attendanceIntervals</span><span class="sxs-lookup"><span data-stu-id="ababb-119">attendanceIntervals</span></span> | <span data-ttu-id="ababb-120">[attendanceInterval](attendanceInterval.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ababb-120">[attendanceInterval](attendanceInterval.md) collection</span></span> | <span data-ttu-id="ababb-121">加入和离开之间的时间段列表。</span><span class="sxs-lookup"><span data-stu-id="ababb-121">List of time periods between joining and leaving.</span></span> |
| <span data-ttu-id="ababb-122">role</span><span class="sxs-lookup"><span data-stu-id="ababb-122">role</span></span> | <span data-ttu-id="ababb-123">String</span><span class="sxs-lookup"><span data-stu-id="ababb-123">String</span></span> | <span data-ttu-id="ababb-124">与会者的角色。</span><span class="sxs-lookup"><span data-stu-id="ababb-124">Role of the attendee.</span></span> <span data-ttu-id="ababb-125">可能的值为 `None` `Attendee` 、、 `Presenter` 和 `Organizer` 。</span><span class="sxs-lookup"><span data-stu-id="ababb-125">Possible values are `None`, `Attendee`, `Presenter`, and `Organizer`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="ababb-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ababb-126">JSON representation</span></span>

<span data-ttu-id="ababb-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ababb-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendanceRecord"
}-->

```json

{
    "emailAddress": "String",
    "totalAttendanceInSeconds": "Int32",
    "role": "String(None|Attendee|Presenter|Organizer)",
    "identity": {"@odata.type": "#microsoft.graph.identity"},
    "attendanceIntervals": [{"@odata.type": "#microsoft.graph.attendanceInterval"}]
}

```
