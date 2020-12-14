---
title: aadUserConversationMemberResult 资源类型
description: 用于对 aadUserConversationMember 上的批量操作响应建模的资源。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca8251107c325bdbe2c5ff9e6df95a2d08277dde
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49663903"
---
# <a name="aaduserconversationmemberresult-resource-type"></a><span data-ttu-id="389be-103">aadUserConversationMemberResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="389be-103">aadUserConversationMemberResult resource type</span></span>

<span data-ttu-id="389be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="389be-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="389be-105">表示由请求中的 [aadUserConversationMember ](aadUserConversationMember.md) () 中指定的每个成员的个人响应。</span><span class="sxs-lookup"><span data-stu-id="389be-105">Represents the individual response for each member specified in a bulk operation comprising of [aadUserConversationMember(s)](aadUserConversationMember.md) in the request.</span></span>
<span data-ttu-id="389be-106">此资源是 [actionResultPart 资源的派生](actionresultpart.md) 项。</span><span class="sxs-lookup"><span data-stu-id="389be-106">This resource is the derivative of the [actionResultPart](actionresultpart.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="389be-107">属性</span><span class="sxs-lookup"><span data-stu-id="389be-107">Properties</span></span>

| <span data-ttu-id="389be-108">属性</span><span class="sxs-lookup"><span data-stu-id="389be-108">Property</span></span> | <span data-ttu-id="389be-109">类型</span><span class="sxs-lookup"><span data-stu-id="389be-109">Type</span></span>   | <span data-ttu-id="389be-110">描述</span><span class="sxs-lookup"><span data-stu-id="389be-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="389be-111">userId</span><span class="sxs-lookup"><span data-stu-id="389be-111">userId</span></span>|`String`|<span data-ttu-id="389be-112">作为批量操作一部分添加的 Azure AD 用户的用户对象 ID。</span><span class="sxs-lookup"><span data-stu-id="389be-112">The user object ID of the Azure AD user that was being added as part of the bulk operation.</span></span>|
|<span data-ttu-id="389be-113">error</span><span class="sxs-lookup"><span data-stu-id="389be-113">error</span></span>|[<span data-ttu-id="389be-114">publicError</span><span class="sxs-lookup"><span data-stu-id="389be-114">publicError</span></span>](publicerror.md) |<span data-ttu-id="389be-115">在批量操作过程中发生的错误（如果有）。</span><span class="sxs-lookup"><span data-stu-id="389be-115">The error that occurred, if any, during the course of the bulk operation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="389be-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="389be-116">JSON representation</span></span>

<span data-ttu-id="389be-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="389be-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.aadUserConversationMemberResult"
}-->

```json
{
    "userId": "string",
    "error": "microsoft.graph.publicError"
}
```

## <a name="see-also"></a><span data-ttu-id="389be-118">另请参阅</span><span class="sxs-lookup"><span data-stu-id="389be-118">See also</span></span>

- [<span data-ttu-id="389be-119">将成员批量添加到团队</span><span class="sxs-lookup"><span data-stu-id="389be-119">Add members in bulk to team</span></span>](../api/conversationmembers-add.md)

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "actionResultPart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


