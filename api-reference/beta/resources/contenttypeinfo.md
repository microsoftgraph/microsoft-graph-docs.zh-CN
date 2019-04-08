---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentTypeInfo
localization_priority: Normal
ms.openlocfilehash: 196a71be06b4e3c02330aba21559341650caa550
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530060"
---
# <a name="contenttypeinfo-resource-type"></a><span data-ttu-id="d9612-102">ContentTypeInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9612-102">ContentTypeInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9612-103">**contentTypeInfo** 资源指示项的 SharePoint 内容类型。</span><span class="sxs-lookup"><span data-stu-id="d9612-103">The **contentTypeInfo** resource indicates the SharePoint content type of an item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9612-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9612-104">JSON representation</span></span>

<span data-ttu-id="d9612-105">下面是 **contentTypeInfo** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9612-105">Here is a JSON representation of a **contentTypeInfo** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentTypeInfo", "@type.aka": "oneDrive.contentTypeFacet" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="d9612-106">属性</span><span class="sxs-lookup"><span data-stu-id="d9612-106">Properties</span></span>

| <span data-ttu-id="d9612-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="d9612-107">Property name</span></span>  | <span data-ttu-id="d9612-108">类型</span><span class="sxs-lookup"><span data-stu-id="d9612-108">Type</span></span>    | <span data-ttu-id="d9612-109">说明</span><span class="sxs-lookup"><span data-stu-id="d9612-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="d9612-110">**id**</span><span class="sxs-lookup"><span data-stu-id="d9612-110">**id**</span></span>         | <span data-ttu-id="d9612-111">string</span><span class="sxs-lookup"><span data-stu-id="d9612-111">string</span></span>  | <span data-ttu-id="d9612-112">内容类型的 ID。</span><span class="sxs-lookup"><span data-stu-id="d9612-112">The id of the content type.</span></span>
| <span data-ttu-id="d9612-113">**name**</span><span class="sxs-lookup"><span data-stu-id="d9612-113">**name**</span></span>       | <span data-ttu-id="d9612-114">string</span><span class="sxs-lookup"><span data-stu-id="d9612-114">string</span></span>  | <span data-ttu-id="d9612-115">内容类型的名称。</span><span class="sxs-lookup"><span data-stu-id="d9612-115">The name of the content type.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeInfo",
  "suppressions": [
    "Error: /api-reference/beta/resources/contenttypeinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
