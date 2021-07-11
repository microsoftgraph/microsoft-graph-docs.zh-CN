---
title: externalFile 资源类型
description: 通过连接建立索引Microsoft 搜索文件。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 23a89cb83e85f16fc4cf2faa3c285bafb9fd66cf
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366546"
---
# <a name="externalfile-resource-type"></a><span data-ttu-id="cc4c0-103">externalFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc4c0-103">externalFile resource type</span></span>

<span data-ttu-id="cc4c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc4c0-104">Namespace: microsoft.graph</span></span>

> [!CAUTION]
> <span data-ttu-id="cc4c0-105">`externalFile`类型已弃用。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-105">The `externalFile` type has been deprecated.</span></span> <span data-ttu-id="cc4c0-106">开发人员不应使用此类型。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-106">Developers should not use this type.</span></span> <span data-ttu-id="cc4c0-107">仍可使用 externalItem 类型对 [外部文件编制](externalitem.md) 索引。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-107">External files may still be indexed using the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc4c0-108">通过连接索引的Microsoft 搜索[项](externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-108">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span> <span data-ttu-id="cc4c0-109">此类型派生自 [externalItem](externalitem.md) 类型。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-109">This type derives from the [externalItem](externalitem.md) type.</span></span>

## <a name="methods"></a><span data-ttu-id="cc4c0-110">方法</span><span class="sxs-lookup"><span data-stu-id="cc4c0-110">Methods</span></span>

| <span data-ttu-id="cc4c0-111">方法</span><span class="sxs-lookup"><span data-stu-id="cc4c0-111">Method</span></span>                                                        | <span data-ttu-id="cc4c0-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="cc4c0-112">Return Type</span></span>  | <span data-ttu-id="cc4c0-113">说明</span><span class="sxs-lookup"><span data-stu-id="cc4c0-113">Description</span></span> |
|:--------------------------------------------------------------|:-------------|:--|
| [<span data-ttu-id="cc4c0-114">创建 externalFile</span><span class="sxs-lookup"><span data-stu-id="cc4c0-114">Create externalFile</span></span>](../api/externalconnection-put-items.md) | <span data-ttu-id="cc4c0-115">externalFile</span><span class="sxs-lookup"><span data-stu-id="cc4c0-115">externalFile</span></span> | <span data-ttu-id="cc4c0-116">创建 externalFile。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-116">Create an externalFile.</span></span> |
| [<span data-ttu-id="cc4c0-117">更新 externalFile</span><span class="sxs-lookup"><span data-stu-id="cc4c0-117">Update externalFile</span></span>](../api/externalitem-update.md)          | <span data-ttu-id="cc4c0-118">externalFile</span><span class="sxs-lookup"><span data-stu-id="cc4c0-118">externalFile</span></span> | <span data-ttu-id="cc4c0-119">更新 externalFile。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-119">Update an externalFile.</span></span> |
| [<span data-ttu-id="cc4c0-120">删除</span><span class="sxs-lookup"><span data-stu-id="cc4c0-120">Delete</span></span>](../api/externalitem-delete.md)                       | <span data-ttu-id="cc4c0-121">无</span><span class="sxs-lookup"><span data-stu-id="cc4c0-121">None</span></span>         | <span data-ttu-id="cc4c0-122">删除 externalFile。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-122">Delete an externalFile.</span></span> |

## <a name="properties"></a><span data-ttu-id="cc4c0-123">属性</span><span class="sxs-lookup"><span data-stu-id="cc4c0-123">Properties</span></span>

| <span data-ttu-id="cc4c0-124">属性</span><span class="sxs-lookup"><span data-stu-id="cc4c0-124">Property</span></span>         | <span data-ttu-id="cc4c0-125">类型</span><span class="sxs-lookup"><span data-stu-id="cc4c0-125">Type</span></span>                     | <span data-ttu-id="cc4c0-126">说明</span><span class="sxs-lookup"><span data-stu-id="cc4c0-126">Description</span></span>                    |
|:-----------------|:-------------------------|:-------------------------------|
| <span data-ttu-id="cc4c0-127">acl</span><span class="sxs-lookup"><span data-stu-id="cc4c0-127">acl</span></span>              | <span data-ttu-id="cc4c0-128">[acl](acl.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cc4c0-128">[acl](acl.md) collection</span></span> | <span data-ttu-id="cc4c0-129">访问控制项数组。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-129">An array of access control entries.</span></span> <span data-ttu-id="cc4c0-130">每个条目指定授予用户或组的访问权限。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-130">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="cc4c0-131">必填。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-131">Required.</span></span> |
| <span data-ttu-id="cc4c0-132">内容</span><span class="sxs-lookup"><span data-stu-id="cc4c0-132">content</span></span>          | <span data-ttu-id="cc4c0-133">String</span><span class="sxs-lookup"><span data-stu-id="cc4c0-133">String</span></span>                   | <span data-ttu-id="cc4c0-134">项目内容的纯文本表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-134">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="cc4c0-135">此属性中的文本已编制全文索引。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-135">The text in this property is full-text indexed.</span></span> <span data-ttu-id="cc4c0-136">可选。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-136">Optional.</span></span> |
| <span data-ttu-id="cc4c0-137">id</span><span class="sxs-lookup"><span data-stu-id="cc4c0-137">id</span></span>               | <span data-ttu-id="cc4c0-138">String</span><span class="sxs-lookup"><span data-stu-id="cc4c0-138">String</span></span>                   | <span data-ttu-id="cc4c0-139">开发人员提供的项目在包含[externalConnection 中的唯一 ID。](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="cc4c0-139">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="cc4c0-140">必须为字母数字，最多为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-140">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="cc4c0-141">必填。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-141">Required.</span></span> |
| <span data-ttu-id="cc4c0-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="cc4c0-142">createdBy</span></span>        | <span data-ttu-id="cc4c0-143">String</span><span class="sxs-lookup"><span data-stu-id="cc4c0-143">String</span></span>                   | <span data-ttu-id="cc4c0-144">创建文件的用户的名称。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-144">The name of the user that created the file.</span></span> |
| <span data-ttu-id="cc4c0-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc4c0-145">createdDateTime</span></span>  | <span data-ttu-id="cc4c0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc4c0-146">DateTimeOffset</span></span>           | <span data-ttu-id="cc4c0-147">文件的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-147">The date and time that the file was created.</span></span> <span data-ttu-id="cc4c0-148">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-148">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cc4c0-149">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="cc4c0-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span> |
| <span data-ttu-id="cc4c0-150">extension</span><span class="sxs-lookup"><span data-stu-id="cc4c0-150">extension</span></span>        | <span data-ttu-id="cc4c0-151">String</span><span class="sxs-lookup"><span data-stu-id="cc4c0-151">String</span></span>                   | <span data-ttu-id="cc4c0-152">文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-152">The file extension.</span></span>            |
| <span data-ttu-id="cc4c0-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="cc4c0-153">lastModifiedBy</span></span>   | <span data-ttu-id="cc4c0-154">String</span><span class="sxs-lookup"><span data-stu-id="cc4c0-154">String</span></span>                   | <span data-ttu-id="cc4c0-155">上次修改文件的用户的名称。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-155">The name of the user that last modified the file.</span></span> |
| <span data-ttu-id="cc4c0-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc4c0-156">modifiedDateTime</span></span> | <span data-ttu-id="cc4c0-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc4c0-157">DateTimeOffset</span></span>           | <span data-ttu-id="cc4c0-158">上次修改文件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-158">The date and time that the file was last modified.</span></span> <span data-ttu-id="cc4c0-159">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-159">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cc4c0-160">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="cc4c0-160">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span> |
| <span data-ttu-id="cc4c0-161">name</span><span class="sxs-lookup"><span data-stu-id="cc4c0-161">name</span></span>             | <span data-ttu-id="cc4c0-162">String</span><span class="sxs-lookup"><span data-stu-id="cc4c0-162">String</span></span>                   | <span data-ttu-id="cc4c0-163">文件名。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-163">The file name.</span></span> <span data-ttu-id="cc4c0-164">必填。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-164">Required.</span></span>       |
| <span data-ttu-id="cc4c0-165">size</span><span class="sxs-lookup"><span data-stu-id="cc4c0-165">size</span></span>             | <span data-ttu-id="cc4c0-166">Int64</span><span class="sxs-lookup"><span data-stu-id="cc4c0-166">Int64</span></span>                    | <span data-ttu-id="cc4c0-167">文件大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-167">The size of the file in bytes.</span></span> |
| <span data-ttu-id="cc4c0-168">title</span><span class="sxs-lookup"><span data-stu-id="cc4c0-168">title</span></span>            | <span data-ttu-id="cc4c0-169">String</span><span class="sxs-lookup"><span data-stu-id="cc4c0-169">String</span></span>                   | <span data-ttu-id="cc4c0-170">文件的标题。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-170">The title of the file.</span></span>         |
| <span data-ttu-id="cc4c0-171">url</span><span class="sxs-lookup"><span data-stu-id="cc4c0-171">url</span></span>              | <span data-ttu-id="cc4c0-172">String</span><span class="sxs-lookup"><span data-stu-id="cc4c0-172">String</span></span>                   | <span data-ttu-id="cc4c0-173">用于访问文件的 URL。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-173">The URL to access the file.</span></span> <span data-ttu-id="cc4c0-174">必填。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-174">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cc4c0-175">关系</span><span class="sxs-lookup"><span data-stu-id="cc4c0-175">Relationships</span></span>

<span data-ttu-id="cc4c0-176">无</span><span class="sxs-lookup"><span data-stu-id="cc4c0-176">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc4c0-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc4c0-177">JSON representation</span></span>

<span data-ttu-id="cc4c0-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc4c0-178">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalFile",
  "baseType": "microsoft.graph.externalItem"
}-->

```json
{
  "acl": [{"@odata.type": "microsoft.graph.acl"}],
  "content": "String",
  "id": "String (identifier)",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "extension": "String",
  "lastModifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "title": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


