---
title: journalLines 资源类型
description: Dynamics 365 Business Central 中的日志行。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 99d06b5a49bd2881ea6f329e8b0d3692a25444b4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013795"
---
# <a name="journallines-resource-type"></a><span data-ttu-id="a448b-103">journalLines 资源类型</span><span class="sxs-lookup"><span data-stu-id="a448b-103">journalLines resource type</span></span>

<span data-ttu-id="a448b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a448b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a448b-105">代表 Dynamics 365 Business Central 中的日记中的一条线。</span><span class="sxs-lookup"><span data-stu-id="a448b-105">Represents a line in a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="a448b-106">方法</span><span class="sxs-lookup"><span data-stu-id="a448b-106">Methods</span></span>

| <span data-ttu-id="a448b-107">方法</span><span class="sxs-lookup"><span data-stu-id="a448b-107">Method</span></span>                                                    | <span data-ttu-id="a448b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a448b-108">Return Type</span></span>|<span data-ttu-id="a448b-109">说明</span><span class="sxs-lookup"><span data-stu-id="a448b-109">Description</span></span>         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[<span data-ttu-id="a448b-110">获取 journalLines</span><span class="sxs-lookup"><span data-stu-id="a448b-110">Get journalLines</span></span>](../api/dynamics-journalline-get.md)      |<span data-ttu-id="a448b-111">journalLines</span><span class="sxs-lookup"><span data-stu-id="a448b-111">journalLines</span></span>|<span data-ttu-id="a448b-112">获取日志行。</span><span class="sxs-lookup"><span data-stu-id="a448b-112">Gets a journal line.</span></span>   |
|[<span data-ttu-id="a448b-113">Post journalLines</span><span class="sxs-lookup"><span data-stu-id="a448b-113">Post journalLines</span></span>](../api/dynamics-create-journalline.md)  |<span data-ttu-id="a448b-114">journalLines</span><span class="sxs-lookup"><span data-stu-id="a448b-114">journalLines</span></span>|<span data-ttu-id="a448b-115">创建日志行。</span><span class="sxs-lookup"><span data-stu-id="a448b-115">Creates a journal line.</span></span>|
|[<span data-ttu-id="a448b-116">修补程序 journalLines</span><span class="sxs-lookup"><span data-stu-id="a448b-116">Patch journalLines</span></span>](../api/dynamics-journalline-update.md) |<span data-ttu-id="a448b-117">journalLines</span><span class="sxs-lookup"><span data-stu-id="a448b-117">journalLines</span></span>|<span data-ttu-id="a448b-118">更新日记行。</span><span class="sxs-lookup"><span data-stu-id="a448b-118">Updates a journal line.</span></span>|
|[<span data-ttu-id="a448b-119">删除 journalLines</span><span class="sxs-lookup"><span data-stu-id="a448b-119">Delete journalLines</span></span>](../api/dynamics-journalline-delete.md)|<span data-ttu-id="a448b-120">无</span><span class="sxs-lookup"><span data-stu-id="a448b-120">none</span></span>        |<span data-ttu-id="a448b-121">删除日志行。</span><span class="sxs-lookup"><span data-stu-id="a448b-121">Deletes a journal line.</span></span>|

