---
author: JeremyKelley
description: baseItemVersion 资源表示项或实体的以前版本。
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 47865e388616763b60ce3cd45195bf9919c7acf2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508036"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="4eb7a-103">BaseItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="4eb7a-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="4eb7a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4eb7a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eb7a-105">**baseItemVersion** 资源表示项或实体的以前版本。</span><span class="sxs-lookup"><span data-stu-id="4eb7a-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4eb7a-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4eb7a-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4eb7a-107">属性</span><span class="sxs-lookup"><span data-stu-id="4eb7a-107">Properties</span></span>

|      <span data-ttu-id="4eb7a-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="4eb7a-108">Property name</span></span>       |                         <span data-ttu-id="4eb7a-109">类型</span><span class="sxs-lookup"><span data-stu-id="4eb7a-109">Type</span></span>                         |                               <span data-ttu-id="4eb7a-110">说明</span><span class="sxs-lookup"><span data-stu-id="4eb7a-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="4eb7a-111">**id**</span><span class="sxs-lookup"><span data-stu-id="4eb7a-111">**id**</span></span>                   | <span data-ttu-id="4eb7a-112">string</span><span class="sxs-lookup"><span data-stu-id="4eb7a-112">string</span></span>                                               | <span data-ttu-id="4eb7a-113">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="4eb7a-113">The ID of the version.</span></span> <span data-ttu-id="4eb7a-114">只读。</span><span class="sxs-lookup"><span data-stu-id="4eb7a-114">Read-only.</span></span>                                       |
| <span data-ttu-id="4eb7a-115">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="4eb7a-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="4eb7a-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="4eb7a-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="4eb7a-117">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="4eb7a-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="4eb7a-118">只读。</span><span class="sxs-lookup"><span data-stu-id="4eb7a-118">Read-only.</span></span>        |
| <span data-ttu-id="4eb7a-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="4eb7a-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="4eb7a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eb7a-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="4eb7a-121">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4eb7a-121">Date and time the version was last modified.</span></span> <span data-ttu-id="4eb7a-122">只读。</span><span class="sxs-lookup"><span data-stu-id="4eb7a-122">Read-only.</span></span>                 |
| <span data-ttu-id="4eb7a-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="4eb7a-123">**publication**</span></span>          | [<span data-ttu-id="4eb7a-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="4eb7a-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="4eb7a-125">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="4eb7a-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="4eb7a-126">只读。</span><span class="sxs-lookup"><span data-stu-id="4eb7a-126">Read-only.</span></span> |


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
