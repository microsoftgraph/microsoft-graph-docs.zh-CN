---
title: persistentBrowserSessionControl 资源类型
description: 用于定义是否保持 cookie 的会话控制。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a747f2d51d43b30da7dd7566a767cfb5f8c3fcd5
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384638"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a><span data-ttu-id="99de5-103">persistentBrowserSessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="99de5-103">persistentBrowserSessionControl resource type</span></span>

<span data-ttu-id="99de5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99de5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="99de5-105">用于定义是否保持 cookie 的会话控制。</span><span class="sxs-lookup"><span data-stu-id="99de5-105">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="99de5-106">继承自[条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="99de5-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="99de5-107">属性</span><span class="sxs-lookup"><span data-stu-id="99de5-107">Properties</span></span>

| <span data-ttu-id="99de5-108">属性</span><span class="sxs-lookup"><span data-stu-id="99de5-108">Property</span></span>     | <span data-ttu-id="99de5-109">类型</span><span class="sxs-lookup"><span data-stu-id="99de5-109">Type</span></span>        | <span data-ttu-id="99de5-110">说明</span><span class="sxs-lookup"><span data-stu-id="99de5-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="99de5-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="99de5-111">isEnabled</span></span>     |<span data-ttu-id="99de5-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="99de5-112">Boolean</span></span>      | <span data-ttu-id="99de5-113">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="99de5-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="99de5-114">mode</span><span class="sxs-lookup"><span data-stu-id="99de5-114">mode</span></span>|<span data-ttu-id="99de5-115">String</span><span class="sxs-lookup"><span data-stu-id="99de5-115">String</span></span>| <span data-ttu-id="99de5-116">可取值为：`always`、`never`。</span><span class="sxs-lookup"><span data-stu-id="99de5-116">Possible values are: `always`, `never`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99de5-117">关系</span><span class="sxs-lookup"><span data-stu-id="99de5-117">Relationships</span></span>

<span data-ttu-id="99de5-118">无。</span><span class="sxs-lookup"><span data-stu-id="99de5-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="99de5-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99de5-119">JSON representation</span></span>

<span data-ttu-id="99de5-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99de5-120">The following is a JSON representation of the resource.</span></span>

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
