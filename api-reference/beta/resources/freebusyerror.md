---
title: freeBusyError 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 63cfc4b14ba6176d582155df57b7f7f787e63cf4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889766"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="aa03a-104">freeBusyError 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa03a-104">freeBusyError resource type</span></span>

 > <span data-ttu-id="aa03a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aa03a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa03a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aa03a-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="aa03a-107">表示从尝试获取用户、 通讯组列表或资源的可用性的错误信息。</span><span class="sxs-lookup"><span data-stu-id="aa03a-107">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="aa03a-108">属性</span><span class="sxs-lookup"><span data-stu-id="aa03a-108">Properties</span></span>
| <span data-ttu-id="aa03a-109">属性</span><span class="sxs-lookup"><span data-stu-id="aa03a-109">Property</span></span>     | <span data-ttu-id="aa03a-110">类型</span><span class="sxs-lookup"><span data-stu-id="aa03a-110">Type</span></span>   |<span data-ttu-id="aa03a-111">Description</span><span class="sxs-lookup"><span data-stu-id="aa03a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa03a-112">message</span><span class="sxs-lookup"><span data-stu-id="aa03a-112">message</span></span> |<span data-ttu-id="aa03a-113">字符串</span><span class="sxs-lookup"><span data-stu-id="aa03a-113">String</span></span> |<span data-ttu-id="aa03a-114">描述的错误。</span><span class="sxs-lookup"><span data-stu-id="aa03a-114">Describes the error.</span></span> |
|<span data-ttu-id="aa03a-115">responseCode</span><span class="sxs-lookup"><span data-stu-id="aa03a-115">responseCode</span></span> |<span data-ttu-id="aa03a-116">字符串</span><span class="sxs-lookup"><span data-stu-id="aa03a-116">String</span></span> |<span data-ttu-id="aa03a-117">从查询的用户、 通讯组列表或资源可用性响应代码。</span><span class="sxs-lookup"><span data-stu-id="aa03a-117">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="aa03a-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa03a-118">JSON representation</span></span>

<span data-ttu-id="aa03a-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa03a-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
