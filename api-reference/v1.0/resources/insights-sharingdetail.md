---
title: sharingDetail 资源类型
description: '包含共享项目的属性的复杂类型。 '
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c441dcdc3b743e5bf55786ad1b43bfe2010b01b8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531288"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="d4922-103">sharingDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4922-103">sharingDetail resource type</span></span>

<span data-ttu-id="d4922-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4922-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d4922-105">包含[sharedInsight](insights-shared.md)项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="d4922-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="d4922-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4922-106">JSON representation</span></span>
<span data-ttu-id="d4922-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4922-107">Here is a JSON representation of the resource</span></span>
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
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="d4922-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4922-108">Properties</span></span>

| <span data-ttu-id="d4922-109">属性</span><span class="sxs-lookup"><span data-stu-id="d4922-109">Property</span></span>              | <span data-ttu-id="d4922-110">类型</span><span class="sxs-lookup"><span data-stu-id="d4922-110">Type</span></span>          | <span data-ttu-id="d4922-111">说明</span><span class="sxs-lookup"><span data-stu-id="d4922-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="d4922-112">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4922-112">sharedDateTime</span></span>        | <span data-ttu-id="d4922-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4922-113">DateTimeOffset</span></span>| <span data-ttu-id="d4922-114">上次共享文件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d4922-114">The date and time the file was last shared.</span></span> <span data-ttu-id="d4922-115">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d4922-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d4922-116">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="d4922-116">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="d4922-117">只读。</span><span class="sxs-lookup"><span data-stu-id="d4922-117">Read-only.</span></span>  |
| <span data-ttu-id="d4922-118">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="d4922-118">sharingSubject</span></span>        | <span data-ttu-id="d4922-119">字符串</span><span class="sxs-lookup"><span data-stu-id="d4922-119">String</span></span>          | <span data-ttu-id="d4922-120">共享文档的主题。</span><span class="sxs-lookup"><span data-stu-id="d4922-120">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="d4922-121">sharingType</span><span class="sxs-lookup"><span data-stu-id="d4922-121">sharingType</span></span>             | <span data-ttu-id="d4922-122">字符串</span><span class="sxs-lookup"><span data-stu-id="d4922-122">String</span></span>        | <span data-ttu-id="d4922-123">确定文档的共享方式，可以是 "链接"、"附件"、"组"、"网站"。</span><span class="sxs-lookup"><span data-stu-id="d4922-123">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="d4922-124">sharedBy</span><span class="sxs-lookup"><span data-stu-id="d4922-124">sharedBy</span></span>                | [<span data-ttu-id="d4922-125">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="d4922-125">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="d4922-126">共享文档的用户。</span><span class="sxs-lookup"><span data-stu-id="d4922-126">The user who shared the document.</span></span>  |
| <span data-ttu-id="d4922-127">sharingReference</span><span class="sxs-lookup"><span data-stu-id="d4922-127">sharingReference</span></span>        | [<span data-ttu-id="d4922-128">resourceReference</span><span class="sxs-lookup"><span data-stu-id="d4922-128">resourceReference</span></span>](insights-resourcereference.md)      |  |
