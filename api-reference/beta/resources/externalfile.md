---
title: externalFile 资源类型
description: 通过 Microsoft Search 连接编制索引的文件。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bee1ad36769066550e1a6adc3ce7427602c66e66
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938981"
---
# <a name="externalfile-resource-type"></a><span data-ttu-id="40134-103">externalFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="40134-103">externalFile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40134-104">通过 Microsoft Search[连接](externalconnection.md)编制索引的项目。</span><span class="sxs-lookup"><span data-stu-id="40134-104">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span> <span data-ttu-id="40134-105">此类型派生自[externalItem](externalitem.md)类型。</span><span class="sxs-lookup"><span data-stu-id="40134-105">This type derives from the [externalItem](externalitem.md) type.</span></span>

## <a name="methods"></a><span data-ttu-id="40134-106">方法</span><span class="sxs-lookup"><span data-stu-id="40134-106">Methods</span></span>

| <span data-ttu-id="40134-107">方法</span><span class="sxs-lookup"><span data-stu-id="40134-107">Method</span></span>                                                        | <span data-ttu-id="40134-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="40134-108">Return Type</span></span>  | <span data-ttu-id="40134-109">说明</span><span class="sxs-lookup"><span data-stu-id="40134-109">Description</span></span> |
|:--------------------------------------------------------------|:-------------|:--|
| [<span data-ttu-id="40134-110">创建 externalFile</span><span class="sxs-lookup"><span data-stu-id="40134-110">Create externalFile</span></span>](../api/externalconnection-put-items.md) | <span data-ttu-id="40134-111">externalFile</span><span class="sxs-lookup"><span data-stu-id="40134-111">externalFile</span></span> | <span data-ttu-id="40134-112">创建 externalFile。</span><span class="sxs-lookup"><span data-stu-id="40134-112">Create an externalFile.</span></span> |
| [<span data-ttu-id="40134-113">更新 externalFile</span><span class="sxs-lookup"><span data-stu-id="40134-113">Update externalFile</span></span>](../api/externalitem-update.md)          | <span data-ttu-id="40134-114">externalFile</span><span class="sxs-lookup"><span data-stu-id="40134-114">externalFile</span></span> | <span data-ttu-id="40134-115">更新 externalFile。</span><span class="sxs-lookup"><span data-stu-id="40134-115">Update an externalFile.</span></span> |
| [<span data-ttu-id="40134-116">删除</span><span class="sxs-lookup"><span data-stu-id="40134-116">Delete</span></span>](../api/externalitem-delete.md)                       | <span data-ttu-id="40134-117">无</span><span class="sxs-lookup"><span data-stu-id="40134-117">None</span></span>         | <span data-ttu-id="40134-118">删除 externalFile。</span><span class="sxs-lookup"><span data-stu-id="40134-118">Delete an externalFile.</span></span> |

## <a name="properties"></a><span data-ttu-id="40134-119">属性</span><span class="sxs-lookup"><span data-stu-id="40134-119">Properties</span></span>

