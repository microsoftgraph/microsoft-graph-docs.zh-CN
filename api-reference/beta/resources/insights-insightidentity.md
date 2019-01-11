---
title: insightIdentity
description: 包含共享项目的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 395c865a38ebe6ea84dc64857f441cd529e4f2d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886574"
---
# <a name="insightidentity"></a><span data-ttu-id="2cb11-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="2cb11-103">insightIdentity</span></span>

> <span data-ttu-id="2cb11-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2cb11-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2cb11-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2cb11-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2cb11-106">包含[共享](insights-shared.md)项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="2cb11-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="2cb11-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2cb11-107">JSON representation</span></span>
<span data-ttu-id="2cb11-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2cb11-108">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="2cb11-109">属性</span><span class="sxs-lookup"><span data-stu-id="2cb11-109">Properties</span></span>

| <span data-ttu-id="2cb11-110">属性</span><span class="sxs-lookup"><span data-stu-id="2cb11-110">Property</span></span>              | <span data-ttu-id="2cb11-111">类型</span><span class="sxs-lookup"><span data-stu-id="2cb11-111">Type</span></span>          | <span data-ttu-id="2cb11-112">说明</span><span class="sxs-lookup"><span data-stu-id="2cb11-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="2cb11-113">displayName</span><span class="sxs-lookup"><span data-stu-id="2cb11-113">displayName</span></span>       | <span data-ttu-id="2cb11-114">字符串</span><span class="sxs-lookup"><span data-stu-id="2cb11-114">String</span></span>          | <span data-ttu-id="2cb11-115">共享项目的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2cb11-115">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="2cb11-116">id</span><span class="sxs-lookup"><span data-stu-id="2cb11-116">id</span></span>              | <span data-ttu-id="2cb11-117">字符串</span><span class="sxs-lookup"><span data-stu-id="2cb11-117">String</span></span>        | <span data-ttu-id="2cb11-118">共享项目的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="2cb11-118">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="2cb11-119">address</span><span class="sxs-lookup"><span data-stu-id="2cb11-119">address</span></span>             | <span data-ttu-id="2cb11-120">String</span><span class="sxs-lookup"><span data-stu-id="2cb11-120">String</span></span>      | <span data-ttu-id="2cb11-121">共享项目的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="2cb11-121">The email address of the user who shared the item.</span></span>  |
