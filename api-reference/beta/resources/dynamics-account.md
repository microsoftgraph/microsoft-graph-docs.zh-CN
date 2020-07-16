---
title: 帐户资源类型
description: Dynamics 365 Business Central 中的 account 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 54cd9f43c5232778b5887f17974d4f556a1f3842
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142202"
---
# <a name="accounts-resource-type"></a><span data-ttu-id="90710-103">帐户资源类型</span><span class="sxs-lookup"><span data-stu-id="90710-103">accounts resource type</span></span>

<span data-ttu-id="90710-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90710-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90710-105">表示 Dynamics 365 Business Central 中的 account 对象。</span><span class="sxs-lookup"><span data-stu-id="90710-105">Represents an account object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="90710-106">方法</span><span class="sxs-lookup"><span data-stu-id="90710-106">Methods</span></span>

| <span data-ttu-id="90710-107">方法</span><span class="sxs-lookup"><span data-stu-id="90710-107">Method</span></span>       | <span data-ttu-id="90710-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="90710-108">Return Type</span></span>  |<span data-ttu-id="90710-109">说明</span><span class="sxs-lookup"><span data-stu-id="90710-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="90710-110">获取帐户</span><span class="sxs-lookup"><span data-stu-id="90710-110">Get accounts</span></span>](../api/dynamics-account-get.md)|<span data-ttu-id="90710-111">帐户</span><span class="sxs-lookup"><span data-stu-id="90710-111">accounts</span></span>|<span data-ttu-id="90710-112">获取帐户对象。</span><span class="sxs-lookup"><span data-stu-id="90710-112">Get accounts object.</span></span>|

## <a name="properties"></a><span data-ttu-id="90710-113">属性</span><span class="sxs-lookup"><span data-stu-id="90710-113">Properties</span></span>
| <span data-ttu-id="90710-114">属性</span><span class="sxs-lookup"><span data-stu-id="90710-114">Property</span></span>     | <span data-ttu-id="90710-115">类型</span><span class="sxs-lookup"><span data-stu-id="90710-115">Type</span></span>   |<span data-ttu-id="90710-116">说明</span><span class="sxs-lookup"><span data-stu-id="90710-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90710-117">id</span><span class="sxs-lookup"><span data-stu-id="90710-117">id</span></span>|<span data-ttu-id="90710-118">GUID</span><span class="sxs-lookup"><span data-stu-id="90710-118">GUID</span></span>|<span data-ttu-id="90710-119">帐户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="90710-119">The unique ID of the account.</span></span>|
|<span data-ttu-id="90710-120">数字</span><span class="sxs-lookup"><span data-stu-id="90710-120">number</span></span>|<span data-ttu-id="90710-121">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="90710-121">string, maximum size 20</span></span>|<span data-ttu-id="90710-122">指定 G/L 帐号的号码。</span><span class="sxs-lookup"><span data-stu-id="90710-122">Specifies the number of the G/L account.</span></span>|
|<span data-ttu-id="90710-123">displayName</span><span class="sxs-lookup"><span data-stu-id="90710-123">displayName</span></span>|<span data-ttu-id="90710-124">字符串，最大大小为50</span><span class="sxs-lookup"><span data-stu-id="90710-124">string, maximum size 50</span></span>|<span data-ttu-id="90710-125">指定 G/L 帐户的名称。</span><span class="sxs-lookup"><span data-stu-id="90710-125">Specifies the name of the G/L account.</span></span>|
|<span data-ttu-id="90710-126">“类别”</span><span class="sxs-lookup"><span data-stu-id="90710-126">category</span></span>|<span data-ttu-id="90710-127">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="90710-127">string, maximum size 20</span></span>|<span data-ttu-id="90710-128">指定 G/L 帐户的类别。</span><span class="sxs-lookup"><span data-stu-id="90710-128">Specifies the category of the G/L account.</span></span>|
|<span data-ttu-id="90710-129">子类别</span><span class="sxs-lookup"><span data-stu-id="90710-129">subCategory</span></span>|<span data-ttu-id="90710-130">字符串，最大大小为80</span><span class="sxs-lookup"><span data-stu-id="90710-130">string, maximum size 80</span></span>|<span data-ttu-id="90710-131">指定 G/L 帐户的帐户类别的子类别。</span><span class="sxs-lookup"><span data-stu-id="90710-131">Specifies the subcategory of the account category of the G/L account.</span></span>|
|<span data-ttu-id="90710-132">堵塞</span><span class="sxs-lookup"><span data-stu-id="90710-132">blocked</span></span>|<span data-ttu-id="90710-133">boolean</span><span class="sxs-lookup"><span data-stu-id="90710-133">boolean</span></span>|<span data-ttu-id="90710-134">指定无法将条目投递到 G/L 帐户。</span><span class="sxs-lookup"><span data-stu-id="90710-134">Specifies that entries cannot be posted to the G/L account.</span></span> <span data-ttu-id="90710-135">**如果为 True** ，则表示帐户被阻止，不允许进行发布。</span><span class="sxs-lookup"><span data-stu-id="90710-135">**True** indicates account is blocked and posting is not allowed.</span></span>|
|<span data-ttu-id="90710-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90710-136">lastModifiedDateTime</span></span>|<span data-ttu-id="90710-137">datetime</span><span class="sxs-lookup"><span data-stu-id="90710-137">datetime</span></span>|<span data-ttu-id="90710-138">帐户修改后的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="90710-138">The last datetime the account was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="90710-139">关系</span><span class="sxs-lookup"><span data-stu-id="90710-139">Relationships</span></span>
<span data-ttu-id="90710-140">无</span><span class="sxs-lookup"><span data-stu-id="90710-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90710-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90710-141">JSON representation</span></span>

<span data-ttu-id="90710-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90710-142">Here is a JSON representation of the resource.</span></span>


```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "category": "string",
  "subCategory": "string",
  "blocked": "boolean",
  "lastModifiedDateTime": "datetime"
}
```
