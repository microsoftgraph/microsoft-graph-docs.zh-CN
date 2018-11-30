---
title: schemaExtension 资源类型（架构扩展）
description: '可以通过架构扩展定义架构来扩展强类型的自定义数据并将其添加到资源类型。自定义数据在扩展资源上作为复杂类型显示。 '
ms.openlocfilehash: bb0cc70ea07501bda5fe2ae208cce048825c3aac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042330"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="c2b62-104">schemaExtension 资源类型（架构扩展）</span><span class="sxs-lookup"><span data-stu-id="c2b62-104">schemaExtension resource type (schema extensions)</span></span>

> <span data-ttu-id="c2b62-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c2b62-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2b62-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c2b62-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c2b62-p103">可以通过架构扩展定义架构来扩展强类型的自定义数据并将其添加到资源类型。自定义数据在扩展资源上作为复杂类型显示。</span><span class="sxs-lookup"><span data-stu-id="c2b62-p103">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="c2b62-109">以下资源类型支持架构扩展：</span><span class="sxs-lookup"><span data-stu-id="c2b62-109">Schema extensions are supported by the following resource types:</span></span>

 - [<span data-ttu-id="c2b62-110">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="c2b62-110">administrativeUnit</span></span>](administrativeunit.md)
 - [<span data-ttu-id="c2b62-111">联系人</span><span class="sxs-lookup"><span data-stu-id="c2b62-111">contact</span></span>](contact.md)
 - [<span data-ttu-id="c2b62-112">设备</span><span class="sxs-lookup"><span data-stu-id="c2b62-112">device</span></span>](device.md)
 - <span data-ttu-id="c2b62-113">用户或 Office 365 组日历上的[事件](event.md)。</span><span class="sxs-lookup"><span data-stu-id="c2b62-113">[event](event.md) on a user or Office 365 group calendar</span></span>
 - <span data-ttu-id="c2b62-114">Office 365 组的[帖子](post.md)</span><span class="sxs-lookup"><span data-stu-id="c2b62-114">[post](post.md) of an Office 365 group</span></span>
 - [<span data-ttu-id="c2b62-115">组</span><span class="sxs-lookup"><span data-stu-id="c2b62-115">group</span></span>](group.md)
 - [<span data-ttu-id="c2b62-116">邮件</span><span class="sxs-lookup"><span data-stu-id="c2b62-116">message</span></span>](message.md) 
 - [<span data-ttu-id="c2b62-117">组织</span><span class="sxs-lookup"><span data-stu-id="c2b62-117">organization</span></span>](organization.md)
 - [<span data-ttu-id="c2b62-118">用户</span><span class="sxs-lookup"><span data-stu-id="c2b62-118">user</span></span>](user.md)

<span data-ttu-id="c2b62-119">请参阅[架构扩展示例](/graph/extensibility-schema-groups)了解如何将自定义数据添加到组。</span><span class="sxs-lookup"><span data-stu-id="c2b62-119">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="c2b62-120">方法</span><span class="sxs-lookup"><span data-stu-id="c2b62-120">Methods</span></span>

