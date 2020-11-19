---
title: schemaExtension 资源类型（架构扩展）
description: '可以通过架构扩展定义架构来扩展强类型的自定义数据并将其添加到资源类型。自定义数据在扩展资源上作为复杂类型显示。 '
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: 3dd12d1d595c5dbec52b21eec52ad45e6c80ce15
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352368"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="d2150-104">schemaExtension 资源类型（架构扩展）</span><span class="sxs-lookup"><span data-stu-id="d2150-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="d2150-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2150-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2150-p102">可以通过架构扩展定义架构来扩展强类型的自定义数据并将其添加到资源类型。自定义数据在扩展资源上作为复杂类型显示。</span><span class="sxs-lookup"><span data-stu-id="d2150-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="d2150-108">以下资源类型支持架构扩展：</span><span class="sxs-lookup"><span data-stu-id="d2150-108">Schema extensions are supported by the following resource types:</span></span>

- [<span data-ttu-id="d2150-109">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="d2150-109">administrativeUnit</span></span>](administrativeunit.md)
- [<span data-ttu-id="d2150-110">联系人</span><span class="sxs-lookup"><span data-stu-id="d2150-110">contact</span></span>](contact.md)
- [<span data-ttu-id="d2150-111">设备</span><span class="sxs-lookup"><span data-stu-id="d2150-111">device</span></span>](device.md)
- <span data-ttu-id="d2150-112">用户或 Microsoft 365 组日历上的[事件](event.md)。</span><span class="sxs-lookup"><span data-stu-id="d2150-112">[event](event.md) on a user or Microsoft 365 group calendar</span></span>
- <span data-ttu-id="d2150-113">Microsoft 365 组中的[帖子](post.md)</span><span class="sxs-lookup"><span data-stu-id="d2150-113">[post](post.md) of a Microsoft 365 group</span></span>
- [<span data-ttu-id="d2150-114">组</span><span class="sxs-lookup"><span data-stu-id="d2150-114">group</span></span>](group.md)
- [<span data-ttu-id="d2150-115">邮件</span><span class="sxs-lookup"><span data-stu-id="d2150-115">message</span></span>](message.md) 
- [<span data-ttu-id="d2150-116">组织</span><span class="sxs-lookup"><span data-stu-id="d2150-116">organization</span></span>](organization.md)
- [<span data-ttu-id="d2150-117">用户</span><span class="sxs-lookup"><span data-stu-id="d2150-117">user</span></span>](user.md)

<span data-ttu-id="d2150-118">请参阅[架构扩展示例](/graph/extensibility-schema-groups)了解如何将自定义数据添加到组。</span><span class="sxs-lookup"><span data-stu-id="d2150-118">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="d2150-119">方法</span><span class="sxs-lookup"><span data-stu-id="d2150-119">Methods</span></span>

