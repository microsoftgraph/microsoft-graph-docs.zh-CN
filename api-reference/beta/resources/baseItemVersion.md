---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: BaseItemVersion
ms.openlocfilehash: dfda19af6057bc1d6e1757d24f6a2c99979a8622
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041472"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="4a8ca-102">BaseItemVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a8ca-102">BaseItemVersion resource type</span></span>

> <span data-ttu-id="4a8ca-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4a8ca-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a8ca-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4a8ca-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a8ca-105">**baseItemVersion** 资源表示项或实体的以前版本。</span><span class="sxs-lookup"><span data-stu-id="4a8ca-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4a8ca-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a8ca-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4a8ca-107">属性</span><span class="sxs-lookup"><span data-stu-id="4a8ca-107">Properties</span></span>

|      <span data-ttu-id="4a8ca-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="4a8ca-108">Property name</span></span>       |                         <span data-ttu-id="4a8ca-109">类型</span><span class="sxs-lookup"><span data-stu-id="4a8ca-109">Type</span></span>                         |                               <span data-ttu-id="4a8ca-110">说明</span><span class="sxs-lookup"><span data-stu-id="4a8ca-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="4a8ca-111">**id**</span><span class="sxs-lookup"><span data-stu-id="4a8ca-111">**id**</span></span>                   | <span data-ttu-id="4a8ca-112">string</span><span class="sxs-lookup"><span data-stu-id="4a8ca-112">string</span></span>                                               | <span data-ttu-id="4a8ca-113">版本 ID。</span><span class="sxs-lookup"><span data-stu-id="4a8ca-113">The ID of the version.</span></span> <span data-ttu-id="4a8ca-114">只读。</span><span class="sxs-lookup"><span data-stu-id="4a8ca-114">Read-only.</span></span>                                       |
| <span data-ttu-id="4a8ca-115">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="4a8ca-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="4a8ca-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="4a8ca-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="4a8ca-117">上次修改版本的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="4a8ca-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="4a8ca-118">只读。</span><span class="sxs-lookup"><span data-stu-id="4a8ca-118">Read-only.</span></span>        |
| <span data-ttu-id="4a8ca-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="4a8ca-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="4a8ca-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a8ca-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="4a8ca-121">上次修改版本的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4a8ca-121">Date and time the version was last modified.</span></span> <span data-ttu-id="4a8ca-122">只读。</span><span class="sxs-lookup"><span data-stu-id="4a8ca-122">Read-only.</span></span>                 |
| <span data-ttu-id="4a8ca-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="4a8ca-123">**publication**</span></span>          | [<span data-ttu-id="4a8ca-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="4a8ca-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="4a8ca-125">指示此特定版本的发布状态。</span><span class="sxs-lookup"><span data-stu-id="4a8ca-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="4a8ca-126">只读。</span><span class="sxs-lookup"><span data-stu-id="4a8ca-126">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->