| <span data-ttu-id="c2b62-121">方法</span><span class="sxs-lookup"><span data-stu-id="c2b62-121">Method</span></span>           | <span data-ttu-id="c2b62-122">返回类型</span><span class="sxs-lookup"><span data-stu-id="c2b62-122">Return Type</span></span>    |<span data-ttu-id="c2b62-123">说明</span><span class="sxs-lookup"><span data-stu-id="c2b62-123">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c2b62-124">Create</span><span class="sxs-lookup"><span data-stu-id="c2b62-124">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="c2b62-125">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="c2b62-125">schemaExtension</span></span> |<span data-ttu-id="c2b62-126">创建架构扩展定义。</span><span class="sxs-lookup"><span data-stu-id="c2b62-126">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="c2b62-127">List</span><span class="sxs-lookup"><span data-stu-id="c2b62-127">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="c2b62-128">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="c2b62-128">schemaExtension</span></span> |<span data-ttu-id="c2b62-129">列出 avaialbe schemaExtension 定义和及其属性。</span><span class="sxs-lookup"><span data-stu-id="c2b62-129">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="c2b62-130">Get</span><span class="sxs-lookup"><span data-stu-id="c2b62-130">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="c2b62-131">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="c2b62-131">schemaExtension</span></span> |<span data-ttu-id="c2b62-132">读取特定的 schemaExtension 定义的属性。</span><span class="sxs-lookup"><span data-stu-id="c2b62-132">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="c2b62-133">Update</span><span class="sxs-lookup"><span data-stu-id="c2b62-133">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="c2b62-134">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="c2b62-134">schemaExtension</span></span>   |<span data-ttu-id="c2b62-135">更新 schemaExtension 定义。</span><span class="sxs-lookup"><span data-stu-id="c2b62-135">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="c2b62-136">Delete</span><span class="sxs-lookup"><span data-stu-id="c2b62-136">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="c2b62-137">无</span><span class="sxs-lookup"><span data-stu-id="c2b62-137">None</span></span> |<span data-ttu-id="c2b62-138">删除 schemaExtension 定义。</span><span class="sxs-lookup"><span data-stu-id="c2b62-138">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="c2b62-139">属性</span><span class="sxs-lookup"><span data-stu-id="c2b62-139">Properties</span></span>
| <span data-ttu-id="c2b62-140">属性</span><span class="sxs-lookup"><span data-stu-id="c2b62-140">Property</span></span>     | <span data-ttu-id="c2b62-141">类型</span><span class="sxs-lookup"><span data-stu-id="c2b62-141">Type</span></span>   |<span data-ttu-id="c2b62-142">说明</span><span class="sxs-lookup"><span data-stu-id="c2b62-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2b62-143">说明</span><span class="sxs-lookup"><span data-stu-id="c2b62-143">description</span></span>|<span data-ttu-id="c2b62-144">String</span><span class="sxs-lookup"><span data-stu-id="c2b62-144">String</span></span>|<span data-ttu-id="c2b62-145">架构扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="c2b62-145">Description for the schema extension.</span></span>|
|<span data-ttu-id="c2b62-146">id</span><span class="sxs-lookup"><span data-stu-id="c2b62-146">id</span></span>|<span data-ttu-id="c2b62-147">String</span><span class="sxs-lookup"><span data-stu-id="c2b62-147">String</span></span>|<span data-ttu-id="c2b62-148">架构扩展定义的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c2b62-148">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="c2b62-149">你可以使用下面两种方法之一分配值：</span><span class="sxs-lookup"><span data-stu-id="c2b62-149">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="c2b62-p104">连接已验证域名与架构扩展名称，形成此格式的唯一字符串：\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。例如 `contoso_mySchema`。 </span><span class="sxs-lookup"><span data-stu-id="c2b62-p104">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="c2b62-p105">提供一个架构名称，并让 Microsoft Graph 使用此格式的架构名称完成 **id** 分配：ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。例如 `extkvbmkofy_mySchema`。</span><span class="sxs-lookup"><span data-stu-id="c2b62-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="c2b62-154">此属性一旦创建，便无法更改。</span><span class="sxs-lookup"><span data-stu-id="c2b62-154">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="c2b62-155">owner</span><span class="sxs-lookup"><span data-stu-id="c2b62-155">owner</span></span>|<span data-ttu-id="c2b62-156">String</span><span class="sxs-lookup"><span data-stu-id="c2b62-156">String</span></span>|<span data-ttu-id="c2b62-157">属于架构扩展的所有者的应用程序的 `appId`。</span><span class="sxs-lookup"><span data-stu-id="c2b62-157">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="c2b62-158">可在创建时提供此属性以设置所有者。</span><span class="sxs-lookup"><span data-stu-id="c2b62-158">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="c2b62-159">如果未提供，则会将调用应用程序的 `appId` 设置为所有者。</span><span class="sxs-lookup"><span data-stu-id="c2b62-159">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="c2b62-160">在任一情况下，已登录用户均必须是应用程序的所有者。</span><span class="sxs-lookup"><span data-stu-id="c2b62-160">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="c2b62-161">设置后，此属性为只读，且无法更改。</span><span class="sxs-lookup"><span data-stu-id="c2b62-161">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="c2b62-162">properties</span><span class="sxs-lookup"><span data-stu-id="c2b62-162">properties</span></span>|<span data-ttu-id="c2b62-163">[extensionSchemaProperty](extensionschemaproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c2b62-163">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="c2b62-164">构成架构扩展定义的属性名称和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="c2b62-164">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="c2b62-165">status</span><span class="sxs-lookup"><span data-stu-id="c2b62-165">status</span></span>|<span data-ttu-id="c2b62-166">字符串</span><span class="sxs-lookup"><span data-stu-id="c2b62-166">String</span></span>|<span data-ttu-id="c2b62-p107">架构扩展的生命周期状态。可能的值为 **InDevelopment**、**Available** 和 **Deprecated**。创建后将自动设置为 **InDevelopment**。[架构扩展](/graph/extensibility-overview#schema-extensions)将提供关于可能的状态转换和行为的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c2b62-p107">The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="c2b62-171">targetTypes</span><span class="sxs-lookup"><span data-stu-id="c2b62-171">targetTypes</span></span>|<span data-ttu-id="c2b62-172">String collection</span><span class="sxs-lookup"><span data-stu-id="c2b62-172">String collection</span></span>|<span data-ttu-id="c2b62-173">架构扩展适用的支持扩展的 Microsoft Graph 类型集。</span><span class="sxs-lookup"><span data-stu-id="c2b62-173">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="c2b62-174">从**administrativeUnit**、**联系人**、**设备**、**事件**、**组**、**消息**、**组织**、**发布**或**用户**选择。</span><span class="sxs-lookup"><span data-stu-id="c2b62-174">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2b62-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2b62-175">JSON representation</span></span>

<span data-ttu-id="c2b62-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2b62-176">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "schemaExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->