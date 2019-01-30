---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
ms.openlocfilehash: fcf427300007277f7ea6382579ad3a0929ca97d1
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643022"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="0bc9a-102">BaseItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="0bc9a-102">BaseItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bc9a-103">**baseItemVersion** 资源表示项或实体的以前版本。</span><span class="sxs-lookup"><span data-stu-id="0bc9a-103">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0bc9a-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0bc9a-104">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.baseItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="0bc9a-105">属性</span><span class="sxs-lookup"><span data-stu-id="0bc9a-105">Properties</span></span>

|      <span data-ttu-id="0bc9a-106">属性名称</span><span class="sxs-lookup"><span data-stu-id="0bc9a-106">Property name</span></span>       |                         <span data-ttu-id="0bc9a-107">类型</span><span class="sxs-lookup"><span data-stu-id="0bc9a-107">Type</span></span>                         |                               <span data-ttu-id="0bc9a-108">说明</span><span class="sxs-lookup"><span data-stu-id="0bc9a-108">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="0bc9a-109">**id**</span><span class="sxs-lookup"><span data-stu-id="0bc9a-109">**id**</span></span>                   | <span data-ttu-id="0bc9a-110">string</span><span class="sxs-lookup"><span data-stu-id="0bc9a-110">string</span></span>                                               | <span data-ttu-id="0bc9a-111">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="0bc9a-111">The ID of the version.</span></span> <span data-ttu-id="0bc9a-112">只读。</span><span class="sxs-lookup"><span data-stu-id="0bc9a-112">Read-only.</span></span>                                       |
| <span data-ttu-id="0bc9a-113">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="0bc9a-113">**lastModifiedBy**</span></span>       | [<span data-ttu-id="0bc9a-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="0bc9a-114">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="0bc9a-115">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="0bc9a-115">Identity of the user which last modified the version.</span></span> <span data-ttu-id="0bc9a-116">只读。</span><span class="sxs-lookup"><span data-stu-id="0bc9a-116">Read-only.</span></span>        |
| <span data-ttu-id="0bc9a-117">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="0bc9a-117">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="0bc9a-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bc9a-118">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="0bc9a-119">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0bc9a-119">Date and time the version was last modified.</span></span> <span data-ttu-id="0bc9a-120">只读。</span><span class="sxs-lookup"><span data-stu-id="0bc9a-120">Read-only.</span></span>                 |
| <span data-ttu-id="0bc9a-121">**publication**</span><span class="sxs-lookup"><span data-stu-id="0bc9a-121">**publication**</span></span>          | [<span data-ttu-id="0bc9a-122">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="0bc9a-122">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="0bc9a-123">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="0bc9a-123">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="0bc9a-124">只读。</span><span class="sxs-lookup"><span data-stu-id="0bc9a-124">Read-only.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/baseItemVersion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
