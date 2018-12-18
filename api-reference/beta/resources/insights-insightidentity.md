---
title: insightIdentity
description: 包含共享项目的属性的复杂类型。
author: simonhult
ms.openlocfilehash: 648242b827c0390029522955b0fe6347b98100c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331330"
---
# <a name="insightidentity"></a><span data-ttu-id="f6f95-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="f6f95-103">insightIdentity</span></span>

> <span data-ttu-id="f6f95-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f6f95-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6f95-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f6f95-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f6f95-106">包含[共享](insights-shared.md)项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="f6f95-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="f6f95-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6f95-107">JSON representation</span></span>
<span data-ttu-id="f6f95-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6f95-108">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="f6f95-109">属性</span><span class="sxs-lookup"><span data-stu-id="f6f95-109">Properties</span></span>

| <span data-ttu-id="f6f95-110">属性</span><span class="sxs-lookup"><span data-stu-id="f6f95-110">Property</span></span>              | <span data-ttu-id="f6f95-111">类型</span><span class="sxs-lookup"><span data-stu-id="f6f95-111">Type</span></span>          | <span data-ttu-id="f6f95-112">说明</span><span class="sxs-lookup"><span data-stu-id="f6f95-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="f6f95-113">displayName</span><span class="sxs-lookup"><span data-stu-id="f6f95-113">displayName</span></span>       | <span data-ttu-id="f6f95-114">字符串</span><span class="sxs-lookup"><span data-stu-id="f6f95-114">String</span></span>          | <span data-ttu-id="f6f95-115">共享项目的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f6f95-115">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="f6f95-116">id</span><span class="sxs-lookup"><span data-stu-id="f6f95-116">id</span></span>              | <span data-ttu-id="f6f95-117">字符串</span><span class="sxs-lookup"><span data-stu-id="f6f95-117">String</span></span>        | <span data-ttu-id="f6f95-118">共享项目的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="f6f95-118">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="f6f95-119">address</span><span class="sxs-lookup"><span data-stu-id="f6f95-119">address</span></span>             | <span data-ttu-id="f6f95-120">String</span><span class="sxs-lookup"><span data-stu-id="f6f95-120">String</span></span>      | <span data-ttu-id="f6f95-121">共享项目的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="f6f95-121">The email address of the user who shared the item.</span></span>  |