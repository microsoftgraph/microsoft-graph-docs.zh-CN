---
title: timeZoneBase 资源类型
description: 时区的基本表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: 4869fafb20150a06a6da323359664f98b83d3eee
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133341"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="d23da-103">timeZoneBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="d23da-103">timeZoneBase resource type</span></span>

<span data-ttu-id="d23da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d23da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d23da-105">时区的基本表示形式。</span><span class="sxs-lookup"><span data-stu-id="d23da-105">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="d23da-106">属性</span><span class="sxs-lookup"><span data-stu-id="d23da-106">Properties</span></span>
| <span data-ttu-id="d23da-107">属性</span><span class="sxs-lookup"><span data-stu-id="d23da-107">Property</span></span>     | <span data-ttu-id="d23da-108">类型</span><span class="sxs-lookup"><span data-stu-id="d23da-108">Type</span></span>   |<span data-ttu-id="d23da-109">说明</span><span class="sxs-lookup"><span data-stu-id="d23da-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d23da-110">name</span><span class="sxs-lookup"><span data-stu-id="d23da-110">name</span></span> | <span data-ttu-id="d23da-111">string</span><span class="sxs-lookup"><span data-stu-id="d23da-111">string</span></span> | <span data-ttu-id="d23da-112">时区的名称。</span><span class="sxs-lookup"><span data-stu-id="d23da-112">The name of a time zone.</span></span> <span data-ttu-id="d23da-113">它可以是一个标准时区名称，例如“夏威夷-阿留申标准时间”，或自定义时区的“自定义时区”。</span><span class="sxs-lookup"><span data-stu-id="d23da-113">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d23da-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d23da-114">JSON representation</span></span>

<span data-ttu-id="d23da-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d23da-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


