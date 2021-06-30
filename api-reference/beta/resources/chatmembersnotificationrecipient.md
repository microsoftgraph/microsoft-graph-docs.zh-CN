---
title: chatMembersNotificationRecipient 资源类型
description: 表示在活动源中发送的通知Microsoft Teams收件人。 收件人由聊天成员组成。
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3743d9d37e934cd61f699febfcc148afb8e84e98
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211283"
---
# <a name="chatmembersnotificationrecipient-resource-type"></a><span data-ttu-id="63019-104">chatMembersNotificationRecipient 资源类型</span><span class="sxs-lookup"><span data-stu-id="63019-104">chatMembersNotificationRecipient resource type</span></span>

<span data-ttu-id="63019-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63019-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63019-106">表示在活动源中发送的通知Microsoft Teams收件人。</span><span class="sxs-lookup"><span data-stu-id="63019-106">Represents the recipient of a notification sent in a Microsoft Teams activity feed.</span></span> <span data-ttu-id="63019-107">收件人由聊天成员组成。</span><span class="sxs-lookup"><span data-stu-id="63019-107">The recipient consists of the chat members.</span></span>

<span data-ttu-id="63019-108">继承自 [teamworkNotificationRecipient](teamworknotificationrecipient.md)。</span><span class="sxs-lookup"><span data-stu-id="63019-108">Inherits from [teamworkNotificationRecipient](teamworknotificationrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="63019-109">属性</span><span class="sxs-lookup"><span data-stu-id="63019-109">Properties</span></span>
|<span data-ttu-id="63019-110">属性</span><span class="sxs-lookup"><span data-stu-id="63019-110">Property</span></span>|<span data-ttu-id="63019-111">类型</span><span class="sxs-lookup"><span data-stu-id="63019-111">Type</span></span>|<span data-ttu-id="63019-112">说明</span><span class="sxs-lookup"><span data-stu-id="63019-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63019-113">chatId</span><span class="sxs-lookup"><span data-stu-id="63019-113">chatId</span></span>|<span data-ttu-id="63019-114">String</span><span class="sxs-lookup"><span data-stu-id="63019-114">String</span></span>|<span data-ttu-id="63019-115">聊天的标识符。</span><span class="sxs-lookup"><span data-stu-id="63019-115">The chat's identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63019-116">关系</span><span class="sxs-lookup"><span data-stu-id="63019-116">Relationships</span></span>
<span data-ttu-id="63019-117">无。</span><span class="sxs-lookup"><span data-stu-id="63019-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63019-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63019-118">JSON representation</span></span>
<span data-ttu-id="63019-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63019-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMembersNotificationRecipient"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.chatMembersNotificationRecipient",
  "chatId": "String"
}
```

