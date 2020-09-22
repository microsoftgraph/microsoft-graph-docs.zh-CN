---
title: freeBusyError 资源类型
description: 表示尝试获取用户、通讯组列表或资源可用性的错误信息。
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b161d47ff7a89c79a04e9400ff0d4756692f49c9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018218"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="0940b-103">freeBusyError 资源类型</span><span class="sxs-lookup"><span data-stu-id="0940b-103">freeBusyError resource type</span></span>

<span data-ttu-id="0940b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0940b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0940b-105">表示尝试获取用户、通讯组列表或资源可用性的错误信息。</span><span class="sxs-lookup"><span data-stu-id="0940b-105">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="0940b-106">属性</span><span class="sxs-lookup"><span data-stu-id="0940b-106">Properties</span></span>
| <span data-ttu-id="0940b-107">属性</span><span class="sxs-lookup"><span data-stu-id="0940b-107">Property</span></span>     | <span data-ttu-id="0940b-108">类型</span><span class="sxs-lookup"><span data-stu-id="0940b-108">Type</span></span>   |<span data-ttu-id="0940b-109">描述</span><span class="sxs-lookup"><span data-stu-id="0940b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0940b-110">message</span><span class="sxs-lookup"><span data-stu-id="0940b-110">message</span></span> |<span data-ttu-id="0940b-111">String</span><span class="sxs-lookup"><span data-stu-id="0940b-111">String</span></span> |<span data-ttu-id="0940b-112">描述错误。</span><span class="sxs-lookup"><span data-stu-id="0940b-112">Describes the error.</span></span> |
|<span data-ttu-id="0940b-113">responseCode</span><span class="sxs-lookup"><span data-stu-id="0940b-113">responseCode</span></span> |<span data-ttu-id="0940b-114">String</span><span class="sxs-lookup"><span data-stu-id="0940b-114">String</span></span> |<span data-ttu-id="0940b-115">对用户、通讯组列表或资源的可用性进行查询的响应代码。</span><span class="sxs-lookup"><span data-stu-id="0940b-115">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="0940b-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0940b-116">JSON representation</span></span>

<span data-ttu-id="0940b-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0940b-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

