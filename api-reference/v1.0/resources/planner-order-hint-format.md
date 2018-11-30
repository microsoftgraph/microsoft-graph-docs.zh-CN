---
title: 使用规划器中的排序提示
description: '`)'
ms.openlocfilehash: eaacbcad509fd778990f7f73834897ff6cf79e15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010934"
---
# <a name="using-order-hints-in-planner"></a><span data-ttu-id="11796-103">使用规划器中的排序提示</span><span class="sxs-lookup"><span data-stu-id="11796-103">Using order hints in Planner</span></span>

<span data-ttu-id="11796-p101">规划器中的对象可根据排序提示识别排序顺序。排序提示值均为字符串。客户端可以根据其中的字符的序数值对字符串进行排序以识别项目的顺序。从字符串开头比较字符，直到字符的序数值中出现差异，或一个字符串结束，在这种情况下，较短字符串将优先于较长字符串进行排序。此类值可包括序数 32（空格）和 126（`~`）之间的任何字符</span><span class="sxs-lookup"><span data-stu-id="11796-p101">Objects in Planner identify their sort order by order hints. The order hint values are strings. The clients can sort the strings based on ordinal value of characters in them to identify the order of items. The characters are compared from the beginning of the string, until a difference is encountered in the ordinal values of characters, or one string ends, in which case the shorter string would be sorted before the longer. The values can contain any character between ordinals 32 (space) and 126 (`~`)</span></span>

<span data-ttu-id="11796-p102">例如，带有排序提示 `a` 的项目（序数值 97）将置于另一个带有排序提示 `z` 的项目（序数值 122）之前。带有排序提示 `abc` 的项目（序数值 97、98、99）将置于另一个带有排序提示 `abd` 的项目（序数值 97、98、100）之前。由于现有的所有字符均相同，而 `a` 较短，带有排序提示 `a` 的项目将置于另一个带有排序提示 `ab` 的项目之前。</span><span class="sxs-lookup"><span data-stu-id="11796-p102">As an example, an item with order hint `a` (ordinal value 97) would be placed before another item with order hint `z` (ordinal value 122). An item with order hint `abc` (ordinal values 97, 98, 99), would be placed before another item with order hint `abd` (ordinal values 97, 98, 100). An item with order hint `a` would be placed before another item with order hint `ab` since all existing characters are the same, and `a` is shorter.</span></span>

<span data-ttu-id="11796-p103">由此服务计算所有排序提示值。客户端可通过指定项目的排序提示为项目重新排序，而在两个项目之间移动此项目可通过将排序提示设为以下值实现：`<previous order hint> <next order hint>!`，其中，在所需的新位置前出现的项目的排序提示会替换 `<previous order hint>`，而在所需的新位置后出现的项目的排序提示会替换 `<next order hint>`。这些排序提示值之间有空格字符，整个值以 `!` 为后缀。如果任何一项不存在，应使用空字符串代替。此值由之前的计算构成，可以在客户端中使用，为像服务返回的排序提示这样的项目排序。一旦客户端在更新中发送这些值，服务将计算在所需位置排序的短型值。</span><span class="sxs-lookup"><span data-stu-id="11796-p103">The values for all order hints are calculated by the service. The client can reorder items by specifying the order hint for the item that got moved between two items with by setting the order hint to the following value: `<previous order hint> <next order hint>!`, where `<previous order hint>` is to be replaced by the order hint of the item that comes before the new desired location, and `<next order hint>` is to be replaced by the order hint of the item that comes after the new desired location. There is a space character between these order hint values, and the entire value is suffixed with `!`. If either item isn't present, empty string should be used instead. This value can also be composed of previous calculations, and can be used in the client to sort items exactly like service returned order hints. Once the client sends these values in an update, the service will calculate a short value that sorts in the desired location.</span></span>

<span data-ttu-id="11796-118">**请注意**，为了清楚起见，在下列示例中，实际的排序提示值用单引号字符 (`'`) 括起，但这些字符不属于数据，不可发送到服务。</span><span class="sxs-lookup"><span data-stu-id="11796-118">**Please note** that in the following examples the actual order hint values are surrounded in single quote characters (`'`) for clarity, however these are not part of the data, and must not be sent to the service.</span></span>
 
