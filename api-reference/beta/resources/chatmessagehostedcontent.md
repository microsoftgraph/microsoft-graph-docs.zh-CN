---
title: chatMessageHostedContent 资源类型
description: 聊天消息中承载的内容
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a34e09b233a60858e23155f87808e40d080867f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507703"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="1852e-103">chatMessageHostedContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="1852e-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="1852e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1852e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1852e-105">表示在聊天消息中托管的内容，如图像或代码段。</span><span class="sxs-lookup"><span data-stu-id="1852e-105">Represents content hosted in a chat message, such as images or code snippets.</span></span>

## <a name="methods"></a><span data-ttu-id="1852e-106">方法</span><span class="sxs-lookup"><span data-stu-id="1852e-106">Methods</span></span>

| <span data-ttu-id="1852e-107">方法</span><span class="sxs-lookup"><span data-stu-id="1852e-107">Method</span></span>       | <span data-ttu-id="1852e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1852e-108">Return Type</span></span> | <span data-ttu-id="1852e-109">说明</span><span class="sxs-lookup"><span data-stu-id="1852e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1852e-110">列出 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="1852e-110">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="1852e-111">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="1852e-111">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="1852e-112">检索邮件的**chatMessageHostedContent**列表。</span><span class="sxs-lookup"><span data-stu-id="1852e-112">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="1852e-113">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="1852e-113">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="1852e-114">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="1852e-114">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="1852e-115">读取**chatMessageHostedContent**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1852e-115">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1852e-116">属性</span><span class="sxs-lookup"><span data-stu-id="1852e-116">Properties</span></span>

| <span data-ttu-id="1852e-117">属性</span><span class="sxs-lookup"><span data-stu-id="1852e-117">Property</span></span>     | <span data-ttu-id="1852e-118">类型</span><span class="sxs-lookup"><span data-stu-id="1852e-118">Type</span></span>        | <span data-ttu-id="1852e-119">说明</span><span class="sxs-lookup"><span data-stu-id="1852e-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1852e-120">id</span><span class="sxs-lookup"><span data-stu-id="1852e-120">id</span></span>|<span data-ttu-id="1852e-121">String</span><span class="sxs-lookup"><span data-stu-id="1852e-121">String</span></span>| <span data-ttu-id="1852e-122">只读。</span><span class="sxs-lookup"><span data-stu-id="1852e-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1852e-123">关系</span><span class="sxs-lookup"><span data-stu-id="1852e-123">Relationships</span></span>

<span data-ttu-id="1852e-124">无。</span><span class="sxs-lookup"><span data-stu-id="1852e-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1852e-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1852e-125">JSON representation</span></span>

<span data-ttu-id="1852e-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1852e-126">The following is a JSON representation of the resource.</span></span>

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
