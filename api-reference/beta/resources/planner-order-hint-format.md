---
title: 使用规划器中的排序提示
description: '`)'
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: conceptualPageType
ms.openlocfilehash: c381f3507df9b979fd409add56975ac79db008a2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521833"
---
# <a name="using-order-hints-in-planner"></a><span data-ttu-id="868da-103">使用规划器中的排序提示</span><span class="sxs-lookup"><span data-stu-id="868da-103">Using order hints in Planner</span></span>

<span data-ttu-id="868da-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="868da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="868da-105">规划器中的对象可根据排序提示识别排序顺序。</span><span class="sxs-lookup"><span data-stu-id="868da-105">Objects in Planner identify their sort order by order hints.</span></span> <span data-ttu-id="868da-106">排序提示值均为字符串。</span><span class="sxs-lookup"><span data-stu-id="868da-106">The order hint values are strings.</span></span> <span data-ttu-id="868da-107">客户端可以根据其中的字符的序数值对字符串进行排序以识别项目的顺序。</span><span class="sxs-lookup"><span data-stu-id="868da-107">The clients can sort the strings based on ordinal value of characters in them to identify the order of items.</span></span> <span data-ttu-id="868da-108">从字符串开头比较字符，直到字符的序数值中出现差异，或一个字符串结束，在这种情况下，较短字符串将优先于较长字符串进行排序。</span><span class="sxs-lookup"><span data-stu-id="868da-108">The characters are compared from the beginning of the string, until a difference is encountered in the ordinal values of characters, or one string ends, in which case the shorter string would be sorted before the longer.</span></span> <span data-ttu-id="868da-109">此类值可包括序数 32（空格）和 126（`~`）之间的任何字符</span><span class="sxs-lookup"><span data-stu-id="868da-109">The values can contain any character between ordinals 32 (space) and 126 (`~`)</span></span>

<span data-ttu-id="868da-110">例如，带有排序提示 `a` 的项目（序数值 97）将置于另一个带有排序提示 `z` 的项目（序数值 122）之前。</span><span class="sxs-lookup"><span data-stu-id="868da-110">As an example, an item with order hint `a` (ordinal value 97) would be placed before another item with order hint `z` (ordinal value 122).</span></span> <span data-ttu-id="868da-111">带有排序提示 `abc` 的项目（序数值 97、98、99）将置于另一个带有排序提示 `abd` 的项目（序数值 97、98、100）之前。</span><span class="sxs-lookup"><span data-stu-id="868da-111">An item with order hint `abc` (ordinal values 97, 98, 99), would be placed before another item with order hint `abd` (ordinal values 97, 98, 100).</span></span> <span data-ttu-id="868da-112">由于所有现有的字符均相同，而 `a` 较短，带有排序提示 `a` 的项目将置于另一个带有排序提示 `ab` 的项目之前。</span><span class="sxs-lookup"><span data-stu-id="868da-112">An item with order hint `a` would be placed before another item with order hint `ab` since all existing characters are the same, and `a` is shorter.</span></span>

<span data-ttu-id="868da-113">由此服务计算所有排序提示值。</span><span class="sxs-lookup"><span data-stu-id="868da-113">The values for all order hints are calculated by the service.</span></span> <span data-ttu-id="868da-114">客户端可通过指定项目的排序提示为项目重新排序，而在两个项目之间移动此项目可通过将排序提示设为以下值实现：`<previous order hint> <next order hint>!`，其中，在所需的新位置前出现的项目的排序提示会替换 `<previous order hint>`，而在所需的新位置后出现的项目的排序提示会替换 `<next order hint>`。</span><span class="sxs-lookup"><span data-stu-id="868da-114">The client can reorder items by specifying the order hint for the item that got moved between two items with by setting the order hint to the following value: `<previous order hint> <next order hint>!`, where `<previous order hint>` is to be replaced by the order hint of the item that comes before the new desired location, and `<next order hint>` is to be replaced by the order hint of the item that comes after the new desired location.</span></span> <span data-ttu-id="868da-115">这些排序提示值之间有空格字符，整个值以 `!` 为后缀。</span><span class="sxs-lookup"><span data-stu-id="868da-115">There is a space character between these order hint values, and the entire value is suffixed with `!`.</span></span> <span data-ttu-id="868da-116">如果任何一项不存在，应使用空字符串代替。</span><span class="sxs-lookup"><span data-stu-id="868da-116">If either item isn't present, empty string should be used instead.</span></span> <span data-ttu-id="868da-117">此值由之前的计算构成，可以在客户端中使用，为像服务返回的排序提示这样的项目排序。</span><span class="sxs-lookup"><span data-stu-id="868da-117">This value can also be composed of previous calculations, and can be used in the client to sort items exactly like service returned order hints.</span></span> <span data-ttu-id="868da-118">一旦客户端在更新中发送这些值，服务将计算在所需位置排序的短型值。</span><span class="sxs-lookup"><span data-stu-id="868da-118">Once the client sends these values in an update, the service will calculate a short value that sorts in the desired location.</span></span>