| <span data-ttu-id="40134-120">属性</span><span class="sxs-lookup"><span data-stu-id="40134-120">Property</span></span>         | <span data-ttu-id="40134-121">类型</span><span class="sxs-lookup"><span data-stu-id="40134-121">Type</span></span>                     | <span data-ttu-id="40134-122">描述</span><span class="sxs-lookup"><span data-stu-id="40134-122">Description</span></span>                    |
|:-----------------|:-------------------------|:-------------------------------|
| <span data-ttu-id="40134-123">acl</span><span class="sxs-lookup"><span data-stu-id="40134-123">acl</span></span>              | <span data-ttu-id="40134-124">[acl](acl.md)集合</span><span class="sxs-lookup"><span data-stu-id="40134-124">[acl](acl.md) collection</span></span> | <span data-ttu-id="40134-125">一组访问控制项。</span><span class="sxs-lookup"><span data-stu-id="40134-125">An array of access control entries.</span></span> <span data-ttu-id="40134-126">每个条目指定向用户或组授予的访问权限。</span><span class="sxs-lookup"><span data-stu-id="40134-126">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="40134-127">必填。</span><span class="sxs-lookup"><span data-stu-id="40134-127">Required.</span></span> |
| <span data-ttu-id="40134-128">内容</span><span class="sxs-lookup"><span data-stu-id="40134-128">content</span></span>          | <span data-ttu-id="40134-129">字符串</span><span class="sxs-lookup"><span data-stu-id="40134-129">String</span></span>                   | <span data-ttu-id="40134-130">项目内容的纯文本表示形式。</span><span class="sxs-lookup"><span data-stu-id="40134-130">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="40134-131">此属性中的文本为全文检索的文本。</span><span class="sxs-lookup"><span data-stu-id="40134-131">The text in this property is full-text indexed.</span></span> <span data-ttu-id="40134-132">可选。</span><span class="sxs-lookup"><span data-stu-id="40134-132">Optional.</span></span> |
| <span data-ttu-id="40134-133">id</span><span class="sxs-lookup"><span data-stu-id="40134-133">id</span></span>               | <span data-ttu-id="40134-134">String</span><span class="sxs-lookup"><span data-stu-id="40134-134">String</span></span>                   | <span data-ttu-id="40134-135">开发人员提供的包含[externalConnection](externalconnection.md)中的项的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="40134-135">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="40134-136">必须为字母数字，最多为128个字符。</span><span class="sxs-lookup"><span data-stu-id="40134-136">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="40134-137">必填。</span><span class="sxs-lookup"><span data-stu-id="40134-137">Required.</span></span> |
| <span data-ttu-id="40134-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="40134-138">createdBy</span></span>        | <span data-ttu-id="40134-139">字符串</span><span class="sxs-lookup"><span data-stu-id="40134-139">String</span></span>                   | <span data-ttu-id="40134-140">创建文件的用户的名称。</span><span class="sxs-lookup"><span data-stu-id="40134-140">The name of the user that created the file.</span></span> |
| <span data-ttu-id="40134-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40134-141">createdDateTime</span></span>  | <span data-ttu-id="40134-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40134-142">DateTimeOffset</span></span>           | <span data-ttu-id="40134-143">创建文件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="40134-143">The date and time that the file was created.</span></span> <span data-ttu-id="40134-144">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="40134-144">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="40134-145">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="40134-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="40134-146">扩展</span><span class="sxs-lookup"><span data-stu-id="40134-146">extension</span></span>        | <span data-ttu-id="40134-147">字符串</span><span class="sxs-lookup"><span data-stu-id="40134-147">String</span></span>                   | <span data-ttu-id="40134-148">文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="40134-148">The file extension.</span></span>            |
| <span data-ttu-id="40134-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="40134-149">lastModifiedBy</span></span>   | <span data-ttu-id="40134-150">字符串</span><span class="sxs-lookup"><span data-stu-id="40134-150">String</span></span>                   | <span data-ttu-id="40134-151">上次修改文件的用户的名称。</span><span class="sxs-lookup"><span data-stu-id="40134-151">The name of the user that last modified the file.</span></span> |
| <span data-ttu-id="40134-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="40134-152">modifiedDateTime</span></span> | <span data-ttu-id="40134-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40134-153">DateTimeOffset</span></span>           | <span data-ttu-id="40134-154">上次修改文件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="40134-154">The date and time that the file was last modified.</span></span> <span data-ttu-id="40134-155">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="40134-155">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="40134-156">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="40134-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="40134-157">name</span><span class="sxs-lookup"><span data-stu-id="40134-157">name</span></span>             | <span data-ttu-id="40134-158">字符串</span><span class="sxs-lookup"><span data-stu-id="40134-158">String</span></span>                   | <span data-ttu-id="40134-159">文件名。</span><span class="sxs-lookup"><span data-stu-id="40134-159">The file name.</span></span> <span data-ttu-id="40134-160">必填。</span><span class="sxs-lookup"><span data-stu-id="40134-160">Required.</span></span>       |
| <span data-ttu-id="40134-161">size</span><span class="sxs-lookup"><span data-stu-id="40134-161">size</span></span>             | <span data-ttu-id="40134-162">Int64</span><span class="sxs-lookup"><span data-stu-id="40134-162">Int64</span></span>                    | <span data-ttu-id="40134-163">文件的大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="40134-163">The size of the file in bytes.</span></span> |
| <span data-ttu-id="40134-164">title</span><span class="sxs-lookup"><span data-stu-id="40134-164">title</span></span>            | <span data-ttu-id="40134-165">String</span><span class="sxs-lookup"><span data-stu-id="40134-165">String</span></span>                   | <span data-ttu-id="40134-166">文件的标题。</span><span class="sxs-lookup"><span data-stu-id="40134-166">The title of the file.</span></span>         |
| <span data-ttu-id="40134-167">url</span><span class="sxs-lookup"><span data-stu-id="40134-167">url</span></span>              | <span data-ttu-id="40134-168">String</span><span class="sxs-lookup"><span data-stu-id="40134-168">String</span></span>                   | <span data-ttu-id="40134-169">用于访问文件的 URL。</span><span class="sxs-lookup"><span data-stu-id="40134-169">The URL to access the file.</span></span> <span data-ttu-id="40134-170">必填。</span><span class="sxs-lookup"><span data-stu-id="40134-170">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="40134-171">关系</span><span class="sxs-lookup"><span data-stu-id="40134-171">Relationships</span></span>

<span data-ttu-id="40134-172">无</span><span class="sxs-lookup"><span data-stu-id="40134-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40134-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40134-173">JSON representation</span></span>

<span data-ttu-id="40134-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40134-174">The following is a JSON representation of the resource.</span></span>

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
