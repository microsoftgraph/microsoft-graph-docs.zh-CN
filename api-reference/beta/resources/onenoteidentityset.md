---
title: oneNoteIdentitySet 资源类型
description: '**支持即将推出**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: e149d5548ce3585bbcda1f0a199fa97d7543af77
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568878"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="ba233-103">oneNoteIdentitySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba233-103">oneNoteIdentitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba233-104">**支持即将推出**</span><span class="sxs-lookup"><span data-stu-id="ba233-104">**Support coming soon**</span></span>

<span data-ttu-id="ba233-105">OneNoteIdentitySet 类型是[OneNoteIdentity](onenoteidentity.md)对象的键控集合。</span><span class="sxs-lookup"><span data-stu-id="ba233-105">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="ba233-106">它用于表示一组与_笔记本_、_节_或_页面_的各种事件相关联的标识, 如 "_创建者_" 或 "_上次修改者_"。</span><span class="sxs-lookup"><span data-stu-id="ba233-106">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="ba233-107">当前它包含单个密钥, 即_**user**_。</span><span class="sxs-lookup"><span data-stu-id="ba233-107">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="ba233-108">将来, 可能会添加用于更改项目的设备或应用程序等键。</span><span class="sxs-lookup"><span data-stu-id="ba233-108">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="ba233-109">将来, 此类型将与[了解 identityset](identityset.md)合并。</span><span class="sxs-lookup"><span data-stu-id="ba233-109">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba233-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba233-110">JSON representation</span></span>

<span data-ttu-id="ba233-111">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba233-111">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentityset"
}-->

```json
{
  "user": {"@odata.type": "microsoft.graph.onenoteIdentity"}
}

```
## <a name="properties"></a><span data-ttu-id="ba233-112">属性</span><span class="sxs-lookup"><span data-stu-id="ba233-112">Properties</span></span>
| <span data-ttu-id="ba233-113">属性</span><span class="sxs-lookup"><span data-stu-id="ba233-113">Property</span></span>     | <span data-ttu-id="ba233-114">类型</span><span class="sxs-lookup"><span data-stu-id="ba233-114">Type</span></span>   |<span data-ttu-id="ba233-115">说明</span><span class="sxs-lookup"><span data-stu-id="ba233-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba233-116">user</span><span class="sxs-lookup"><span data-stu-id="ba233-116">user</span></span>|[<span data-ttu-id="ba233-117">oneNoteIdentity</span><span class="sxs-lookup"><span data-stu-id="ba233-117">oneNoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="ba233-118">一个代表用户的 OneNoteIdentity 资源。</span><span class="sxs-lookup"><span data-stu-id="ba233-118">A OneNoteIdentity resource that represents a user.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentitySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
