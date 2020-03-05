---
title: persistentBrowserSessionControl 资源类型
description: 用于定义是否保持 cookie 的会话控制。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d46ffa5cc3f0eee423b4800ee13f19677bf7c41f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521944"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a><span data-ttu-id="0b731-103">persistentBrowserSessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b731-103">persistentBrowserSessionControl resource type</span></span>

<span data-ttu-id="0b731-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0b731-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b731-105">用于定义是否保持 cookie 的会话控制。</span><span class="sxs-lookup"><span data-stu-id="0b731-105">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="0b731-106">Inehrits 来自[条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="0b731-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0b731-107">属性</span><span class="sxs-lookup"><span data-stu-id="0b731-107">Properties</span></span>

| <span data-ttu-id="0b731-108">属性</span><span class="sxs-lookup"><span data-stu-id="0b731-108">Property</span></span>     | <span data-ttu-id="0b731-109">类型</span><span class="sxs-lookup"><span data-stu-id="0b731-109">Type</span></span>        | <span data-ttu-id="0b731-110">说明</span><span class="sxs-lookup"><span data-stu-id="0b731-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0b731-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0b731-111">isEnabled</span></span>     |<span data-ttu-id="0b731-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b731-112">Boolean</span></span>      | <span data-ttu-id="0b731-113">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="0b731-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="0b731-114">mode</span><span class="sxs-lookup"><span data-stu-id="0b731-114">mode</span></span>|<span data-ttu-id="0b731-115">String</span><span class="sxs-lookup"><span data-stu-id="0b731-115">String</span></span>| <span data-ttu-id="0b731-116">可取值为：`always`、`never`。</span><span class="sxs-lookup"><span data-stu-id="0b731-116">Possible values are: `always`, `never`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b731-117">关系</span><span class="sxs-lookup"><span data-stu-id="0b731-117">Relationships</span></span>

<span data-ttu-id="0b731-118">无。</span><span class="sxs-lookup"><span data-stu-id="0b731-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b731-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b731-119">JSON representation</span></span>

<span data-ttu-id="0b731-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b731-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.persistentBrowserSessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "mode": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "persistentBrowserSessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->