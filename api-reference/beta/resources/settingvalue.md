---
title: settingValue 资源类型
description: 由名称/值对表示的设置。
localization_priority: Normal
ms.openlocfilehash: 0ddd6388e14ea3deff99e927541694a97c594195
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815524"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="f63e4-103">settingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="f63e4-103">settingValue resource type</span></span>

> <span data-ttu-id="f63e4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f63e4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f63e4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f63e4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f63e4-106">由名称/值对表示的设置。</span><span class="sxs-lookup"><span data-stu-id="f63e4-106">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="f63e4-107">属性</span><span class="sxs-lookup"><span data-stu-id="f63e4-107">Properties</span></span>
| <span data-ttu-id="f63e4-108">属性</span><span class="sxs-lookup"><span data-stu-id="f63e4-108">Property</span></span>     | <span data-ttu-id="f63e4-109">类型</span><span class="sxs-lookup"><span data-stu-id="f63e4-109">Type</span></span>   |<span data-ttu-id="f63e4-110">说明</span><span class="sxs-lookup"><span data-stu-id="f63e4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f63e4-111">name</span><span class="sxs-lookup"><span data-stu-id="f63e4-111">name</span></span>|<span data-ttu-id="f63e4-112">string</span><span class="sxs-lookup"><span data-stu-id="f63e4-112">string</span></span>|<span data-ttu-id="f63e4-113">设置 （如由 directorySettingTemplate 定义） 的名称。</span><span class="sxs-lookup"><span data-stu-id="f63e4-113">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="f63e4-114">值</span><span class="sxs-lookup"><span data-stu-id="f63e4-114">value</span></span>|<span data-ttu-id="f63e4-115">string</span><span class="sxs-lookup"><span data-stu-id="f63e4-115">string</span></span>|<span data-ttu-id="f63e4-116">设置的值。</span><span class="sxs-lookup"><span data-stu-id="f63e4-116">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f63e4-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f63e4-117">JSON representation</span></span>

<span data-ttu-id="f63e4-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f63e4-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
