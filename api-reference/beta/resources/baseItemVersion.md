---
author: JeremyKelley
description: baseItemVersion 资源表示项或实体的以前版本。
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 0d007d18f6329763fa6a7a426f1f944ef1fb4106
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089727"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="d5280-103">BaseItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5280-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="d5280-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5280-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5280-105">**baseItemVersion** 资源表示项或实体的以前版本。</span><span class="sxs-lookup"><span data-stu-id="d5280-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d5280-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5280-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d5280-107">属性</span><span class="sxs-lookup"><span data-stu-id="d5280-107">Properties</span></span>

|      <span data-ttu-id="d5280-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="d5280-108">Property name</span></span>       |                         <span data-ttu-id="d5280-109">类型</span><span class="sxs-lookup"><span data-stu-id="d5280-109">Type</span></span>                         |                               <span data-ttu-id="d5280-110">说明</span><span class="sxs-lookup"><span data-stu-id="d5280-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="d5280-111">**id**</span><span class="sxs-lookup"><span data-stu-id="d5280-111">**id**</span></span>                   | <span data-ttu-id="d5280-112">string</span><span class="sxs-lookup"><span data-stu-id="d5280-112">string</span></span>                                               | <span data-ttu-id="d5280-113">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="d5280-113">The ID of the version.</span></span> <span data-ttu-id="d5280-114">只读。</span><span class="sxs-lookup"><span data-stu-id="d5280-114">Read-only.</span></span>                                       |
| <span data-ttu-id="d5280-115">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="d5280-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="d5280-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="d5280-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="d5280-117">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="d5280-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="d5280-118">只读。</span><span class="sxs-lookup"><span data-stu-id="d5280-118">Read-only.</span></span>        |
| <span data-ttu-id="d5280-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="d5280-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="d5280-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5280-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="d5280-121">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d5280-121">Date and time the version was last modified.</span></span> <span data-ttu-id="d5280-122">只读。</span><span class="sxs-lookup"><span data-stu-id="d5280-122">Read-only.</span></span>                 |
| <span data-ttu-id="d5280-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="d5280-123">**publication**</span></span>          | [<span data-ttu-id="d5280-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="d5280-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="d5280-125">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="d5280-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="d5280-126">只读。</span><span class="sxs-lookup"><span data-stu-id="d5280-126">Read-only.</span></span> |


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


