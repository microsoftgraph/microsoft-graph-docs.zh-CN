---
title: personDataSource 资源类型
description: 表示用户数据来自的源，例如目录和 Outlook 联系人。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: b0682bae37c060b92df96fb6c92979b7ab57c259
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521916"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="ad465-103">personDataSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad465-103">personDataSource resource type</span></span>

<span data-ttu-id="ad465-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ad465-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad465-105">表示用户数据来自的源，例如目录和 Outlook 联系人。</span><span class="sxs-lookup"><span data-stu-id="ad465-105">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad465-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad465-106">JSON representation</span></span>

<span data-ttu-id="ad465-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad465-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="ad465-108">属性</span><span class="sxs-lookup"><span data-stu-id="ad465-108">Properties</span></span>
| <span data-ttu-id="ad465-109">属性</span><span class="sxs-lookup"><span data-stu-id="ad465-109">Property</span></span>     | <span data-ttu-id="ad465-110">类型</span><span class="sxs-lookup"><span data-stu-id="ad465-110">Type</span></span>   |<span data-ttu-id="ad465-111">说明</span><span class="sxs-lookup"><span data-stu-id="ad465-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad465-112">type</span><span class="sxs-lookup"><span data-stu-id="ad465-112">type</span></span>|<span data-ttu-id="ad465-113">String</span><span class="sxs-lookup"><span data-stu-id="ad465-113">String</span></span>|<span data-ttu-id="ad465-114">数据源的类型。</span><span class="sxs-lookup"><span data-stu-id="ad465-114">The type of data source.</span></span>|

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
