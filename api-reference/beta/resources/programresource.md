---
title: programResource 资源类型
description: 表示对作为访问评审目标的对象的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5ad3720587523e6937b4c3713a1c5a8c06d1e6e5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601494"
---
# <a name="programresource-resource-type"></a><span data-ttu-id="c679b-103">programResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="c679b-103">programResource resource type</span></span>

<span data-ttu-id="c679b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c679b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c679b-105">包含在[programControl](programcontrol.md)对象中的**programResource**对象表示对作为访问审核目标的对象的引用。</span><span class="sxs-lookup"><span data-stu-id="c679b-105">The **programResource** object, contained within a [programControl](programcontrol.md) object, represents a reference to an object that is the target of the access review.</span></span>

<span data-ttu-id="c679b-106">此类型继承自 [标识](identity.md)。</span><span class="sxs-lookup"><span data-stu-id="c679b-106">This type inherits from [identity](identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c679b-107">属性</span><span class="sxs-lookup"><span data-stu-id="c679b-107">Properties</span></span>

| <span data-ttu-id="c679b-108">属性</span><span class="sxs-lookup"><span data-stu-id="c679b-108">Property</span></span> | <span data-ttu-id="c679b-109">类型</span><span class="sxs-lookup"><span data-stu-id="c679b-109">Type</span></span> | <span data-ttu-id="c679b-110">说明</span><span class="sxs-lookup"><span data-stu-id="c679b-110">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="c679b-111">type</span><span class="sxs-lookup"><span data-stu-id="c679b-111">type</span></span> | <span data-ttu-id="c679b-112">String</span><span class="sxs-lookup"><span data-stu-id="c679b-112">String</span></span> | <span data-ttu-id="c679b-113">资源的类型，指示它是一个组还是一个应用程序。</span><span class="sxs-lookup"><span data-stu-id="c679b-113">Type of the resource, indicating whether it is a group or an app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c679b-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c679b-114">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.programResource"
}-->
```json
{
  "type": "string"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "programResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
