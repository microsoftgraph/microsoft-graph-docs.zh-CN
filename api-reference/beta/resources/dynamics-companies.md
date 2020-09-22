---
title: 公司资源类型
description: Dynamics 365 Business Central 中的公司。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 3fedbd9407a4124c38a6ff08a95dbf4cd22c9fe1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081760"
---
# <a name="companies-resource-type"></a><span data-ttu-id="131a1-103">公司资源类型</span><span class="sxs-lookup"><span data-stu-id="131a1-103">companies resource type</span></span>

<span data-ttu-id="131a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="131a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="131a1-105">代表 "Dynamics 365 Business Central 中的公司" 资源类型。</span><span class="sxs-lookup"><span data-stu-id="131a1-105">Represents a companies resource type in Dynamics 365 Business Central.</span></span> 

## <a name="methods"></a><span data-ttu-id="131a1-106">方法</span><span class="sxs-lookup"><span data-stu-id="131a1-106">Methods</span></span>

| <span data-ttu-id="131a1-107">方法</span><span class="sxs-lookup"><span data-stu-id="131a1-107">Method</span></span>         | <span data-ttu-id="131a1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="131a1-108">Return Type</span></span>  |<span data-ttu-id="131a1-109">说明</span><span class="sxs-lookup"><span data-stu-id="131a1-109">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="131a1-110">获取公司</span><span class="sxs-lookup"><span data-stu-id="131a1-110">Get companies</span></span>](../api/dynamics-companies-get.md)|<span data-ttu-id="131a1-111">companies</span><span class="sxs-lookup"><span data-stu-id="131a1-111">companies</span></span>|<span data-ttu-id="131a1-112">获取公司。</span><span class="sxs-lookup"><span data-stu-id="131a1-112">Get a company.</span></span>|

## <a name="properties"></a><span data-ttu-id="131a1-113">属性</span><span class="sxs-lookup"><span data-stu-id="131a1-113">Properties</span></span>
| <span data-ttu-id="131a1-114">属性</span><span class="sxs-lookup"><span data-stu-id="131a1-114">Property</span></span>        | <span data-ttu-id="131a1-115">类型</span><span class="sxs-lookup"><span data-stu-id="131a1-115">Type</span></span> |<span data-ttu-id="131a1-116">说明</span><span class="sxs-lookup"><span data-stu-id="131a1-116">Description</span></span>                             |
|:----------------|:-----|:---------------------------------------|
|<span data-ttu-id="131a1-117">id</span><span class="sxs-lookup"><span data-stu-id="131a1-117">id</span></span>               |<span data-ttu-id="131a1-118">GUID</span><span class="sxs-lookup"><span data-stu-id="131a1-118">GUID</span></span>  |<span data-ttu-id="131a1-119">公司的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="131a1-119">The unique ID of the company.</span></span> <span data-ttu-id="131a1-120">只读。</span><span class="sxs-lookup"><span data-stu-id="131a1-120">Read-Only.</span></span>|
|<span data-ttu-id="131a1-121">name</span><span class="sxs-lookup"><span data-stu-id="131a1-121">name</span></span>             |<span data-ttu-id="131a1-122">string</span><span class="sxs-lookup"><span data-stu-id="131a1-122">string</span></span>|<span data-ttu-id="131a1-123">指定公司。</span><span class="sxs-lookup"><span data-stu-id="131a1-123">Specifies the Company.</span></span>                  |
|<span data-ttu-id="131a1-124">displayName</span><span class="sxs-lookup"><span data-stu-id="131a1-124">displayName</span></span>      |<span data-ttu-id="131a1-125">string</span><span class="sxs-lookup"><span data-stu-id="131a1-125">string</span></span>|<span data-ttu-id="131a1-126">指定公司显示名称。</span><span class="sxs-lookup"><span data-stu-id="131a1-126">Specifies the company display name.</span></span>     |
|<span data-ttu-id="131a1-127">systemVersion</span><span class="sxs-lookup"><span data-stu-id="131a1-127">systemVersion</span></span>    |<span data-ttu-id="131a1-128">string</span><span class="sxs-lookup"><span data-stu-id="131a1-128">string</span></span>|<span data-ttu-id="131a1-129">指定公司的内部版本。</span><span class="sxs-lookup"><span data-stu-id="131a1-129">Specifies the internal version of the company.</span></span>|
|<span data-ttu-id="131a1-130">businessProfileId</span><span class="sxs-lookup"><span data-stu-id="131a1-130">businessProfileId</span></span>|<span data-ttu-id="131a1-131">string</span><span class="sxs-lookup"><span data-stu-id="131a1-131">string</span></span>|<span data-ttu-id="131a1-132">指定链接到公司的业务配置文件 ID。</span><span class="sxs-lookup"><span data-stu-id="131a1-132">Specifies the Business Profile ID linked to the company.</span></span>|


## <a name="relationships"></a><span data-ttu-id="131a1-133">关系</span><span class="sxs-lookup"><span data-stu-id="131a1-133">Relationships</span></span>
<span data-ttu-id="131a1-134">无</span><span class="sxs-lookup"><span data-stu-id="131a1-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="131a1-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="131a1-135">JSON representation</span></span>

<span data-ttu-id="131a1-136">下面是公司的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="131a1-136">Here is a JSON representation of the company.</span></span>

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}

```




