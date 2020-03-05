---
title: dimensionValues 资源类型
description: Dynamics 365 Business Central 中的维度值。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 368fc28f7bd46d8d5385b6e6041cd82255e0271f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504137"
---
# <a name="dimensionvalues-resource-type"></a><span data-ttu-id="1c200-103">dimensionValues 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c200-103">dimensionValues resource type</span></span>

<span data-ttu-id="1c200-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1c200-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c200-105">表示 Dynamics 365 Business Central 中的维度值。</span><span class="sxs-lookup"><span data-stu-id="1c200-105">Represents a dimension value in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="1c200-106">方法</span><span class="sxs-lookup"><span data-stu-id="1c200-106">Methods</span></span>

| <span data-ttu-id="1c200-107">方法</span><span class="sxs-lookup"><span data-stu-id="1c200-107">Method</span></span>       | <span data-ttu-id="1c200-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1c200-108">Return Type</span></span>  |<span data-ttu-id="1c200-109">说明</span><span class="sxs-lookup"><span data-stu-id="1c200-109">Description</span></span>                   |
|:-------------|:-------------|:-----------------------------|
|[<span data-ttu-id="1c200-110">获取 dimensionValues</span><span class="sxs-lookup"><span data-stu-id="1c200-110">Get dimensionValues</span></span>](../api/dynamics-dimensionvalue-get.md)|<span data-ttu-id="1c200-111">dimensionValues</span><span class="sxs-lookup"><span data-stu-id="1c200-111">dimensionValues</span></span>|<span data-ttu-id="1c200-112">获取一个维度值对象。</span><span class="sxs-lookup"><span data-stu-id="1c200-112">Gets a dimension value object.</span></span>|


## <a name="properties"></a><span data-ttu-id="1c200-113">属性</span><span class="sxs-lookup"><span data-stu-id="1c200-113">Properties</span></span>
| <span data-ttu-id="1c200-114">属性</span><span class="sxs-lookup"><span data-stu-id="1c200-114">Property</span></span>           | <span data-ttu-id="1c200-115">类型</span><span class="sxs-lookup"><span data-stu-id="1c200-115">Type</span></span>                  |<span data-ttu-id="1c200-116">说明</span><span class="sxs-lookup"><span data-stu-id="1c200-116">Description</span></span>                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|<span data-ttu-id="1c200-117">id</span><span class="sxs-lookup"><span data-stu-id="1c200-117">id</span></span>                  |<span data-ttu-id="1c200-118">GUID</span><span class="sxs-lookup"><span data-stu-id="1c200-118">GUID</span></span>                   |<span data-ttu-id="1c200-119">项目的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="1c200-119">The unique ID of the item.</span></span>                         |
|<span data-ttu-id="1c200-120">code</span><span class="sxs-lookup"><span data-stu-id="1c200-120">code</span></span>                |<span data-ttu-id="1c200-121">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="1c200-121">string, maximum size 20</span></span>|<span data-ttu-id="1c200-122">维度值代码。</span><span class="sxs-lookup"><span data-stu-id="1c200-122">The dimension value code.</span></span>                          |
|<span data-ttu-id="1c200-123">displayName</span><span class="sxs-lookup"><span data-stu-id="1c200-123">displayName</span></span>         |<span data-ttu-id="1c200-124">string</span><span class="sxs-lookup"><span data-stu-id="1c200-124">string</span></span>                 |<span data-ttu-id="1c200-125">指定维度值的名称。</span><span class="sxs-lookup"><span data-stu-id="1c200-125">Specifies the dimension value's name.</span></span> <span data-ttu-id="1c200-126">此名称将显示在使用维度值的位置。</span><span class="sxs-lookup"><span data-stu-id="1c200-126">This name will appear where the dimension value is used.</span></span>|
|<span data-ttu-id="1c200-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c200-127">lastModifiedDateTime</span></span>|<span data-ttu-id="1c200-128">datetime</span><span class="sxs-lookup"><span data-stu-id="1c200-128">datetime</span></span>               |<span data-ttu-id="1c200-129">修改了维度值的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1c200-129">The last datetime the dimension value was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="1c200-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c200-130">JSON representation</span></span>

<span data-ttu-id="1c200-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c200-131">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```