> <span data-ttu-id="868da-119">**注意：** 在下面的示例中，实际的 order 提示值将括在单引号字符（`'`）中，以清楚起见，但这些值不是数据的一部分，并且不得发送到服务。</span><span class="sxs-lookup"><span data-stu-id="868da-119">**Note:** In the following examples, the actual order hint values are surrounded in single quote characters (`'`) for clarity, however these are not part of the data, and must not be sent to the service.</span></span>
 
<span data-ttu-id="868da-120">例如，请考虑以下按排序提示顺序排列的列表：</span><span class="sxs-lookup"><span data-stu-id="868da-120">As an example, consider the following list of sorted order hints:</span></span>

1. <span data-ttu-id="868da-121">第 1 项（排序提示：`'5637'`）</span><span class="sxs-lookup"><span data-stu-id="868da-121">Item 1 (Order Hint: `'5637'`)</span></span>
2. <span data-ttu-id="868da-122">第 2 项（排序提示：`'adhg'`）</span><span class="sxs-lookup"><span data-stu-id="868da-122">Item 2 (Order Hint: `'adhg'`)</span></span>

<span data-ttu-id="868da-123">将第 3 项放置在第 1 项之前，然后将第 4 项置于第 1 项和第 2 项之间，再将第 5 项置于第 2 项之后，即可在客户端上创建下列排序提示。</span><span class="sxs-lookup"><span data-stu-id="868da-123">Placing an Item 3 before Item 1, then placing item 4 between Item 1 and Item 2, and then placing item 5 after Item 2, would create the following order hints on the client.</span></span> 

1. <span data-ttu-id="868da-124">第 3 项（排序提示：`' 5637!'`）</span><span class="sxs-lookup"><span data-stu-id="868da-124">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="868da-125">第 1 项（排序提示：`'5637'`）</span><span class="sxs-lookup"><span data-stu-id="868da-125">Item 1 (Order Hint: `'5637'`)</span></span>
3. <span data-ttu-id="868da-126">第 4 项（排序提示：`'5637 adhg!'`）</span><span class="sxs-lookup"><span data-stu-id="868da-126">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="868da-127">第 2 项（排序提示：`'adhg'`）</span><span class="sxs-lookup"><span data-stu-id="868da-127">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="868da-128">第 5 项（排序提示：`'adhg !'`）</span><span class="sxs-lookup"><span data-stu-id="868da-128">Item 5 (Order Hint: `'adhg !'`)</span></span>

<span data-ttu-id="868da-129">然后，将第 1 项移动至列表末尾，会生成：</span><span class="sxs-lookup"><span data-stu-id="868da-129">Then, moving item 1 to the end of the list would generate:</span></span>

1. <span data-ttu-id="868da-130">第 3 项（排序提示：`' 5637!'`）</span><span class="sxs-lookup"><span data-stu-id="868da-130">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="868da-131">第 4 项（排序提示：`'5637 adhg!'`）</span><span class="sxs-lookup"><span data-stu-id="868da-131">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
3. <span data-ttu-id="868da-132">第 2 项（排序提示：`'adhg'`）</span><span class="sxs-lookup"><span data-stu-id="868da-132">Item 2 (Order Hint: `'adhg'`)</span></span>
4. <span data-ttu-id="868da-133">第 5 项（排序提示：`'adhg !'`）</span><span class="sxs-lookup"><span data-stu-id="868da-133">Item 5 (Order Hint: `'adhg !'`)</span></span>
5. <span data-ttu-id="868da-134">第 1 项（排序提示：`'adhg ! !'`）</span><span class="sxs-lookup"><span data-stu-id="868da-134">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="868da-135">最后将第 5 项移动至第 3 项和第 4 项之间，会生成：</span><span class="sxs-lookup"><span data-stu-id="868da-135">Finally moving Item 5 between Item 3 and Item 4 would generate:</span></span>

