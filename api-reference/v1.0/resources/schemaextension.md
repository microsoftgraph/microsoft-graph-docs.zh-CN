---
title: schemaExtension 资源类型（架构扩展）
description: '可以通过架构扩展定义架构来扩展强类型的自定义数据并将其添加到资源类型。自定义数据在扩展资源上作为复杂类型显示。 '
localization_priority: Priority
author: dkershaw10
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7c0bf49bc0de24cda47e309fdbfb1c4e75b42283
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034613"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="1ea71-104">schemaExtension 资源类型（架构扩展）</span><span class="sxs-lookup"><span data-stu-id="1ea71-104">schemaExtension resource type (schema extensions)</span></span>

<span data-ttu-id="1ea71-p102">可以通过架构扩展定义架构来扩展强类型的自定义数据并将其添加到资源类型。自定义数据在扩展资源上作为复杂类型显示。</span><span class="sxs-lookup"><span data-stu-id="1ea71-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="1ea71-107">以下资源类型支持架构扩展：</span><span class="sxs-lookup"><span data-stu-id="1ea71-107">Schema extensions are supported by the following resource types:</span></span>

- [<span data-ttu-id="1ea71-108">联系人</span><span class="sxs-lookup"><span data-stu-id="1ea71-108">contact</span></span>](contact.md)
- [<span data-ttu-id="1ea71-109">设备</span><span class="sxs-lookup"><span data-stu-id="1ea71-109">device</span></span>](device.md)
- <span data-ttu-id="1ea71-110">用户或 Office 365 组日历上的[事件](event.md)。</span><span class="sxs-lookup"><span data-stu-id="1ea71-110">[event](event.md) on a user or Office 365 group calendar</span></span>
- <span data-ttu-id="1ea71-111">Office 365 组的[帖子](post.md)</span><span class="sxs-lookup"><span data-stu-id="1ea71-111">[post](post.md) of an Office 365 group</span></span>
- [<span data-ttu-id="1ea71-112">组</span><span class="sxs-lookup"><span data-stu-id="1ea71-112">group</span></span>](group.md)
- [<span data-ttu-id="1ea71-113">邮件</span><span class="sxs-lookup"><span data-stu-id="1ea71-113">message</span></span>](message.md) 
- [<span data-ttu-id="1ea71-114">组织</span><span class="sxs-lookup"><span data-stu-id="1ea71-114">organization</span></span>](organization.md)
- [<span data-ttu-id="1ea71-115">用户</span><span class="sxs-lookup"><span data-stu-id="1ea71-115">user</span></span>](user.md)

<span data-ttu-id="1ea71-116">请参阅[架构扩展示例](/graph/extensibility-schema-groups)了解如何将自定义数据添加到组。</span><span class="sxs-lookup"><span data-stu-id="1ea71-116">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="1ea71-117">方法</span><span class="sxs-lookup"><span data-stu-id="1ea71-117">Methods</span></span>