<span data-ttu-id="11796-119">例如，请考虑以下按排序提示顺序排列的列表：</span><span class="sxs-lookup"><span data-stu-id="11796-119">As an example, consider the following list of sorted order hints:</span></span>

1. <span data-ttu-id="11796-120">第 1 项（排序提示：`'5637'`）</span><span class="sxs-lookup"><span data-stu-id="11796-120">Item 1 (Order Hint: `'5637'`)</span></span>
2. <span data-ttu-id="11796-121">第 2 项（排序提示：`'adhg'`）</span><span class="sxs-lookup"><span data-stu-id="11796-121">Item 2 (Order Hint: `'adhg'`)</span></span>

<span data-ttu-id="11796-122">将第 3 项放置在第 1 项之前，然后将第 4 项置于第 1 项和第 2 项之间，再将第 5 项置于第 2 项之后，即可在客户端上创建下列排序提示。</span><span class="sxs-lookup"><span data-stu-id="11796-122">Placing an Item 3 before Item 1, then placing item 4 between Item 1 and Item 2, and then placing item 5 after Item 2, would create the following order hints on the client.</span></span> 

1. <span data-ttu-id="11796-123">第 3 项（排序提示：`' 5637!'`）</span><span class="sxs-lookup"><span data-stu-id="11796-123">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="11796-124">第 1 项（排序提示：`'5637'`）</span><span class="sxs-lookup"><span data-stu-id="11796-124">Item 1 (Order Hint: `'5637'`)</span></span>
3. <span data-ttu-id="11796-125">第 4 项（排序提示：`'5637 adhg!'`）</span><span class="sxs-lookup"><span data-stu-id="11796-125">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="11796-126">第 2 项（排序提示：`'adhg'`）</span><span class="sxs-lookup"><span data-stu-id="11796-126">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="11796-127">第 5 项（排序提示：`'adhg !'`）</span><span class="sxs-lookup"><span data-stu-id="11796-127">Item 5 (Order Hint: `'adhg !'`)</span></span>

<span data-ttu-id="11796-128">然后，将第 1 项移动至列表末尾，会生成：</span><span class="sxs-lookup"><span data-stu-id="11796-128">Then, moving item 1 to the end of the list would generate:</span></span>

1. <span data-ttu-id="11796-129">第 3 项（排序提示：`' 5637!'`）</span><span class="sxs-lookup"><span data-stu-id="11796-129">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="11796-130">第 4 项（排序提示：`'5637 adhg!'`）</span><span class="sxs-lookup"><span data-stu-id="11796-130">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
3. <span data-ttu-id="11796-131">第 2 项（排序提示：`'adhg'`）</span><span class="sxs-lookup"><span data-stu-id="11796-131">Item 2 (Order Hint: `'adhg'`)</span></span>
4. <span data-ttu-id="11796-132">第 5 项（排序提示：`'adhg !'`）</span><span class="sxs-lookup"><span data-stu-id="11796-132">Item 5 (Order Hint: `'adhg !'`)</span></span>
5. <span data-ttu-id="11796-133">第 1 项（排序提示：`'adhg ! !'`）</span><span class="sxs-lookup"><span data-stu-id="11796-133">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="11796-134">最后将第 5 项移动至第 3 项和第 4 项之间，会生成：</span><span class="sxs-lookup"><span data-stu-id="11796-134">Finally moving Item 5 between Item 3 and Item 4 would generate:</span></span>