## <a name="properties"></a><span data-ttu-id="a448b-122">属性</span><span class="sxs-lookup"><span data-stu-id="a448b-122">Properties</span></span>
| <span data-ttu-id="a448b-123">属性</span><span class="sxs-lookup"><span data-stu-id="a448b-123">Property</span></span>             | <span data-ttu-id="a448b-124">类型</span><span class="sxs-lookup"><span data-stu-id="a448b-124">Type</span></span>                   |<span data-ttu-id="a448b-125">说明</span><span class="sxs-lookup"><span data-stu-id="a448b-125">Description</span></span>                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|<span data-ttu-id="a448b-126">id</span><span class="sxs-lookup"><span data-stu-id="a448b-126">id</span></span>                    |<span data-ttu-id="a448b-127">GUID</span><span class="sxs-lookup"><span data-stu-id="a448b-127">GUID</span></span>                    |<span data-ttu-id="a448b-128">日记行的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="a448b-128">The unique ID of the journal line.</span></span> <span data-ttu-id="a448b-129">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="a448b-129">Non-editable.</span></span>                   |
|<span data-ttu-id="a448b-130">journalDisplayName</span><span class="sxs-lookup"><span data-stu-id="a448b-130">journalDisplayName</span></span>    |<span data-ttu-id="a448b-131">字符串，最大值为10</span><span class="sxs-lookup"><span data-stu-id="a448b-131">string, maximum size 10</span></span> |<span data-ttu-id="a448b-132">此行所属的日记的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a448b-132">The display name of the journal that this line belongs to.</span></span> <span data-ttu-id="a448b-133">只读。</span><span class="sxs-lookup"><span data-stu-id="a448b-133">Read-Only.</span></span>|
|<span data-ttu-id="a448b-134">lineNumber</span><span class="sxs-lookup"><span data-stu-id="a448b-134">lineNumber</span></span>            |<span data-ttu-id="a448b-135">integer</span><span class="sxs-lookup"><span data-stu-id="a448b-135">integer</span></span>                 |<span data-ttu-id="a448b-136">日志行的编号。</span><span class="sxs-lookup"><span data-stu-id="a448b-136">The number of the journal line.</span></span>                                    |
|<span data-ttu-id="a448b-137">accountId</span><span class="sxs-lookup"><span data-stu-id="a448b-137">accountId</span></span>             |<span data-ttu-id="a448b-138">GUID</span><span class="sxs-lookup"><span data-stu-id="a448b-138">GUID</span></span>                    |<span data-ttu-id="a448b-139">与日志行相关的帐户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="a448b-139">The unique ID of the account that the journal line is related to.</span></span>  |
|<span data-ttu-id="a448b-140">accountNumber</span><span class="sxs-lookup"><span data-stu-id="a448b-140">accountNumber</span></span>         |<span data-ttu-id="a448b-141">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="a448b-141">string, maximum size 20</span></span> |<span data-ttu-id="a448b-142">与日志行相关的帐户的编号。</span><span class="sxs-lookup"><span data-stu-id="a448b-142">The number of the account that the journal line is related to.</span></span>     |
|<span data-ttu-id="a448b-143">postingDate</span><span class="sxs-lookup"><span data-stu-id="a448b-143">postingDate</span></span>           |<span data-ttu-id="a448b-144">date</span><span class="sxs-lookup"><span data-stu-id="a448b-144">date</span></span>                    |<span data-ttu-id="a448b-145">日志行的过帐日期。</span><span class="sxs-lookup"><span data-stu-id="a448b-145">The date that the journal line is posted.</span></span>                          |
|<span data-ttu-id="a448b-146">documentNumber</span><span class="sxs-lookup"><span data-stu-id="a448b-146">documentNumber</span></span>        |<span data-ttu-id="a448b-147">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="a448b-147">string, maximum size 20</span></span> |<span data-ttu-id="a448b-148">指定日记行的文档编号。</span><span class="sxs-lookup"><span data-stu-id="a448b-148">Specifies a document number for the journal line.</span></span>                  |
|<span data-ttu-id="a448b-149">externalDocumentNumber</span><span class="sxs-lookup"><span data-stu-id="a448b-149">externalDocumentNumber</span></span>|<span data-ttu-id="a448b-150">字符串，最大大小为20</span><span class="sxs-lookup"><span data-stu-id="a448b-150">string, maximum size 20</span></span> |<span data-ttu-id="a448b-151">指定日记行的外部文档编号。</span><span class="sxs-lookup"><span data-stu-id="a448b-151">Specifies an external document number for the journal line.</span></span>        |
|<span data-ttu-id="a448b-152">量</span><span class="sxs-lookup"><span data-stu-id="a448b-152">amount</span></span>                |<span data-ttu-id="a448b-153">数位</span><span class="sxs-lookup"><span data-stu-id="a448b-153">decimal</span></span>                 |<span data-ttu-id="a448b-154">指定日志行所包含的增值税)  (总金额。</span><span class="sxs-lookup"><span data-stu-id="a448b-154">Specifies the total amount (including VAT) that the journal line consists of.</span></span>|
|<span data-ttu-id="a448b-155">description</span><span class="sxs-lookup"><span data-stu-id="a448b-155">description</span></span>           |<span data-ttu-id="a448b-156">字符串，最大大小为50</span><span class="sxs-lookup"><span data-stu-id="a448b-156">string, maximum size 50</span></span> |<span data-ttu-id="a448b-157">日记行的说明，由用户或 autocreated 提供。</span><span class="sxs-lookup"><span data-stu-id="a448b-157">The description of the journal line, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="a448b-158">comment</span><span class="sxs-lookup"><span data-stu-id="a448b-158">comment</span></span>               |<span data-ttu-id="a448b-159">字符串，最大大小为250</span><span class="sxs-lookup"><span data-stu-id="a448b-159">string, maximum size 250</span></span>|<span data-ttu-id="a448b-160">用户在日志行上指定的注释。</span><span class="sxs-lookup"><span data-stu-id="a448b-160">A user specified comment on the journal line.</span></span>                      |
|<span data-ttu-id="a448b-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a448b-161">lastModifiedDateTime</span></span>  |<span data-ttu-id="a448b-162">datetime</span><span class="sxs-lookup"><span data-stu-id="a448b-162">datetime</span></span>                |<span data-ttu-id="a448b-163">修改日记行的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a448b-163">The last datetime the journal line was modified.</span></span> <span data-ttu-id="a448b-164">只读。</span><span class="sxs-lookup"><span data-stu-id="a448b-164">Read-Only.</span></span>        |

## <a name="relationships"></a><span data-ttu-id="a448b-165">关系</span><span class="sxs-lookup"><span data-stu-id="a448b-165">Relationships</span></span>
<span data-ttu-id="a448b-166">日志行是日记的子页。</span><span class="sxs-lookup"><span data-stu-id="a448b-166">A journal line is a subpage of a journal.</span></span> <span data-ttu-id="a448b-167">不能直接访问它。</span><span class="sxs-lookup"><span data-stu-id="a448b-167">It cannot be accessed directly.</span></span>

<span data-ttu-id="a448b-168">日志行可以是维行的 "父实体"。</span><span class="sxs-lookup"><span data-stu-id="a448b-168">A journal line can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="a448b-169">帐户表中必须存在 (accountId) 帐户。</span><span class="sxs-lookup"><span data-stu-id="a448b-169">An Account (accountId) must exist in the Accounts table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a448b-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a448b-170">JSON representation</span></span>

<span data-ttu-id="a448b-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a448b-171">Here is a JSON representation of the resource.</span></span>


```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "accountId": "GUID",
    "accountNumber": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```


