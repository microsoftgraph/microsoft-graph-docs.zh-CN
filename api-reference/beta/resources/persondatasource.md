---
title: personDataSource 资源类型
description: 表示用户数据来自的源, 例如目录和 Outlook 联系人。
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 431cd9163873305508d5244005e6fe0a80501771
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573745"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="8c887-103">personDataSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c887-103">personDataSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c887-104">表示用户数据来自的源, 例如目录和 Outlook 联系人。</span><span class="sxs-lookup"><span data-stu-id="8c887-104">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c887-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c887-105">JSON representation</span></span>

<span data-ttu-id="8c887-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c887-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personDataSource"
}-->

```json
{
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="8c887-107">属性</span><span class="sxs-lookup"><span data-stu-id="8c887-107">Properties</span></span>
| <span data-ttu-id="8c887-108">属性</span><span class="sxs-lookup"><span data-stu-id="8c887-108">Property</span></span>     | <span data-ttu-id="8c887-109">类型</span><span class="sxs-lookup"><span data-stu-id="8c887-109">Type</span></span>   |<span data-ttu-id="8c887-110">说明</span><span class="sxs-lookup"><span data-stu-id="8c887-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c887-111">type</span><span class="sxs-lookup"><span data-stu-id="8c887-111">type</span></span>|<span data-ttu-id="8c887-112">String</span><span class="sxs-lookup"><span data-stu-id="8c887-112">String</span></span>|<span data-ttu-id="8c887-113">数据源的类型。</span><span class="sxs-lookup"><span data-stu-id="8c887-113">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/persondatasource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
