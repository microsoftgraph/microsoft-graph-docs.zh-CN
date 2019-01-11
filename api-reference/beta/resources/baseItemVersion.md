---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
ms.openlocfilehash: 9a5181e9cbc089832e8f73e0b8222ca63b69ca30
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894479"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="e2f39-102">BaseItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2f39-102">BaseItemVersion resource type</span></span>

> <span data-ttu-id="e2f39-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e2f39-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2f39-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e2f39-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2f39-105">**baseItemVersion** 资源表示项或实体的以前版本。</span><span class="sxs-lookup"><span data-stu-id="e2f39-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e2f39-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2f39-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e2f39-107">属性</span><span class="sxs-lookup"><span data-stu-id="e2f39-107">Properties</span></span>

|      <span data-ttu-id="e2f39-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="e2f39-108">Property name</span></span>       |                         <span data-ttu-id="e2f39-109">类型</span><span class="sxs-lookup"><span data-stu-id="e2f39-109">Type</span></span>                         |                               <span data-ttu-id="e2f39-110">说明</span><span class="sxs-lookup"><span data-stu-id="e2f39-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="e2f39-111">**id**</span><span class="sxs-lookup"><span data-stu-id="e2f39-111">**id**</span></span>                   | <span data-ttu-id="e2f39-112">string</span><span class="sxs-lookup"><span data-stu-id="e2f39-112">string</span></span>                                               | <span data-ttu-id="e2f39-113">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="e2f39-113">The ID of the version.</span></span> <span data-ttu-id="e2f39-114">只读。</span><span class="sxs-lookup"><span data-stu-id="e2f39-114">Read-only.</span></span>                                       |
| <span data-ttu-id="e2f39-115">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="e2f39-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="e2f39-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="e2f39-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="e2f39-117">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="e2f39-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="e2f39-118">只读。</span><span class="sxs-lookup"><span data-stu-id="e2f39-118">Read-only.</span></span>        |
| <span data-ttu-id="e2f39-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e2f39-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="e2f39-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2f39-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="e2f39-121">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e2f39-121">Date and time the version was last modified.</span></span> <span data-ttu-id="e2f39-122">只读。</span><span class="sxs-lookup"><span data-stu-id="e2f39-122">Read-only.</span></span>                 |
| <span data-ttu-id="e2f39-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="e2f39-123">**publication**</span></span>          | [<span data-ttu-id="e2f39-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="e2f39-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="e2f39-125">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="e2f39-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="e2f39-126">只读。</span><span class="sxs-lookup"><span data-stu-id="e2f39-126">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
