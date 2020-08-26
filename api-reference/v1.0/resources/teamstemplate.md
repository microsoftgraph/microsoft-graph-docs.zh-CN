---
title: teamsTemplate 资源类型
description: 介绍 teamsTemplate 实体。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c32c8cfa770bd7633915e0e8f9b6d371458d4173
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873412"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="31621-103">teamsTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="31621-103">teamsTemplate resource type</span></span>

<span data-ttu-id="31621-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31621-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="31621-105">团队模板是在 Microsoft 团队中创建 [团队](../resources/team.md) 的蓝图。</span><span class="sxs-lookup"><span data-stu-id="31621-105">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="31621-106">模板指定应在使用模板创建的新团队中设置的结构、设置和偶数内容。</span><span class="sxs-lookup"><span data-stu-id="31621-106">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="31621-107">Microsoft 提供了一套基本模板，并且客户可以保存自己的自定义模板。</span><span class="sxs-lookup"><span data-stu-id="31621-107">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="31621-108">属性</span><span class="sxs-lookup"><span data-stu-id="31621-108">Properties</span></span>

| <span data-ttu-id="31621-109">属性</span><span class="sxs-lookup"><span data-stu-id="31621-109">Property</span></span>            | <span data-ttu-id="31621-110">类型</span><span class="sxs-lookup"><span data-stu-id="31621-110">Type</span></span>     | <span data-ttu-id="31621-111">说明</span><span class="sxs-lookup"><span data-stu-id="31621-111">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="31621-112">id</span><span class="sxs-lookup"><span data-stu-id="31621-112">id</span></span>                  | <span data-ttu-id="31621-113">String</span><span class="sxs-lookup"><span data-stu-id="31621-113">String</span></span>   | <span data-ttu-id="31621-114">模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="31621-114">Unique identifier of the template.</span></span> <span data-ttu-id="31621-115">不能为 null。</span><span class="sxs-lookup"><span data-stu-id="31621-115">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="31621-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31621-116">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="31621-117">另请参阅</span><span class="sxs-lookup"><span data-stu-id="31621-117">See also</span></span>

- [<span data-ttu-id="31621-118">team</span><span class="sxs-lookup"><span data-stu-id="31621-118">team</span></span>](team.md)

