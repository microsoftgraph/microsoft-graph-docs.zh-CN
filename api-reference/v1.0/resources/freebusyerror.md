---
title: freeBusyError 资源类型
description: 表示尝试获取用户、通讯组列表或资源可用性的错误信息。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ca306ba5a40ffc08147c8e8449ab03bf51afd745
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030280"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="1a681-103">freeBusyError 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a681-103">freeBusyError resource type</span></span>

<span data-ttu-id="1a681-104">表示尝试获取用户、通讯组列表或资源可用性的错误信息。</span><span class="sxs-lookup"><span data-stu-id="1a681-104">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="1a681-105">属性</span><span class="sxs-lookup"><span data-stu-id="1a681-105">Properties</span></span>
| <span data-ttu-id="1a681-106">属性</span><span class="sxs-lookup"><span data-stu-id="1a681-106">Property</span></span>     | <span data-ttu-id="1a681-107">类型</span><span class="sxs-lookup"><span data-stu-id="1a681-107">Type</span></span>   |<span data-ttu-id="1a681-108">描述</span><span class="sxs-lookup"><span data-stu-id="1a681-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a681-109">message</span><span class="sxs-lookup"><span data-stu-id="1a681-109">message</span></span> |<span data-ttu-id="1a681-110">String</span><span class="sxs-lookup"><span data-stu-id="1a681-110">String</span></span> |<span data-ttu-id="1a681-111">描述错误。</span><span class="sxs-lookup"><span data-stu-id="1a681-111">Describes the error.</span></span> |
|<span data-ttu-id="1a681-112">responseCode</span><span class="sxs-lookup"><span data-stu-id="1a681-112">responseCode</span></span> |<span data-ttu-id="1a681-113">String</span><span class="sxs-lookup"><span data-stu-id="1a681-113">String</span></span> |<span data-ttu-id="1a681-114">对用户、通讯组列表或资源的可用性进行查询的响应代码。</span><span class="sxs-lookup"><span data-stu-id="1a681-114">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="1a681-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a681-115">JSON representation</span></span>

<span data-ttu-id="1a681-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a681-116">The following is a JSON representation of the resource.</span></span>

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
