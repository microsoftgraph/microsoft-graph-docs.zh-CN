---
title: schemaExtension 资源类型（架构扩展）
description: 'Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource. '
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: 6959a21d2341c9868c8a3e20e39098c1fe048277
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896964"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="42e8c-104">schemaExtension 资源类型（架构扩展）</span><span class="sxs-lookup"><span data-stu-id="42e8c-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="42e8c-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42e8c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42e8c-106">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type.</span><span class="sxs-lookup"><span data-stu-id="42e8c-106">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type.</span></span> <span data-ttu-id="42e8c-107">The custom data appears as a complex type on the extended resource.</span><span class="sxs-lookup"><span data-stu-id="42e8c-107">The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="42e8c-108">以下资源类型支持架构扩展：</span><span class="sxs-lookup"><span data-stu-id="42e8c-108">Schema extensions are supported by the following resource types:</span></span>

- [<span data-ttu-id="42e8c-109">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="42e8c-109">administrativeUnit</span></span>](administrativeunit.md)
- [<span data-ttu-id="42e8c-110">联系人</span><span class="sxs-lookup"><span data-stu-id="42e8c-110">contact</span></span>](contact.md)
- [<span data-ttu-id="42e8c-111">设备</span><span class="sxs-lookup"><span data-stu-id="42e8c-111">device</span></span>](device.md)
- <span data-ttu-id="42e8c-112">用户或 Microsoft 365 组日历上的[事件](event.md)</span><span class="sxs-lookup"><span data-stu-id="42e8c-112">[event](event.md) on a user or Microsoft 365 group calendar</span></span>
- <span data-ttu-id="42e8c-113">Microsoft 365 组的[帖子](post.md)</span><span class="sxs-lookup"><span data-stu-id="42e8c-113">[post](post.md) of a Microsoft 365 group</span></span>
- [<span data-ttu-id="42e8c-114">组</span><span class="sxs-lookup"><span data-stu-id="42e8c-114">group</span></span>](group.md)
- [<span data-ttu-id="42e8c-115">邮件</span><span class="sxs-lookup"><span data-stu-id="42e8c-115">message</span></span>](message.md) 
- [<span data-ttu-id="42e8c-116">组织</span><span class="sxs-lookup"><span data-stu-id="42e8c-116">organization</span></span>](organization.md)
- [<span data-ttu-id="42e8c-117">用户</span><span class="sxs-lookup"><span data-stu-id="42e8c-117">user</span></span>](user.md)

<span data-ttu-id="42e8c-118">请参阅[架构扩展示例](/graph/extensibility-schema-groups)了解如何将自定义数据添加到组。</span><span class="sxs-lookup"><span data-stu-id="42e8c-118">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="42e8c-119">方法</span><span class="sxs-lookup"><span data-stu-id="42e8c-119">Methods</span></span>

