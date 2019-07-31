---
title: dimensionValues 资源类型
description: Dynamics 365 Business Central 中的维度值。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: af7ba3b49051a4e89fcdf2a4a408a1f72fc547ad
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973613"
---
# <a name="dimensionvalues-resource-type"></a><span data-ttu-id="5fad1-103">dimensionValues 资源类型</span><span class="sxs-lookup"><span data-stu-id="5fad1-103">dimensionValues resource type</span></span>
<span data-ttu-id="5fad1-104">表示 Dynamics 365 Business Central 中的维度值。</span><span class="sxs-lookup"><span data-stu-id="5fad1-104">Represents a dimension value in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="5fad1-105">方法</span><span class="sxs-lookup"><span data-stu-id="5fad1-105">Methods</span></span>

| <span data-ttu-id="5fad1-106">方法</span><span class="sxs-lookup"><span data-stu-id="5fad1-106">Method</span></span>       | <span data-ttu-id="5fad1-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="5fad1-107">Return Type</span></span>  |<span data-ttu-id="5fad1-108">说明</span><span class="sxs-lookup"><span data-stu-id="5fad1-108">Description</span></span>                   |
|:-------------|:-------------|:-----------------------------|
|[<span data-ttu-id="5fad1-109">获取 dimensionValues</span><span class="sxs-lookup"><span data-stu-id="5fad1-109">Get dimensionValues</span></span>](../api/dynamics-dimensionvalue-get.md)|<span data-ttu-id="5fad1-110">dimensionValues</span><span class="sxs-lookup"><span data-stu-id="5fad1-110">dimensionValues</span></span>|<span data-ttu-id="5fad1-111">获取一个维度值对象。</span><span class="sxs-lookup"><span data-stu-id="5fad1-111">Gets a dimension value object.</span></span>|


## <a name="properties"></a><span data-ttu-id="5fad1-112">属性</span><span class="sxs-lookup"><span data-stu-id="5fad1-112">Properties</span></span>
| <span data-ttu-id="5fad1-113">属性</span><span class="sxs-lookup"><span data-stu-id="5fad1-113">Property</span></span>           | <span data-ttu-id="5fad1-114">类型</span><span class="sxs-lookup"><span data-stu-id="5fad1-114">Type</span></span>                  |<span data-ttu-id="5fad1-115">说明</span><span class="sxs-lookup"><span data-stu-id="5fad1-115">Description</span></span>                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|<span data-ttu-id="5fad1-116">id</span><span class="sxs-lookup"><span data-stu-id="5fad1-116">id</span></span>                  |<span data-ttu-id="5fad1-117">GUID</span><span class="sxs-lookup"><span data-stu-id="5fad1-117">GUID</span></span>                   |<span data-ttu-id="5fad1-118">项目的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="5fad1-118">The unique ID of the item.</span></span>                         |
|<span data-ttu-id="5fad1-119">code</span><span class="sxs-lookup"><span data-stu-id="5fad1-119">code</span></span>                |<span data-ttu-id="5fad1-120">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="5fad1-120">string, maximum size 20</span></span>|<span data-ttu-id="5fad1-121">维度值代码。</span><span class="sxs-lookup"><span data-stu-id="5fad1-121">The dimension value code.</span></span>                          |
|<span data-ttu-id="5fad1-122">displayName</span><span class="sxs-lookup"><span data-stu-id="5fad1-122">displayName</span></span>         |<span data-ttu-id="5fad1-123">string</span><span class="sxs-lookup"><span data-stu-id="5fad1-123">string</span></span>                 |<span data-ttu-id="5fad1-124">指定维度值的名称。</span><span class="sxs-lookup"><span data-stu-id="5fad1-124">Specifies the dimension value's name.</span></span> <span data-ttu-id="5fad1-125">此名称将显示在使用维度值的位置。</span><span class="sxs-lookup"><span data-stu-id="5fad1-125">This name will appear where the dimension value is used.</span></span>|
|<span data-ttu-id="5fad1-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5fad1-126">lastModifiedDateTime</span></span>|<span data-ttu-id="5fad1-127">datetime</span><span class="sxs-lookup"><span data-stu-id="5fad1-127">datetime</span></span>               |<span data-ttu-id="5fad1-128">修改了维度值的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5fad1-128">The last datetime the dimension value was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="5fad1-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5fad1-129">JSON representation</span></span>

<span data-ttu-id="5fad1-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5fad1-130">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```


