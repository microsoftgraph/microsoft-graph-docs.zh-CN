---
title: schemaExtension 资源类型（架构扩展）
description: '可以通过架构扩展定义架构来扩展强类型的自定义数据并将其添加到资源类型。自定义数据在扩展资源上作为复杂类型显示。 '
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: 43e5600ea7e8fb8a484216e8068c9ac3f29ac90d
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456402"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="901d1-104">schemaExtension 资源类型（架构扩展）</span><span class="sxs-lookup"><span data-stu-id="901d1-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="901d1-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="901d1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="901d1-p102">可以通过架构扩展定义架构来扩展强类型的自定义数据并将其添加到资源类型。自定义数据在扩展资源上作为复杂类型显示。</span><span class="sxs-lookup"><span data-stu-id="901d1-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="901d1-108">以下资源类型支持架构扩展：</span><span class="sxs-lookup"><span data-stu-id="901d1-108">Schema extensions are supported by the following resource types:</span></span>

- [<span data-ttu-id="901d1-109">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="901d1-109">administrativeUnit</span></span>](administrativeunit.md)
- [<span data-ttu-id="901d1-110">联系人</span><span class="sxs-lookup"><span data-stu-id="901d1-110">contact</span></span>](contact.md)
- [<span data-ttu-id="901d1-111">设备</span><span class="sxs-lookup"><span data-stu-id="901d1-111">device</span></span>](device.md)
- <span data-ttu-id="901d1-112">用户或 Microsoft 365 组日历上的[事件](event.md)。</span><span class="sxs-lookup"><span data-stu-id="901d1-112">[event](event.md) on a user or Microsoft 365 group calendar</span></span>
- <span data-ttu-id="901d1-113">Microsoft 365 组中的[帖子](post.md)</span><span class="sxs-lookup"><span data-stu-id="901d1-113">[post](post.md) of a Microsoft 365 group</span></span>
- [<span data-ttu-id="901d1-114">组</span><span class="sxs-lookup"><span data-stu-id="901d1-114">group</span></span>](group.md)
- [<span data-ttu-id="901d1-115">邮件</span><span class="sxs-lookup"><span data-stu-id="901d1-115">message</span></span>](message.md) 
- [<span data-ttu-id="901d1-116">组织</span><span class="sxs-lookup"><span data-stu-id="901d1-116">organization</span></span>](organization.md)
- [<span data-ttu-id="901d1-117">用户</span><span class="sxs-lookup"><span data-stu-id="901d1-117">user</span></span>](user.md)

<span data-ttu-id="901d1-118">请参阅[架构扩展示例](/graph/extensibility-schema-groups)了解如何将自定义数据添加到组。</span><span class="sxs-lookup"><span data-stu-id="901d1-118">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="901d1-119">方法</span><span class="sxs-lookup"><span data-stu-id="901d1-119">Methods</span></span>

