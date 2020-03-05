---
title: companyDetail 资源类型
description: companyDetail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: dc8da38c9da8d6631e8e46199f420ae0b3ab652e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507581"
---
# <a name="companydetail-resource-type"></a><span data-ttu-id="986f7-103">companyDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="986f7-103">companyDetail resource type</span></span>

<span data-ttu-id="986f7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="986f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="986f7-105">表示有关与其[配置文件](profile.md)中的实体相关的公司的信息。</span><span class="sxs-lookup"><span data-stu-id="986f7-105">Represents information about companies related to entities within their [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="986f7-106">属性</span><span class="sxs-lookup"><span data-stu-id="986f7-106">Properties</span></span>

| <span data-ttu-id="986f7-107">属性</span><span class="sxs-lookup"><span data-stu-id="986f7-107">Property</span></span>       | <span data-ttu-id="986f7-108">类型</span><span class="sxs-lookup"><span data-stu-id="986f7-108">Type</span></span>                                | <span data-ttu-id="986f7-109">说明</span><span class="sxs-lookup"><span data-stu-id="986f7-109">Description</span></span>                                 |
|:---------------|:------------------------------------|:--------------------------------------------|
|<span data-ttu-id="986f7-110">address</span><span class="sxs-lookup"><span data-stu-id="986f7-110">address</span></span>         |[<span data-ttu-id="986f7-111">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="986f7-111">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="986f7-112">公司的地址。</span><span class="sxs-lookup"><span data-stu-id="986f7-112">Address of the company.</span></span>                     |
|<span data-ttu-id="986f7-113">department</span><span class="sxs-lookup"><span data-stu-id="986f7-113">department</span></span>      |<span data-ttu-id="986f7-114">String</span><span class="sxs-lookup"><span data-stu-id="986f7-114">String</span></span>                               | <span data-ttu-id="986f7-115">公司内的部门名称。</span><span class="sxs-lookup"><span data-stu-id="986f7-115">Department Name within a company.</span></span>           |
|<span data-ttu-id="986f7-116">displayName</span><span class="sxs-lookup"><span data-stu-id="986f7-116">displayName</span></span>     |<span data-ttu-id="986f7-117">String</span><span class="sxs-lookup"><span data-stu-id="986f7-117">String</span></span>                               | <span data-ttu-id="986f7-118">公司名称。</span><span class="sxs-lookup"><span data-stu-id="986f7-118">Company name.</span></span>                               |
|<span data-ttu-id="986f7-119">officeLocation</span><span class="sxs-lookup"><span data-stu-id="986f7-119">officeLocation</span></span>  |<span data-ttu-id="986f7-120">String</span><span class="sxs-lookup"><span data-stu-id="986f7-120">String</span></span>                               | <span data-ttu-id="986f7-121">所引用人员的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="986f7-121">Office Location of the person referred to.</span></span>  |
|<span data-ttu-id="986f7-122">拼音</span><span class="sxs-lookup"><span data-stu-id="986f7-122">pronunciation</span></span>   |<span data-ttu-id="986f7-123">String</span><span class="sxs-lookup"><span data-stu-id="986f7-123">String</span></span>                               | <span data-ttu-id="986f7-124">公司名称的发音指南。</span><span class="sxs-lookup"><span data-stu-id="986f7-124">Pronunciation guide for the company name.</span></span>   |
|<span data-ttu-id="986f7-125">webUrl</span><span class="sxs-lookup"><span data-stu-id="986f7-125">webUrl</span></span>          |<span data-ttu-id="986f7-126">String</span><span class="sxs-lookup"><span data-stu-id="986f7-126">String</span></span>                               | <span data-ttu-id="986f7-127">链接到公司主页。</span><span class="sxs-lookup"><span data-stu-id="986f7-127">Link to the company home page.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="986f7-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="986f7-128">JSON representation</span></span>

<span data-ttu-id="986f7-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="986f7-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.companyDetail",
  "baseType": null
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "department": "String",
  "displayName": "String",
  "officeLocation": "String",
  "pronunciation": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "companyDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->