---
title: channelMembersNotificationRecipient 资源类型
description: 表示在活动源中发送的通知Microsoft Teams收件人。 收件人由频道成员组成。
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 821d4f2ee41c15cb93cd3d53b9af9cf1e63db97b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211286"
---
# <a name="channelmembersnotificationrecipient-resource-type"></a><span data-ttu-id="11384-104">channelMembersNotificationRecipient 资源类型</span><span class="sxs-lookup"><span data-stu-id="11384-104">channelMembersNotificationRecipient resource type</span></span>

<span data-ttu-id="11384-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11384-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11384-106">表示在活动源中发送的通知Microsoft Teams收件人。</span><span class="sxs-lookup"><span data-stu-id="11384-106">Represents the recipient of a notification sent in a Microsoft Teams activity feed.</span></span> <span data-ttu-id="11384-107">收件人由频道成员组成。</span><span class="sxs-lookup"><span data-stu-id="11384-107">The recipient consists of the channel members.</span></span>

<span data-ttu-id="11384-108">继承自 [teamworkNotificationRecipient](teamworknotificationrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="11384-108">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="11384-109">属性</span><span class="sxs-lookup"><span data-stu-id="11384-109">Properties</span></span>
| <span data-ttu-id="11384-110">属性</span><span class="sxs-lookup"><span data-stu-id="11384-110">Property</span></span>  | <span data-ttu-id="11384-111">类型</span><span class="sxs-lookup"><span data-stu-id="11384-111">Type</span></span>   | <span data-ttu-id="11384-112">说明</span><span class="sxs-lookup"><span data-stu-id="11384-112">Description</span></span>                                            |
| :-------- | :----- | :----------------------------------------------------- |
| <span data-ttu-id="11384-113">teamId</span><span class="sxs-lookup"><span data-stu-id="11384-113">teamId</span></span>    | <span data-ttu-id="11384-114">String</span><span class="sxs-lookup"><span data-stu-id="11384-114">String</span></span> | <span data-ttu-id="11384-115">频道所在的团队的标识符。</span><span class="sxs-lookup"><span data-stu-id="11384-115">The team's identifier under which the channel resides.</span></span> |
| <span data-ttu-id="11384-116">channelId</span><span class="sxs-lookup"><span data-stu-id="11384-116">channelId</span></span> | <span data-ttu-id="11384-117">String</span><span class="sxs-lookup"><span data-stu-id="11384-117">String</span></span> | <span data-ttu-id="11384-118">频道的标识符。</span><span class="sxs-lookup"><span data-stu-id="11384-118">The channel's identifier.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="11384-119">关系</span><span class="sxs-lookup"><span data-stu-id="11384-119">Relationships</span></span>
<span data-ttu-id="11384-120">无。</span><span class="sxs-lookup"><span data-stu-id="11384-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="11384-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11384-121">JSON representation</span></span>
<span data-ttu-id="11384-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11384-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelMembersNotificationRecipient"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.channelMembersNotificationRecipient",
  "teamId": "String",
  "channelId": "String"
}
```
