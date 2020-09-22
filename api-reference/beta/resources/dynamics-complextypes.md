---
title: 复杂类型 JSON
description: JSON for Dynamics 365 Business Central 中的复杂数据类型。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 77d2f7c5c491bf6e86a6df1a05b4a1cdd7788187
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040058"
---
# <a name="complex-types-json"></a><span data-ttu-id="ff409-103">复杂类型 JSON</span><span class="sxs-lookup"><span data-stu-id="ff409-103">complex types JSON</span></span>

<span data-ttu-id="ff409-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff409-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff409-105">这些是 Dynamics 365 Business Central 中的各种复杂类型。</span><span class="sxs-lookup"><span data-stu-id="ff409-105">These are the various complex types in Dynamics 365 Business Central.</span></span> <span data-ttu-id="ff409-106">您可以在使用这些复杂类型的各种不同方法中查看这些复杂类型的用法。</span><span class="sxs-lookup"><span data-stu-id="ff409-106">You can see usage of these complex types in the various individual methods that make use of them.</span></span>

## <a name="postal-address"></a><span data-ttu-id="ff409-107">邮政地址</span><span class="sxs-lookup"><span data-stu-id="ff409-107">Postal address</span></span>

<span data-ttu-id="ff409-108">代表 Dynamics 365 Business Central 中的邮政地址复杂类型。</span><span class="sxs-lookup"><span data-stu-id="ff409-108">Represents a Postal Address complex type in Dynamics 365 Business Central.</span></span>

### <a name="properties"></a><span data-ttu-id="ff409-109">属性</span><span class="sxs-lookup"><span data-stu-id="ff409-109">Properties</span></span>
| <span data-ttu-id="ff409-110">属性</span><span class="sxs-lookup"><span data-stu-id="ff409-110">Property</span></span>     | <span data-ttu-id="ff409-111">类型</span><span class="sxs-lookup"><span data-stu-id="ff409-111">Type</span></span>       |<span data-ttu-id="ff409-112">说明</span><span class="sxs-lookup"><span data-stu-id="ff409-112">Description</span></span>             |
|:-------------|:---------|:-----------------------|
|<span data-ttu-id="ff409-113">street</span><span class="sxs-lookup"><span data-stu-id="ff409-113">street</span></span>        |<span data-ttu-id="ff409-114">string</span><span class="sxs-lookup"><span data-stu-id="ff409-114">string</span></span>    |<span data-ttu-id="ff409-115">邮政地址街道。</span><span class="sxs-lookup"><span data-stu-id="ff409-115">Postal address street.</span></span>  |
|<span data-ttu-id="ff409-116">城市</span><span class="sxs-lookup"><span data-stu-id="ff409-116">city</span></span>          |<span data-ttu-id="ff409-117">string</span><span class="sxs-lookup"><span data-stu-id="ff409-117">string</span></span>    |<span data-ttu-id="ff409-118">邮政地址（城市）。</span><span class="sxs-lookup"><span data-stu-id="ff409-118">Postal address city.</span></span>    |
|<span data-ttu-id="ff409-119">state</span><span class="sxs-lookup"><span data-stu-id="ff409-119">state</span></span>         |<span data-ttu-id="ff409-120">string</span><span class="sxs-lookup"><span data-stu-id="ff409-120">string</span></span>    |<span data-ttu-id="ff409-121">邮政地址状态。</span><span class="sxs-lookup"><span data-stu-id="ff409-121">Postal address state.</span></span>   |
|<span data-ttu-id="ff409-122">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="ff409-122">countryLetterCode</span></span>|<span data-ttu-id="ff409-123">string</span><span class="sxs-lookup"><span data-stu-id="ff409-123">string</span></span> |<span data-ttu-id="ff409-124">邮政地址国家/地区字母代码 (双字符单词) </span><span class="sxs-lookup"><span data-stu-id="ff409-124">Postal address country letter code (two character word)</span></span>|
|<span data-ttu-id="ff409-125">postalCode</span><span class="sxs-lookup"><span data-stu-id="ff409-125">postalCode</span></span>    |<span data-ttu-id="ff409-126">string</span><span class="sxs-lookup"><span data-stu-id="ff409-126">string</span></span>    |<span data-ttu-id="ff409-127">邮政地址发布代码</span><span class="sxs-lookup"><span data-stu-id="ff409-127">Postal address post code</span></span>|

```json
"PostalAddress" 
{ 
"street": "string",
"city": "string", 
"state": "string", 
"countryLetterCode": "string", 
"postalCode": "string" 
} 
 ```



