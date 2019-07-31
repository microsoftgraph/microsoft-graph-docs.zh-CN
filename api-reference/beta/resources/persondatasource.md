---
title: personDataSource 资源类型
description: 表示用户数据来自的源, 例如目录和 Outlook 联系人。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 80c7ec18094af2cd84671e095515566bfc52a10e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966112"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="27cf9-103">personDataSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="27cf9-103">personDataSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27cf9-104">表示用户数据来自的源, 例如目录和 Outlook 联系人。</span><span class="sxs-lookup"><span data-stu-id="27cf9-104">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="27cf9-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="27cf9-105">JSON representation</span></span>

<span data-ttu-id="27cf9-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27cf9-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="27cf9-107">属性</span><span class="sxs-lookup"><span data-stu-id="27cf9-107">Properties</span></span>
| <span data-ttu-id="27cf9-108">属性</span><span class="sxs-lookup"><span data-stu-id="27cf9-108">Property</span></span>     | <span data-ttu-id="27cf9-109">类型</span><span class="sxs-lookup"><span data-stu-id="27cf9-109">Type</span></span>   |<span data-ttu-id="27cf9-110">说明</span><span class="sxs-lookup"><span data-stu-id="27cf9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="27cf9-111">type</span><span class="sxs-lookup"><span data-stu-id="27cf9-111">type</span></span>|<span data-ttu-id="27cf9-112">String</span><span class="sxs-lookup"><span data-stu-id="27cf9-112">String</span></span>|<span data-ttu-id="27cf9-113">数据源的类型。</span><span class="sxs-lookup"><span data-stu-id="27cf9-113">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
