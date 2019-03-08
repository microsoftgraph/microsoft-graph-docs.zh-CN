---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
ms.openlocfilehash: 56a2c230c53c4b5bd50e8c123dd69eedec67a141
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480668"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="c2dff-102">BaseItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2dff-102">BaseItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2dff-103">**baseItemVersion** 资源表示项或实体的以前版本。</span><span class="sxs-lookup"><span data-stu-id="c2dff-103">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c2dff-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2dff-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c2dff-105">属性</span><span class="sxs-lookup"><span data-stu-id="c2dff-105">Properties</span></span>

|      <span data-ttu-id="c2dff-106">属性名称</span><span class="sxs-lookup"><span data-stu-id="c2dff-106">Property name</span></span>       |                         <span data-ttu-id="c2dff-107">类型</span><span class="sxs-lookup"><span data-stu-id="c2dff-107">Type</span></span>                         |                               <span data-ttu-id="c2dff-108">说明</span><span class="sxs-lookup"><span data-stu-id="c2dff-108">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="c2dff-109">**id**</span><span class="sxs-lookup"><span data-stu-id="c2dff-109">**id**</span></span>                   | <span data-ttu-id="c2dff-110">string</span><span class="sxs-lookup"><span data-stu-id="c2dff-110">string</span></span>                                               | <span data-ttu-id="c2dff-111">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="c2dff-111">The ID of the version.</span></span> <span data-ttu-id="c2dff-112">只读。</span><span class="sxs-lookup"><span data-stu-id="c2dff-112">Read-only.</span></span>                                       |
| <span data-ttu-id="c2dff-113">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="c2dff-113">**lastModifiedBy**</span></span>       | [<span data-ttu-id="c2dff-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="c2dff-114">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="c2dff-115">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="c2dff-115">Identity of the user which last modified the version.</span></span> <span data-ttu-id="c2dff-116">只读。</span><span class="sxs-lookup"><span data-stu-id="c2dff-116">Read-only.</span></span>        |
| <span data-ttu-id="c2dff-117">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="c2dff-117">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="c2dff-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2dff-118">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="c2dff-119">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c2dff-119">Date and time the version was last modified.</span></span> <span data-ttu-id="c2dff-120">只读。</span><span class="sxs-lookup"><span data-stu-id="c2dff-120">Read-only.</span></span>                 |
| <span data-ttu-id="c2dff-121">**publication**</span><span class="sxs-lookup"><span data-stu-id="c2dff-121">**publication**</span></span>          | [<span data-ttu-id="c2dff-122">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="c2dff-122">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="c2dff-123">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="c2dff-123">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="c2dff-124">只读。</span><span class="sxs-lookup"><span data-stu-id="c2dff-124">Read-only.</span></span> |


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
