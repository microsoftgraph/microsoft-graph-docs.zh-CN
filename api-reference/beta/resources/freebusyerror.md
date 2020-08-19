---
title: freeBusyError 资源类型
description: 表示尝试获取用户、通讯组列表或资源可用性的错误信息。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: e259685415a37e89429b5e0522e89a4fbe2f9fd2
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809535"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="5cc5d-103">freeBusyError 资源类型</span><span class="sxs-lookup"><span data-stu-id="5cc5d-103">freeBusyError resource type</span></span>

<span data-ttu-id="5cc5d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cc5d-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cc5d-105">表示尝试获取用户、通讯组列表或资源可用性的错误信息。</span><span class="sxs-lookup"><span data-stu-id="5cc5d-105">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="5cc5d-106">属性</span><span class="sxs-lookup"><span data-stu-id="5cc5d-106">Properties</span></span>
| <span data-ttu-id="5cc5d-107">属性</span><span class="sxs-lookup"><span data-stu-id="5cc5d-107">Property</span></span>     | <span data-ttu-id="5cc5d-108">类型</span><span class="sxs-lookup"><span data-stu-id="5cc5d-108">Type</span></span>   |<span data-ttu-id="5cc5d-109">描述</span><span class="sxs-lookup"><span data-stu-id="5cc5d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5cc5d-110">message</span><span class="sxs-lookup"><span data-stu-id="5cc5d-110">message</span></span> |<span data-ttu-id="5cc5d-111">String</span><span class="sxs-lookup"><span data-stu-id="5cc5d-111">String</span></span> |<span data-ttu-id="5cc5d-112">描述错误。</span><span class="sxs-lookup"><span data-stu-id="5cc5d-112">Describes the error.</span></span> |
|<span data-ttu-id="5cc5d-113">responseCode</span><span class="sxs-lookup"><span data-stu-id="5cc5d-113">responseCode</span></span> |<span data-ttu-id="5cc5d-114">String</span><span class="sxs-lookup"><span data-stu-id="5cc5d-114">String</span></span> |<span data-ttu-id="5cc5d-115">对用户、通讯组列表或资源的可用性进行查询的响应代码。</span><span class="sxs-lookup"><span data-stu-id="5cc5d-115">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="5cc5d-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5cc5d-116">JSON representation</span></span>

<span data-ttu-id="5cc5d-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cc5d-117">The following is a JSON representation of the resource.</span></span>

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
  "tocPath": "",
  "suppressions": []
}
-->
