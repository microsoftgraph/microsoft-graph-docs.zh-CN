---
title: sharingDetail 资源类型
description: '包含共享项目的属性的复杂类型。 '
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 463ba207d7b160bffb96319a994b82ee82f14b8d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888457"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="edbb1-103">sharingDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="edbb1-103">sharingDetail resource type</span></span>

> <span data-ttu-id="edbb1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="edbb1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="edbb1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="edbb1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="edbb1-106">包含[共享](insights-shared.md)项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="edbb1-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="edbb1-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edbb1-107">JSON representation</span></span>
<span data-ttu-id="edbb1-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edbb1-108">Here is a JSON representation of the resource</span></span>

```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="edbb1-109">属性</span><span class="sxs-lookup"><span data-stu-id="edbb1-109">Properties</span></span>

| <span data-ttu-id="edbb1-110">属性</span><span class="sxs-lookup"><span data-stu-id="edbb1-110">Property</span></span>              | <span data-ttu-id="edbb1-111">类型</span><span class="sxs-lookup"><span data-stu-id="edbb1-111">Type</span></span>          | <span data-ttu-id="edbb1-112">Description</span><span class="sxs-lookup"><span data-stu-id="edbb1-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="edbb1-113">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="edbb1-113">sharedDateTime</span></span>        | <span data-ttu-id="edbb1-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edbb1-114">DateTimeOffset</span></span>| <span data-ttu-id="edbb1-115">日期和时间上次共享文件。</span><span class="sxs-lookup"><span data-stu-id="edbb1-115">The date and time the file was last shared.</span></span> <span data-ttu-id="edbb1-116">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="edbb1-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="edbb1-117">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="edbb1-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="edbb1-118">只读。</span><span class="sxs-lookup"><span data-stu-id="edbb1-118">Read-only.</span></span>  |
| <span data-ttu-id="edbb1-119">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="edbb1-119">sharingSubject</span></span>        | <span data-ttu-id="edbb1-120">字符串</span><span class="sxs-lookup"><span data-stu-id="edbb1-120">String</span></span>          | <span data-ttu-id="edbb1-121">与共享文档主题。</span><span class="sxs-lookup"><span data-stu-id="edbb1-121">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="edbb1-122">sharingType</span><span class="sxs-lookup"><span data-stu-id="edbb1-122">sharingType</span></span>             | <span data-ttu-id="edbb1-123">字符串</span><span class="sxs-lookup"><span data-stu-id="edbb1-123">String</span></span>        | <span data-ttu-id="edbb1-124">确定文档的方式共享，则可以通过"链接"、"附件"、"组"、"Site"。</span><span class="sxs-lookup"><span data-stu-id="edbb1-124">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="edbb1-125">sharedBy</span><span class="sxs-lookup"><span data-stu-id="edbb1-125">sharedBy</span></span>                | [<span data-ttu-id="edbb1-126">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="edbb1-126">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="edbb1-127">共享文档的用户。</span><span class="sxs-lookup"><span data-stu-id="edbb1-127">The user who shared the document.</span></span>  |
| <span data-ttu-id="edbb1-128">sharingReference</span><span class="sxs-lookup"><span data-stu-id="edbb1-128">sharingReference</span></span>        | [<span data-ttu-id="edbb1-129">resourceReference</span><span class="sxs-lookup"><span data-stu-id="edbb1-129">resourceReference</span></span>](insights-resourcereference.md)      |  |
