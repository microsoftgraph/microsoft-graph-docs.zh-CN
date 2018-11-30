---
title: directoryRoleTemplate 资源类型
description: 表示目录角色模板。 目录角色模板指定一个目录角色 (directoryRole) 的属性值。 没有可能在租户中激活目录角色的每个关联的目录角色 template 对象。 若要读取目录角色或更新其成员，它必须首先激活在租户中。 默认情况下已激活公司管理员的目录角色。 若要激活其他可用的目录角色您发送一个 POST 请求到`/directoryRoles`终结点请求的**roleTemplateId**参数中指定的目录角色模板目录角色所基于的 id。 在此请求成功完成，您就可以开始读取和分配目录角色的成员。 **注意**： 目录角色模板公开用户目录角色。 用户目录角色是隐式，而不是对目录客户端可见。 基础结构的情况下，为租户中的每个用户分配给此角色。 已激活的角色。 不要使用此模板。
ms.openlocfilehash: 088b630a05044f4b3dba59dd1ff6c9a11dce6c0f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041494"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="5e10d-114">directoryRoleTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e10d-114">directoryRoleTemplate resource type</span></span>

> <span data-ttu-id="5e10d-115">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5e10d-115">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e10d-116">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5e10d-116">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e10d-p103">表示目录角色模板。目录角色模板指定目录角色 ([directoryRole](directoryrole.md)) 的属性值。租户中每个已激活的目录角色都有一个相关的目录角色模板对象。要读取目录角色或更新其成员，首先必须在租户中将其激活。默认情况下，仅激活公司管理员目录角色。要激活其他可用目录角色，发送 POST 请求到此目录角色模板 ID 的 `/directoryRoles` 端点，角色基于此模板，且此模板在请求的 **roleTemplateId** 参数中指定。在成功完成请求后，你可以开始读取，并将成员分配给目录角色。**注意**：目录角色模板针对用户目录角色公开。用户目录角色是隐式的，对目录客户端不可见。租户中的每个用户按基础结构分配到此角色。已激活该角色。请勿使用此模板。</span><span class="sxs-lookup"><span data-stu-id="5e10d-p103">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="5e10d-129">方法</span><span class="sxs-lookup"><span data-stu-id="5e10d-129">Methods</span></span>

| <span data-ttu-id="5e10d-130">方法</span><span class="sxs-lookup"><span data-stu-id="5e10d-130">Method</span></span>       | <span data-ttu-id="5e10d-131">返回类型</span><span class="sxs-lookup"><span data-stu-id="5e10d-131">Return Type</span></span>  |<span data-ttu-id="5e10d-132">说明</span><span class="sxs-lookup"><span data-stu-id="5e10d-132">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5e10d-133">获取 directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="5e10d-133">Get directoryRoleTemplate</span></span>](../api/directoryroletemplate-get.md) | [<span data-ttu-id="5e10d-134">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="5e10d-134">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="5e10d-135">读取 directoryroletemplate 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5e10d-135">Read properties and relationships of directoryRoleTemplate object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5e10d-136">属性</span><span class="sxs-lookup"><span data-stu-id="5e10d-136">Properties</span></span>
| <span data-ttu-id="5e10d-137">属性</span><span class="sxs-lookup"><span data-stu-id="5e10d-137">Property</span></span>     | <span data-ttu-id="5e10d-138">类型</span><span class="sxs-lookup"><span data-stu-id="5e10d-138">Type</span></span>   |<span data-ttu-id="5e10d-139">说明</span><span class="sxs-lookup"><span data-stu-id="5e10d-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e10d-140">说明</span><span class="sxs-lookup"><span data-stu-id="5e10d-140">description</span></span>|<span data-ttu-id="5e10d-141">String</span><span class="sxs-lookup"><span data-stu-id="5e10d-141">String</span></span>|<span data-ttu-id="5e10d-p104">可设置目录角色说明。只读。</span><span class="sxs-lookup"><span data-stu-id="5e10d-p104">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="5e10d-144">displayName</span><span class="sxs-lookup"><span data-stu-id="5e10d-144">displayName</span></span>|<span data-ttu-id="5e10d-145">String</span><span class="sxs-lookup"><span data-stu-id="5e10d-145">String</span></span>|<span data-ttu-id="5e10d-p105">可设置目录角色显示名称。只读。</span><span class="sxs-lookup"><span data-stu-id="5e10d-p105">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="5e10d-148">id</span><span class="sxs-lookup"><span data-stu-id="5e10d-148">id</span></span>|<span data-ttu-id="5e10d-149">字符串</span><span class="sxs-lookup"><span data-stu-id="5e10d-149">String</span></span>|<span data-ttu-id="5e10d-p106">模板的的唯一标识符。继承自 [directoryObject](directoryobject.md)。在 POST 请求中指定 **roleTemplateId** 属性的目录角色模板的 **id** 将在租户中激活 [directoryRole](directoryrole.md)。密钥，不可为 NULL。只读。</span><span class="sxs-lookup"><span data-stu-id="5e10d-p106">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e10d-155">Relationships</span><span class="sxs-lookup"><span data-stu-id="5e10d-155">Relationships</span></span>
<span data-ttu-id="5e10d-156">无</span><span class="sxs-lookup"><span data-stu-id="5e10d-156">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="5e10d-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e10d-157">JSON representation</span></span>

<span data-ttu-id="5e10d-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e10d-158">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRoleTemplate"
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
