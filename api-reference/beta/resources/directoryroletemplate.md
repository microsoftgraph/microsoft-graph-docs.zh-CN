---
title: directoryRoleTemplate 资源类型
description: 表示目录角色模板。目录角色模板指定目录角色 (directoryRole) 的属性值。租户中每个已激活的目录角色都有一个相关的目录角色模板对象。要读取目录角色或更新其成员，首先必须在租户中将其激活。默认情况下，仅激活公司管理员目录角色。要激活其他可用目录角色，发送 POST 请求到此目录角色模板 ID 的  端点，角色基于此模板，且此模板在请求的 roleTemplateId 参数中指定。在成功完成请求后，你可以开始读取，并将成员分配给目录角色。注意：目录角色模板针对用户目录角色公开。用户目录角色是隐式的，对目录客户端不可见。租户中的每个用户按基础结构分配到此角色。已激活该角色。请勿使用此模板。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd813c9f7676e7190e5aedbb6d9b950e9ffc6aac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526156"
---
# <a name="directoryroletemplate-resource-type"></a><span data-ttu-id="8fcdc-114">directoryRoleTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="8fcdc-114">directoryRoleTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fcdc-p102">表示目录角色模板。目录角色模板指定目录角色 ([directoryRole](directoryrole.md)) 的属性值。租户中每个已激活的目录角色都有一个相关的目录角色模板对象。要读取目录角色或更新其成员，首先必须在租户中将其激活。默认情况下，仅激活公司管理员目录角色。要激活其他可用目录角色，发送 POST 请求到此目录角色模板 ID 的 `/directoryRoles` 端点，角色基于此模板，且此模板在请求的 **roleTemplateId** 参数中指定。在成功完成请求后，你可以开始读取，并将成员分配给目录角色。**注意**：目录角色模板针对用户目录角色公开。用户目录角色是隐式的，对目录客户端不可见。租户中的每个用户按基础结构分配到此角色。已激活该角色。请勿使用此模板。</span><span class="sxs-lookup"><span data-stu-id="8fcdc-p102">Represents a directory role template. A directory role template specifies the property values of a directory role ([directoryRole](directoryrole.md)). There is an associated directory role template object for each of the directory roles that may be activated in a tenant. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles you send a POST request to the `/directoryRoles` endpoint with the ID of the directory role template on which the directory role is based specified in the **roleTemplateId** parameter of the request. Upon successful completion of this request, you can then start to read and assign members to the directory role. **Note**: A directory role template is exposed for the Users directory role. The Users directory role is implicit and is not visible to directory clients. Every User in the tenant is assigned to this role by the infrastructure. The role is already activated. Do not use this template.</span></span>


## <a name="methods"></a><span data-ttu-id="8fcdc-127">方法</span><span class="sxs-lookup"><span data-stu-id="8fcdc-127">Methods</span></span>

| <span data-ttu-id="8fcdc-128">方法</span><span class="sxs-lookup"><span data-stu-id="8fcdc-128">Method</span></span>       | <span data-ttu-id="8fcdc-129">返回类型</span><span class="sxs-lookup"><span data-stu-id="8fcdc-129">Return Type</span></span>  |<span data-ttu-id="8fcdc-130">说明</span><span class="sxs-lookup"><span data-stu-id="8fcdc-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fcdc-131">获取 directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="8fcdc-131">[Get directoryRoleTemplate](../api/directoryroletemplate-get.md)</span></span> | [<span data-ttu-id="8fcdc-132">directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="8fcdc-132">directoryRoleTemplate</span></span>](directoryroletemplate.md) |<span data-ttu-id="8fcdc-133">读取 directoryroletemplate 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8fcdc-133">Read properties and relationships of directoryRoleTemplate object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8fcdc-134">属性</span><span class="sxs-lookup"><span data-stu-id="8fcdc-134">Properties</span></span>
| <span data-ttu-id="8fcdc-135">属性</span><span class="sxs-lookup"><span data-stu-id="8fcdc-135">Property</span></span>     | <span data-ttu-id="8fcdc-136">类型</span><span class="sxs-lookup"><span data-stu-id="8fcdc-136">Type</span></span>   |<span data-ttu-id="8fcdc-137">说明</span><span class="sxs-lookup"><span data-stu-id="8fcdc-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fcdc-138">说明</span><span class="sxs-lookup"><span data-stu-id="8fcdc-138">description</span></span>|<span data-ttu-id="8fcdc-139">String</span><span class="sxs-lookup"><span data-stu-id="8fcdc-139">String</span></span>|<span data-ttu-id="8fcdc-p103">可设置目录角色说明。只读。</span><span class="sxs-lookup"><span data-stu-id="8fcdc-p103">The description to set for the directory role. Read-only.</span></span>|
|<span data-ttu-id="8fcdc-142">displayName</span><span class="sxs-lookup"><span data-stu-id="8fcdc-142">displayName</span></span>|<span data-ttu-id="8fcdc-143">String</span><span class="sxs-lookup"><span data-stu-id="8fcdc-143">String</span></span>|<span data-ttu-id="8fcdc-p104">可设置目录角色显示名称。只读。</span><span class="sxs-lookup"><span data-stu-id="8fcdc-p104">The display name to set for the directory role. Read-only.</span></span> |
|<span data-ttu-id="8fcdc-146">id</span><span class="sxs-lookup"><span data-stu-id="8fcdc-146">id</span></span>|<span data-ttu-id="8fcdc-147">String</span><span class="sxs-lookup"><span data-stu-id="8fcdc-147">String</span></span>|<span data-ttu-id="8fcdc-p105">模板的的唯一标识符。继承自 [directoryObject](directoryobject.md)。在 POST 请求中指定 **roleTemplateId** 属性的目录角色模板的 **id** 将在租户中激活 [directoryRole](directoryrole.md)。密钥，不可为 NULL。只读。</span><span class="sxs-lookup"><span data-stu-id="8fcdc-p105">The unique identifier for the template. Inherited from [directoryObject](directoryobject.md). You specify the **id** of the directory role template for the **roleTemplateId** property in the POST request activate a [directoryRole](directoryrole.md) in a tenant. Key, Not nullable. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fcdc-153">关系</span><span class="sxs-lookup"><span data-stu-id="8fcdc-153">Relationships</span></span>
<span data-ttu-id="8fcdc-154">无</span><span class="sxs-lookup"><span data-stu-id="8fcdc-154">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="8fcdc-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8fcdc-155">JSON representation</span></span>

<span data-ttu-id="8fcdc-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fcdc-156">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryroletemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
