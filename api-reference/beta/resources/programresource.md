---
title: programResource 资源类型
description: 表示对作为访问评审目标的对象的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0ef610650887b1d34569465bd5babb7ec91c194d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761826"
---
# <a name="programresource-resource-type"></a><span data-ttu-id="30a3d-103">programResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="30a3d-103">programResource resource type</span></span>

<span data-ttu-id="30a3d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30a3d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30a3d-105">**programResource** 对象包含在 [programControl](programcontrol.md)对象中，表示对作为访问评审目标的对象的引用。</span><span class="sxs-lookup"><span data-stu-id="30a3d-105">The **programResource** object, contained within a [programControl](programcontrol.md) object, represents a reference to an object that is the target of the access review.</span></span>

<span data-ttu-id="30a3d-106">此类型继承自 [标识](identity.md)。</span><span class="sxs-lookup"><span data-stu-id="30a3d-106">This type inherits from [identity](identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="30a3d-107">属性</span><span class="sxs-lookup"><span data-stu-id="30a3d-107">Properties</span></span>

| <span data-ttu-id="30a3d-108">属性</span><span class="sxs-lookup"><span data-stu-id="30a3d-108">Property</span></span> | <span data-ttu-id="30a3d-109">类型</span><span class="sxs-lookup"><span data-stu-id="30a3d-109">Type</span></span> | <span data-ttu-id="30a3d-110">说明</span><span class="sxs-lookup"><span data-stu-id="30a3d-110">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="30a3d-111">type</span><span class="sxs-lookup"><span data-stu-id="30a3d-111">type</span></span> | <span data-ttu-id="30a3d-112">String</span><span class="sxs-lookup"><span data-stu-id="30a3d-112">String</span></span> | <span data-ttu-id="30a3d-113">资源的类型，指示它是组还是应用。</span><span class="sxs-lookup"><span data-stu-id="30a3d-113">Type of the resource, indicating whether it is a group or an app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="30a3d-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30a3d-114">JSON representation</span></span>

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
