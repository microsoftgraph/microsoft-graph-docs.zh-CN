---
title: schemaExtension 资源类型（架构扩展）
description: '可以通过架构扩展定义架构来扩展强类型的自定义数据并将其添加到资源类型。自定义数据在扩展资源上作为复杂类型显示。 '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 90acbfb0e7a6b031303ae3286f1a5ed366a2a8c9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523853"
---
# <a name="schemaextension-resource-type-schema-extensions"></a><span data-ttu-id="c5fa7-104">schemaExtension 资源类型（架构扩展）</span><span class="sxs-lookup"><span data-stu-id="c5fa7-104">schemaExtension resource type (schema extensions)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5fa7-p102">可以通过架构扩展定义架构来扩展强类型的自定义数据并将其添加到资源类型。自定义数据在扩展资源上作为复杂类型显示。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-p102">Schema extensions allow you to define a schema to extend and add strongly-typed custom data to a resource type. The custom data appears as a complex type on the extended resource.</span></span> 

<span data-ttu-id="c5fa7-107">以下资源类型支持架构扩展：</span><span class="sxs-lookup"><span data-stu-id="c5fa7-107">Schema extensions are supported by the following resource types:</span></span>

 - [<span data-ttu-id="c5fa7-108">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="c5fa7-108">administrativeUnit</span></span>](administrativeunit.md)
 - [<span data-ttu-id="c5fa7-109">联系人</span><span class="sxs-lookup"><span data-stu-id="c5fa7-109">contact</span></span>](contact.md)
 - [<span data-ttu-id="c5fa7-110">设备</span><span class="sxs-lookup"><span data-stu-id="c5fa7-110">device</span></span>](device.md)
 - <span data-ttu-id="c5fa7-111">用户或 Office 365 组日历上的[事件](event.md)。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-111">[event](event.md) on a user or Office 365 group calendar</span></span>
 - <span data-ttu-id="c5fa7-112">Office 365 组的[帖子](post.md)</span><span class="sxs-lookup"><span data-stu-id="c5fa7-112">[post](post.md) of an Office 365 group</span></span>
 - [<span data-ttu-id="c5fa7-113">组</span><span class="sxs-lookup"><span data-stu-id="c5fa7-113">group</span></span>](group.md)
 - [<span data-ttu-id="c5fa7-114">邮件</span><span class="sxs-lookup"><span data-stu-id="c5fa7-114">message</span></span>](message.md) 
 - [<span data-ttu-id="c5fa7-115">组织</span><span class="sxs-lookup"><span data-stu-id="c5fa7-115">organization</span></span>](organization.md)
 - [<span data-ttu-id="c5fa7-116">用户</span><span class="sxs-lookup"><span data-stu-id="c5fa7-116">user</span></span>](user.md)

<span data-ttu-id="c5fa7-117">请参阅[架构扩展示例](/graph/extensibility-schema-groups)了解如何将自定义数据添加到组。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-117">See the [schema extension example](/graph/extensibility-schema-groups) to learn how to add custom data to groups.</span></span>

## <a name="methods"></a><span data-ttu-id="c5fa7-118">方法</span><span class="sxs-lookup"><span data-stu-id="c5fa7-118">Methods</span></span>

| <span data-ttu-id="c5fa7-119">方法</span><span class="sxs-lookup"><span data-stu-id="c5fa7-119">Method</span></span>           | <span data-ttu-id="c5fa7-120">返回类型</span><span class="sxs-lookup"><span data-stu-id="c5fa7-120">Return Type</span></span>    |<span data-ttu-id="c5fa7-121">说明</span><span class="sxs-lookup"><span data-stu-id="c5fa7-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c5fa7-122">Create</span><span class="sxs-lookup"><span data-stu-id="c5fa7-122">Create</span></span>](../api/schemaextension-post-schemaextensions.md) | <span data-ttu-id="c5fa7-123">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="c5fa7-123">schemaExtension</span></span> |<span data-ttu-id="c5fa7-124">创建架构扩展定义。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-124">Create a schema extension definition.</span></span>|
|[<span data-ttu-id="c5fa7-125">List</span><span class="sxs-lookup"><span data-stu-id="c5fa7-125">List</span></span>](../api/schemaextension-list.md) | <span data-ttu-id="c5fa7-126">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="c5fa7-126">schemaExtension</span></span> |<span data-ttu-id="c5fa7-127">列出 avaialbe schemaExtension 定义和及其属性。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-127">List the avaialbe schemaExtension defintions and their properties.</span></span>|
|[<span data-ttu-id="c5fa7-128">Get</span><span class="sxs-lookup"><span data-stu-id="c5fa7-128">Get</span></span>](../api/schemaextension-get.md) | <span data-ttu-id="c5fa7-129">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="c5fa7-129">schemaExtension</span></span> |<span data-ttu-id="c5fa7-130">读取特定的 schemaExtension 定义的属性。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-130">Read the properties of a specific schemaExtension definition.</span></span>|
|[<span data-ttu-id="c5fa7-131">Update</span><span class="sxs-lookup"><span data-stu-id="c5fa7-131">Update</span></span>](../api/schemaextension-update.md) | <span data-ttu-id="c5fa7-132">schemaExtension</span><span class="sxs-lookup"><span data-stu-id="c5fa7-132">schemaExtension</span></span>   |<span data-ttu-id="c5fa7-133">更新 schemaExtension 定义。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-133">Update a schemaExtension definition.</span></span> |
|[<span data-ttu-id="c5fa7-134">Delete</span><span class="sxs-lookup"><span data-stu-id="c5fa7-134">Delete</span></span>](../api/schemaextension-delete.md) | <span data-ttu-id="c5fa7-135">无</span><span class="sxs-lookup"><span data-stu-id="c5fa7-135">None</span></span> |<span data-ttu-id="c5fa7-136">删除 schemaExtension 定义。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-136">Delete a schemaExtension definition.</span></span> |

