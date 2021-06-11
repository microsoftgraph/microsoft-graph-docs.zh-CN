---
title: attendanceInterval 资源类型
description: 包含与 attendanceRecord 中的出席间隔关联的信息。
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 13b4e20a5233b865dd5417eed4d159bce07c8717
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896513"
---
# <a name="attendanceinterval-resource-type"></a><span data-ttu-id="933e4-103">attendanceInterval 资源类型</span><span class="sxs-lookup"><span data-stu-id="933e4-103">attendanceInterval resource type</span></span>

<span data-ttu-id="933e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="933e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="933e4-105">包含与 attendanceRecord 中的出席间隔关联的信息。</span><span class="sxs-lookup"><span data-stu-id="933e4-105">Contains information associated with attendance interval in attendanceRecord.</span></span>

## <a name="properties"></a><span data-ttu-id="933e4-106">属性</span><span class="sxs-lookup"><span data-stu-id="933e4-106">Properties</span></span>

| <span data-ttu-id="933e4-107">属性</span><span class="sxs-lookup"><span data-stu-id="933e4-107">Property</span></span>            | <span data-ttu-id="933e4-108">类型</span><span class="sxs-lookup"><span data-stu-id="933e4-108">Type</span></span>    | <span data-ttu-id="933e4-109">说明</span><span class="sxs-lookup"><span data-stu-id="933e4-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="933e4-110">joinDateTime</span><span class="sxs-lookup"><span data-stu-id="933e4-110">joinDateTime</span></span> | <span data-ttu-id="933e4-111">日期时间</span><span class="sxs-lookup"><span data-stu-id="933e4-111">DateTime</span></span> | <span data-ttu-id="933e4-112">加入 UTC 时间与会者的时间。</span><span class="sxs-lookup"><span data-stu-id="933e4-112">Time attendee joined in UTC.</span></span> |
| <span data-ttu-id="933e4-113">leaveDateTime</span><span class="sxs-lookup"><span data-stu-id="933e4-113">leaveDateTime</span></span> | <span data-ttu-id="933e4-114">日期时间</span><span class="sxs-lookup"><span data-stu-id="933e4-114">DateTime</span></span> | <span data-ttu-id="933e4-115">时间与会者以 UTC 时间离开。</span><span class="sxs-lookup"><span data-stu-id="933e4-115">Time attendee left in UTC.</span></span> |
| <span data-ttu-id="933e4-116">durationInSeconds</span><span class="sxs-lookup"><span data-stu-id="933e4-116">durationInSeconds</span></span> | <span data-ttu-id="933e4-117">Int32</span><span class="sxs-lookup"><span data-stu-id="933e4-117">Int32</span></span> | <span data-ttu-id="933e4-118">会议间隔的持续时间（以秒为单位）;即 **joinDateTime** 和 **leaveDateTime 之间的差** 值。</span><span class="sxs-lookup"><span data-stu-id="933e4-118">Duration of the meeting interval in seconds; that is, the difference between **joinDateTime** and **leaveDateTime**.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="933e4-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="933e4-119">JSON representation</span></span>

<span data-ttu-id="933e4-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="933e4-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendanceInterval"
}-->

```json

{
    "joinDateTime": "String (timestamp)",
    "leaveDateTime": "String (timestamp)",
    "durationInSeconds": "Int32"
}
    
```
