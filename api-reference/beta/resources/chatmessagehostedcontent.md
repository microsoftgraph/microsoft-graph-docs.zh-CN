---
title: chatMessageHostedContent 资源类型
description: 聊天消息中承载的内容
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 39939d9d61d992e5fd77fd21360ab05e8f83dbd4
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333358"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="6f62a-103">chatMessageHostedContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f62a-103">chatMessageHostedContent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f62a-104">表示在聊天消息中托管的内容，如图像或代码段。</span><span class="sxs-lookup"><span data-stu-id="6f62a-104">Represents content hosted in a chat message, such as images or code snippets.</span></span>

## <a name="methods"></a><span data-ttu-id="6f62a-105">方法</span><span class="sxs-lookup"><span data-stu-id="6f62a-105">Methods</span></span>

| <span data-ttu-id="6f62a-106">方法</span><span class="sxs-lookup"><span data-stu-id="6f62a-106">Method</span></span>       | <span data-ttu-id="6f62a-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="6f62a-107">Return Type</span></span> | <span data-ttu-id="6f62a-108">说明</span><span class="sxs-lookup"><span data-stu-id="6f62a-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6f62a-109">列出 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6f62a-109">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="6f62a-110">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6f62a-110">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="6f62a-111">检索邮件的**chatMessageHostedContent**列表。</span><span class="sxs-lookup"><span data-stu-id="6f62a-111">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="6f62a-112">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6f62a-112">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="6f62a-113">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="6f62a-113">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="6f62a-114">读取**chatMessageHostedContent**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6f62a-114">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6f62a-115">属性</span><span class="sxs-lookup"><span data-stu-id="6f62a-115">Properties</span></span>

| <span data-ttu-id="6f62a-116">属性</span><span class="sxs-lookup"><span data-stu-id="6f62a-116">Property</span></span>     | <span data-ttu-id="6f62a-117">类型</span><span class="sxs-lookup"><span data-stu-id="6f62a-117">Type</span></span>        | <span data-ttu-id="6f62a-118">说明</span><span class="sxs-lookup"><span data-stu-id="6f62a-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6f62a-119">id</span><span class="sxs-lookup"><span data-stu-id="6f62a-119">id</span></span>|<span data-ttu-id="6f62a-120">String</span><span class="sxs-lookup"><span data-stu-id="6f62a-120">String</span></span>| <span data-ttu-id="6f62a-121">只读。</span><span class="sxs-lookup"><span data-stu-id="6f62a-121">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f62a-122">关系</span><span class="sxs-lookup"><span data-stu-id="6f62a-122">Relationships</span></span>

<span data-ttu-id="6f62a-123">无。</span><span class="sxs-lookup"><span data-stu-id="6f62a-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f62a-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f62a-124">JSON representation</span></span>

<span data-ttu-id="6f62a-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f62a-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageHostedContent",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageHostedContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