1. <span data-ttu-id="11796-135">第 3 项（排序提示：`' 5637!'`）</span><span class="sxs-lookup"><span data-stu-id="11796-135">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="11796-136">第 5 项（排序提示：`' 5637! 5637 adhg!!'`）</span><span class="sxs-lookup"><span data-stu-id="11796-136">Item 5 (Order Hint: `' 5637! 5637 adhg!!'`)</span></span>
3. <span data-ttu-id="11796-137">第 4 项（排序提示：`'5637 adhg!'`）</span><span class="sxs-lookup"><span data-stu-id="11796-137">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="11796-138">第 2 项（排序提示：`'adhg'`）</span><span class="sxs-lookup"><span data-stu-id="11796-138">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="11796-139">第 1 项（排序提示：`'adhg ! !'`）</span><span class="sxs-lookup"><span data-stu-id="11796-139">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="11796-p104">一旦将这些排序提示值更改发送到修补程序请求，此服务将计算相应的值，这些值可以保持客户端安排的顺序。如果在 `PATCH` 请求中指定 `return=representation` 首选项，客户端可立即获取此类值。适用于上述情况的值可能类似于以下内容（实际值可能有所不同）。</span><span class="sxs-lookup"><span data-stu-id="11796-p104">Once these changes to order hint values are sent to the service in patch requests, the service will calculate proper values that keep the order intended by the client. The client can obtain the values immediate if `return=representation` preference is specified in the `PATCH` requests. The values for the case above may look like the following (the actual values may differ).</span></span> 

1. <span data-ttu-id="11796-143">第 3 项（排序提示：`'432b'`）</span><span class="sxs-lookup"><span data-stu-id="11796-143">Item 3 (Order Hint: `'432b'`)</span></span>
2. <span data-ttu-id="11796-144">第 5 项（排序提示：`'6F"#'`）</span><span class="sxs-lookup"><span data-stu-id="11796-144">Item 5 (Order Hint: `'6F"#'`)</span></span>
3. <span data-ttu-id="11796-145">第 4 项（排序提示：`'7A$6'`）</span><span class="sxs-lookup"><span data-stu-id="11796-145">Item 4 (Order Hint: `'7A$6'`)</span></span>
4. <span data-ttu-id="11796-146">第 2 项（排序提示：`'adhg'`）</span><span class="sxs-lookup"><span data-stu-id="11796-146">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="11796-147">第 1 项（排序提示：`'de5%'`）</span><span class="sxs-lookup"><span data-stu-id="11796-147">Item 1 (Order Hint: `'de5%'`)</span></span>

<span data-ttu-id="11796-p105">排序提示可指定为在列表中创建为 ` !` 的首个项目，因为在这种情况下，根本不存在上一个或下一个项目，然而，这不是必须的，因为如果未在创建项目期间指定值，服务会为项目上的所有排序提示值自动生成值。以下示例表明将项目置于之前为空的列表中时，应使用排序提示。添加第一项：</span><span class="sxs-lookup"><span data-stu-id="11796-p105">Order Hints can be specified for creating the first item in the list as ` !`, since neither a previous or a next item exists in that case, however this is unnecessary, as the service will auto-generate values for all order hint values on items if they are not specified during creation of the item. Following example illustrates the order hints should be used when placing items in a previously empty list. Add the first item:</span></span>

1. <span data-ttu-id="11796-151">第 1 项（排序提示：`' !'`）</span><span class="sxs-lookup"><span data-stu-id="11796-151">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="11796-152">将第二项添加到顶部：</span><span class="sxs-lookup"><span data-stu-id="11796-152">Add the second item to top:</span></span>

1. <span data-ttu-id="11796-153">第 2 项（排序提示：`'  !!'`）</span><span class="sxs-lookup"><span data-stu-id="11796-153">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="11796-154">第 1 项（排序提示：`' !'`）</span><span class="sxs-lookup"><span data-stu-id="11796-154">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="11796-155">将第三项添加到底部：</span><span class="sxs-lookup"><span data-stu-id="11796-155">Add the third item to bottom:</span></span>

1. <span data-ttu-id="11796-156">第 2 项（排序提示：`'  !!'`）</span><span class="sxs-lookup"><span data-stu-id="11796-156">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="11796-157">第 1 项（排序提示：`' !'`）</span><span class="sxs-lookup"><span data-stu-id="11796-157">Item 1 (Order Hint: `' !'`)</span></span>
3. <span data-ttu-id="11796-158">第 3 项（排序提示：`' ! !'`）</span><span class="sxs-lookup"><span data-stu-id="11796-158">Item 3 (Order Hint: `' ! !'`)</span></span>







