---
title: chatMessageMention 资源类型
description: '代表 chatMessage 实体中的某个提及。 提及的可向用户、 团队、 自动程序或通道。 '
localization_priority: Normal
ms.openlocfilehash: 7b24d2af6f61f3da69480557e1c5b5f32c009c25
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876134"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="4d1f9-104">chatMessageMention 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d1f9-104">chatMessageMention resource type</span></span>

> <span data-ttu-id="4d1f9-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4d1f9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d1f9-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4d1f9-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d1f9-107">代表[chatMessage](chatmessage.md)实体中的某个提及。</span><span class="sxs-lookup"><span data-stu-id="4d1f9-107">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="4d1f9-108">提及的可向用户、 团队、 自动程序或通道。</span><span class="sxs-lookup"><span data-stu-id="4d1f9-108">The mention can be to a user, team, bot or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="4d1f9-109">属性</span><span class="sxs-lookup"><span data-stu-id="4d1f9-109">Properties</span></span>
| <span data-ttu-id="4d1f9-110">属性</span><span class="sxs-lookup"><span data-stu-id="4d1f9-110">Property</span></span>     | <span data-ttu-id="4d1f9-111">类型</span><span class="sxs-lookup"><span data-stu-id="4d1f9-111">Type</span></span>   |<span data-ttu-id="4d1f9-112">说明</span><span class="sxs-lookup"><span data-stu-id="4d1f9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d1f9-113">ID</span><span class="sxs-lookup"><span data-stu-id="4d1f9-113">id</span></span>|<span data-ttu-id="4d1f9-114">string</span><span class="sxs-lookup"><span data-stu-id="4d1f9-114">string</span></span>|<span data-ttu-id="4d1f9-115">正在提到的实体的 id</span><span class="sxs-lookup"><span data-stu-id="4d1f9-115">Id of the entity being mentioned</span></span>|
|<span data-ttu-id="4d1f9-116">mentionText</span><span class="sxs-lookup"><span data-stu-id="4d1f9-116">mentionText</span></span>|<span data-ttu-id="4d1f9-117">string</span><span class="sxs-lookup"><span data-stu-id="4d1f9-117">string</span></span>|<span data-ttu-id="4d1f9-118">用来表示 Ex 提及的字符串： 用户的显示名称、 工作组名称等</span><span class="sxs-lookup"><span data-stu-id="4d1f9-118">String used to represent the mention Ex: User display name, Team name etc</span></span>|
|<span data-ttu-id="4d1f9-119">提到</span><span class="sxs-lookup"><span data-stu-id="4d1f9-119">mentioned</span></span>|[<span data-ttu-id="4d1f9-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="4d1f9-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="4d1f9-121">已提及用户</span><span class="sxs-lookup"><span data-stu-id="4d1f9-121">The user that was mentioned</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d1f9-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d1f9-122">JSON representation</span></span>

<span data-ttu-id="4d1f9-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d1f9-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "string (identifier)",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
