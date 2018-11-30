---
title: timeZoneBase 资源类型
description: 时区的基本表示形式。
ms.openlocfilehash: 00e09b064a083aa72316838c213f9c84e1139a19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048142"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="12406-103">timeZoneBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="12406-103">timeZoneBase resource type</span></span>

> <span data-ttu-id="12406-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="12406-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12406-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="12406-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="12406-106">时区的基本表示形式。</span><span class="sxs-lookup"><span data-stu-id="12406-106">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="12406-107">属性</span><span class="sxs-lookup"><span data-stu-id="12406-107">Properties</span></span>
| <span data-ttu-id="12406-108">属性</span><span class="sxs-lookup"><span data-stu-id="12406-108">Property</span></span>     | <span data-ttu-id="12406-109">类型</span><span class="sxs-lookup"><span data-stu-id="12406-109">Type</span></span>   |<span data-ttu-id="12406-110">说明</span><span class="sxs-lookup"><span data-stu-id="12406-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="12406-111">name</span><span class="sxs-lookup"><span data-stu-id="12406-111">name</span></span> | <span data-ttu-id="12406-112">string</span><span class="sxs-lookup"><span data-stu-id="12406-112">string</span></span> | <span data-ttu-id="12406-113">时区的名称。</span><span class="sxs-lookup"><span data-stu-id="12406-113">The name of a time zone.</span></span> <span data-ttu-id="12406-114">它可以是一个标准时区名称，例如“夏威夷-阿留申标准时间”，或自定义时区的“自定义时区”。</span><span class="sxs-lookup"><span data-stu-id="12406-114">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="12406-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12406-115">JSON representation</span></span>

<span data-ttu-id="12406-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12406-116">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->