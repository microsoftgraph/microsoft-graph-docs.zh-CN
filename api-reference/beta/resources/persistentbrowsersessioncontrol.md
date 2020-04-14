---
title: persistentBrowserSessionControl 资源类型
description: 用于定义是否保持 cookie 的会话控制。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 151259c98330c1319e71c8d9b9d44b1e9183f7b3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469057"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a><span data-ttu-id="09a53-103">persistentBrowserSessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="09a53-103">persistentBrowserSessionControl resource type</span></span>

<span data-ttu-id="09a53-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09a53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09a53-105">用于定义是否保持 cookie 的会话控制。</span><span class="sxs-lookup"><span data-stu-id="09a53-105">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="09a53-106">继承自[条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="09a53-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="09a53-107">属性</span><span class="sxs-lookup"><span data-stu-id="09a53-107">Properties</span></span>

| <span data-ttu-id="09a53-108">属性</span><span class="sxs-lookup"><span data-stu-id="09a53-108">Property</span></span>     | <span data-ttu-id="09a53-109">类型</span><span class="sxs-lookup"><span data-stu-id="09a53-109">Type</span></span>        | <span data-ttu-id="09a53-110">说明</span><span class="sxs-lookup"><span data-stu-id="09a53-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="09a53-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="09a53-111">isEnabled</span></span>     |<span data-ttu-id="09a53-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a53-112">Boolean</span></span>      | <span data-ttu-id="09a53-113">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="09a53-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="09a53-114">mode</span><span class="sxs-lookup"><span data-stu-id="09a53-114">mode</span></span>|<span data-ttu-id="09a53-115">String</span><span class="sxs-lookup"><span data-stu-id="09a53-115">String</span></span>| <span data-ttu-id="09a53-116">可取值为：`always`、`never`。</span><span class="sxs-lookup"><span data-stu-id="09a53-116">Possible values are: `always`, `never`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09a53-117">关系</span><span class="sxs-lookup"><span data-stu-id="09a53-117">Relationships</span></span>

<span data-ttu-id="09a53-118">无。</span><span class="sxs-lookup"><span data-stu-id="09a53-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="09a53-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09a53-119">JSON representation</span></span>

<span data-ttu-id="09a53-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09a53-120">The following is a JSON representation of the resource.</span></span>

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