| <span data-ttu-id="42e8c-120">方法</span><span class="sxs-lookup"><span data-stu-id="42e8c-120">Method</span></span>           | <span data-ttu-id="42e8c-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="42e8c-121">Return Type</span></span>    |<span data-ttu-id="42e8c-122">说明</span><span class="sxs-lookup"><span data-stu-id="42e8c-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="42e8c-123">Create</span><span class="sxs-lookup"><span data-stu-id="42e8c-123">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="42e8c-124">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="42e8c-124">schemaExtension</span></span> |<span data-ttu-id="42e8c-125">创建架构扩展定义。</span><span class="sxs-lookup"><span data-stu-id="42e8c-125">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="42e8c-126">List</span><span class="sxs-lookup"><span data-stu-id="42e8c-126">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="42e8c-127">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="42e8c-127">schemaExtension</span></span> |<span data-ttu-id="42e8c-128">列出 avaialbe schemaExtension defintions 及其属性。</span><span class="sxs-lookup"><span data-stu-id="42e8c-128">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="42e8c-129">Get</span><span class="sxs-lookup"><span data-stu-id="42e8c-129">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="42e8c-130">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="42e8c-130">schemaExtension</span></span> |<span data-ttu-id="42e8c-131">读取特定的 schemaExtension 定义的属性。</span><span class="sxs-lookup"><span data-stu-id="42e8c-131">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="42e8c-132">Update</span><span class="sxs-lookup"><span data-stu-id="42e8c-132">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="42e8c-133">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="42e8c-133">schemaExtension</span></span>   |<span data-ttu-id="42e8c-134">更新 schemaExtension 定义。</span><span class="sxs-lookup"><span data-stu-id="42e8c-134">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="42e8c-135">Delete</span><span class="sxs-lookup"><span data-stu-id="42e8c-135">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="42e8c-136">无</span><span class="sxs-lookup"><span data-stu-id="42e8c-136">None</span></span> |<span data-ttu-id="42e8c-137">删除 schemaExtension 定义。</span><span class="sxs-lookup"><span data-stu-id="42e8c-137">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="42e8c-138">属性</span><span class="sxs-lookup"><span data-stu-id="42e8c-138">Properties</span></span>
| <span data-ttu-id="42e8c-139">属性</span><span class="sxs-lookup"><span data-stu-id="42e8c-139">Property</span></span>     | <span data-ttu-id="42e8c-140">类型</span><span class="sxs-lookup"><span data-stu-id="42e8c-140">Type</span></span>   |<span data-ttu-id="42e8c-141">说明</span><span class="sxs-lookup"><span data-stu-id="42e8c-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42e8c-142">说明</span><span class="sxs-lookup"><span data-stu-id="42e8c-142">description</span></span>|<span data-ttu-id="42e8c-143">String</span><span class="sxs-lookup"><span data-stu-id="42e8c-143">String</span></span>|<span data-ttu-id="42e8c-144">架构扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="42e8c-144">Description for the schema extension.</span></span>|
|<span data-ttu-id="42e8c-145">id</span><span class="sxs-lookup"><span data-stu-id="42e8c-145">id</span></span>|<span data-ttu-id="42e8c-146">String</span><span class="sxs-lookup"><span data-stu-id="42e8c-146">String</span></span>|<span data-ttu-id="42e8c-147">架构扩展定义的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="42e8c-147">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="42e8c-148">你可以使用下面两种方法之一分配值：</span><span class="sxs-lookup"><span data-stu-id="42e8c-148">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="42e8c-149">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span><span class="sxs-lookup"><span data-stu-id="42e8c-149">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span> <span data-ttu-id="42e8c-150">As an example, `contoso_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="42e8c-150">As an example, `contoso_mySchema`.</span></span> </li><li><span data-ttu-id="42e8c-151">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span><span class="sxs-lookup"><span data-stu-id="42e8c-151">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span></span> <span data-ttu-id="42e8c-152">An example would be `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="42e8c-152">An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="42e8c-153">此属性一旦创建，便无法更改。</span><span class="sxs-lookup"><span data-stu-id="42e8c-153">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="42e8c-154">owner</span><span class="sxs-lookup"><span data-stu-id="42e8c-154">owner</span></span>|<span data-ttu-id="42e8c-155">String</span><span class="sxs-lookup"><span data-stu-id="42e8c-155">String</span></span>|<span data-ttu-id="42e8c-156">属于架构扩展的所有者的应用程序的 `appId`。</span><span class="sxs-lookup"><span data-stu-id="42e8c-156">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="42e8c-157">可在创建时提供此属性以设置所有者。</span><span class="sxs-lookup"><span data-stu-id="42e8c-157">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="42e8c-158">如果未提供，则会将调用应用程序的 `appId` 设置为所有者。</span><span class="sxs-lookup"><span data-stu-id="42e8c-158">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="42e8c-159">在任一情况下，已登录用户均必须是应用程序的所有者。</span><span class="sxs-lookup"><span data-stu-id="42e8c-159">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="42e8c-160">设置后，此属性为只读，且无法更改。</span><span class="sxs-lookup"><span data-stu-id="42e8c-160">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="42e8c-161">properties</span><span class="sxs-lookup"><span data-stu-id="42e8c-161">properties</span></span>|<span data-ttu-id="42e8c-162">[extensionSchemaProperty](extensionschemaproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42e8c-162">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="42e8c-163">构成架构扩展定义的属性名称和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="42e8c-163">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="42e8c-164">status</span><span class="sxs-lookup"><span data-stu-id="42e8c-164">status</span></span>|<span data-ttu-id="42e8c-165">String</span><span class="sxs-lookup"><span data-stu-id="42e8c-165">String</span></span>|<span data-ttu-id="42e8c-166">架构扩展的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="42e8c-166">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="42e8c-167">可能的状态为 **InDevelopment**、**Available** 和 **Deprecated**。</span><span class="sxs-lookup"><span data-stu-id="42e8c-167">Possible states are **InDevelopment**, **Available**, and **Deprecated**.</span></span> <span data-ttu-id="42e8c-168">创建后将自动设置为 **InDevelopment**。</span><span class="sxs-lookup"><span data-stu-id="42e8c-168">Automatically set to **InDevelopment** on creation.</span></span> <span data-ttu-id="42e8c-169">[架构扩展](/graph/extensibility-overview#schema-extensions)将提供关于可能的状态转换和行为的详细信息。</span><span class="sxs-lookup"><span data-stu-id="42e8c-169">[Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="42e8c-170">targetTypes</span><span class="sxs-lookup"><span data-stu-id="42e8c-170">targetTypes</span></span>|<span data-ttu-id="42e8c-171">String collection</span><span class="sxs-lookup"><span data-stu-id="42e8c-171">String collection</span></span>|<span data-ttu-id="42e8c-172">架构扩展适用的支持扩展的 Microsoft Graph 类型集。</span><span class="sxs-lookup"><span data-stu-id="42e8c-172">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="42e8c-173">从**administrativeUnit**、**联系人**、**设备**、**事件**、**组**、**邮件**、**组织**、**公告**或**用户**中进行选择。</span><span class="sxs-lookup"><span data-stu-id="42e8c-173">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42e8c-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42e8c-174">JSON representation</span></span>

<span data-ttu-id="42e8c-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42e8c-175">Here is a JSON representation of the resource.</span></span>

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
