---
title: meetingAttendanceReport 资源类型
description: 包含与会议出席报告关联的信息。
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f1ea75f6e57d0e095a470e715e080c7def05ab46
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896723"
---
# <a name="meetingattendancereport-resource-type"></a><span data-ttu-id="eacf1-103">meetingAttendanceReport 资源类型</span><span class="sxs-lookup"><span data-stu-id="eacf1-103">meetingAttendanceReport resource type</span></span>

<span data-ttu-id="eacf1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eacf1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eacf1-105">包含与会议出席报告关联的信息。</span><span class="sxs-lookup"><span data-stu-id="eacf1-105">Contains information associated with meeting attendance report.</span></span>

## <a name="properties"></a><span data-ttu-id="eacf1-106">属性</span><span class="sxs-lookup"><span data-stu-id="eacf1-106">Properties</span></span>

| <span data-ttu-id="eacf1-107">属性</span><span class="sxs-lookup"><span data-stu-id="eacf1-107">Property</span></span>            | <span data-ttu-id="eacf1-108">类型</span><span class="sxs-lookup"><span data-stu-id="eacf1-108">Type</span></span>    | <span data-ttu-id="eacf1-109">说明</span><span class="sxs-lookup"><span data-stu-id="eacf1-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="eacf1-110">attendanceRecords</span><span class="sxs-lookup"><span data-stu-id="eacf1-110">attendanceRecords</span></span>           | <span data-ttu-id="eacf1-111">[attendanceRecord](attendanceRecord.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eacf1-111">[attendanceRecord](attendanceRecord.md) collection</span></span>  | <span data-ttu-id="eacf1-112">考勤记录列表。</span><span class="sxs-lookup"><span data-stu-id="eacf1-112">The list of attendance records.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eacf1-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eacf1-113">JSON representation</span></span>

<span data-ttu-id="eacf1-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eacf1-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingAttendanceReport"
}-->

```json
{
  "attendanceRecords": [{"@odata.type": "#microsoft.graph.attendanceRecord"}]
}
```
