---
title: oneNoteIdentitySet 资源类型
description: '**支持即将推出**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: c0d2f0b4ed65ac83a59036c362136b7af772d21c
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290579"
---
# <a name="onenoteidentityset-resource-type"></a><span data-ttu-id="fb262-103">oneNoteIdentitySet 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb262-103">oneNoteIdentitySet resource type</span></span>

<span data-ttu-id="fb262-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb262-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb262-105">**支持即将推出**</span><span class="sxs-lookup"><span data-stu-id="fb262-105">**Support coming soon**</span></span>

<span data-ttu-id="fb262-106">OneNoteIdentitySet 类型是[OneNoteIdentity](onenoteidentity.md)对象的键控集合。</span><span class="sxs-lookup"><span data-stu-id="fb262-106">The OneNoteIdentitySet type is a keyed collection of [OneNoteIdentity](onenoteidentity.md) objects.</span></span>
<span data-ttu-id="fb262-107">它用于表示一组与_笔记本_、_节_或_页面_的各种事件相关联的标识，如 "_创建者_" 或 "_上次修改者_"。</span><span class="sxs-lookup"><span data-stu-id="fb262-107">It is used to represent a set of identities associated with various events for a _Notebook_, _Section_ or _Page_, such as _created by_ or _last modified by_.</span></span> 
 
<span data-ttu-id="fb262-108">当前它包含单个密钥，即_**user**_。</span><span class="sxs-lookup"><span data-stu-id="fb262-108">Currently it contains a single key, _**user**_.</span></span>  <span data-ttu-id="fb262-109">将来，可能会添加用于更改项目的设备或应用程序等键。</span><span class="sxs-lookup"><span data-stu-id="fb262-109">In future, keys such as the device or application to change the item may be added.</span></span>

<span data-ttu-id="fb262-110">将来，此类型将与[了解 identityset](identityset.md)合并。</span><span class="sxs-lookup"><span data-stu-id="fb262-110">In future, this type will be merged with [IdentitySet](identityset.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb262-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb262-111">JSON representation</span></span>

<span data-ttu-id="fb262-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb262-112">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="fb262-113">属性</span><span class="sxs-lookup"><span data-stu-id="fb262-113">Properties</span></span>
| <span data-ttu-id="fb262-114">属性</span><span class="sxs-lookup"><span data-stu-id="fb262-114">Property</span></span>     | <span data-ttu-id="fb262-115">类型</span><span class="sxs-lookup"><span data-stu-id="fb262-115">Type</span></span>   |<span data-ttu-id="fb262-116">说明</span><span class="sxs-lookup"><span data-stu-id="fb262-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb262-117">user</span><span class="sxs-lookup"><span data-stu-id="fb262-117">user</span></span>|[<span data-ttu-id="fb262-118">onenoteIdentity</span><span class="sxs-lookup"><span data-stu-id="fb262-118">onenoteIdentity</span></span>](onenoteidentity.md)|<span data-ttu-id="fb262-119">一个代表用户的 OneNoteIdentity 资源。</span><span class="sxs-lookup"><span data-stu-id="fb262-119">A OneNoteIdentity resource that represents a user.</span></span>|

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
