---
author: JeremyKelley
description: baseItemVersion 资源表示项或实体的以前版本。
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d5265004eac969fa827e5456183180a4c6434f96
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974232"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="656ef-103">BaseItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="656ef-103">BaseItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="656ef-104">**baseItemVersion** 资源表示项或实体的以前版本。</span><span class="sxs-lookup"><span data-stu-id="656ef-104">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="656ef-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="656ef-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="656ef-106">属性</span><span class="sxs-lookup"><span data-stu-id="656ef-106">Properties</span></span>

|      <span data-ttu-id="656ef-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="656ef-107">Property name</span></span>       |                         <span data-ttu-id="656ef-108">类型</span><span class="sxs-lookup"><span data-stu-id="656ef-108">Type</span></span>                         |                               <span data-ttu-id="656ef-109">说明</span><span class="sxs-lookup"><span data-stu-id="656ef-109">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="656ef-110">**id**</span><span class="sxs-lookup"><span data-stu-id="656ef-110">**id**</span></span>                   | <span data-ttu-id="656ef-111">string</span><span class="sxs-lookup"><span data-stu-id="656ef-111">string</span></span>                                               | <span data-ttu-id="656ef-112">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="656ef-112">The ID of the version.</span></span> <span data-ttu-id="656ef-113">只读。</span><span class="sxs-lookup"><span data-stu-id="656ef-113">Read-only.</span></span>                                       |
| <span data-ttu-id="656ef-114">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="656ef-114">**lastModifiedBy**</span></span>       | [<span data-ttu-id="656ef-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="656ef-115">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="656ef-116">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="656ef-116">Identity of the user which last modified the version.</span></span> <span data-ttu-id="656ef-117">只读。</span><span class="sxs-lookup"><span data-stu-id="656ef-117">Read-only.</span></span>        |
| <span data-ttu-id="656ef-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="656ef-118">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="656ef-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="656ef-119">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="656ef-120">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="656ef-120">Date and time the version was last modified.</span></span> <span data-ttu-id="656ef-121">只读。</span><span class="sxs-lookup"><span data-stu-id="656ef-121">Read-only.</span></span>                 |
| <span data-ttu-id="656ef-122">**publication**</span><span class="sxs-lookup"><span data-stu-id="656ef-122">**publication**</span></span>          | [<span data-ttu-id="656ef-123">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="656ef-123">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="656ef-124">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="656ef-124">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="656ef-125">只读。</span><span class="sxs-lookup"><span data-stu-id="656ef-125">Read-only.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": []
}
-->
