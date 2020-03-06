---
title: freeBusyError 资源类型
description: 表示尝试获取用户、通讯组列表或资源可用性的错误信息。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8e069aef1d26a409e9ebe29a516136a952604ee6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531386"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="1f44f-103">freeBusyError 资源类型</span><span class="sxs-lookup"><span data-stu-id="1f44f-103">freeBusyError resource type</span></span>

<span data-ttu-id="1f44f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f44f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f44f-105">表示尝试获取用户、通讯组列表或资源可用性的错误信息。</span><span class="sxs-lookup"><span data-stu-id="1f44f-105">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="1f44f-106">属性</span><span class="sxs-lookup"><span data-stu-id="1f44f-106">Properties</span></span>
| <span data-ttu-id="1f44f-107">属性</span><span class="sxs-lookup"><span data-stu-id="1f44f-107">Property</span></span>     | <span data-ttu-id="1f44f-108">类型</span><span class="sxs-lookup"><span data-stu-id="1f44f-108">Type</span></span>   |<span data-ttu-id="1f44f-109">描述</span><span class="sxs-lookup"><span data-stu-id="1f44f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f44f-110">message</span><span class="sxs-lookup"><span data-stu-id="1f44f-110">message</span></span> |<span data-ttu-id="1f44f-111">String</span><span class="sxs-lookup"><span data-stu-id="1f44f-111">String</span></span> |<span data-ttu-id="1f44f-112">描述错误。</span><span class="sxs-lookup"><span data-stu-id="1f44f-112">Describes the error.</span></span> |
|<span data-ttu-id="1f44f-113">responseCode</span><span class="sxs-lookup"><span data-stu-id="1f44f-113">responseCode</span></span> |<span data-ttu-id="1f44f-114">字符串</span><span class="sxs-lookup"><span data-stu-id="1f44f-114">String</span></span> |<span data-ttu-id="1f44f-115">对用户、通讯组列表或资源的可用性进行查询的响应代码。</span><span class="sxs-lookup"><span data-stu-id="1f44f-115">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="1f44f-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f44f-116">JSON representation</span></span>

<span data-ttu-id="1f44f-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f44f-117">The following is a JSON representation of the resource.</span></span>

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
