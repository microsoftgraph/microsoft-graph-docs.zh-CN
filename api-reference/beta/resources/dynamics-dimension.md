---
title: 维度资源类型
description: Dynamics 365 Business Central 中的维度。
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 5bd5382ae020baaf726db53f9252c4d3498833ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973623"
---
# <a name="dimensions-resource-type"></a><span data-ttu-id="43e6c-103">维度资源类型</span><span class="sxs-lookup"><span data-stu-id="43e6c-103">Dimensions resource type</span></span>
<span data-ttu-id="43e6c-104">表示 Dynamics 365 Business Central 中的维度。</span><span class="sxs-lookup"><span data-stu-id="43e6c-104">Represents a dimension in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="43e6c-105">方法</span><span class="sxs-lookup"><span data-stu-id="43e6c-105">Methods</span></span>
| <span data-ttu-id="43e6c-106">方法</span><span class="sxs-lookup"><span data-stu-id="43e6c-106">Method</span></span>       | <span data-ttu-id="43e6c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="43e6c-107">Return Type</span></span>  |<span data-ttu-id="43e6c-108">说明</span><span class="sxs-lookup"><span data-stu-id="43e6c-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="43e6c-109">获取尺寸</span><span class="sxs-lookup"><span data-stu-id="43e6c-109">Get dimensions</span></span>](../api/dynamics-dimension-get.md)|<span data-ttu-id="43e6c-110">维度</span><span class="sxs-lookup"><span data-stu-id="43e6c-110">dimension</span></span>|<span data-ttu-id="43e6c-111">获取一个维。</span><span class="sxs-lookup"><span data-stu-id="43e6c-111">Gets a dimension.</span></span>|


## <a name="properties"></a><span data-ttu-id="43e6c-112">属性</span><span class="sxs-lookup"><span data-stu-id="43e6c-112">Properties</span></span>
| <span data-ttu-id="43e6c-113">属性</span><span class="sxs-lookup"><span data-stu-id="43e6c-113">Property</span></span>           | <span data-ttu-id="43e6c-114">类型</span><span class="sxs-lookup"><span data-stu-id="43e6c-114">Type</span></span>                  |<span data-ttu-id="43e6c-115">说明</span><span class="sxs-lookup"><span data-stu-id="43e6c-115">Description</span></span>               |
|:-------------------|:----------------------|:-------------------------|
|<span data-ttu-id="43e6c-116">id</span><span class="sxs-lookup"><span data-stu-id="43e6c-116">id</span></span>                  |<span data-ttu-id="43e6c-117">GUID</span><span class="sxs-lookup"><span data-stu-id="43e6c-117">GUID</span></span>                   |<span data-ttu-id="43e6c-118">项目的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="43e6c-118">The unique ID of the item.</span></span>|
|<span data-ttu-id="43e6c-119">code</span><span class="sxs-lookup"><span data-stu-id="43e6c-119">code</span></span>                |<span data-ttu-id="43e6c-120">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="43e6c-120">string, maximum size 20</span></span>|<span data-ttu-id="43e6c-121">维度代码。</span><span class="sxs-lookup"><span data-stu-id="43e6c-121">The dimension code.</span></span>       |
|<span data-ttu-id="43e6c-122">displayName</span><span class="sxs-lookup"><span data-stu-id="43e6c-122">displayName</span></span>         |<span data-ttu-id="43e6c-123">string</span><span class="sxs-lookup"><span data-stu-id="43e6c-123">string</span></span>                 |<span data-ttu-id="43e6c-124">指定维度的名称。</span><span class="sxs-lookup"><span data-stu-id="43e6c-124">Specifies the dimension's name.</span></span> <span data-ttu-id="43e6c-125">此名称将显示在使用该维度的位置。</span><span class="sxs-lookup"><span data-stu-id="43e6c-125">This name will appear where the dimension is used.</span></span>|
|<span data-ttu-id="43e6c-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43e6c-126">lastModifiedDateTime</span></span>|<span data-ttu-id="43e6c-127">datetime</span><span class="sxs-lookup"><span data-stu-id="43e6c-127">datetime</span></span>               |<span data-ttu-id="43e6c-128">修改了该维度的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="43e6c-128">The last datetime the dimension was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="43e6c-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43e6c-129">JSON representation</span></span>

<span data-ttu-id="43e6c-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43e6c-130">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```

