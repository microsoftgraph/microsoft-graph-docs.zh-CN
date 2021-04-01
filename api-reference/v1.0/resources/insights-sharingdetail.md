---
title: sharingDetail 资源类型
description: '包含共享项的属性的复杂类型。 '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 31ae4dd98949938cf14c2b5d57cb8b7f9ef3c1e5
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473981"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="35c78-103">sharingDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="35c78-103">sharingDetail resource type</span></span>

<span data-ttu-id="35c78-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35c78-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35c78-105">包含 [sharedInsight 项的属性的复杂](insights-shared.md) 类型。</span><span class="sxs-lookup"><span data-stu-id="35c78-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="35c78-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35c78-106">JSON representation</span></span>
<span data-ttu-id="35c78-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35c78-107">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingDetail"
}-->
```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "sharingReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="35c78-108">属性</span><span class="sxs-lookup"><span data-stu-id="35c78-108">Properties</span></span>

| <span data-ttu-id="35c78-109">属性</span><span class="sxs-lookup"><span data-stu-id="35c78-109">Property</span></span>              | <span data-ttu-id="35c78-110">类型</span><span class="sxs-lookup"><span data-stu-id="35c78-110">Type</span></span>          | <span data-ttu-id="35c78-111">说明</span><span class="sxs-lookup"><span data-stu-id="35c78-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="35c78-112">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="35c78-112">sharedDateTime</span></span>        | <span data-ttu-id="35c78-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35c78-113">DateTimeOffset</span></span>| <span data-ttu-id="35c78-114">上次共享文件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="35c78-114">The date and time the file was last shared.</span></span> <span data-ttu-id="35c78-115">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="35c78-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="35c78-116">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="35c78-116">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="35c78-117">只读。</span><span class="sxs-lookup"><span data-stu-id="35c78-117">Read-only.</span></span>  |
| <span data-ttu-id="35c78-118">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="35c78-118">sharingSubject</span></span>        | <span data-ttu-id="35c78-119">String</span><span class="sxs-lookup"><span data-stu-id="35c78-119">String</span></span>          | <span data-ttu-id="35c78-120">与文档共享的主题。</span><span class="sxs-lookup"><span data-stu-id="35c78-120">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="35c78-121">sharingType</span><span class="sxs-lookup"><span data-stu-id="35c78-121">sharingType</span></span>             | <span data-ttu-id="35c78-122">String</span><span class="sxs-lookup"><span data-stu-id="35c78-122">String</span></span>        | <span data-ttu-id="35c78-123">确定文档的共享方式，可通过"Link"、"Attachment"、"Group"、"Site"来表示。</span><span class="sxs-lookup"><span data-stu-id="35c78-123">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="35c78-124">sharedBy</span><span class="sxs-lookup"><span data-stu-id="35c78-124">sharedBy</span></span>                | [<span data-ttu-id="35c78-125">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="35c78-125">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="35c78-126">共享文档的用户。</span><span class="sxs-lookup"><span data-stu-id="35c78-126">The user who shared the document.</span></span>  |
| <span data-ttu-id="35c78-127">sharingReference</span><span class="sxs-lookup"><span data-stu-id="35c78-127">sharingReference</span></span>        | [<span data-ttu-id="35c78-128">resourceReference</span><span class="sxs-lookup"><span data-stu-id="35c78-128">resourceReference</span></span>](insights-resourcereference.md)      |  |

