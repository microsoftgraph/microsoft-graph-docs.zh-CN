---
title: 帐户资源类型
description: Dynamics 365 Business Central 中的 account 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4252c20e9d11f67a6de40871b1649a165cbd787c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507572"
---
# <a name="accounts-resource-type"></a><span data-ttu-id="68be5-103">帐户资源类型</span><span class="sxs-lookup"><span data-stu-id="68be5-103">accounts resource type</span></span>
<span data-ttu-id="68be5-104">表示 Dynamics 365 Business Central 中的 account 对象。</span><span class="sxs-lookup"><span data-stu-id="68be5-104">Represents an account object in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="68be5-105">方法</span><span class="sxs-lookup"><span data-stu-id="68be5-105">Methods</span></span>

| <span data-ttu-id="68be5-106">方法</span><span class="sxs-lookup"><span data-stu-id="68be5-106">Method</span></span>       | <span data-ttu-id="68be5-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="68be5-107">Return Type</span></span>  |<span data-ttu-id="68be5-108">说明</span><span class="sxs-lookup"><span data-stu-id="68be5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="68be5-109">获取帐户</span><span class="sxs-lookup"><span data-stu-id="68be5-109">Get accounts</span></span>](../api/dynamics-account-get.md)|<span data-ttu-id="68be5-110">accounts</span><span class="sxs-lookup"><span data-stu-id="68be5-110">accounts</span></span>|<span data-ttu-id="68be5-111">获取帐户对象。</span><span class="sxs-lookup"><span data-stu-id="68be5-111">Get accounts object.</span></span>|

## <a name="properties"></a><span data-ttu-id="68be5-112">属性</span><span class="sxs-lookup"><span data-stu-id="68be5-112">Properties</span></span>
| <span data-ttu-id="68be5-113">属性</span><span class="sxs-lookup"><span data-stu-id="68be5-113">Property</span></span>     | <span data-ttu-id="68be5-114">类型</span><span class="sxs-lookup"><span data-stu-id="68be5-114">Type</span></span>   |<span data-ttu-id="68be5-115">说明</span><span class="sxs-lookup"><span data-stu-id="68be5-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68be5-116">id</span><span class="sxs-lookup"><span data-stu-id="68be5-116">id</span></span>|<span data-ttu-id="68be5-117">GUID</span><span class="sxs-lookup"><span data-stu-id="68be5-117">GUID</span></span>|<span data-ttu-id="68be5-118">帐户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="68be5-118">The unique ID of the account.</span></span>|
|<span data-ttu-id="68be5-119">number</span><span class="sxs-lookup"><span data-stu-id="68be5-119">number</span></span>|<span data-ttu-id="68be5-120">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="68be5-120">string, maximum size 20</span></span>|<span data-ttu-id="68be5-121">指定 G/L 帐号的号码。</span><span class="sxs-lookup"><span data-stu-id="68be5-121">Specifies the number of the G/L account.</span></span>|
|<span data-ttu-id="68be5-122">displayName</span><span class="sxs-lookup"><span data-stu-id="68be5-122">displayName</span></span>|<span data-ttu-id="68be5-123">字符串, 最大大小为50</span><span class="sxs-lookup"><span data-stu-id="68be5-123">string, maximum size 50</span></span>|<span data-ttu-id="68be5-124">指定 G/L 帐户的名称。</span><span class="sxs-lookup"><span data-stu-id="68be5-124">Specifies the name of the G/L account.</span></span>|
|<span data-ttu-id="68be5-125">category</span><span class="sxs-lookup"><span data-stu-id="68be5-125">category</span></span>|<span data-ttu-id="68be5-126">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="68be5-126">string, maximum size 20</span></span>|<span data-ttu-id="68be5-127">指定 G/L 帐户的类别。</span><span class="sxs-lookup"><span data-stu-id="68be5-127">Specifies the category of the G/L account.</span></span>|
|<span data-ttu-id="68be5-128">子类别</span><span class="sxs-lookup"><span data-stu-id="68be5-128">subCategory</span></span>|<span data-ttu-id="68be5-129">字符串, 最大大小为80</span><span class="sxs-lookup"><span data-stu-id="68be5-129">string, maximum size 80</span></span>|<span data-ttu-id="68be5-130">指定 G/L 帐户的帐户类别的子类别。</span><span class="sxs-lookup"><span data-stu-id="68be5-130">Specifies the subcategory of the account category of the G/L account.</span></span>|
|<span data-ttu-id="68be5-131">堵塞</span><span class="sxs-lookup"><span data-stu-id="68be5-131">blocked</span></span>|<span data-ttu-id="68be5-132">布尔</span><span class="sxs-lookup"><span data-stu-id="68be5-132">boolean</span></span>|<span data-ttu-id="68be5-133">指定无法将条目投递到 G/L 帐户。</span><span class="sxs-lookup"><span data-stu-id="68be5-133">Specifies that entries cannot be posted to the G/L account.</span></span> <span data-ttu-id="68be5-134">**如果为 True** , 则表示帐户被阻止, 不允许进行发布。</span><span class="sxs-lookup"><span data-stu-id="68be5-134">**True** indicates account is blocked and posting is not allowed.</span></span>|
|<span data-ttu-id="68be5-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="68be5-135">lastModifiedDateTime</span></span>|<span data-ttu-id="68be5-136">datetime</span><span class="sxs-lookup"><span data-stu-id="68be5-136">datetime</span></span>|<span data-ttu-id="68be5-137">帐户修改后的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="68be5-137">The last datetime the account was modified.</span></span>|


## <a name="relationships"></a><span data-ttu-id="68be5-138">关系</span><span class="sxs-lookup"><span data-stu-id="68be5-138">Relationships</span></span>
<span data-ttu-id="68be5-139">无</span><span class="sxs-lookup"><span data-stu-id="68be5-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68be5-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68be5-140">JSON representation</span></span>

<span data-ttu-id="68be5-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68be5-141">Here is a JSON representation of the resource.</span></span>


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