| <span data-ttu-id="901d1-120">方法</span><span class="sxs-lookup"><span data-stu-id="901d1-120">Method</span></span>           | <span data-ttu-id="901d1-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="901d1-121">Return Type</span></span>    |<span data-ttu-id="901d1-122">说明</span><span class="sxs-lookup"><span data-stu-id="901d1-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="901d1-123">Create</span><span class="sxs-lookup"><span data-stu-id="901d1-123">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="901d1-124">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="901d1-124">schemaExtension</span></span> |<span data-ttu-id="901d1-125">创建架构扩展定义。</span><span class="sxs-lookup"><span data-stu-id="901d1-125">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="901d1-126">List</span><span class="sxs-lookup"><span data-stu-id="901d1-126">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="901d1-127">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="901d1-127">schemaExtension</span></span> |<span data-ttu-id="901d1-128">列出 avaialbe schemaExtension 定义及其属性。</span><span class="sxs-lookup"><span data-stu-id="901d1-128">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="901d1-129">Get</span><span class="sxs-lookup"><span data-stu-id="901d1-129">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="901d1-130">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="901d1-130">schemaExtension</span></span> |<span data-ttu-id="901d1-131">读取特定的 schemaExtension 定义的属性。</span><span class="sxs-lookup"><span data-stu-id="901d1-131">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="901d1-132">Update</span><span class="sxs-lookup"><span data-stu-id="901d1-132">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="901d1-133">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="901d1-133">schemaExtension</span></span>   |<span data-ttu-id="901d1-134">更新 schemaExtension 定义。</span><span class="sxs-lookup"><span data-stu-id="901d1-134">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="901d1-135">Delete</span><span class="sxs-lookup"><span data-stu-id="901d1-135">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="901d1-136">无</span><span class="sxs-lookup"><span data-stu-id="901d1-136">None</span></span> |<span data-ttu-id="901d1-137">删除 schemaExtension 定义。</span><span class="sxs-lookup"><span data-stu-id="901d1-137">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="901d1-138">属性</span><span class="sxs-lookup"><span data-stu-id="901d1-138">Properties</span></span>
| <span data-ttu-id="901d1-139">属性</span><span class="sxs-lookup"><span data-stu-id="901d1-139">Property</span></span>     | <span data-ttu-id="901d1-140">类型</span><span class="sxs-lookup"><span data-stu-id="901d1-140">Type</span></span>   |<span data-ttu-id="901d1-141">说明</span><span class="sxs-lookup"><span data-stu-id="901d1-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="901d1-142">说明</span><span class="sxs-lookup"><span data-stu-id="901d1-142">description</span></span>|<span data-ttu-id="901d1-143">String</span><span class="sxs-lookup"><span data-stu-id="901d1-143">String</span></span>|<span data-ttu-id="901d1-144">架构扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="901d1-144">Description for the schema extension.</span></span> <span data-ttu-id="901d1-145">支持 `$filter`（`eq`）。</span><span class="sxs-lookup"><span data-stu-id="901d1-145">Supports `$filter` (`eq`).</span></span>|
|<span data-ttu-id="901d1-146">id</span><span class="sxs-lookup"><span data-stu-id="901d1-146">id</span></span>|<span data-ttu-id="901d1-147">String</span><span class="sxs-lookup"><span data-stu-id="901d1-147">String</span></span>|<span data-ttu-id="901d1-148">架构扩展定义的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="901d1-148">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="901d1-149">你可以使用下面两种方法之一分配值：</span><span class="sxs-lookup"><span data-stu-id="901d1-149">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="901d1-p104">连接已验证域名与架构扩展名称，形成此格式的唯一字符串：\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。例如 `contoso_mySchema`。 </span><span class="sxs-lookup"><span data-stu-id="901d1-p104">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="901d1-p105">提供一个架构名称，并让 Microsoft Graph 使用此格式的架构名称完成 **id** 分配：ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。例如 `extkvbmkofy_mySchema`。</span><span class="sxs-lookup"><span data-stu-id="901d1-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="901d1-154">此属性一旦创建，便无法更改。</span><span class="sxs-lookup"><span data-stu-id="901d1-154">This property cannot be changed after creation.</span></span> <span data-ttu-id="901d1-155">支持 `$filter`（`eq`）。</span><span class="sxs-lookup"><span data-stu-id="901d1-155">Supports `$filter` (`eq`).</span></span> |
|<span data-ttu-id="901d1-156">所有者</span><span class="sxs-lookup"><span data-stu-id="901d1-156">owner</span></span>|<span data-ttu-id="901d1-157">String</span><span class="sxs-lookup"><span data-stu-id="901d1-157">String</span></span>| <span data-ttu-id="901d1-158">属于架构扩展的所有者的应用程序的 `appId`。</span><span class="sxs-lookup"><span data-stu-id="901d1-158">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="901d1-159">可在创建时提供此属性以设置所有者。</span><span class="sxs-lookup"><span data-stu-id="901d1-159">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="901d1-160">如果未提供，则会将调用应用程序的 `appId` 设置为所有者。</span><span class="sxs-lookup"><span data-stu-id="901d1-160">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="901d1-161">在任一情况下，已登录用户均必须是应用程序的所有者。</span><span class="sxs-lookup"><span data-stu-id="901d1-161">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="901d1-162">因此，如果使用 Graph 浏览器新建一个架构扩展定义，则 **必须** 提供 owner 属性（以此为例）。</span><span class="sxs-lookup"><span data-stu-id="901d1-162">So, for example, if creating a new schema extension definition using Graph Explorer, you **must** supply the owner property.</span></span> <span data-ttu-id="901d1-163">设置后，此属性为只读，且无法更改。</span><span class="sxs-lookup"><span data-stu-id="901d1-163">Once set, this property is read-only and cannot be changed.</span></span> <span data-ttu-id="901d1-164">支持 `$filter`（`eq`）。</span><span class="sxs-lookup"><span data-stu-id="901d1-164">Supports `$filter` (`eq`).</span></span>|
|<span data-ttu-id="901d1-165">properties</span><span class="sxs-lookup"><span data-stu-id="901d1-165">properties</span></span>|<span data-ttu-id="901d1-166">[extensionSchemaProperty](extensionschemaproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="901d1-166">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="901d1-167">构成架构扩展定义的属性名称和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="901d1-167">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="901d1-168">status</span><span class="sxs-lookup"><span data-stu-id="901d1-168">status</span></span>|<span data-ttu-id="901d1-169">String</span><span class="sxs-lookup"><span data-stu-id="901d1-169">String</span></span>|<span data-ttu-id="901d1-170">架构扩展的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="901d1-170">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="901d1-171">可能的状态为 **InDevelopment**、**Available** 和 **Deprecated**。</span><span class="sxs-lookup"><span data-stu-id="901d1-171">Possible states are **InDevelopment**, **Available**, and **Deprecated**.</span></span> <span data-ttu-id="901d1-172">创建后将自动设置为 **InDevelopment**。</span><span class="sxs-lookup"><span data-stu-id="901d1-172">Automatically set to **InDevelopment** on creation.</span></span> <span data-ttu-id="901d1-173">[架构扩展](/graph/extensibility-overview#schema-extensions)将提供关于可能的状态转换和行为的详细信息。</span><span class="sxs-lookup"><span data-stu-id="901d1-173">[Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span> <span data-ttu-id="901d1-174">支持 `$filter`（`eq`）。</span><span class="sxs-lookup"><span data-stu-id="901d1-174">Supports `$filter` (`eq`).</span></span>|
|<span data-ttu-id="901d1-175">targetTypes</span><span class="sxs-lookup"><span data-stu-id="901d1-175">targetTypes</span></span>|<span data-ttu-id="901d1-176">String collection</span><span class="sxs-lookup"><span data-stu-id="901d1-176">String collection</span></span>|<span data-ttu-id="901d1-177">架构扩展适用的支持扩展的 Microsoft Graph 类型集。</span><span class="sxs-lookup"><span data-stu-id="901d1-177">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="901d1-178">从administrativeUnit、contact、device、event、group、message、organization、post 或 user 中选择。        </span><span class="sxs-lookup"><span data-stu-id="901d1-178">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="901d1-179">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="901d1-179">JSON representation</span></span>

<span data-ttu-id="901d1-180">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="901d1-180">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schemaExtension"
}-->

```json
{
  "description": "String",
  "id": "String (identifier)",
  "owner": "String",
  "properties": [{"@odata.type": "microsoft.graph.extensionSchemaProperty"}],
  "status": "String",
  "targetTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


