---
title: teamsTemplate 资源类型
description: 描述 teamsTemplate 实体。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e75b3d8df318b116d5d908a40d4f756d9ee70864
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583163"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="1c8da-103">teamsTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c8da-103">teamsTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c8da-104">团队模板是在 Microsoft 团队中创建[团队](../resources/team.md)的蓝图。</span><span class="sxs-lookup"><span data-stu-id="1c8da-104">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="1c8da-105">模板指定应在使用模板创建的新团队中设置的结构、设置和偶数内容。</span><span class="sxs-lookup"><span data-stu-id="1c8da-105">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="1c8da-106">Microsoft 提供了一套基本模板, 并且客户可以保存自己的自定义模板。</span><span class="sxs-lookup"><span data-stu-id="1c8da-106">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="1c8da-107">属性</span><span class="sxs-lookup"><span data-stu-id="1c8da-107">Properties</span></span>

| <span data-ttu-id="1c8da-108">属性</span><span class="sxs-lookup"><span data-stu-id="1c8da-108">Property</span></span>            | <span data-ttu-id="1c8da-109">类型</span><span class="sxs-lookup"><span data-stu-id="1c8da-109">Type</span></span>     | <span data-ttu-id="1c8da-110">说明</span><span class="sxs-lookup"><span data-stu-id="1c8da-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="1c8da-111">id</span><span class="sxs-lookup"><span data-stu-id="1c8da-111">id</span></span>                  | <span data-ttu-id="1c8da-112">String</span><span class="sxs-lookup"><span data-stu-id="1c8da-112">String</span></span>   | <span data-ttu-id="1c8da-113">模板的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1c8da-113">Unique identifier of the template.</span></span> <span data-ttu-id="1c8da-114">不能为 null。</span><span class="sxs-lookup"><span data-stu-id="1c8da-114">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1c8da-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c8da-115">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="1c8da-116">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1c8da-116">See also</span></span>

- [<span data-ttu-id="1c8da-117">团队</span><span class="sxs-lookup"><span data-stu-id="1c8da-117">team</span></span>](team.md)

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
