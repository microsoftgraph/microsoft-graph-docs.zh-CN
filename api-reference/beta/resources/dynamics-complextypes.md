---
title: 复杂类型 JSON
description: JSON for Dynamics 365 Business Central 中的复杂数据类型。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: bb61450ab7f1d62d459f525f6341093f25b1686f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012637"
---
# <a name="complex-types-json"></a><span data-ttu-id="86d2c-103">复杂类型 JSON</span><span class="sxs-lookup"><span data-stu-id="86d2c-103">complex types JSON</span></span>
<span data-ttu-id="86d2c-104">这些是 Dynamics 365 Business Central 中的各种复杂类型。</span><span class="sxs-lookup"><span data-stu-id="86d2c-104">These are the various complex types in Dynamics 365 Business Central.</span></span> <span data-ttu-id="86d2c-105">您可以在使用这些复杂类型的各种不同方法中查看这些复杂类型的用法。</span><span class="sxs-lookup"><span data-stu-id="86d2c-105">You can see usage of these complex types in the various individual methods that make use of them.</span></span>

## <a name="postal-address"></a><span data-ttu-id="86d2c-106">邮政地址</span><span class="sxs-lookup"><span data-stu-id="86d2c-106">Postal address</span></span>

<span data-ttu-id="86d2c-107">代表 Dynamics 365 Business Central 中的邮政地址复杂类型。</span><span class="sxs-lookup"><span data-stu-id="86d2c-107">Represents a Postal Address complex type in Dynamics 365 Business Central.</span></span>

### <a name="properties"></a><span data-ttu-id="86d2c-108">属性</span><span class="sxs-lookup"><span data-stu-id="86d2c-108">Properties</span></span>
| <span data-ttu-id="86d2c-109">属性</span><span class="sxs-lookup"><span data-stu-id="86d2c-109">Property</span></span>     | <span data-ttu-id="86d2c-110">类型</span><span class="sxs-lookup"><span data-stu-id="86d2c-110">Type</span></span>       |<span data-ttu-id="86d2c-111">说明</span><span class="sxs-lookup"><span data-stu-id="86d2c-111">Description</span></span>             |
|:-------------|:---------|:-----------------------|
|<span data-ttu-id="86d2c-112">street</span><span class="sxs-lookup"><span data-stu-id="86d2c-112">street</span></span>        |<span data-ttu-id="86d2c-113">string</span><span class="sxs-lookup"><span data-stu-id="86d2c-113">string</span></span>    |<span data-ttu-id="86d2c-114">邮政地址街道。</span><span class="sxs-lookup"><span data-stu-id="86d2c-114">Postal address street.</span></span>  |
|<span data-ttu-id="86d2c-115">city</span><span class="sxs-lookup"><span data-stu-id="86d2c-115">city</span></span>          |<span data-ttu-id="86d2c-116">string</span><span class="sxs-lookup"><span data-stu-id="86d2c-116">string</span></span>    |<span data-ttu-id="86d2c-117">邮政地址 (城市)。</span><span class="sxs-lookup"><span data-stu-id="86d2c-117">Postal address city.</span></span>    |
|<span data-ttu-id="86d2c-118">state</span><span class="sxs-lookup"><span data-stu-id="86d2c-118">state</span></span>         |<span data-ttu-id="86d2c-119">string</span><span class="sxs-lookup"><span data-stu-id="86d2c-119">string</span></span>    |<span data-ttu-id="86d2c-120">邮政地址状态。</span><span class="sxs-lookup"><span data-stu-id="86d2c-120">Postal address state.</span></span>   |
|<span data-ttu-id="86d2c-121">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="86d2c-121">countryLetterCode</span></span>|<span data-ttu-id="86d2c-122">string</span><span class="sxs-lookup"><span data-stu-id="86d2c-122">string</span></span> |<span data-ttu-id="86d2c-123">通信地址国家/地区字母代码 (两个字符的单词)</span><span class="sxs-lookup"><span data-stu-id="86d2c-123">Postal address country letter code (two character word)</span></span>|
|<span data-ttu-id="86d2c-124">postalCode</span><span class="sxs-lookup"><span data-stu-id="86d2c-124">postalCode</span></span>    |<span data-ttu-id="86d2c-125">string</span><span class="sxs-lookup"><span data-stu-id="86d2c-125">string</span></span>    |<span data-ttu-id="86d2c-126">邮政地址发布代码</span><span class="sxs-lookup"><span data-stu-id="86d2c-126">Postal address post code</span></span>|

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

