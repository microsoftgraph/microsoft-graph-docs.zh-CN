---
title: aadUserConversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: fd326482869d9f72778edc9d4c55996f7aa59045
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236459"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="54f9b-103">aadUserConversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="54f9b-103">aadUserConversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54f9b-104">表示[聊天](chat.md)中的 Azure Active Directory 用户。</span><span class="sxs-lookup"><span data-stu-id="54f9b-104">Represents an Azure Active Directory user in a [chat](chat.md).</span></span> <span data-ttu-id="54f9b-105">此类型继承自 [conversationMember](conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="54f9b-105">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="54f9b-106">方法</span><span class="sxs-lookup"><span data-stu-id="54f9b-106">Methods</span></span>

| <span data-ttu-id="54f9b-107">方法</span><span class="sxs-lookup"><span data-stu-id="54f9b-107">Method</span></span>       | <span data-ttu-id="54f9b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="54f9b-108">Return Type</span></span>  |<span data-ttu-id="54f9b-109">说明</span><span class="sxs-lookup"><span data-stu-id="54f9b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="54f9b-110">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="54f9b-110">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="54f9b-111">[conversationmember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="54f9b-111">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="54f9b-112">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="54f9b-112">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="54f9b-113">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="54f9b-113">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="54f9b-114">conversationmember</span><span class="sxs-lookup"><span data-stu-id="54f9b-114">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="54f9b-115">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="54f9b-115">Get a single user in the chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="54f9b-116">属性</span><span class="sxs-lookup"><span data-stu-id="54f9b-116">Properties</span></span>
| <span data-ttu-id="54f9b-117">属性</span><span class="sxs-lookup"><span data-stu-id="54f9b-117">Property</span></span>     | <span data-ttu-id="54f9b-118">类型</span><span class="sxs-lookup"><span data-stu-id="54f9b-118">Type</span></span>   |<span data-ttu-id="54f9b-119">说明</span><span class="sxs-lookup"><span data-stu-id="54f9b-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54f9b-120">id</span><span class="sxs-lookup"><span data-stu-id="54f9b-120">id</span></span>|<span data-ttu-id="54f9b-121">String</span><span class="sxs-lookup"><span data-stu-id="54f9b-121">String</span></span>| <span data-ttu-id="54f9b-122">只读。</span><span class="sxs-lookup"><span data-stu-id="54f9b-122">Read-only.</span></span> <span data-ttu-id="54f9b-123">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="54f9b-123">Unique ID of the message.</span></span>|
|<span data-ttu-id="54f9b-124">displayName</span><span class="sxs-lookup"><span data-stu-id="54f9b-124">displayName</span></span>| <span data-ttu-id="54f9b-125">string</span><span class="sxs-lookup"><span data-stu-id="54f9b-125">string</span></span> | <span data-ttu-id="54f9b-126">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="54f9b-126">The display name of the user.</span></span> |
|<span data-ttu-id="54f9b-127">角色</span><span class="sxs-lookup"><span data-stu-id="54f9b-127">roles</span></span>| <span data-ttu-id="54f9b-128">string 集合</span><span class="sxs-lookup"><span data-stu-id="54f9b-128">string collection</span></span> | <span data-ttu-id="54f9b-129">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="54f9b-129">The roles for that user.</span></span> |
|<span data-ttu-id="54f9b-130">userId</span><span class="sxs-lookup"><span data-stu-id="54f9b-130">userId</span></span>| <span data-ttu-id="54f9b-131">string</span><span class="sxs-lookup"><span data-stu-id="54f9b-131">string</span></span> | <span data-ttu-id="54f9b-132">用户的 GUID。</span><span class="sxs-lookup"><span data-stu-id="54f9b-132">The guid of the user.</span></span> |
|<span data-ttu-id="54f9b-133">email</span><span class="sxs-lookup"><span data-stu-id="54f9b-133">email</span></span>| <span data-ttu-id="54f9b-134">string</span><span class="sxs-lookup"><span data-stu-id="54f9b-134">string</span></span>  | <span data-ttu-id="54f9b-135">用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="54f9b-135">The e-mail address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="54f9b-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54f9b-136">JSON representation</span></span>

<span data-ttu-id="54f9b-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54f9b-137">The following is a JSON representation of the resource.</span></span>

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
