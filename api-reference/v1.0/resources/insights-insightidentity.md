---
title: insightIdentity
description: 包含共享项目的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: f4b8bc6b66598753c0755d249ab37283810e8db7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054866"
---
# <a name="insightidentity"></a><span data-ttu-id="74958-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="74958-103">insightIdentity</span></span>

<span data-ttu-id="74958-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74958-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74958-105">包含 [sharedInsight](insights-shared.md) 项目的属性的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="74958-105">Complex type containing properties of [sharedInsight](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="74958-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74958-106">JSON representation</span></span>
<span data-ttu-id="74958-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74958-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.insightIdentity"
}-->
```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="74958-108">属性</span><span class="sxs-lookup"><span data-stu-id="74958-108">Properties</span></span>

| <span data-ttu-id="74958-109">属性</span><span class="sxs-lookup"><span data-stu-id="74958-109">Property</span></span>              | <span data-ttu-id="74958-110">类型</span><span class="sxs-lookup"><span data-stu-id="74958-110">Type</span></span>          | <span data-ttu-id="74958-111">说明</span><span class="sxs-lookup"><span data-stu-id="74958-111">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="74958-112">displayName</span><span class="sxs-lookup"><span data-stu-id="74958-112">displayName</span></span>       | <span data-ttu-id="74958-113">String</span><span class="sxs-lookup"><span data-stu-id="74958-113">String</span></span>          | <span data-ttu-id="74958-114">共享项目的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="74958-114">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="74958-115">id</span><span class="sxs-lookup"><span data-stu-id="74958-115">id</span></span>              | <span data-ttu-id="74958-116">String</span><span class="sxs-lookup"><span data-stu-id="74958-116">String</span></span>        | <span data-ttu-id="74958-117">共享项的用户的 id。</span><span class="sxs-lookup"><span data-stu-id="74958-117">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="74958-118">address</span><span class="sxs-lookup"><span data-stu-id="74958-118">address</span></span>             | <span data-ttu-id="74958-119">String</span><span class="sxs-lookup"><span data-stu-id="74958-119">String</span></span>      | <span data-ttu-id="74958-120">共享项目的用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="74958-120">The email address of the user who shared the item.</span></span>  |

