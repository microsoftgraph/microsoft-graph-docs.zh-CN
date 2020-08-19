---
title: BaseItemVersion 资源类型
description: '**baseItemVersion** 资源表示项或实体的以前版本。'
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cc432af84b67e1781be4193a3e8d2bba29ff67a7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808289"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="6f70d-103">BaseItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f70d-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="6f70d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f70d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6f70d-105">**baseItemVersion** 资源表示项或实体的以前版本。</span><span class="sxs-lookup"><span data-stu-id="6f70d-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6f70d-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f70d-106">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="6f70d-107">属性</span><span class="sxs-lookup"><span data-stu-id="6f70d-107">Properties</span></span>

|      <span data-ttu-id="6f70d-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="6f70d-108">Property name</span></span>       |                         <span data-ttu-id="6f70d-109">类型</span><span class="sxs-lookup"><span data-stu-id="6f70d-109">Type</span></span>                         |                               <span data-ttu-id="6f70d-110">说明</span><span class="sxs-lookup"><span data-stu-id="6f70d-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="6f70d-111">**id**</span><span class="sxs-lookup"><span data-stu-id="6f70d-111">**id**</span></span>                   | <span data-ttu-id="6f70d-112">string</span><span class="sxs-lookup"><span data-stu-id="6f70d-112">string</span></span>                                               | <span data-ttu-id="6f70d-113">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="6f70d-113">The ID of the version.</span></span> <span data-ttu-id="6f70d-114">只读。</span><span class="sxs-lookup"><span data-stu-id="6f70d-114">Read-only.</span></span>                                       |
| <span data-ttu-id="6f70d-115">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="6f70d-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="6f70d-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="6f70d-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="6f70d-117">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="6f70d-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="6f70d-118">只读。</span><span class="sxs-lookup"><span data-stu-id="6f70d-118">Read-only.</span></span>        |
| <span data-ttu-id="6f70d-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="6f70d-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="6f70d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f70d-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="6f70d-121">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="6f70d-121">Date and time the version was last modified.</span></span> <span data-ttu-id="6f70d-122">只读。</span><span class="sxs-lookup"><span data-stu-id="6f70d-122">Read-only.</span></span>                 |
| <span data-ttu-id="6f70d-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="6f70d-123">**publication**</span></span>          | [<span data-ttu-id="6f70d-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="6f70d-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="6f70d-125">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="6f70d-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="6f70d-126">只读。</span><span class="sxs-lookup"><span data-stu-id="6f70d-126">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
