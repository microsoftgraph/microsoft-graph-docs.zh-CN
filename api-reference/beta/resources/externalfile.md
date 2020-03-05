---
title: externalFile 资源类型
description: 通过 Microsoft Search 连接编制索引的文件。
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 91de559bd365b9d6141e10a82af9ee06593f08ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498775"
---
# <a name="externalfile-resource-type"></a><span data-ttu-id="35445-103">externalFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="35445-103">externalFile resource type</span></span>

<span data-ttu-id="35445-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="35445-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35445-105">通过 Microsoft Search[连接](externalconnection.md)编制索引的项目。</span><span class="sxs-lookup"><span data-stu-id="35445-105">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span> <span data-ttu-id="35445-106">此类型派生自[externalItem](externalitem.md)类型。</span><span class="sxs-lookup"><span data-stu-id="35445-106">This type derives from the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="35445-107">方法</span><span class="sxs-lookup"><span data-stu-id="35445-107">Methods</span></span>

| <span data-ttu-id="35445-108">方法</span><span class="sxs-lookup"><span data-stu-id="35445-108">Method</span></span>                                                        | <span data-ttu-id="35445-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="35445-109">Return Type</span></span>  | <span data-ttu-id="35445-110">说明</span><span class="sxs-lookup"><span data-stu-id="35445-110">Description</span></span> |
|:--------------------------------------------------------------|:-------------|:--|
| [<span data-ttu-id="35445-111">创建 externalFile</span><span class="sxs-lookup"><span data-stu-id="35445-111">Create externalFile</span></span>](../api/externalconnection-put-items.md) | <span data-ttu-id="35445-112">externalFile</span><span class="sxs-lookup"><span data-stu-id="35445-112">externalFile</span></span> | <span data-ttu-id="35445-113">创建 externalFile。</span><span class="sxs-lookup"><span data-stu-id="35445-113">Create an externalFile.</span></span> |
| [<span data-ttu-id="35445-114">更新 externalFile</span><span class="sxs-lookup"><span data-stu-id="35445-114">Update externalFile</span></span>](../api/externalitem-update.md)          | <span data-ttu-id="35445-115">externalFile</span><span class="sxs-lookup"><span data-stu-id="35445-115">externalFile</span></span> | <span data-ttu-id="35445-116">更新 externalFile。</span><span class="sxs-lookup"><span data-stu-id="35445-116">Update an externalFile.</span></span> |
| [<span data-ttu-id="35445-117">删除</span><span class="sxs-lookup"><span data-stu-id="35445-117">Delete</span></span>](../api/externalitem-delete.md)                       | <span data-ttu-id="35445-118">无</span><span class="sxs-lookup"><span data-stu-id="35445-118">None</span></span>         | <span data-ttu-id="35445-119">删除 externalFile。</span><span class="sxs-lookup"><span data-stu-id="35445-119">Delete an externalFile.</span></span> |

## <a name="properties"></a><span data-ttu-id="35445-120">属性</span><span class="sxs-lookup"><span data-stu-id="35445-120">Properties</span></span>

