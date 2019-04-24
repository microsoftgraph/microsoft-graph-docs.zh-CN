---
title: journalLines 资源类型
description: Dynamics 365 Business Central 中的日志行。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 7a6841bcc2f893f8ca794e7d8e6aeafbcd4e48ca
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507292"
---
# <a name="journallines-resource-type"></a><span data-ttu-id="e2b14-103">journalLines 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2b14-103">journalLines resource type</span></span>
<span data-ttu-id="e2b14-104">代表 Dynamics 365 Business Central 中的日记中的一条线。</span><span class="sxs-lookup"><span data-stu-id="e2b14-104">Represents a line in a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="e2b14-105">方法</span><span class="sxs-lookup"><span data-stu-id="e2b14-105">Methods</span></span>

| <span data-ttu-id="e2b14-106">方法</span><span class="sxs-lookup"><span data-stu-id="e2b14-106">Method</span></span>                                                    | <span data-ttu-id="e2b14-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="e2b14-107">Return Type</span></span>|<span data-ttu-id="e2b14-108">说明</span><span class="sxs-lookup"><span data-stu-id="e2b14-108">Description</span></span>         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[<span data-ttu-id="e2b14-109">获取 journalLines</span><span class="sxs-lookup"><span data-stu-id="e2b14-109">Get journalLines</span></span>](../api/dynamics-journalline-get.md)      |<span data-ttu-id="e2b14-110">journalLines</span><span class="sxs-lookup"><span data-stu-id="e2b14-110">journalLines</span></span>|<span data-ttu-id="e2b14-111">获取日志行。</span><span class="sxs-lookup"><span data-stu-id="e2b14-111">Gets a journal line.</span></span>   |
|[<span data-ttu-id="e2b14-112">Post journalLines</span><span class="sxs-lookup"><span data-stu-id="e2b14-112">Post journalLines</span></span>](../api/dynamics-create-journalline.md)  |<span data-ttu-id="e2b14-113">journalLines</span><span class="sxs-lookup"><span data-stu-id="e2b14-113">journalLines</span></span>|<span data-ttu-id="e2b14-114">创建日志行。</span><span class="sxs-lookup"><span data-stu-id="e2b14-114">Creates a journal line.</span></span>|
|[<span data-ttu-id="e2b14-115">修补程序 journalLines</span><span class="sxs-lookup"><span data-stu-id="e2b14-115">Patch journalLines</span></span>](../api/dynamics-journalline-update.md) |<span data-ttu-id="e2b14-116">journalLines</span><span class="sxs-lookup"><span data-stu-id="e2b14-116">journalLines</span></span>|<span data-ttu-id="e2b14-117">更新日记行。</span><span class="sxs-lookup"><span data-stu-id="e2b14-117">Updates a journal line.</span></span>|
|[<span data-ttu-id="e2b14-118">删除 journalLines</span><span class="sxs-lookup"><span data-stu-id="e2b14-118">Delete journalLines</span></span>](../api/dynamics-journalline-delete.md)|<span data-ttu-id="e2b14-119">无</span><span class="sxs-lookup"><span data-stu-id="e2b14-119">none</span></span>        |<span data-ttu-id="e2b14-120">删除日志行。</span><span class="sxs-lookup"><span data-stu-id="e2b14-120">Deletes a journal line.</span></span>|

