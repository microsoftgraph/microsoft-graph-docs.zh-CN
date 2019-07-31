---
title: aadUserConversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c4e937d88a1e504c6774b2dcb657dee443d54843
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013631"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="b0d06-103">aadUserConversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0d06-103">aadUserConversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0d06-104">表示[聊天](chat.md)中的 Azure Active Directory 用户。</span><span class="sxs-lookup"><span data-stu-id="b0d06-104">Represents an Azure Active Directory user in a [chat](chat.md).</span></span> <span data-ttu-id="b0d06-105">此类型继承自 [conversationMember](conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="b0d06-105">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b0d06-106">方法</span><span class="sxs-lookup"><span data-stu-id="b0d06-106">Methods</span></span>

| <span data-ttu-id="b0d06-107">方法</span><span class="sxs-lookup"><span data-stu-id="b0d06-107">Method</span></span>       | <span data-ttu-id="b0d06-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b0d06-108">Return Type</span></span>  |<span data-ttu-id="b0d06-109">说明</span><span class="sxs-lookup"><span data-stu-id="b0d06-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b0d06-110">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="b0d06-110">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="b0d06-111">[conversationmember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b0d06-111">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="b0d06-112">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="b0d06-112">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="b0d06-113">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="b0d06-113">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="b0d06-114">conversationmember</span><span class="sxs-lookup"><span data-stu-id="b0d06-114">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="b0d06-115">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="b0d06-115">Get a single user in the chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0d06-116">属性</span><span class="sxs-lookup"><span data-stu-id="b0d06-116">Properties</span></span>
| <span data-ttu-id="b0d06-117">属性</span><span class="sxs-lookup"><span data-stu-id="b0d06-117">Property</span></span>     | <span data-ttu-id="b0d06-118">类型</span><span class="sxs-lookup"><span data-stu-id="b0d06-118">Type</span></span>   |<span data-ttu-id="b0d06-119">说明</span><span class="sxs-lookup"><span data-stu-id="b0d06-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0d06-120">id</span><span class="sxs-lookup"><span data-stu-id="b0d06-120">id</span></span>|<span data-ttu-id="b0d06-121">String</span><span class="sxs-lookup"><span data-stu-id="b0d06-121">String</span></span>| <span data-ttu-id="b0d06-122">只读。</span><span class="sxs-lookup"><span data-stu-id="b0d06-122">Read-only.</span></span> <span data-ttu-id="b0d06-123">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="b0d06-123">Unique ID of the message.</span></span>|
|<span data-ttu-id="b0d06-124">displayName</span><span class="sxs-lookup"><span data-stu-id="b0d06-124">displayName</span></span>| <span data-ttu-id="b0d06-125">string</span><span class="sxs-lookup"><span data-stu-id="b0d06-125">string</span></span> | <span data-ttu-id="b0d06-126">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b0d06-126">The display name of the user.</span></span> |
|<span data-ttu-id="b0d06-127">角色</span><span class="sxs-lookup"><span data-stu-id="b0d06-127">roles</span></span>| <span data-ttu-id="b0d06-128">string 集合</span><span class="sxs-lookup"><span data-stu-id="b0d06-128">string collection</span></span> | <span data-ttu-id="b0d06-129">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="b0d06-129">The roles for that user.</span></span> |
|<span data-ttu-id="b0d06-130">userId</span><span class="sxs-lookup"><span data-stu-id="b0d06-130">userId</span></span>| <span data-ttu-id="b0d06-131">string</span><span class="sxs-lookup"><span data-stu-id="b0d06-131">string</span></span> | <span data-ttu-id="b0d06-132">用户的 GUID。</span><span class="sxs-lookup"><span data-stu-id="b0d06-132">The guid of the user.</span></span> |
|<span data-ttu-id="b0d06-133">email</span><span class="sxs-lookup"><span data-stu-id="b0d06-133">email</span></span>| <span data-ttu-id="b0d06-134">string</span><span class="sxs-lookup"><span data-stu-id="b0d06-134">string</span></span>  | <span data-ttu-id="b0d06-135">用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b0d06-135">The e-mail address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b0d06-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0d06-136">JSON representation</span></span>

<span data-ttu-id="b0d06-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0d06-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.aadUserConversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "aadUserConversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
