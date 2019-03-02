---
title: 公司资源类型
description: Dynamics 365 Business Central 中的公司。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: f1faca36af25bc8cb3e9019e0dc5b4460991e70d
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365680"
---
# <a name="companies-resource-type"></a><span data-ttu-id="1da44-103">公司资源类型</span><span class="sxs-lookup"><span data-stu-id="1da44-103">companies resource type</span></span>
<span data-ttu-id="1da44-104">代表 "Dynamics 365 Business Central 中的公司" 资源类型。</span><span class="sxs-lookup"><span data-stu-id="1da44-104">Represents a companies resource type in Dynamics 365 Business Central.</span></span> 

## <a name="methods"></a><span data-ttu-id="1da44-105">方法</span><span class="sxs-lookup"><span data-stu-id="1da44-105">Methods</span></span>

| <span data-ttu-id="1da44-106">方法</span><span class="sxs-lookup"><span data-stu-id="1da44-106">Method</span></span>         | <span data-ttu-id="1da44-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="1da44-107">Return Type</span></span>  |<span data-ttu-id="1da44-108">说明</span><span class="sxs-lookup"><span data-stu-id="1da44-108">Description</span></span>|
|:---------------|:-------------|:----------|
|[<span data-ttu-id="1da44-109">获取公司</span><span class="sxs-lookup"><span data-stu-id="1da44-109">Get companies</span></span>](../api/dynamics-companies-get.md)|<span data-ttu-id="1da44-110">保险公司</span><span class="sxs-lookup"><span data-stu-id="1da44-110">companies</span></span>|<span data-ttu-id="1da44-111">获取公司。</span><span class="sxs-lookup"><span data-stu-id="1da44-111">Get a company.</span></span>|

## <a name="properties"></a><span data-ttu-id="1da44-112">属性</span><span class="sxs-lookup"><span data-stu-id="1da44-112">Properties</span></span>
| <span data-ttu-id="1da44-113">属性</span><span class="sxs-lookup"><span data-stu-id="1da44-113">Property</span></span>        | <span data-ttu-id="1da44-114">类型</span><span class="sxs-lookup"><span data-stu-id="1da44-114">Type</span></span> |<span data-ttu-id="1da44-115">说明</span><span class="sxs-lookup"><span data-stu-id="1da44-115">Description</span></span>                             |
|:----------------|:-----|:---------------------------------------|
|<span data-ttu-id="1da44-116">id</span><span class="sxs-lookup"><span data-stu-id="1da44-116">id</span></span>               |<span data-ttu-id="1da44-117">GUID</span><span class="sxs-lookup"><span data-stu-id="1da44-117">GUID</span></span>  |<span data-ttu-id="1da44-118">公司的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="1da44-118">The unique ID of the company.</span></span> <span data-ttu-id="1da44-119">只读。</span><span class="sxs-lookup"><span data-stu-id="1da44-119">Read-Only.</span></span>|
|<span data-ttu-id="1da44-120">name</span><span class="sxs-lookup"><span data-stu-id="1da44-120">name</span></span>             |<span data-ttu-id="1da44-121">string</span><span class="sxs-lookup"><span data-stu-id="1da44-121">string</span></span>|<span data-ttu-id="1da44-122">指定公司。</span><span class="sxs-lookup"><span data-stu-id="1da44-122">Specifies the Company.</span></span>                  |
|<span data-ttu-id="1da44-123">displayName</span><span class="sxs-lookup"><span data-stu-id="1da44-123">displayName</span></span>      |<span data-ttu-id="1da44-124">string</span><span class="sxs-lookup"><span data-stu-id="1da44-124">string</span></span>|<span data-ttu-id="1da44-125">指定公司显示名称。</span><span class="sxs-lookup"><span data-stu-id="1da44-125">Specifies the company display name.</span></span>     |
|<span data-ttu-id="1da44-126">systemVersion</span><span class="sxs-lookup"><span data-stu-id="1da44-126">systemVersion</span></span>    |<span data-ttu-id="1da44-127">string</span><span class="sxs-lookup"><span data-stu-id="1da44-127">string</span></span>|<span data-ttu-id="1da44-128">指定公司的内部版本。</span><span class="sxs-lookup"><span data-stu-id="1da44-128">Specifies the internal version of the company.</span></span>|
|<span data-ttu-id="1da44-129">businessProfileId</span><span class="sxs-lookup"><span data-stu-id="1da44-129">businessProfileId</span></span>|<span data-ttu-id="1da44-130">string</span><span class="sxs-lookup"><span data-stu-id="1da44-130">string</span></span>|<span data-ttu-id="1da44-131">指定链接到公司的业务配置文件 ID。</span><span class="sxs-lookup"><span data-stu-id="1da44-131">Specifies the Business Profile ID linked to the company.</span></span>|


## <a name="relationships"></a><span data-ttu-id="1da44-132">关系</span><span class="sxs-lookup"><span data-stu-id="1da44-132">Relationships</span></span>
<span data-ttu-id="1da44-133">无</span><span class="sxs-lookup"><span data-stu-id="1da44-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1da44-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1da44-134">JSON representation</span></span>

<span data-ttu-id="1da44-135">下面是公司的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1da44-135">Here is a JSON representation of the company.</span></span>

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}

```


