---
title: persistentBrowserSessionControl 资源类型
description: 用于定义是否保留 Cookie 的会话控件。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a4870720f02c0b88299ebfa7337ce9725fbcb220
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130875"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a><span data-ttu-id="425fe-103">persistentBrowserSessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="425fe-103">persistentBrowserSessionControl resource type</span></span>

<span data-ttu-id="425fe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="425fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="425fe-105">用于定义是否保留 Cookie 的会话控件。</span><span class="sxs-lookup"><span data-stu-id="425fe-105">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="425fe-106">继承自 [条件访问会话控件](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="425fe-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="425fe-107">属性</span><span class="sxs-lookup"><span data-stu-id="425fe-107">Properties</span></span>

| <span data-ttu-id="425fe-108">属性</span><span class="sxs-lookup"><span data-stu-id="425fe-108">Property</span></span>     | <span data-ttu-id="425fe-109">类型</span><span class="sxs-lookup"><span data-stu-id="425fe-109">Type</span></span>        | <span data-ttu-id="425fe-110">说明</span><span class="sxs-lookup"><span data-stu-id="425fe-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="425fe-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="425fe-111">isEnabled</span></span>     |<span data-ttu-id="425fe-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="425fe-112">Boolean</span></span>      | <span data-ttu-id="425fe-113">指定是否启用会话控件。</span><span class="sxs-lookup"><span data-stu-id="425fe-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="425fe-114">mode</span><span class="sxs-lookup"><span data-stu-id="425fe-114">mode</span></span>|<span data-ttu-id="425fe-115">String</span><span class="sxs-lookup"><span data-stu-id="425fe-115">String</span></span>| <span data-ttu-id="425fe-116">可取值为：`always`、`never`。</span><span class="sxs-lookup"><span data-stu-id="425fe-116">Possible values are: `always`, `never`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="425fe-117">关系</span><span class="sxs-lookup"><span data-stu-id="425fe-117">Relationships</span></span>

<span data-ttu-id="425fe-118">无。</span><span class="sxs-lookup"><span data-stu-id="425fe-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="425fe-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="425fe-119">JSON representation</span></span>

<span data-ttu-id="425fe-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="425fe-120">The following is a JSON representation of the resource.</span></span>

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

