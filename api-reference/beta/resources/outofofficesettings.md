---
title: outOfOfficeSettings 资源类型
description: 表示联机会议的电话访问信息。
author: elvinyang-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4e3e179ec752cfffc4ae4711d9fd0bc541f1506d
ms.sourcegitcommit: 6d04db95bf233d6819d24b01fd7f8b6db57a524c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2021
ms.locfileid: "49796730"
---
# <a name="outofofficesettings-resource-type"></a><span data-ttu-id="9a171-103">outOfOfficeSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a171-103">outOfOfficeSettings resource type</span></span>

<span data-ttu-id="9a171-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a171-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a171-105">表示与用户状态相关的外出设置。 [](presence.md)</span><span class="sxs-lookup"><span data-stu-id="9a171-105">Represents the out of office settings related to the [presence](presence.md) of a user.</span></span>

## <a name="properties"></a><span data-ttu-id="9a171-106">属性</span><span class="sxs-lookup"><span data-stu-id="9a171-106">Properties</span></span>

| <span data-ttu-id="9a171-107">属性</span><span class="sxs-lookup"><span data-stu-id="9a171-107">Property</span></span>            | <span data-ttu-id="9a171-108">类型</span><span class="sxs-lookup"><span data-stu-id="9a171-108">Type</span></span>    | <span data-ttu-id="9a171-109">描述</span><span class="sxs-lookup"><span data-stu-id="9a171-109">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="9a171-110">message</span><span class="sxs-lookup"><span data-stu-id="9a171-110">message</span></span>           | <span data-ttu-id="9a171-111">String</span><span class="sxs-lookup"><span data-stu-id="9a171-111">String</span></span>  | <span data-ttu-id="9a171-112">用户在 Outlook 客户端上配置的外出邮件 (自动答复 (外出) ) 或 Teams 客户端 (计划外出) 。</span><span class="sxs-lookup"><span data-stu-id="9a171-112">The out of office message that the user configured on Outlook client (Automatic Replies (Out of Office)) or the Teams client (Schedule out of office).</span></span> |
| <span data-ttu-id="9a171-113">isOutOfOffice</span><span class="sxs-lookup"><span data-stu-id="9a171-113">isOutOfOffice</span></span>      | <span data-ttu-id="9a171-114">布尔</span><span class="sxs-lookup"><span data-stu-id="9a171-114">Boolean</span></span>  | <span data-ttu-id="9a171-115">如此 如果：</span><span class="sxs-lookup"><span data-stu-id="9a171-115">True if either:</span></span></br><ul><li><span data-ttu-id="9a171-116">它当前处于 Outlook 或 Teams 客户端上配置的外出时间窗口。</span><span class="sxs-lookup"><span data-stu-id="9a171-116">It is currently in the out of office time window configured on the Outlook or Teams client.</span></span></li><li><span data-ttu-id="9a171-117">用户日历上当前有一个标记为"外出"的事件</span><span class="sxs-lookup"><span data-stu-id="9a171-117">There is currently an event on the user's calendar that's marked as Show as Out of Office</span></span></li></ul></br><span data-ttu-id="9a171-118">否则为 false。</span><span class="sxs-lookup"><span data-stu-id="9a171-118">Otherwise, false.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9a171-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a171-119">JSON representation</span></span>

<span data-ttu-id="9a171-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a171-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.outOfOfficeSettings"
}-->
```json
{
  "message": "String",
  "isOutOfOffice": "Boolean"
}
```
