---
title: personDataSource 资源类型
description: 代表用户数据来自，例如目录和 Outlook 联系人的源。
localization_priority: Normal
ms.openlocfilehash: 80e61bd1cd91c0b2a780936a5a311b0916743a17
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824967"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="04c92-103">personDataSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="04c92-103">personDataSource resource type</span></span>

> <span data-ttu-id="04c92-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="04c92-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04c92-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="04c92-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="04c92-106">代表用户数据来自，例如目录和 Outlook 联系人的源。</span><span class="sxs-lookup"><span data-stu-id="04c92-106">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="04c92-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04c92-107">JSON representation</span></span>

<span data-ttu-id="04c92-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04c92-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="04c92-109">属性</span><span class="sxs-lookup"><span data-stu-id="04c92-109">Properties</span></span>
| <span data-ttu-id="04c92-110">属性</span><span class="sxs-lookup"><span data-stu-id="04c92-110">Property</span></span>     | <span data-ttu-id="04c92-111">类型</span><span class="sxs-lookup"><span data-stu-id="04c92-111">Type</span></span>   |<span data-ttu-id="04c92-112">说明</span><span class="sxs-lookup"><span data-stu-id="04c92-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04c92-113">type</span><span class="sxs-lookup"><span data-stu-id="04c92-113">type</span></span>|<span data-ttu-id="04c92-114">字符串</span><span class="sxs-lookup"><span data-stu-id="04c92-114">String</span></span>|<span data-ttu-id="04c92-115">数据源的类型。</span><span class="sxs-lookup"><span data-stu-id="04c92-115">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
