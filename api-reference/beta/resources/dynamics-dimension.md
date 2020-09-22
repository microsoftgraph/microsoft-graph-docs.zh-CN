---
title: 维度资源类型
description: Dynamics 365 Business Central 中的维度。
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 61666cdaf87e095707e90345128b5ad2cda47426
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071353"
---
# <a name="dimensions-resource-type"></a><span data-ttu-id="b6a73-103">维度资源类型</span><span class="sxs-lookup"><span data-stu-id="b6a73-103">Dimensions resource type</span></span>

<span data-ttu-id="b6a73-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6a73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6a73-105">表示 Dynamics 365 Business Central 中的维度。</span><span class="sxs-lookup"><span data-stu-id="b6a73-105">Represents a dimension in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="b6a73-106">方法</span><span class="sxs-lookup"><span data-stu-id="b6a73-106">Methods</span></span>
| <span data-ttu-id="b6a73-107">方法</span><span class="sxs-lookup"><span data-stu-id="b6a73-107">Method</span></span>       | <span data-ttu-id="b6a73-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b6a73-108">Return Type</span></span>  |<span data-ttu-id="b6a73-109">说明</span><span class="sxs-lookup"><span data-stu-id="b6a73-109">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="b6a73-110">获取尺寸</span><span class="sxs-lookup"><span data-stu-id="b6a73-110">Get dimensions</span></span>](../api/dynamics-dimension-get.md)|<span data-ttu-id="b6a73-111">维度</span><span class="sxs-lookup"><span data-stu-id="b6a73-111">dimension</span></span>|<span data-ttu-id="b6a73-112">获取一个维。</span><span class="sxs-lookup"><span data-stu-id="b6a73-112">Gets a dimension.</span></span>|


## <a name="properties"></a><span data-ttu-id="b6a73-113">属性</span><span class="sxs-lookup"><span data-stu-id="b6a73-113">Properties</span></span>
| <span data-ttu-id="b6a73-114">属性</span><span class="sxs-lookup"><span data-stu-id="b6a73-114">Property</span></span>           | <span data-ttu-id="b6a73-115">类型</span><span class="sxs-lookup"><span data-stu-id="b6a73-115">Type</span></span>                  |<span data-ttu-id="b6a73-116">说明</span><span class="sxs-lookup"><span data-stu-id="b6a73-116">Description</span></span>               |
|:-------------------|:----------------------|:-------------------------|
|<span data-ttu-id="b6a73-117">id</span><span class="sxs-lookup"><span data-stu-id="b6a73-117">id</span></span>                  |<span data-ttu-id="b6a73-118">GUID</span><span class="sxs-lookup"><span data-stu-id="b6a73-118">GUID</span></span>                   |<span data-ttu-id="b6a73-119">项目的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="b6a73-119">The unique ID of the item.</span></span>|
|<span data-ttu-id="b6a73-120">code</span><span class="sxs-lookup"><span data-stu-id="b6a73-120">code</span></span>                |<span data-ttu-id="b6a73-121">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="b6a73-121">string, maximum size 20</span></span>|<span data-ttu-id="b6a73-122">维度代码。</span><span class="sxs-lookup"><span data-stu-id="b6a73-122">The dimension code.</span></span>       |
|<span data-ttu-id="b6a73-123">displayName</span><span class="sxs-lookup"><span data-stu-id="b6a73-123">displayName</span></span>         |<span data-ttu-id="b6a73-124">string</span><span class="sxs-lookup"><span data-stu-id="b6a73-124">string</span></span>                 |<span data-ttu-id="b6a73-125">指定维度的名称。</span><span class="sxs-lookup"><span data-stu-id="b6a73-125">Specifies the dimension's name.</span></span> <span data-ttu-id="b6a73-126">此名称将显示在使用该维度的位置。</span><span class="sxs-lookup"><span data-stu-id="b6a73-126">This name will appear where the dimension is used.</span></span>|
|<span data-ttu-id="b6a73-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6a73-127">lastModifiedDateTime</span></span>|<span data-ttu-id="b6a73-128">datetime</span><span class="sxs-lookup"><span data-stu-id="b6a73-128">datetime</span></span>               |<span data-ttu-id="b6a73-129">修改了该维度的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b6a73-129">The last datetime the dimension was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="b6a73-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6a73-130">JSON representation</span></span>

<span data-ttu-id="b6a73-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6a73-131">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```



