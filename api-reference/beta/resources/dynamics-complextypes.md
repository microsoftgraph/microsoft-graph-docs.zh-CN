---
title: 复杂类型 JSON
description: JSON for Dynamics 365 Business Central 中的复杂数据类型。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4fc4d4f53014f5b8c656cd069cadf7b19190e0f0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366765"
---
# <a name="complex-types-json"></a><span data-ttu-id="eecc3-103">复杂类型 JSON</span><span class="sxs-lookup"><span data-stu-id="eecc3-103">complex types JSON</span></span>
<span data-ttu-id="eecc3-104">这些是 Dynamics 365 Business Central 中的各种复杂类型。</span><span class="sxs-lookup"><span data-stu-id="eecc3-104">These are the various complex types in Dynamics 365 Business Central.</span></span> <span data-ttu-id="eecc3-105">您可以在使用这些复杂类型的各种不同方法中查看这些复杂类型的用法。</span><span class="sxs-lookup"><span data-stu-id="eecc3-105">You can see usage of these complex types in the various individual methods that make use of them.</span></span>

## <a name="postal-address"></a><span data-ttu-id="eecc3-106">邮政地址</span><span class="sxs-lookup"><span data-stu-id="eecc3-106">Postal address</span></span>

<span data-ttu-id="eecc3-107">代表 Dynamics 365 Business Central 中的邮政地址复杂类型。</span><span class="sxs-lookup"><span data-stu-id="eecc3-107">Represents a Postal Address complex type in Dynamics 365 Business Central.</span></span>

### <a name="properties"></a><span data-ttu-id="eecc3-108">属性</span><span class="sxs-lookup"><span data-stu-id="eecc3-108">Properties</span></span>
| <span data-ttu-id="eecc3-109">属性</span><span class="sxs-lookup"><span data-stu-id="eecc3-109">Property</span></span>     | <span data-ttu-id="eecc3-110">类型</span><span class="sxs-lookup"><span data-stu-id="eecc3-110">Type</span></span>       |<span data-ttu-id="eecc3-111">说明</span><span class="sxs-lookup"><span data-stu-id="eecc3-111">Description</span></span>             |
|:-------------|:---------|:-----------------------|
|<span data-ttu-id="eecc3-112">street</span><span class="sxs-lookup"><span data-stu-id="eecc3-112">street</span></span>        |<span data-ttu-id="eecc3-113">string</span><span class="sxs-lookup"><span data-stu-id="eecc3-113">string</span></span>    |<span data-ttu-id="eecc3-114">邮政地址街道。</span><span class="sxs-lookup"><span data-stu-id="eecc3-114">Postal address street.</span></span>  |
|<span data-ttu-id="eecc3-115">city</span><span class="sxs-lookup"><span data-stu-id="eecc3-115">city</span></span>          |<span data-ttu-id="eecc3-116">string</span><span class="sxs-lookup"><span data-stu-id="eecc3-116">string</span></span>    |<span data-ttu-id="eecc3-117">邮政地址 (城市)。</span><span class="sxs-lookup"><span data-stu-id="eecc3-117">Postal address city.</span></span>    |
|<span data-ttu-id="eecc3-118">state</span><span class="sxs-lookup"><span data-stu-id="eecc3-118">state</span></span>         |<span data-ttu-id="eecc3-119">string</span><span class="sxs-lookup"><span data-stu-id="eecc3-119">string</span></span>    |<span data-ttu-id="eecc3-120">邮政地址状态。</span><span class="sxs-lookup"><span data-stu-id="eecc3-120">Postal address state.</span></span>   |
|<span data-ttu-id="eecc3-121">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="eecc3-121">countryLetterCode</span></span>|<span data-ttu-id="eecc3-122">string</span><span class="sxs-lookup"><span data-stu-id="eecc3-122">string</span></span> |<span data-ttu-id="eecc3-123">通信地址国家/地区字母代码 (两个字符的单词)</span><span class="sxs-lookup"><span data-stu-id="eecc3-123">Postal address country letter code (two character word)</span></span>|
|<span data-ttu-id="eecc3-124">postalCode</span><span class="sxs-lookup"><span data-stu-id="eecc3-124">postalCode</span></span>    |<span data-ttu-id="eecc3-125">string</span><span class="sxs-lookup"><span data-stu-id="eecc3-125">string</span></span>    |<span data-ttu-id="eecc3-126">邮政地址发布代码</span><span class="sxs-lookup"><span data-stu-id="eecc3-126">Postal address post code</span></span>|

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

