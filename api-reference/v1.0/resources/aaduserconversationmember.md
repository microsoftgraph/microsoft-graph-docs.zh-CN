---
title: aadUserConversationMember 资源类型
description: 表示聊天或频道中的 Azure Active Directory 用户。
localization_priority: Priority
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9714605cabbc25d3eeae7a68b2bc8f09d6131836
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873416"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="f1870-103">aadUserConversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1870-103">aadUserConversationMember resource type</span></span>

<span data-ttu-id="f1870-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1870-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1870-105">表示[团队](team.md)中的 Azure Active Directory 用户。</span><span class="sxs-lookup"><span data-stu-id="f1870-105">Represents an Azure Active Directory user in a [team](team.md).</span></span>
<span data-ttu-id="f1870-106">此类型继承自 [conversationMember](conversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="f1870-106">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f1870-107">属性</span><span class="sxs-lookup"><span data-stu-id="f1870-107">Properties</span></span>

| <span data-ttu-id="f1870-108">属性</span><span class="sxs-lookup"><span data-stu-id="f1870-108">Property</span></span>   | <span data-ttu-id="f1870-109">类型</span><span class="sxs-lookup"><span data-stu-id="f1870-109">Type</span></span> |<span data-ttu-id="f1870-110">说明</span><span class="sxs-lookup"><span data-stu-id="f1870-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1870-111">id</span><span class="sxs-lookup"><span data-stu-id="f1870-111">id</span></span>|<span data-ttu-id="f1870-112">String</span><span class="sxs-lookup"><span data-stu-id="f1870-112">String</span></span>| <span data-ttu-id="f1870-113">只读。</span><span class="sxs-lookup"><span data-stu-id="f1870-113">Read-only.</span></span> <span data-ttu-id="f1870-114">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="f1870-114">Unique ID of the user.</span></span>|
|<span data-ttu-id="f1870-115">displayName</span><span class="sxs-lookup"><span data-stu-id="f1870-115">displayName</span></span>| <span data-ttu-id="f1870-116">string</span><span class="sxs-lookup"><span data-stu-id="f1870-116">string</span></span> | <span data-ttu-id="f1870-117">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f1870-117">The display name of the user.</span></span> |
|<span data-ttu-id="f1870-118">角色</span><span class="sxs-lookup"><span data-stu-id="f1870-118">roles</span></span>| <span data-ttu-id="f1870-119">string 集合</span><span class="sxs-lookup"><span data-stu-id="f1870-119">string collection</span></span> | <span data-ttu-id="f1870-120">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="f1870-120">The roles for that user.</span></span> |
|<span data-ttu-id="f1870-121">userId</span><span class="sxs-lookup"><span data-stu-id="f1870-121">userId</span></span>| <span data-ttu-id="f1870-122">string</span><span class="sxs-lookup"><span data-stu-id="f1870-122">string</span></span> | <span data-ttu-id="f1870-123">用户的 GUID。</span><span class="sxs-lookup"><span data-stu-id="f1870-123">The guid of the user.</span></span> |
|<span data-ttu-id="f1870-124">email</span><span class="sxs-lookup"><span data-stu-id="f1870-124">email</span></span>| <span data-ttu-id="f1870-125">string</span><span class="sxs-lookup"><span data-stu-id="f1870-125">string</span></span>  | <span data-ttu-id="f1870-126">用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="f1870-126">The email address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f1870-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1870-127">JSON representation</span></span>

<span data-ttu-id="f1870-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1870-128">The following is a JSON representation of the resource.</span></span>

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
