---
title: freeBusyError 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: f1ff7717034798830a610b35dbbff5c987cf7371
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529843"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="406e2-104">freeBusyError 资源类型</span><span class="sxs-lookup"><span data-stu-id="406e2-104">freeBusyError resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="406e2-105">表示从尝试获取用户、 通讯组列表或资源的可用性的错误信息。</span><span class="sxs-lookup"><span data-stu-id="406e2-105">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="406e2-106">属性</span><span class="sxs-lookup"><span data-stu-id="406e2-106">Properties</span></span>
| <span data-ttu-id="406e2-107">属性</span><span class="sxs-lookup"><span data-stu-id="406e2-107">Property</span></span>     | <span data-ttu-id="406e2-108">类型</span><span class="sxs-lookup"><span data-stu-id="406e2-108">Type</span></span>   |<span data-ttu-id="406e2-109">说明</span><span class="sxs-lookup"><span data-stu-id="406e2-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="406e2-110">message</span><span class="sxs-lookup"><span data-stu-id="406e2-110">message</span></span> |<span data-ttu-id="406e2-111">String</span><span class="sxs-lookup"><span data-stu-id="406e2-111">String</span></span> |<span data-ttu-id="406e2-112">描述的错误。</span><span class="sxs-lookup"><span data-stu-id="406e2-112">Describes the error.</span></span> |
|<span data-ttu-id="406e2-113">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="406e2-113">responseCode</span></span> |<span data-ttu-id="406e2-114">String</span><span class="sxs-lookup"><span data-stu-id="406e2-114">String</span></span> |<span data-ttu-id="406e2-115">从查询的用户、 通讯组列表或资源可用性响应代码。</span><span class="sxs-lookup"><span data-stu-id="406e2-115">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="406e2-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="406e2-116">JSON representation</span></span>

<span data-ttu-id="406e2-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="406e2-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/freebusyerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
