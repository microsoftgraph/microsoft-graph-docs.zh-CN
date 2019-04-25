---
title: genericError 资源类型
description: 常规用途的错误。
localization_priority: Normal
ms.openlocfilehash: d3c7e9cd7ff7be635adfbf329170068cd944f0b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547493"
---
# <a name="genericerror-resource-type"></a><span data-ttu-id="8afdb-103">genericError 资源类型</span><span class="sxs-lookup"><span data-stu-id="8afdb-103">genericError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8afdb-104">常规用途的错误。</span><span class="sxs-lookup"><span data-stu-id="8afdb-104">A general-purpose error.</span></span>

## <a name="properties"></a><span data-ttu-id="8afdb-105">属性</span><span class="sxs-lookup"><span data-stu-id="8afdb-105">Properties</span></span>

| <span data-ttu-id="8afdb-106">属性</span><span class="sxs-lookup"><span data-stu-id="8afdb-106">Property</span></span> | <span data-ttu-id="8afdb-107">类型</span><span class="sxs-lookup"><span data-stu-id="8afdb-107">Type</span></span> | <span data-ttu-id="8afdb-108">描述</span><span class="sxs-lookup"><span data-stu-id="8afdb-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="8afdb-109">message</span><span class="sxs-lookup"><span data-stu-id="8afdb-109">message</span></span> | <span data-ttu-id="8afdb-110">String</span><span class="sxs-lookup"><span data-stu-id="8afdb-110">String</span></span> | <span data-ttu-id="8afdb-111">错误消息。</span><span class="sxs-lookup"><span data-stu-id="8afdb-111">The error message.</span></span> |
| <span data-ttu-id="8afdb-112">code</span><span class="sxs-lookup"><span data-stu-id="8afdb-112">code</span></span> | <span data-ttu-id="8afdb-113">String</span><span class="sxs-lookup"><span data-stu-id="8afdb-113">String</span></span> | <span data-ttu-id="8afdb-114">错误代码。</span><span class="sxs-lookup"><span data-stu-id="8afdb-114">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8afdb-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8afdb-115">JSON representation</span></span>

<span data-ttu-id="8afdb-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8afdb-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/genericerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
