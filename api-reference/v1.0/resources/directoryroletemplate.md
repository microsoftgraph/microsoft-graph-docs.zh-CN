---
title: directoryRoleTemplate 资源类型
description: 表示目录角色模板。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b13fa5eada7202ed240fe748f0fc92bc15ba8648
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439889"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="26319-103">directoryRoleTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="26319-103">directoryRoleTemplate resource type</span></span>

<span data-ttu-id="26319-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26319-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="26319-p101">表示目录角色模板。目录角色模板指定目录角色 ([directoryRole](directoryrole.md)) 的属性值。租户中每个已激活的目录角色都有一个相关的目录角色模板对象。要读取目录角色或更新其成员，首先必须在租户中将其激活。默认情况下，仅激活公司管理员目录角色。要激活其他可用目录角色，发送 POST 请求到此目录角色模板 ID 的 `/directoryRoles` 端点，角色基于此模板，且此模板在请求的 **roleTemplateId** 参数中指定。在成功完成请求后，你可以开始读取，并将成员分配给目录角色。**注意**：目录角色模板针对用户目录角色公开。用户目录角色是隐式的，对目录客户端不可见。租户中的每个用户按基础结构分配到此角色。已激活该角色。请勿使用此模板。</span><span class="sxs-lookup"><span data-stu-id="26319-p101">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="26319-117">Methods</span><span class="sxs-lookup"><span data-stu-id="26319-117">Methods</span></span>

| <span data-ttu-id="26319-118">方法</span><span class="sxs-lookup"><span data-stu-id="26319-118">Method</span></span>       | <span data-ttu-id="26319-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="26319-119">Return Type</span></span>  |<span data-ttu-id="26319-120">说明</span><span class="sxs-lookup"><span data-stu-id="26319-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="26319-121">获取 directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="26319-121">Get directoryRoleTemplate</span></span>](../api/directoryroletemplate-get.md) | [<span data-ttu-id="26319-122">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="26319-122">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="26319-123">读取 directoryroletemplate 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="26319-123">Read properties and relationships of directoryRoleTemplate object.</span></span>|
|[<span data-ttu-id="26319-124">列出 directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="26319-124">List directoryRoleTemplate</span></span>](../api/directoryroletemplate-list.md) | <span data-ttu-id="26319-125">[directoryRoleTemplate](directoryroletemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="26319-125">[directoryRoleTemplate](directoryroletemplate.md) collection</span></span> |<span data-ttu-id="26319-126">检索 directoryRoleTemplate 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="26319-126">Retrieve a list of directoryRoleTemplate objects.</span></span>|

## <a name="properties"></a><span data-ttu-id="26319-127">属性</span><span class="sxs-lookup"><span data-stu-id="26319-127">Properties</span></span>
| <span data-ttu-id="26319-128">属性</span><span class="sxs-lookup"><span data-stu-id="26319-128">Property</span></span>     | <span data-ttu-id="26319-129">类型</span><span class="sxs-lookup"><span data-stu-id="26319-129">Type</span></span>   |<span data-ttu-id="26319-130">说明</span><span class="sxs-lookup"><span data-stu-id="26319-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="26319-131">说明</span><span class="sxs-lookup"><span data-stu-id="26319-131">description</span></span>|<span data-ttu-id="26319-132">String</span><span class="sxs-lookup"><span data-stu-id="26319-132">String</span></span>|<span data-ttu-id="26319-p102">可设置目录角色说明。只读。</span><span class="sxs-lookup"><span data-stu-id="26319-p102">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="26319-135">displayName</span><span class="sxs-lookup"><span data-stu-id="26319-135">displayName</span></span>|<span data-ttu-id="26319-136">String</span><span class="sxs-lookup"><span data-stu-id="26319-136">String</span></span>|<span data-ttu-id="26319-p103">可设置目录角色显示名称。只读。</span><span class="sxs-lookup"><span data-stu-id="26319-p103">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="26319-139">id</span><span class="sxs-lookup"><span data-stu-id="26319-139">id</span></span>|<span data-ttu-id="26319-140">String</span><span class="sxs-lookup"><span data-stu-id="26319-140">String</span></span>|<span data-ttu-id="26319-p104">模板的的唯一标识符。继承自 [directoryObject](directoryobject.md)。在 POST 请求中指定 **roleTemplateId** 属性的目录角色模板的 **id** 将在租户中激活 [directoryRole](directoryrole.md)。密钥，不可为 NULL。只读。</span><span class="sxs-lookup"><span data-stu-id="26319-p104">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26319-146">关系</span><span class="sxs-lookup"><span data-stu-id="26319-146">Relationships</span></span>
<span data-ttu-id="26319-147">无</span><span class="sxs-lookup"><span data-stu-id="26319-147">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="26319-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26319-148">JSON representation</span></span>

<span data-ttu-id="26319-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26319-149">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

