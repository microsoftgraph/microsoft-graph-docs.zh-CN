---
title: BaseItemVersion 资源类型
description: '**baseItemVersion** 资源表示项或实体的以前版本。'
ms.openlocfilehash: c4fc95fd419bf8b2f20ab202874ca31a2b1d63f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009114"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="4b259-103">BaseItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b259-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="4b259-104">**baseItemVersion** 资源表示项或实体的以前版本。</span><span class="sxs-lookup"><span data-stu-id="4b259-104">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4b259-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b259-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4b259-106">属性</span><span class="sxs-lookup"><span data-stu-id="4b259-106">Properties</span></span>

|      <span data-ttu-id="4b259-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="4b259-107">Property name</span></span>       |                         <span data-ttu-id="4b259-108">类型</span><span class="sxs-lookup"><span data-stu-id="4b259-108">Type</span></span>                         |                               <span data-ttu-id="4b259-109">说明</span><span class="sxs-lookup"><span data-stu-id="4b259-109">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="4b259-110">**id**</span><span class="sxs-lookup"><span data-stu-id="4b259-110">**id**</span></span>                   | <span data-ttu-id="4b259-111">string</span><span class="sxs-lookup"><span data-stu-id="4b259-111">string</span></span>                                               | <span data-ttu-id="4b259-112">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="4b259-112">The ID of the version.</span></span> <span data-ttu-id="4b259-113">只读。</span><span class="sxs-lookup"><span data-stu-id="4b259-113">Read-only.</span></span>                                       |
| <span data-ttu-id="4b259-114">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="4b259-114">**lastModifiedBy**</span></span>       | [<span data-ttu-id="4b259-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="4b259-115">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="4b259-116">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="4b259-116">Identity of the user which last modified the version.</span></span> <span data-ttu-id="4b259-117">只读。</span><span class="sxs-lookup"><span data-stu-id="4b259-117">Read-only.</span></span>        |
| <span data-ttu-id="4b259-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="4b259-118">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="4b259-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b259-119">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="4b259-120">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4b259-120">Date and time the version was last modified.</span></span> <span data-ttu-id="4b259-121">只读。</span><span class="sxs-lookup"><span data-stu-id="4b259-121">Read-only.</span></span>                 |
| <span data-ttu-id="4b259-122">**publication**</span><span class="sxs-lookup"><span data-stu-id="4b259-122">**publication**</span></span>          | [<span data-ttu-id="4b259-123">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="4b259-123">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="4b259-124">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="4b259-124">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="4b259-125">只读。</span><span class="sxs-lookup"><span data-stu-id="4b259-125">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
