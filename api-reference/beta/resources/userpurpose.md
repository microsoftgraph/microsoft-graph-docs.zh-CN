---
title: userPurpose 资源类型
description: 代表 Exchange Online 中的用户的收件人或邮箱类型。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 83abf3bd19434867bbd162b6260ed5f4445d8ffd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057841"
---
# <a name="userpurpose-resource-type"></a><span data-ttu-id="c973a-103">userPurpose 资源类型</span><span class="sxs-lookup"><span data-stu-id="c973a-103">userPurpose resource type</span></span>

<span data-ttu-id="c973a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c973a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c973a-105">邮箱的用途。</span><span class="sxs-lookup"><span data-stu-id="c973a-105">The purpose of the mailbox.</span></span> <span data-ttu-id="c973a-106">用于将单个用户的邮箱与 Exchange Online 中的共享邮箱和设备邮箱区分开来。</span><span class="sxs-lookup"><span data-stu-id="c973a-106">Used to differentiate a mailbox for a single user from a shared mailbox and equipment mailbox in Exchange Online.</span></span>


## <a name="properties"></a><span data-ttu-id="c973a-107">属性</span><span class="sxs-lookup"><span data-stu-id="c973a-107">Properties</span></span>
|<span data-ttu-id="c973a-108">属性</span><span class="sxs-lookup"><span data-stu-id="c973a-108">Property</span></span>|<span data-ttu-id="c973a-109">类型</span><span class="sxs-lookup"><span data-stu-id="c973a-109">Type</span></span>|<span data-ttu-id="c973a-110">说明</span><span class="sxs-lookup"><span data-stu-id="c973a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c973a-111">值</span><span class="sxs-lookup"><span data-stu-id="c973a-111">value</span></span>|[<span data-ttu-id="c973a-112">mailboxRecipientType</span><span class="sxs-lookup"><span data-stu-id="c973a-112">mailboxRecipientType</span></span>](#mailboxrecipienttype-values)|<span data-ttu-id="c973a-113">代表 Exchange Online 中的用户的收件人或邮箱类型。</span><span class="sxs-lookup"><span data-stu-id="c973a-113">Represents the user's recipient or mailbox type in Exchange Online.</span></span> <span data-ttu-id="c973a-114">可能的值为：、、、、、 `unknown` `user` `linked` `shared` `room` `equipment` 和 `others` 。</span><span class="sxs-lookup"><span data-stu-id="c973a-114">Possible values are: `unknown`, `user`, `linked`, `shared`, `room`, `equipment`, and `others`.</span></span> <span data-ttu-id="c973a-115">有关详细信息，请参阅下一节。</span><span class="sxs-lookup"><span data-stu-id="c973a-115">See the next section for more information.</span></span>|

### <a name="mailboxrecipienttype-values"></a><span data-ttu-id="c973a-116">mailboxRecipientType 值</span><span class="sxs-lookup"><span data-stu-id="c973a-116">mailboxRecipientType values</span></span>
|<span data-ttu-id="c973a-117">成员</span><span class="sxs-lookup"><span data-stu-id="c973a-117">Member</span></span>|<span data-ttu-id="c973a-118">说明</span><span class="sxs-lookup"><span data-stu-id="c973a-118">Description</span></span>|
|:---------------|:--------|
|<span data-ttu-id="c973a-119">unknown</span><span class="sxs-lookup"><span data-stu-id="c973a-119">unknown</span></span>|<span data-ttu-id="c973a-120">找不到有关邮箱的任何信息。</span><span class="sxs-lookup"><span data-stu-id="c973a-120">No information found about the mailbox.</span></span>|
|<span data-ttu-id="c973a-121">user</span><span class="sxs-lookup"><span data-stu-id="c973a-121">user</span></span>|<span data-ttu-id="c973a-122">具有本地林中邮箱的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="c973a-122">A user account with a mailbox in the local forest.</span></span>|
|<span data-ttu-id="c973a-123">带有</span><span class="sxs-lookup"><span data-stu-id="c973a-123">linked</span></span>|<span data-ttu-id="c973a-124">链接到另一个林中的用户帐户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="c973a-124">A mailbox linked to a user account in another forest.</span></span>|
|<span data-ttu-id="c973a-125">shared</span><span class="sxs-lookup"><span data-stu-id="c973a-125">shared</span></span>|<span data-ttu-id="c973a-126">由两个或更多用户帐户共享的邮箱。</span><span class="sxs-lookup"><span data-stu-id="c973a-126">A mailbox shared by two or more user accounts.</span></span>|
|<span data-ttu-id="c973a-127">室</span><span class="sxs-lookup"><span data-stu-id="c973a-127">room</span></span>|<span data-ttu-id="c973a-128">表示会议室的邮箱。</span><span class="sxs-lookup"><span data-stu-id="c973a-128">A mailbox representing a conference room.</span></span>|
|<span data-ttu-id="c973a-129">器械</span><span class="sxs-lookup"><span data-stu-id="c973a-129">equipment</span></span>|<span data-ttu-id="c973a-130">表示设备的邮箱。</span><span class="sxs-lookup"><span data-stu-id="c973a-130">A mailbox representing a piece of equipment.</span></span>|
|<span data-ttu-id="c973a-131">一些</span><span class="sxs-lookup"><span data-stu-id="c973a-131">others</span></span>|<span data-ttu-id="c973a-132">找到了邮箱，但用户目的与上面指定的不同。</span><span class="sxs-lookup"><span data-stu-id="c973a-132">Mailbox found but user purpose is different from the ones specified above.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c973a-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c973a-133">JSON representation</span></span>

<span data-ttu-id="c973a-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c973a-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userPurpose"
}-->

```json
{
    "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "userPurpose resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


