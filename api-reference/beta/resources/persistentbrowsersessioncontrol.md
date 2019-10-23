---
title: persistentBrowserSessionControl 资源类型
description: 用于定义是否保持 cookie 的会话控制。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7e2e9304aa8c7e7c8d59602a5710596b14e74636
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638608"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a><span data-ttu-id="676bf-103">persistentBrowserSessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="676bf-103">persistentBrowserSessionControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="676bf-104">用于定义是否保持 cookie 的会话控制。</span><span class="sxs-lookup"><span data-stu-id="676bf-104">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="676bf-105">Inehrits 来自[条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="676bf-105">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="676bf-106">属性</span><span class="sxs-lookup"><span data-stu-id="676bf-106">Properties</span></span>

| <span data-ttu-id="676bf-107">属性</span><span class="sxs-lookup"><span data-stu-id="676bf-107">Property</span></span>     | <span data-ttu-id="676bf-108">类型</span><span class="sxs-lookup"><span data-stu-id="676bf-108">Type</span></span>        | <span data-ttu-id="676bf-109">说明</span><span class="sxs-lookup"><span data-stu-id="676bf-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="676bf-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="676bf-110">isEnabled</span></span>     |<span data-ttu-id="676bf-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="676bf-111">Boolean</span></span>      | <span data-ttu-id="676bf-112">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="676bf-112">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="676bf-113">mode</span><span class="sxs-lookup"><span data-stu-id="676bf-113">mode</span></span>|<span data-ttu-id="676bf-114">String</span><span class="sxs-lookup"><span data-stu-id="676bf-114">String</span></span>| <span data-ttu-id="676bf-115">可取值为：`always`、`never`。</span><span class="sxs-lookup"><span data-stu-id="676bf-115">Possible values are: `always`, `never`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="676bf-116">关系</span><span class="sxs-lookup"><span data-stu-id="676bf-116">Relationships</span></span>

<span data-ttu-id="676bf-117">无。</span><span class="sxs-lookup"><span data-stu-id="676bf-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="676bf-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="676bf-118">JSON representation</span></span>

<span data-ttu-id="676bf-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="676bf-119">The following is a JSON representation of the resource.</span></span>

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