| <span data-ttu-id="d2150-120">方法</span><span class="sxs-lookup"><span data-stu-id="d2150-120">Method</span></span>           | <span data-ttu-id="d2150-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2150-121">Return Type</span></span>    |<span data-ttu-id="d2150-122">说明</span><span class="sxs-lookup"><span data-stu-id="d2150-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d2150-123">Create</span><span class="sxs-lookup"><span data-stu-id="d2150-123">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="d2150-124">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="d2150-124">schemaExtension</span></span> |<span data-ttu-id="d2150-125">创建架构扩展定义。</span><span class="sxs-lookup"><span data-stu-id="d2150-125">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="d2150-126">List</span><span class="sxs-lookup"><span data-stu-id="d2150-126">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="d2150-127">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="d2150-127">schemaExtension</span></span> |<span data-ttu-id="d2150-128">列出 avaialbe schemaExtension defintions 及其属性。</span><span class="sxs-lookup"><span data-stu-id="d2150-128">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="d2150-129">Get</span><span class="sxs-lookup"><span data-stu-id="d2150-129">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="d2150-130">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="d2150-130">schemaExtension</span></span> |<span data-ttu-id="d2150-131">读取特定的 schemaExtension 定义的属性。</span><span class="sxs-lookup"><span data-stu-id="d2150-131">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="d2150-132">Update</span><span class="sxs-lookup"><span data-stu-id="d2150-132">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="d2150-133">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="d2150-133">schemaExtension</span></span>   |<span data-ttu-id="d2150-134">更新 schemaExtension 定义。</span><span class="sxs-lookup"><span data-stu-id="d2150-134">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="d2150-135">Delete</span><span class="sxs-lookup"><span data-stu-id="d2150-135">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="d2150-136">无</span><span class="sxs-lookup"><span data-stu-id="d2150-136">None</span></span> |<span data-ttu-id="d2150-137">删除 schemaExtension 定义。</span><span class="sxs-lookup"><span data-stu-id="d2150-137">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="d2150-138">属性</span><span class="sxs-lookup"><span data-stu-id="d2150-138">Properties</span></span>
| <span data-ttu-id="d2150-139">属性</span><span class="sxs-lookup"><span data-stu-id="d2150-139">Property</span></span>     | <span data-ttu-id="d2150-140">类型</span><span class="sxs-lookup"><span data-stu-id="d2150-140">Type</span></span>   |<span data-ttu-id="d2150-141">说明</span><span class="sxs-lookup"><span data-stu-id="d2150-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d2150-142">说明</span><span class="sxs-lookup"><span data-stu-id="d2150-142">description</span></span>|<span data-ttu-id="d2150-143">String</span><span class="sxs-lookup"><span data-stu-id="d2150-143">String</span></span>|<span data-ttu-id="d2150-144">架构扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="d2150-144">Description for the schema extension.</span></span>|
|<span data-ttu-id="d2150-145">id</span><span class="sxs-lookup"><span data-stu-id="d2150-145">id</span></span>|<span data-ttu-id="d2150-146">String</span><span class="sxs-lookup"><span data-stu-id="d2150-146">String</span></span>|<span data-ttu-id="d2150-147">架构扩展定义的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d2150-147">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="d2150-148">你可以使用下面两种方法之一分配值：</span><span class="sxs-lookup"><span data-stu-id="d2150-148">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="d2150-p103">连接已验证域名与架构扩展名称，形成此格式的唯一字符串：\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。例如 `contoso_mySchema`。 </span><span class="sxs-lookup"><span data-stu-id="d2150-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="d2150-p104">提供一个架构名称，并让 Microsoft Graph 使用此格式的架构名称完成 **id** 分配：ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。例如 `extkvbmkofy_mySchema`。</span><span class="sxs-lookup"><span data-stu-id="d2150-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="d2150-153">此属性一旦创建，便无法更改。</span><span class="sxs-lookup"><span data-stu-id="d2150-153">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="d2150-154">owner</span><span class="sxs-lookup"><span data-stu-id="d2150-154">owner</span></span>|<span data-ttu-id="d2150-155">String</span><span class="sxs-lookup"><span data-stu-id="d2150-155">String</span></span>| <span data-ttu-id="d2150-156">属于架构扩展的所有者的应用程序的 `appId`。</span><span class="sxs-lookup"><span data-stu-id="d2150-156">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="d2150-157">可在创建时提供此属性以设置所有者。</span><span class="sxs-lookup"><span data-stu-id="d2150-157">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="d2150-158">如果未提供，则会将调用应用程序的 `appId` 设置为所有者。</span><span class="sxs-lookup"><span data-stu-id="d2150-158">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="d2150-159">在任一情况下，已登录用户均必须是应用程序的所有者。</span><span class="sxs-lookup"><span data-stu-id="d2150-159">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="d2150-160">因此，如果使用 Graph 浏览器新建一个架构扩展定义，则 **必须** 提供 owner 属性（以此为例）。</span><span class="sxs-lookup"><span data-stu-id="d2150-160">So, for example, if creating a new schema extension definition using Graph Explorer, you **must** supply the owner property.</span></span> <span data-ttu-id="d2150-161">设置后，此属性为只读，且无法更改。</span><span class="sxs-lookup"><span data-stu-id="d2150-161">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="d2150-162">properties</span><span class="sxs-lookup"><span data-stu-id="d2150-162">properties</span></span>|<span data-ttu-id="d2150-163">[extensionSchemaProperty](extensionschemaproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2150-163">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="d2150-164">构成架构扩展定义的属性名称和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="d2150-164">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="d2150-165">status</span><span class="sxs-lookup"><span data-stu-id="d2150-165">status</span></span>|<span data-ttu-id="d2150-166">String</span><span class="sxs-lookup"><span data-stu-id="d2150-166">String</span></span>|<span data-ttu-id="d2150-167">架构扩展的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="d2150-167">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="d2150-168">可能的状态为 **InDevelopment**、**Available** 和 **Deprecated**。</span><span class="sxs-lookup"><span data-stu-id="d2150-168">Possible states are **InDevelopment**, **Available**, and **Deprecated**.</span></span> <span data-ttu-id="d2150-169">创建后将自动设置为 **InDevelopment**。</span><span class="sxs-lookup"><span data-stu-id="d2150-169">Automatically set to **InDevelopment** on creation.</span></span> <span data-ttu-id="d2150-170">[架构扩展](/graph/extensibility-overview#schema-extensions)将提供关于可能的状态转换和行为的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d2150-170">[Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="d2150-171">targetTypes</span><span class="sxs-lookup"><span data-stu-id="d2150-171">targetTypes</span></span>|<span data-ttu-id="d2150-172">String collection</span><span class="sxs-lookup"><span data-stu-id="d2150-172">String collection</span></span>|<span data-ttu-id="d2150-173">架构扩展适用的支持扩展的 Microsoft Graph 类型集。</span><span class="sxs-lookup"><span data-stu-id="d2150-173">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="d2150-174">从 **administrativeUnit**、 **联系人**、 **设备**、 **事件**、 **组**、 **邮件**、 **组织**、 **公告** 或 **用户** 中进行选择。</span><span class="sxs-lookup"><span data-stu-id="d2150-174">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2150-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2150-175">JSON representation</span></span>

<span data-ttu-id="d2150-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2150-176">Here is a JSON representation of the resource.</span></span>

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


