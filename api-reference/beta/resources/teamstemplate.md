---
title: teamsTemplate 资源类型
description: 描述 teamsTemplate 实体。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4e960e85e6e8b3017d8f4e0ab89bb85cb4c12f58
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345743"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="6ee7a-103">teamsTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ee7a-103">teamsTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ee7a-104">团队模板是在 Microsoft 团队中创建[团队](../resources/team.md)的蓝图。</span><span class="sxs-lookup"><span data-stu-id="6ee7a-104">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="6ee7a-105">模板指定应在使用模板创建的新团队中设置的结构、设置和偶数内容。</span><span class="sxs-lookup"><span data-stu-id="6ee7a-105">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="6ee7a-106">Microsoft 提供了一套基本模板, 并且客户可以保存自己的自定义模板。</span><span class="sxs-lookup"><span data-stu-id="6ee7a-106">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="6ee7a-107">属性</span><span class="sxs-lookup"><span data-stu-id="6ee7a-107">Properties</span></span>

| <span data-ttu-id="6ee7a-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ee7a-108">Property</span></span>            | <span data-ttu-id="6ee7a-109">类型</span><span class="sxs-lookup"><span data-stu-id="6ee7a-109">Type</span></span>     | <span data-ttu-id="6ee7a-110">说明</span><span class="sxs-lookup"><span data-stu-id="6ee7a-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="6ee7a-111">id</span><span class="sxs-lookup"><span data-stu-id="6ee7a-111">id</span></span>                  | <span data-ttu-id="6ee7a-112">String</span><span class="sxs-lookup"><span data-stu-id="6ee7a-112">String</span></span>   | <span data-ttu-id="6ee7a-113">模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6ee7a-113">Unique identifier of the template.</span></span> <span data-ttu-id="6ee7a-114">不能为 null。</span><span class="sxs-lookup"><span data-stu-id="6ee7a-114">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6ee7a-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ee7a-115">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="6ee7a-116">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6ee7a-116">See also</span></span>

- [<span data-ttu-id="6ee7a-117">team</span><span class="sxs-lookup"><span data-stu-id="6ee7a-117">team</span></span>](team.md)

