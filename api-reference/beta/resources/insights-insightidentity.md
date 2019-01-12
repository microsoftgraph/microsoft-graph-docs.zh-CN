---
title: insightIdentity
description: 包含共享项目的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: a263caa68280128a67a027b75682407fd4932605
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938935"
---
# <a name="insightidentity"></a><span data-ttu-id="aeb17-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="aeb17-103">insightIdentity</span></span>

> <span data-ttu-id="aeb17-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aeb17-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aeb17-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aeb17-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aeb17-106">包含[共享](insights-shared.md)项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="aeb17-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="aeb17-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aeb17-107">JSON representation</span></span>
<span data-ttu-id="aeb17-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aeb17-108">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="aeb17-109">属性</span><span class="sxs-lookup"><span data-stu-id="aeb17-109">Properties</span></span>

| <span data-ttu-id="aeb17-110">属性</span><span class="sxs-lookup"><span data-stu-id="aeb17-110">Property</span></span>              | <span data-ttu-id="aeb17-111">类型</span><span class="sxs-lookup"><span data-stu-id="aeb17-111">Type</span></span>          | <span data-ttu-id="aeb17-112">说明</span><span class="sxs-lookup"><span data-stu-id="aeb17-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="aeb17-113">displayName</span><span class="sxs-lookup"><span data-stu-id="aeb17-113">displayName</span></span>       | <span data-ttu-id="aeb17-114">字符串</span><span class="sxs-lookup"><span data-stu-id="aeb17-114">String</span></span>          | <span data-ttu-id="aeb17-115">共享项目的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="aeb17-115">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="aeb17-116">id</span><span class="sxs-lookup"><span data-stu-id="aeb17-116">id</span></span>              | <span data-ttu-id="aeb17-117">字符串</span><span class="sxs-lookup"><span data-stu-id="aeb17-117">String</span></span>        | <span data-ttu-id="aeb17-118">共享项目的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="aeb17-118">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="aeb17-119">address</span><span class="sxs-lookup"><span data-stu-id="aeb17-119">address</span></span>             | <span data-ttu-id="aeb17-120">String</span><span class="sxs-lookup"><span data-stu-id="aeb17-120">String</span></span>      | <span data-ttu-id="aeb17-121">共享项目的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="aeb17-121">The email address of the user who shared the item.</span></span>  |
