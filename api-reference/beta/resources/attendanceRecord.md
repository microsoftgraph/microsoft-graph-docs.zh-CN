---
title: attendanceRecord 资源类型
description: 包含与与会者报告中的与会者记录关联的信息。
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 20beeca97c790b8743c9038e7fddf0b5c6f69534
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896499"
---
# <a name="attendancerecord-resource-type"></a><span data-ttu-id="6eb03-103">attendanceRecord 资源类型</span><span class="sxs-lookup"><span data-stu-id="6eb03-103">attendanceRecord resource type</span></span>

<span data-ttu-id="6eb03-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6eb03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6eb03-105">包含与与会者报告中的与会者记录关联的信息。</span><span class="sxs-lookup"><span data-stu-id="6eb03-105">Contains information associated with attendance record in meeting attendance report.</span></span>

## <a name="properties"></a><span data-ttu-id="6eb03-106">属性</span><span class="sxs-lookup"><span data-stu-id="6eb03-106">Properties</span></span>

| <span data-ttu-id="6eb03-107">属性</span><span class="sxs-lookup"><span data-stu-id="6eb03-107">Property</span></span>            | <span data-ttu-id="6eb03-108">类型</span><span class="sxs-lookup"><span data-stu-id="6eb03-108">Type</span></span>    | <span data-ttu-id="6eb03-109">说明</span><span class="sxs-lookup"><span data-stu-id="6eb03-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="6eb03-110">identity</span><span class="sxs-lookup"><span data-stu-id="6eb03-110">identity</span></span> | [<span data-ttu-id="6eb03-111">标识</span><span class="sxs-lookup"><span data-stu-id="6eb03-111">Identity</span></span>](identity.md) | <span data-ttu-id="6eb03-112">标识符，例如显示名称。</span><span class="sxs-lookup"><span data-stu-id="6eb03-112">Identifier, such as display name.</span></span> |
| <span data-ttu-id="6eb03-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6eb03-113">emailAddress</span></span> | <span data-ttu-id="6eb03-114">String</span><span class="sxs-lookup"><span data-stu-id="6eb03-114">String</span></span> | <span data-ttu-id="6eb03-115">电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="6eb03-115">Email address.</span></span> |
| <span data-ttu-id="6eb03-116">totalAttendanceInSeconds</span><span class="sxs-lookup"><span data-stu-id="6eb03-116">totalAttendanceInSeconds</span></span> | <span data-ttu-id="6eb03-117">Int32</span><span class="sxs-lookup"><span data-stu-id="6eb03-117">Int32</span></span> | <span data-ttu-id="6eb03-118">总出席持续时间（以秒表示）。</span><span class="sxs-lookup"><span data-stu-id="6eb03-118">Total duration of the attendances in seconds.</span></span> |
| <span data-ttu-id="6eb03-119">attendanceIntervals</span><span class="sxs-lookup"><span data-stu-id="6eb03-119">attendanceIntervals</span></span> | <span data-ttu-id="6eb03-120">[attendanceInterval](attendanceInterval.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6eb03-120">[attendanceInterval](attendanceInterval.md) collection</span></span> | <span data-ttu-id="6eb03-121">加入和离开之间的时间段列表。</span><span class="sxs-lookup"><span data-stu-id="6eb03-121">List of time periods between joining and leaving.</span></span> |
| <span data-ttu-id="6eb03-122">role</span><span class="sxs-lookup"><span data-stu-id="6eb03-122">role</span></span> | <span data-ttu-id="6eb03-123">String</span><span class="sxs-lookup"><span data-stu-id="6eb03-123">String</span></span> | <span data-ttu-id="6eb03-124">与会者的角色。</span><span class="sxs-lookup"><span data-stu-id="6eb03-124">Role of the attendee.</span></span> <span data-ttu-id="6eb03-125">可能的值为 `None` `Attendee` 、、 `Presenter` 和 `Organizer` 。</span><span class="sxs-lookup"><span data-stu-id="6eb03-125">Possible values are `None`, `Attendee`, `Presenter`, and `Organizer`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="6eb03-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6eb03-126">JSON representation</span></span>

<span data-ttu-id="6eb03-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6eb03-127">The following is a JSON representation of the resource.</span></span>

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