## <a name="properties"></a><span data-ttu-id="c5fa7-137">属性</span><span class="sxs-lookup"><span data-stu-id="c5fa7-137">Properties</span></span>
| <span data-ttu-id="c5fa7-138">属性</span><span class="sxs-lookup"><span data-stu-id="c5fa7-138">Property</span></span>     | <span data-ttu-id="c5fa7-139">类型</span><span class="sxs-lookup"><span data-stu-id="c5fa7-139">Type</span></span>   |<span data-ttu-id="c5fa7-140">说明</span><span class="sxs-lookup"><span data-stu-id="c5fa7-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5fa7-141">说明</span><span class="sxs-lookup"><span data-stu-id="c5fa7-141">description</span></span>|<span data-ttu-id="c5fa7-142">字符串</span><span class="sxs-lookup"><span data-stu-id="c5fa7-142">String</span></span>|<span data-ttu-id="c5fa7-143">架构扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-143">Description for the schema extension.</span></span>|
|<span data-ttu-id="c5fa7-144">id</span><span class="sxs-lookup"><span data-stu-id="c5fa7-144">id</span></span>|<span data-ttu-id="c5fa7-145">字串符号</span><span class="sxs-lookup"><span data-stu-id="c5fa7-145">String</span></span>|<span data-ttu-id="c5fa7-146">架构扩展定义的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-146">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="c5fa7-147">你可以使用下面两种方法之一分配值：</span><span class="sxs-lookup"><span data-stu-id="c5fa7-147">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="c5fa7-p103">连接已验证域名与架构扩展名称，形成此格式的唯一字符串：\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。例如 `contoso_mySchema`。 </span><span class="sxs-lookup"><span data-stu-id="c5fa7-p103">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="c5fa7-p104">提供一个架构名称，并让 Microsoft Graph 使用此格式的架构名称完成 **id** 分配：ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。例如 `extkvbmkofy_mySchema`。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-p104">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="c5fa7-152">此属性一旦创建，便无法更改。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-152">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="c5fa7-153">owner</span><span class="sxs-lookup"><span data-stu-id="c5fa7-153">owner</span></span>|<span data-ttu-id="c5fa7-154">String</span><span class="sxs-lookup"><span data-stu-id="c5fa7-154">String</span></span>|<span data-ttu-id="c5fa7-155">属于架构扩展的所有者的应用程序的 `appId`。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-155">The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="c5fa7-156">可在创建时提供此属性以设置所有者。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-156">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="c5fa7-157">如果未提供，则会将调用应用程序的 `appId` 设置为所有者。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-157">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="c5fa7-158">在任一情况下，已登录用户均必须是应用程序的所有者。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-158">In either case, the signed-in user must be the owner of the application.</span></span> <span data-ttu-id="c5fa7-159">设置后，此属性为只读，且无法更改。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-159">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="c5fa7-160">properties</span><span class="sxs-lookup"><span data-stu-id="c5fa7-160">properties</span></span>|<span data-ttu-id="c5fa7-161">[extensionSchemaProperty](extensionschemaproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c5fa7-161">[extensionSchemaProperty](extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="c5fa7-162">构成架构扩展定义的属性名称和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-162">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="c5fa7-163">status</span><span class="sxs-lookup"><span data-stu-id="c5fa7-163">status</span></span>|<span data-ttu-id="c5fa7-164">String</span><span class="sxs-lookup"><span data-stu-id="c5fa7-164">String</span></span>|<span data-ttu-id="c5fa7-p106">架构扩展的生命周期状态。可能的值为 **InDevelopment**、**Available** 和 **Deprecated**。创建后将自动设置为 **InDevelopment**。[架构扩展](/graph/extensibility-overview#schema-extensions)将提供关于可能的状态转换和行为的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-p106">The lifecycle state of the schema extension. Possible states are **InDevelopment**, **Available**, and **Deprecated**. Automatically set to **InDevelopment** on creation. [Schema extensions](/graph/extensibility-overview#schema-extensions) provides more information on the possible state transitions and behaviors.</span></span>|
|<span data-ttu-id="c5fa7-169">targetTypes</span><span class="sxs-lookup"><span data-stu-id="c5fa7-169">targetTypes</span></span>|<span data-ttu-id="c5fa7-170">String collection</span><span class="sxs-lookup"><span data-stu-id="c5fa7-170">String collection</span></span>|<span data-ttu-id="c5fa7-171">架构扩展适用的支持扩展的 Microsoft Graph 类型集。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-171">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span> <span data-ttu-id="c5fa7-172">从**administrativeUnit**、**联系人**、**设备**、**事件**、**组**、**消息**、**组织**、**发布**或**用户**选择。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-172">Select from **administrativeUnit**, **contact**, **device**, **event**, **group**, **message**, **organization**, **post**, or **user**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5fa7-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5fa7-173">JSON representation</span></span>

<span data-ttu-id="c5fa7-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5fa7-174">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/schemaextension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