| <span data-ttu-id="35445-121">属性</span><span class="sxs-lookup"><span data-stu-id="35445-121">Property</span></span>         | <span data-ttu-id="35445-122">类型</span><span class="sxs-lookup"><span data-stu-id="35445-122">Type</span></span>                     | <span data-ttu-id="35445-123">说明</span><span class="sxs-lookup"><span data-stu-id="35445-123">Description</span></span>                    |
|:-----------------|:-------------------------|:-------------------------------|
| <span data-ttu-id="35445-124">acl</span><span class="sxs-lookup"><span data-stu-id="35445-124">acl</span></span>              | <span data-ttu-id="35445-125">[acl](acl.md)集合</span><span class="sxs-lookup"><span data-stu-id="35445-125">[acl](acl.md) collection</span></span> | <span data-ttu-id="35445-126">一组访问控制项。</span><span class="sxs-lookup"><span data-stu-id="35445-126">An array of access control entries.</span></span> <span data-ttu-id="35445-127">每个条目指定向用户或组授予的访问权限。</span><span class="sxs-lookup"><span data-stu-id="35445-127">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="35445-128">必填。</span><span class="sxs-lookup"><span data-stu-id="35445-128">Required.</span></span> |
| <span data-ttu-id="35445-129">内容</span><span class="sxs-lookup"><span data-stu-id="35445-129">content</span></span>          | <span data-ttu-id="35445-130">String</span><span class="sxs-lookup"><span data-stu-id="35445-130">String</span></span>                   | <span data-ttu-id="35445-131">项目内容的纯文本表示形式。</span><span class="sxs-lookup"><span data-stu-id="35445-131">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="35445-132">此属性中的文本为全文检索的文本。</span><span class="sxs-lookup"><span data-stu-id="35445-132">The text in this property is full-text indexed.</span></span> <span data-ttu-id="35445-133">可选。</span><span class="sxs-lookup"><span data-stu-id="35445-133">Optional.</span></span> |
| <span data-ttu-id="35445-134">id</span><span class="sxs-lookup"><span data-stu-id="35445-134">id</span></span>               | <span data-ttu-id="35445-135">String</span><span class="sxs-lookup"><span data-stu-id="35445-135">String</span></span>                   | <span data-ttu-id="35445-136">开发人员提供的包含[externalConnection](externalconnection.md)中的项的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="35445-136">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="35445-137">必须为字母数字，最多为128个字符。</span><span class="sxs-lookup"><span data-stu-id="35445-137">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="35445-138">必填。</span><span class="sxs-lookup"><span data-stu-id="35445-138">Required.</span></span> |
| <span data-ttu-id="35445-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="35445-139">createdBy</span></span>        | <span data-ttu-id="35445-140">String</span><span class="sxs-lookup"><span data-stu-id="35445-140">String</span></span>                   | <span data-ttu-id="35445-141">创建文件的用户的名称。</span><span class="sxs-lookup"><span data-stu-id="35445-141">The name of the user that created the file.</span></span> |
| <span data-ttu-id="35445-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35445-142">createdDateTime</span></span>  | <span data-ttu-id="35445-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35445-143">DateTimeOffset</span></span>           | <span data-ttu-id="35445-144">创建文件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="35445-144">The date and time that the file was created.</span></span> <span data-ttu-id="35445-145">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="35445-145">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="35445-146">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="35445-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="35445-147">扩展</span><span class="sxs-lookup"><span data-stu-id="35445-147">extension</span></span>        | <span data-ttu-id="35445-148">String</span><span class="sxs-lookup"><span data-stu-id="35445-148">String</span></span>                   | <span data-ttu-id="35445-149">文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="35445-149">The file extension.</span></span>            |
| <span data-ttu-id="35445-150">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="35445-150">lastModifiedBy</span></span>   | <span data-ttu-id="35445-151">String</span><span class="sxs-lookup"><span data-stu-id="35445-151">String</span></span>                   | <span data-ttu-id="35445-152">上次修改文件的用户的名称。</span><span class="sxs-lookup"><span data-stu-id="35445-152">The name of the user that last modified the file.</span></span> |
| <span data-ttu-id="35445-153">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35445-153">modifiedDateTime</span></span> | <span data-ttu-id="35445-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35445-154">DateTimeOffset</span></span>           | <span data-ttu-id="35445-155">上次修改文件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="35445-155">The date and time that the file was last modified.</span></span> <span data-ttu-id="35445-156">DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="35445-156">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="35445-157">例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="35445-157">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="35445-158">name</span><span class="sxs-lookup"><span data-stu-id="35445-158">name</span></span>             | <span data-ttu-id="35445-159">字符串</span><span class="sxs-lookup"><span data-stu-id="35445-159">String</span></span>                   | <span data-ttu-id="35445-160">文件名。</span><span class="sxs-lookup"><span data-stu-id="35445-160">The file name.</span></span> <span data-ttu-id="35445-161">必填。</span><span class="sxs-lookup"><span data-stu-id="35445-161">Required.</span></span>       |
| <span data-ttu-id="35445-162">size</span><span class="sxs-lookup"><span data-stu-id="35445-162">size</span></span>             | <span data-ttu-id="35445-163">Int64</span><span class="sxs-lookup"><span data-stu-id="35445-163">Int64</span></span>                    | <span data-ttu-id="35445-164">文件的大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="35445-164">The size of the file in bytes.</span></span> |
| <span data-ttu-id="35445-165">title</span><span class="sxs-lookup"><span data-stu-id="35445-165">title</span></span>            | <span data-ttu-id="35445-166">String</span><span class="sxs-lookup"><span data-stu-id="35445-166">String</span></span>                   | <span data-ttu-id="35445-167">文件的标题。</span><span class="sxs-lookup"><span data-stu-id="35445-167">The title of the file.</span></span>         |
| <span data-ttu-id="35445-168">url</span><span class="sxs-lookup"><span data-stu-id="35445-168">url</span></span>              | <span data-ttu-id="35445-169">String</span><span class="sxs-lookup"><span data-stu-id="35445-169">String</span></span>                   | <span data-ttu-id="35445-170">用于访问文件的 URL。</span><span class="sxs-lookup"><span data-stu-id="35445-170">The URL to access the file.</span></span> <span data-ttu-id="35445-171">必填。</span><span class="sxs-lookup"><span data-stu-id="35445-171">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="35445-172">关系</span><span class="sxs-lookup"><span data-stu-id="35445-172">Relationships</span></span>

<span data-ttu-id="35445-173">无</span><span class="sxs-lookup"><span data-stu-id="35445-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35445-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35445-174">JSON representation</span></span>

<span data-ttu-id="35445-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35445-175">The following is a JSON representation of the resource.</span></span>

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
