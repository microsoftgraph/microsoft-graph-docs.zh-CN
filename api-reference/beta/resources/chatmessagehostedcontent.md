---
title: chatMessageHostedContent 资源类型
description: 聊天消息中承载的内容
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 421ed3b1c439a7ae550100a113c651ab3e0a34b9
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791067"
---
# <a name="chatmessagehostedcontent-resource-type"></a><span data-ttu-id="e97f8-103">chatMessageHostedContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="e97f8-103">chatMessageHostedContent resource type</span></span>

<span data-ttu-id="e97f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e97f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e97f8-105">表示在聊天消息中托管的团队内容，如图像或代码段。</span><span class="sxs-lookup"><span data-stu-id="e97f8-105">Represents Teams content hosted in a chat message, such as images or code snippets.</span></span>
<span data-ttu-id="e97f8-106">[文件附件](chatmessageattachment.md)不是托管内容，它们存储在 SharePoint 或 OneDrive 中。</span><span class="sxs-lookup"><span data-stu-id="e97f8-106">[File attachments](chatmessageattachment.md) are not hosted content, they are stored in SharePoint or OneDrive.</span></span>

## <a name="methods"></a><span data-ttu-id="e97f8-107">Methods</span><span class="sxs-lookup"><span data-stu-id="e97f8-107">Methods</span></span>

| <span data-ttu-id="e97f8-108">方法</span><span class="sxs-lookup"><span data-stu-id="e97f8-108">Method</span></span>       | <span data-ttu-id="e97f8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e97f8-109">Return Type</span></span> | <span data-ttu-id="e97f8-110">说明</span><span class="sxs-lookup"><span data-stu-id="e97f8-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e97f8-111">列出 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="e97f8-111">List chatMessageHostedContent</span></span>](../api/chatmessage-list-chatmessagehostedcontents.md) | [<span data-ttu-id="e97f8-112">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="e97f8-112">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="e97f8-113">检索邮件的**chatMessageHostedContent**列表。</span><span class="sxs-lookup"><span data-stu-id="e97f8-113">Retrieve the list of **chatMessageHostedContent** for a message.</span></span> |
| [<span data-ttu-id="e97f8-114">获取 chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="e97f8-114">Get chatMessageHostedContent</span></span>](../api/chatmessagehostedcontent-get.md) | [<span data-ttu-id="e97f8-115">chatMessageHostedContent</span><span class="sxs-lookup"><span data-stu-id="e97f8-115">chatMessageHostedContent</span></span>](chatmessagehostedcontent.md) | <span data-ttu-id="e97f8-116">读取**chatMessageHostedContent**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e97f8-116">Read the properties and relationships of a **chatMessageHostedContent** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e97f8-117">属性</span><span class="sxs-lookup"><span data-stu-id="e97f8-117">Properties</span></span>

| <span data-ttu-id="e97f8-118">属性</span><span class="sxs-lookup"><span data-stu-id="e97f8-118">Property</span></span>     | <span data-ttu-id="e97f8-119">类型</span><span class="sxs-lookup"><span data-stu-id="e97f8-119">Type</span></span>        | <span data-ttu-id="e97f8-120">说明</span><span class="sxs-lookup"><span data-stu-id="e97f8-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e97f8-121">id</span><span class="sxs-lookup"><span data-stu-id="e97f8-121">id</span></span>|<span data-ttu-id="e97f8-122">String</span><span class="sxs-lookup"><span data-stu-id="e97f8-122">String</span></span>| <span data-ttu-id="e97f8-123">只读。</span><span class="sxs-lookup"><span data-stu-id="e97f8-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e97f8-124">关系</span><span class="sxs-lookup"><span data-stu-id="e97f8-124">Relationships</span></span>

<span data-ttu-id="e97f8-125">无。</span><span class="sxs-lookup"><span data-stu-id="e97f8-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e97f8-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e97f8-126">JSON representation</span></span>

<span data-ttu-id="e97f8-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e97f8-127">The following is a JSON representation of the resource.</span></span>

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
