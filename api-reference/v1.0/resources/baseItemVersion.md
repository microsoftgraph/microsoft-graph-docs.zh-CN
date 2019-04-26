---
title: BaseItemVersion 资源类型
description: '**baseItemVersion** 资源表示项或实体的以前版本。'
localization_priority: Normal
ms.openlocfilehash: bd28f9c8dc5be2bc6422aca2eb756aba78b8e393
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569436"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="0b28e-103">BaseItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b28e-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="0b28e-104">**baseItemVersion** 资源表示项或实体的以前版本。</span><span class="sxs-lookup"><span data-stu-id="0b28e-104">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0b28e-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b28e-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0b28e-106">属性</span><span class="sxs-lookup"><span data-stu-id="0b28e-106">Properties</span></span>

|      <span data-ttu-id="0b28e-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="0b28e-107">Property name</span></span>       |                         <span data-ttu-id="0b28e-108">类型</span><span class="sxs-lookup"><span data-stu-id="0b28e-108">Type</span></span>                         |                               <span data-ttu-id="0b28e-109">说明</span><span class="sxs-lookup"><span data-stu-id="0b28e-109">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="0b28e-110">**id**</span><span class="sxs-lookup"><span data-stu-id="0b28e-110">**id**</span></span>                   | <span data-ttu-id="0b28e-111">string</span><span class="sxs-lookup"><span data-stu-id="0b28e-111">string</span></span>                                               | <span data-ttu-id="0b28e-112">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="0b28e-112">The ID of the version.</span></span> <span data-ttu-id="0b28e-113">只读。</span><span class="sxs-lookup"><span data-stu-id="0b28e-113">Read-only.</span></span>                                       |
| <span data-ttu-id="0b28e-114">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="0b28e-114">**lastModifiedBy**</span></span>       | [<span data-ttu-id="0b28e-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="0b28e-115">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="0b28e-116">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="0b28e-116">Identity of the user which last modified the version.</span></span> <span data-ttu-id="0b28e-117">只读。</span><span class="sxs-lookup"><span data-stu-id="0b28e-117">Read-only.</span></span>        |
| <span data-ttu-id="0b28e-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="0b28e-118">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="0b28e-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b28e-119">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="0b28e-120">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0b28e-120">Date and time the version was last modified.</span></span> <span data-ttu-id="0b28e-121">只读。</span><span class="sxs-lookup"><span data-stu-id="0b28e-121">Read-only.</span></span>                 |
| <span data-ttu-id="0b28e-122">**publication**</span><span class="sxs-lookup"><span data-stu-id="0b28e-122">**publication**</span></span>          | [<span data-ttu-id="0b28e-123">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="0b28e-123">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="0b28e-124">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="0b28e-124">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="0b28e-125">只读。</span><span class="sxs-lookup"><span data-stu-id="0b28e-125">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