| <span data-ttu-id="1ea71-118">方法</span><span class="sxs-lookup"><span data-stu-id="1ea71-118">Method</span></span>           | <span data-ttu-id="1ea71-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="1ea71-119">Return Type</span></span>    |<span data-ttu-id="1ea71-120">说明</span><span class="sxs-lookup"><span data-stu-id="1ea71-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1ea71-121">Create</span><span class="sxs-lookup"><span data-stu-id="1ea71-121">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="1ea71-122">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="1ea71-122">schemaExtension</span></span> |<span data-ttu-id="1ea71-123">创建架构扩展定义。</span><span class="sxs-lookup"><span data-stu-id="1ea71-123">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="1ea71-124">List</span><span class="sxs-lookup"><span data-stu-id="1ea71-124">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="1ea71-125">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="1ea71-125">schemaExtension</span></span> |<span data-ttu-id="1ea71-126">列出可用的 schemaExtension 定义及其属性。</span><span class="sxs-lookup"><span data-stu-id="1ea71-126">List the available schemaExtension definitions and their properties.</span></span>|
|[<span data-ttu-id="1ea71-127">Get</span><span class="sxs-lookup"><span data-stu-id="1ea71-127">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="1ea71-128">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="1ea71-128">schemaExtension</span></span> |<span data-ttu-id="1ea71-129">读取特定的 schemaExtension 定义的属性。</span><span class="sxs-lookup"><span data-stu-id="1ea71-129">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="1ea71-130">Update</span><span class="sxs-lookup"><span data-stu-id="1ea71-130">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="1ea71-131">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="1ea71-131">schemaExtension</span></span>   |<span data-ttu-id="1ea71-132">更新 schemaExtension 定义。</span><span class="sxs-lookup"><span data-stu-id="1ea71-132">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="1ea71-133">Delete</span><span class="sxs-lookup"><span data-stu-id="1ea71-133">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="1ea71-134">无</span><span class="sxs-lookup"><span data-stu-id="1ea71-134">None</span></span> |<span data-ttu-id="1ea71-135">删除 schemaExtension 定义。</span><span class="sxs-lookup"><span data-stu-id="1ea71-135">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="1ea71-136">属性</span><span class="sxs-lookup"><span data-stu-id="1ea71-136">Properties</span></span>
| <span data-ttu-id="1ea71-137">属性</span><span class="sxs-lookup"><span data-stu-id="1ea71-137">Property</span></span>     | <span data-ttu-id="1ea71-138">类型</span><span class="sxs-lookup"><span data-stu-id="1ea71-138">Type</span></span>   |<span data-ttu-id="1ea71-139">说明</span><span class="sxs-lookup"><span data-stu-id="1ea71-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ea71-140">说明</span><span class="sxs-lookup"><span data-stu-id="1ea71-140">description</span></span>|<span data-ttu-id="1ea71-141">String</span><span class="sxs-lookup"><span data-stu-id="1ea71-141">String</span></span>|<span data-ttu-id="1ea71-142">架构扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="1ea71-142">Description for the schema extension.</span></span>|
|<span data-ttu-id="1ea71-143">id</span><span class="sxs-lookup"><span data-stu-id="1ea71-143">id</span></span>|<span data-ttu-id="1ea71-144">String</span><span class="sxs-lookup"><span data-stu-id="1ea71-144">String</span></span>|<span data-ttu-id="1ea71-145">架构扩展定义的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1ea71-145">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="1ea71-146">你可以使用下面两种方法之一分配值：</span><span class="sxs-lookup"><span data-stu-id="1ea71-146">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="1ea71-p103">连接已验证域名与架构扩展名称，形成此格式的唯一字符串：\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。例如 `contoso_mySchema`。 </span><span class="sxs-lookup"><span data-stu-id="1ea71-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="1ea71-p104">提供一个架构名称，并让 Microsoft Graph 使用此格式的架构名称完成 **id** 分配：ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。例如 `extkvbmkofy_mySchema`。</span><span class="sxs-lookup"><span data-stu-id="1ea71-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="1ea71-151">此属性一旦创建，便无法更改。</span><span class="sxs-lookup"><span data-stu-id="1ea71-151">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="1ea71-152">owner</span><span class="sxs-lookup"><span data-stu-id="1ea71-152">owner</span></span>|<span data-ttu-id="1ea71-153">String</span><span class="sxs-lookup"><span data-stu-id="1ea71-153">String</span></span>|<span data-ttu-id="1ea71-154">属于架构扩展的所有者的应用程序的 `appId`。</span><span class="sxs-lookup"><span data-stu-id="1ea71-154">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="1ea71-155">可在创建时提供此属性以设置所有者。</span><span class="sxs-lookup"><span data-stu-id="1ea71-155">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="1ea71-156">如果未提供，则会将调用应用程序的 `appId` 设置为所有者。</span><span class="sxs-lookup"><span data-stu-id="1ea71-156">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="1ea71-157">在任一情况下，已登录用户均必须是应用程序的所有者。</span><span class="sxs-lookup"><span data-stu-id="1ea71-157">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="1ea71-158">设置后，此属性为只读，且无法更改。</span><span class="sxs-lookup"><span data-stu-id="1ea71-158">Once set, this property is read-only and cannot be changed.</span></span>| 
|<span data-ttu-id="1ea71-159">properties</span><span class="sxs-lookup"><span data-stu-id="1ea71-159">properties</span></span>|<span data-ttu-id="1ea71-160">[extensionSchemaProperty](extensionschemaproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ea71-160">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="1ea71-161">构成架构扩展定义的属性名称和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="1ea71-161">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="1ea71-162">status</span><span class="sxs-lookup"><span data-stu-id="1ea71-162">status</span></span>|<span data-ttu-id="1ea71-163">String</span><span class="sxs-lookup"><span data-stu-id="1ea71-163">String</span></span>|<span data-ttu-id="1ea71-164">架构扩展的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="1ea71-164">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="1ea71-165">可能的状态为 **InDevelopment**、**Available** 和 **Deprecated**。</span><span class="sxs-lookup"><span data-stu-id="1ea71-165">Possible states are **InDevelopment**, **Available**, and **Deprecated**.</span></span> <span data-ttu-id="1ea71-166">创建后将自动设置为 **InDevelopment**。</span><span class="sxs-lookup"><span data-stu-id="1ea71-166">Automatically set to **InDevelopment** on creation.</span></span> <span data-ttu-id="1ea71-167">[架构扩展](/graph/extensibility-overview#schema-extensions)将提供关于可能的状态转换和行为的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1ea71-167">[Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="1ea71-168">targetTypes</span><span class="sxs-lookup"><span data-stu-id="1ea71-168">targetTypes</span></span>|<span data-ttu-id="1ea71-169">String collection</span><span class="sxs-lookup"><span data-stu-id="1ea71-169">String collection</span></span>|<span data-ttu-id="1ea71-170">架构扩展适用的支持扩展的 Microsoft Graph 类型集。</span><span class="sxs-lookup"><span data-stu-id="1ea71-170">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="1ea71-171">从**联系人**、**设备**、**事件**、**组**、**邮件**、**组织**、**帖子**或**用户**中选择。</span><span class="sxs-lookup"><span data-stu-id="1ea71-171">Select from **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ea71-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ea71-172">JSON representation</span></span>

<span data-ttu-id="1ea71-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ea71-173">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
