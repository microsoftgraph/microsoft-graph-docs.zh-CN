---
title: teamsTemplate 资源类型
description: 描述 teamsTemplate 实体。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5fc40b9c2a5789c5bcd7ab5794e41c715223eff3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046384"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="3b6ed-103">teamsTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b6ed-103">teamsTemplate resource type</span></span>

<span data-ttu-id="3b6ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b6ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b6ed-105">团队模板是在 Microsoft 团队中创建 [团队](../resources/team.md) 的蓝图。</span><span class="sxs-lookup"><span data-stu-id="3b6ed-105">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="3b6ed-106">模板指定应在使用模板创建的新团队中设置的结构、设置和偶数内容。</span><span class="sxs-lookup"><span data-stu-id="3b6ed-106">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="3b6ed-107">Microsoft 提供了一套基本模板，并且客户可以保存自己的自定义模板。</span><span class="sxs-lookup"><span data-stu-id="3b6ed-107">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="3b6ed-108">属性</span><span class="sxs-lookup"><span data-stu-id="3b6ed-108">Properties</span></span>

| <span data-ttu-id="3b6ed-109">属性</span><span class="sxs-lookup"><span data-stu-id="3b6ed-109">Property</span></span>            | <span data-ttu-id="3b6ed-110">类型</span><span class="sxs-lookup"><span data-stu-id="3b6ed-110">Type</span></span>     | <span data-ttu-id="3b6ed-111">说明</span><span class="sxs-lookup"><span data-stu-id="3b6ed-111">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="3b6ed-112">id</span><span class="sxs-lookup"><span data-stu-id="3b6ed-112">id</span></span>                  | <span data-ttu-id="3b6ed-113">String</span><span class="sxs-lookup"><span data-stu-id="3b6ed-113">String</span></span>   | <span data-ttu-id="3b6ed-114">模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3b6ed-114">Unique identifier of the template.</span></span> <span data-ttu-id="3b6ed-115">不能为 null。</span><span class="sxs-lookup"><span data-stu-id="3b6ed-115">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3b6ed-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b6ed-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="3b6ed-117">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3b6ed-117">See also</span></span>

- [<span data-ttu-id="3b6ed-118">team</span><span class="sxs-lookup"><span data-stu-id="3b6ed-118">team</span></span>](team.md)