1. <span data-ttu-id="868da-136">第 3 项（排序提示：`' 5637!'`）</span><span class="sxs-lookup"><span data-stu-id="868da-136">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="868da-137">第 5 项（排序提示：`' 5637! 5637 adhg!!'`）</span><span class="sxs-lookup"><span data-stu-id="868da-137">Item 5 (Order Hint: `' 5637! 5637 adhg!!'`)</span></span>
3. <span data-ttu-id="868da-138">第 4 项（排序提示：`'5637 adhg!'`）</span><span class="sxs-lookup"><span data-stu-id="868da-138">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="868da-139">第 2 项（排序提示：`'adhg'`）</span><span class="sxs-lookup"><span data-stu-id="868da-139">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="868da-140">第 1 项（排序提示：`'adhg ! !'`）</span><span class="sxs-lookup"><span data-stu-id="868da-140">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="868da-141">如果将对 order 提示值所做的更改发送到 patch 请求中的服务，则该服务将计算保留客户端预期顺序的正确值。</span><span class="sxs-lookup"><span data-stu-id="868da-141">When these changes to order hint values are sent to the service in patch requests, the service will calculate proper values that keep the order intended by the client.</span></span> <span data-ttu-id="868da-142">如果在`Prefer: return=representation` `PATCH`请求中指定了首选项头，则客户端可以立即获取这些值。</span><span class="sxs-lookup"><span data-stu-id="868da-142">The client can obtain the values immediate if the `Prefer: return=representation` preference header is specified in the `PATCH` requests.</span></span> <span data-ttu-id="868da-143">适用于上述情况的值可能类似于以下内容（实际值可能有所不同）。</span><span class="sxs-lookup"><span data-stu-id="868da-143">The values for the case above may look like the following (the actual values may differ).</span></span> 

1. <span data-ttu-id="868da-144">第 3 项（排序提示：`'432b'`）</span><span class="sxs-lookup"><span data-stu-id="868da-144">Item 3 (Order Hint: `'432b'`)</span></span>
2. <span data-ttu-id="868da-145">第 5 项（排序提示：`'6F"#'`）</span><span class="sxs-lookup"><span data-stu-id="868da-145">Item 5 (Order Hint: `'6F"#'`)</span></span>
3. <span data-ttu-id="868da-146">第 4 项（排序提示：`'7A$6'`）</span><span class="sxs-lookup"><span data-stu-id="868da-146">Item 4 (Order Hint: `'7A$6'`)</span></span>
4. <span data-ttu-id="868da-147">第 2 项（排序提示：`'adhg'`）</span><span class="sxs-lookup"><span data-stu-id="868da-147">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="868da-148">第 1 项（排序提示：`'de5%'`）</span><span class="sxs-lookup"><span data-stu-id="868da-148">Item 1 (Order Hint: `'de5%'`)</span></span>

<span data-ttu-id="868da-149">排序提示可指定为在列表中创建为 `!` 的首个项目，因为在这种情况下，根本不存在上一个或下一个项目，然而，这不是必须的，因为如果未在创建项目期间指定值，服务会为项目上的所有排序提示值自动生成值。</span><span class="sxs-lookup"><span data-stu-id="868da-149">Order Hints can be specified for creating the first item in the list as `!`, since neither a previous or a next item exists in that case, however this is unnecessary, as the service will auto-generate values for all order hint values on items if they are not specified during creation of the item.</span></span> <span data-ttu-id="868da-150">以下示例表明将项目置于之前为空的列表中时，应使用排序提示。</span><span class="sxs-lookup"><span data-stu-id="868da-150">Following example illustrates the order hints should be used when placing items in a previously empty list.</span></span>
<span data-ttu-id="868da-151">添加第一项：</span><span class="sxs-lookup"><span data-stu-id="868da-151">Add the first item:</span></span>

1. <span data-ttu-id="868da-152">第 1 项（排序提示：`' !'`）</span><span class="sxs-lookup"><span data-stu-id="868da-152">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="868da-153">将第二项添加到顶部：</span><span class="sxs-lookup"><span data-stu-id="868da-153">Add the second item to top:</span></span>

1. <span data-ttu-id="868da-154">第 2 项（排序提示：`'  !!'`）</span><span class="sxs-lookup"><span data-stu-id="868da-154">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="868da-155">第 1 项（排序提示：`' !'`）</span><span class="sxs-lookup"><span data-stu-id="868da-155">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="868da-156">将第三项添加到底部：</span><span class="sxs-lookup"><span data-stu-id="868da-156">Add the third item to bottom:</span></span>

1. <span data-ttu-id="868da-157">第 2 项（排序提示：`'  !!'`）</span><span class="sxs-lookup"><span data-stu-id="868da-157">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="868da-158">第 1 项（排序提示：`' !'`）</span><span class="sxs-lookup"><span data-stu-id="868da-158">Item 1 (Order Hint: `' !'`)</span></span>
3. <span data-ttu-id="868da-159">第 3 项（排序提示：`' ! !'`）</span><span class="sxs-lookup"><span data-stu-id="868da-159">Item 3 (Order Hint: `' ! !'`)</span></span>