## <a name="properties"></a><span data-ttu-id="e2b14-121">属性</span><span class="sxs-lookup"><span data-stu-id="e2b14-121">Properties</span></span>
| <span data-ttu-id="e2b14-122">属性</span><span class="sxs-lookup"><span data-stu-id="e2b14-122">Property</span></span>             | <span data-ttu-id="e2b14-123">类型</span><span class="sxs-lookup"><span data-stu-id="e2b14-123">Type</span></span>                   |<span data-ttu-id="e2b14-124">说明</span><span class="sxs-lookup"><span data-stu-id="e2b14-124">Description</span></span>                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|<span data-ttu-id="e2b14-125">id</span><span class="sxs-lookup"><span data-stu-id="e2b14-125">id</span></span>                    |<span data-ttu-id="e2b14-126">GUID</span><span class="sxs-lookup"><span data-stu-id="e2b14-126">GUID</span></span>                    |<span data-ttu-id="e2b14-127">日记行的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="e2b14-127">The unique ID of the journal line.</span></span> <span data-ttu-id="e2b14-128">不可编辑。</span><span class="sxs-lookup"><span data-stu-id="e2b14-128">Non-editable.</span></span>                   |
|<span data-ttu-id="e2b14-129">journalDisplayName</span><span class="sxs-lookup"><span data-stu-id="e2b14-129">journalDisplayName</span></span>    |<span data-ttu-id="e2b14-130">字符串, 最大值为10</span><span class="sxs-lookup"><span data-stu-id="e2b14-130">string, maximum size 10</span></span> |<span data-ttu-id="e2b14-131">此行所属的日记的显示名称。</span><span class="sxs-lookup"><span data-stu-id="e2b14-131">The display name of the journal that this line belongs to.</span></span> <span data-ttu-id="e2b14-132">只读。</span><span class="sxs-lookup"><span data-stu-id="e2b14-132">Read-Only.</span></span>|
|<span data-ttu-id="e2b14-133">lineNumber</span><span class="sxs-lookup"><span data-stu-id="e2b14-133">lineNumber</span></span>            |<span data-ttu-id="e2b14-134">integer</span><span class="sxs-lookup"><span data-stu-id="e2b14-134">integer</span></span>                 |<span data-ttu-id="e2b14-135">日志行的编号。</span><span class="sxs-lookup"><span data-stu-id="e2b14-135">The number of the journal line.</span></span>                                    |
|<span data-ttu-id="e2b14-136">accountId</span><span class="sxs-lookup"><span data-stu-id="e2b14-136">accountId</span></span>             |<span data-ttu-id="e2b14-137">GUID</span><span class="sxs-lookup"><span data-stu-id="e2b14-137">GUID</span></span>                    |<span data-ttu-id="e2b14-138">与日志行相关的帐户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="e2b14-138">The unique ID of the account that the journal line is related to.</span></span>  |
|<span data-ttu-id="e2b14-139">accountNumber</span><span class="sxs-lookup"><span data-stu-id="e2b14-139">accountNumber</span></span>         |<span data-ttu-id="e2b14-140">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="e2b14-140">string, maximum size 20</span></span> |<span data-ttu-id="e2b14-141">与日志行相关的帐户的编号。</span><span class="sxs-lookup"><span data-stu-id="e2b14-141">The number of the account that the journal line is related to.</span></span>     |
|<span data-ttu-id="e2b14-142">postingDate</span><span class="sxs-lookup"><span data-stu-id="e2b14-142">postingDate</span></span>           |<span data-ttu-id="e2b14-143">date</span><span class="sxs-lookup"><span data-stu-id="e2b14-143">date</span></span>                    |<span data-ttu-id="e2b14-144">日志行的过帐日期。</span><span class="sxs-lookup"><span data-stu-id="e2b14-144">The date that the journal line is posted.</span></span>                          |
|<span data-ttu-id="e2b14-145">documentNumber</span><span class="sxs-lookup"><span data-stu-id="e2b14-145">documentNumber</span></span>        |<span data-ttu-id="e2b14-146">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="e2b14-146">string, maximum size 20</span></span> |<span data-ttu-id="e2b14-147">指定日记行的文档编号。</span><span class="sxs-lookup"><span data-stu-id="e2b14-147">Specifies a document number for the journal line.</span></span>                  |
|<span data-ttu-id="e2b14-148">externalDocumentNumber</span><span class="sxs-lookup"><span data-stu-id="e2b14-148">externalDocumentNumber</span></span>|<span data-ttu-id="e2b14-149">字符串, 最大大小为20</span><span class="sxs-lookup"><span data-stu-id="e2b14-149">string, maximum size 20</span></span> |<span data-ttu-id="e2b14-150">指定日记行的外部文档编号。</span><span class="sxs-lookup"><span data-stu-id="e2b14-150">Specifies an external document number for the journal line.</span></span>        |
|<span data-ttu-id="e2b14-151">量</span><span class="sxs-lookup"><span data-stu-id="e2b14-151">amount</span></span>                |<span data-ttu-id="e2b14-152">数位</span><span class="sxs-lookup"><span data-stu-id="e2b14-152">decimal</span></span>                 |<span data-ttu-id="e2b14-153">指定日记行所包含的总金额 (包括 VAT)。</span><span class="sxs-lookup"><span data-stu-id="e2b14-153">Specifies the total amount (including VAT) that the journal line consists of.</span></span>|
|<span data-ttu-id="e2b14-154">description</span><span class="sxs-lookup"><span data-stu-id="e2b14-154">description</span></span>           |<span data-ttu-id="e2b14-155">字符串, 最大大小为50</span><span class="sxs-lookup"><span data-stu-id="e2b14-155">string, maximum size 50</span></span> |<span data-ttu-id="e2b14-156">日记行的说明, 由用户或 autocreated 提供。</span><span class="sxs-lookup"><span data-stu-id="e2b14-156">The description of the journal line, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="e2b14-157">注释</span><span class="sxs-lookup"><span data-stu-id="e2b14-157">comment</span></span>               |<span data-ttu-id="e2b14-158">字符串, 最大大小为250</span><span class="sxs-lookup"><span data-stu-id="e2b14-158">string, maximum size 250</span></span>|<span data-ttu-id="e2b14-159">用户在日志行上指定的注释。</span><span class="sxs-lookup"><span data-stu-id="e2b14-159">A user specified comment on the journal line.</span></span>                      |
|<span data-ttu-id="e2b14-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e2b14-160">lastModifiedDateTime</span></span>  |<span data-ttu-id="e2b14-161">datetime</span><span class="sxs-lookup"><span data-stu-id="e2b14-161">datetime</span></span>                |<span data-ttu-id="e2b14-162">修改日记行的最后一个日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e2b14-162">The last datetime the journal line was modified.</span></span> <span data-ttu-id="e2b14-163">只读。</span><span class="sxs-lookup"><span data-stu-id="e2b14-163">Read-Only.</span></span>        |

## <a name="relationships"></a><span data-ttu-id="e2b14-164">关系</span><span class="sxs-lookup"><span data-stu-id="e2b14-164">Relationships</span></span>
<span data-ttu-id="e2b14-165">日志行是日记的子页。</span><span class="sxs-lookup"><span data-stu-id="e2b14-165">A journal line is a subpage of a journal.</span></span> <span data-ttu-id="e2b14-166">不能直接访问它。</span><span class="sxs-lookup"><span data-stu-id="e2b14-166">It cannot be accessed directly.</span></span>

<span data-ttu-id="e2b14-167">日志行可以是维行的 "父实体"。</span><span class="sxs-lookup"><span data-stu-id="e2b14-167">A journal line can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="e2b14-168">帐户 (accountId) 必须存在于 "帐户" 表中。</span><span class="sxs-lookup"><span data-stu-id="e2b14-168">An Account (accountId) must exist in the Accounts table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e2b14-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2b14-169">JSON representation</span></span>

<span data-ttu-id="e2b14-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2b14-170">Here is a JSON representation of the resource.</span></span>


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
