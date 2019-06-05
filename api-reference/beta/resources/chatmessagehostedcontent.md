---
title: chatMessageHostedContent 资源类型
description: 聊天消息中承载的内容
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2787138819160a25d72fb9ed273950eee326399c
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2019
ms.locfileid: "34720891"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="51680-103">chatMessageHostedContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="51680-103">chatMessageHostedContent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51680-104">表示在聊天消息中托管的内容, 如图像或代码段。</span><span class="sxs-lookup"><span data-stu-id="51680-104">Represents content hosted in a chat message, such as images or code snippets.</span></span>

## <a name="methods"></a><span data-ttu-id="51680-105">方法</span><span class="sxs-lookup"><span data-stu-id="51680-105">Methods</span></span>

| <span data-ttu-id="51680-106">方法</span><span class="sxs-lookup"><span data-stu-id="51680-106">Method</span></span>       | <span data-ttu-id="51680-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="51680-107">Return Type</span></span> | <span data-ttu-id="51680-108">说明</span><span class="sxs-lookup"><span data-stu-id="51680-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="51680-109">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="51680-109">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="51680-110">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="51680-110">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="51680-111">读取**chatMessageHostedContent**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="51680-111">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="51680-112">属性</span><span class="sxs-lookup"><span data-stu-id="51680-112">Properties</span></span>

| <span data-ttu-id="51680-113">属性</span><span class="sxs-lookup"><span data-stu-id="51680-113">Property</span></span>     | <span data-ttu-id="51680-114">类型</span><span class="sxs-lookup"><span data-stu-id="51680-114">Type</span></span>        | <span data-ttu-id="51680-115">说明</span><span class="sxs-lookup"><span data-stu-id="51680-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="51680-116">id</span><span class="sxs-lookup"><span data-stu-id="51680-116">id</span></span>|<span data-ttu-id="51680-117">String</span><span class="sxs-lookup"><span data-stu-id="51680-117">String</span></span>| <span data-ttu-id="51680-118">只读。</span><span class="sxs-lookup"><span data-stu-id="51680-118">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51680-119">关系</span><span class="sxs-lookup"><span data-stu-id="51680-119">Relationships</span></span>

<span data-ttu-id="51680-120">无。</span><span class="sxs-lookup"><span data-stu-id="51680-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="51680-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51680-121">JSON representation</span></span>

<span data-ttu-id="51680-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51680-122">The following is a JSON representation of the resource.</span></span>

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
