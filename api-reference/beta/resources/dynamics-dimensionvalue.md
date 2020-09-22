---
title: dimensionValues 资源类型
description: Dynamics 365 Business Central 中的维度值。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: acb1c8d34f8ee876c39ac99d5f43feb7f9a128c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071344"
---
# <a name="dimensionvalues-resource-type"></a><span data-ttu-id="8769f-103">dimensionValues 资源类型</span><span class="sxs-lookup"><span data-stu-id="8769f-103">dimensionValues resource type</span></span>

<span data-ttu-id="8769f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8769f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8769f-105">表示 Dynamics 365 Business Central 中的维度值。</span><span class="sxs-lookup"><span data-stu-id="8769f-105">Represents a dimension value in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="8769f-106">方法</span><span class="sxs-lookup"><span data-stu-id="8769f-106">Methods</span></span>

| <span data-ttu-id="8769f-107">方法</span><span class="sxs-lookup"><span data-stu-id="8769f-107">Method</span></span>       | <span data-ttu-id="8769f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8769f-108">Return Type</span></span>  |<span data-ttu-id="8769f-109">说明</span><span class="sxs-lookup"><span data-stu-id="8769f-109">Description</span></span>                   |
|:-------------|:-------------|:-----------------------------|
|[<span data-ttu-id="8769f-110">获取 dimensionValues</span><span class="sxs-lookup"><span data-stu-id="8769f-110">Get dimensionValues</span></span>](../api/dynamics-dimensionvalue-get.md)|<span data-ttu-id="8769f-111">dimensionValues</span><span class="sxs-lookup"><span data-stu-id="8769f-111">dimensionValues</span></span>|<span data-ttu-id="8769f-112">获取一个维度值对象。</span><span class="sxs-lookup"><span data-stu-id="8769f-112">Gets a dimension value object.</span></span>|


## <a name="properties"></a><span data-ttu-id="8769f-113">属性</span><span class="sxs-lookup"><span data-stu-id="8769f-113">Properties</span></span>
| <span data-ttu-id="8769f-114">属性</span><span class="sxs-lookup"><span data-stu-id="8769f-114">Property</span></span>           | <span data-ttu-id="8769f-115">类型</span><span class="sxs-lookup"><span data-stu-id="8769f-115">Type</span></span>                  |<span data-ttu-id="8769f-116">说明</span><span class="sxs-lookup"><span data-stu-id="8769f-116">Description</span></span>                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|<span data-ttu-id="8769f-117">id</span><span class="sxs-lookup"><span data-stu-id="8769f-117">id</span></span>                  |<span data-ttu-id="8769f-118">GUID</span><span class="sxs-lookup"><span data-stu-id="8769f-118">GUID</span></span>                   |<span data-ttu-id="8769f-119">项目的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="8769f-119">The unique ID of the item.</span></span>                         |
|<span data-ttu-id="8769f-120">code</span><span class="sxs-lookup"><span data-stu-id="8769f-120">code</span></span>                |<span data-ttu-id="8769f-121">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="8769f-121">string, maximum size 20</span></span>|<span data-ttu-id="8769f-122">维度值代码。</span><span class="sxs-lookup"><span data-stu-id="8769f-122">The dimension value code.</span></span>                          |
|<span data-ttu-id="8769f-123">displayName</span><span class="sxs-lookup"><span data-stu-id="8769f-123">displayName</span></span>         |<span data-ttu-id="8769f-124">string</span><span class="sxs-lookup"><span data-stu-id="8769f-124">string</span></span>                 |<span data-ttu-id="8769f-125">指定维度值的名称。</span><span class="sxs-lookup"><span data-stu-id="8769f-125">Specifies the dimension value's name.</span></span> <span data-ttu-id="8769f-126">此名称将显示在使用维度值的位置。</span><span class="sxs-lookup"><span data-stu-id="8769f-126">This name will appear where the dimension value is used.</span></span>|
|<span data-ttu-id="8769f-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8769f-127">lastModifiedDateTime</span></span>|<span data-ttu-id="8769f-128">datetime</span><span class="sxs-lookup"><span data-stu-id="8769f-128">datetime</span></span>               |<span data-ttu-id="8769f-129">修改了维度值的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8769f-129">The last datetime the dimension value was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="8769f-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8769f-130">JSON representation</span></span>

<span data-ttu-id="8769f-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8769f-131">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```




