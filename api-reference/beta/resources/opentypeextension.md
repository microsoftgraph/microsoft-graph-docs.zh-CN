---
title: openTypeExtension 资源类型（开放扩展）
description: 借助开放扩展（旧称为“Office 365 数据扩展”），可以直接将泛型属性轻松添加到 Microsoft Graph 中的资源。
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: de3a4fa33e44788442d0a2ccf1abb4df80e0ea0d
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516697"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="a7c60-103">openTypeExtension 资源类型（开放扩展）</span><span class="sxs-lookup"><span data-stu-id="a7c60-103">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="a7c60-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7c60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7c60-105">借助开放扩展（旧称为“Office 365 数据扩展”），可以直接将泛型属性轻松添加到 Microsoft Graph 中的资源。</span><span class="sxs-lookup"><span data-stu-id="a7c60-105">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>
<span data-ttu-id="a7c60-106">开放扩展由 **openTypeExtension** 资源表示。</span><span class="sxs-lookup"><span data-stu-id="a7c60-106">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="a7c60-107">添加到资源的所有开放扩展都会显示在派生自 [extension](extension.md) 抽象类型的 **extensions** 导航属性中。</span><span class="sxs-lookup"><span data-stu-id="a7c60-107">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span>  <span data-ttu-id="a7c60-108">每个扩展都有 **extensionName** 属性（这是所有扩展的预定义唯一可写属性）和自定义数据。</span><span class="sxs-lookup"><span data-stu-id="a7c60-108">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span> <span data-ttu-id="a7c60-109">一种有助于确保扩展名称唯一性的方法是，使用反向域名系统 (DNS) 格式，此格式依赖 _用户自己的域_。例如，`Com.Contoso.ContactInfo`。</span><span class="sxs-lookup"><span data-stu-id="a7c60-109">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="a7c60-110">请勿在扩展名称中使用 Microsoft 域（`Com.Microsoft` 或 `Com.OnMicrosoft`）。</span><span class="sxs-lookup"><span data-stu-id="a7c60-110">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="a7c60-111">开放扩展示例：[使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)</span><span class="sxs-lookup"><span data-stu-id="a7c60-111">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="a7c60-112">一般可用性（GA: /v1.0 和 /beta）或预览版 (/beta) 对应版本中的以下资源支持开放扩展。</span><span class="sxs-lookup"><span data-stu-id="a7c60-112">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

| <span data-ttu-id="a7c60-113">资源</span><span class="sxs-lookup"><span data-stu-id="a7c60-113">Resource</span></span> | <span data-ttu-id="a7c60-114">版本</span><span class="sxs-lookup"><span data-stu-id="a7c60-114">Version</span></span> |
|---------------|-------|
| [<span data-ttu-id="a7c60-115">管理单元</span><span class="sxs-lookup"><span data-stu-id="a7c60-115">Administrative unit</span></span>](administrativeunit.md)  | <span data-ttu-id="a7c60-116">GA</span><span class="sxs-lookup"><span data-stu-id="a7c60-116">GA</span></span> |
| [<span data-ttu-id="a7c60-117">日历事件</span><span class="sxs-lookup"><span data-stu-id="a7c60-117">Calendar event</span></span>](event.md) | <span data-ttu-id="a7c60-118">GA</span><span class="sxs-lookup"><span data-stu-id="a7c60-118">GA</span></span> |
| <span data-ttu-id="a7c60-119">组[日历事件](event.md)</span><span class="sxs-lookup"><span data-stu-id="a7c60-119">Group [calendar event](event.md)</span></span> | <span data-ttu-id="a7c60-120">GA</span><span class="sxs-lookup"><span data-stu-id="a7c60-120">GA</span></span> |
| <span data-ttu-id="a7c60-121">组对话线程[帖子](post.md)</span><span class="sxs-lookup"><span data-stu-id="a7c60-121">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="a7c60-122">GA</span><span class="sxs-lookup"><span data-stu-id="a7c60-122">GA</span></span> |
| [<span data-ttu-id="a7c60-123">设备</span><span class="sxs-lookup"><span data-stu-id="a7c60-123">Device</span></span>](device.md) | <span data-ttu-id="a7c60-124">GA</span><span class="sxs-lookup"><span data-stu-id="a7c60-124">GA</span></span> |
| [<span data-ttu-id="a7c60-125">组</span><span class="sxs-lookup"><span data-stu-id="a7c60-125">Group</span></span>](group.md) | <span data-ttu-id="a7c60-126">GA</span><span class="sxs-lookup"><span data-stu-id="a7c60-126">GA</span></span> |
| [<span data-ttu-id="a7c60-127">邮件</span><span class="sxs-lookup"><span data-stu-id="a7c60-127">Message</span></span>](message.md) | <span data-ttu-id="a7c60-128">GA</span><span class="sxs-lookup"><span data-stu-id="a7c60-128">GA</span></span> |
| [<span data-ttu-id="a7c60-129">组织</span><span class="sxs-lookup"><span data-stu-id="a7c60-129">Organization</span></span>](organization.md) | <span data-ttu-id="a7c60-130">GA</span><span class="sxs-lookup"><span data-stu-id="a7c60-130">GA</span></span> |
| [<span data-ttu-id="a7c60-131">个人联系人</span><span class="sxs-lookup"><span data-stu-id="a7c60-131">Personal contact</span></span>](contact.md) | <span data-ttu-id="a7c60-132">GA</span><span class="sxs-lookup"><span data-stu-id="a7c60-132">GA</span></span> |
| [<span data-ttu-id="a7c60-133">用户</span><span class="sxs-lookup"><span data-stu-id="a7c60-133">User</span></span>](user.md) | <span data-ttu-id="a7c60-134">GA</span><span class="sxs-lookup"><span data-stu-id="a7c60-134">GA</span></span> |
| [<span data-ttu-id="a7c60-135">任务</span><span class="sxs-lookup"><span data-stu-id="a7c60-135">Task</span></span>](todotask.md)  | <span data-ttu-id="a7c60-136">GA</span><span class="sxs-lookup"><span data-stu-id="a7c60-136">GA</span></span> |
| [<span data-ttu-id="a7c60-137">任务列表</span><span class="sxs-lookup"><span data-stu-id="a7c60-137">Task list</span></span>](todotasklist.md)  | <span data-ttu-id="a7c60-138">GA</span><span class="sxs-lookup"><span data-stu-id="a7c60-138">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="a7c60-139">Outlook 特定注意事项</span><span class="sxs-lookup"><span data-stu-id="a7c60-139">Outlook-specific considerations</span></span>

<span data-ttu-id="a7c60-140">Outlook 资源（事件、邮件或个人联系人）上存在每个开放扩展均存储在 [MAPI 命名属性](/office/client-developer/outlook/mapi/mapi-named-properties)中。</span><span class="sxs-lookup"><span data-stu-id="a7c60-140">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](/office/client-developer/outlook/mapi/mapi-named-properties).</span></span> <span data-ttu-id="a7c60-141">为 Outlook 创建开放扩展时，请考虑 MAPI 命名属性为用户邮箱中的有限资源。</span><span class="sxs-lookup"><span data-stu-id="a7c60-141">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="a7c60-142">当用户的命名属性配额用尽后，无法再为该用户创建任何其他命名属性。</span><span class="sxs-lookup"><span data-stu-id="a7c60-142">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="a7c60-143">这可能会导致依赖命名属性工作的客户端中出现异常行为。</span><span class="sxs-lookup"><span data-stu-id="a7c60-143">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="a7c60-144">在 Outlook 资源中创建开放扩展时，请遵循以下指导原则：</span><span class="sxs-lookup"><span data-stu-id="a7c60-144">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="a7c60-145">创建所需的最少数量的扩展。</span><span class="sxs-lookup"><span data-stu-id="a7c60-145">Create the minimum number of extensions required.</span></span> <span data-ttu-id="a7c60-146">大多数应用程序只需要一个扩展。</span><span class="sxs-lookup"><span data-stu-id="a7c60-146">Most applications should require no more than one extension.</span></span> <span data-ttu-id="a7c60-147">扩展未设定定义的属性或结构，因此，可以在一个扩展中存储多个值。</span><span class="sxs-lookup"><span data-stu-id="a7c60-147">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="a7c60-148">避免以可变方式命名扩展，如基于用户输入等。</span><span class="sxs-lookup"><span data-stu-id="a7c60-148">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="a7c60-149">每次使用用户邮箱中先前未使用过的新名称创建开放扩展时，将会创建新的 MAP 命名属性。</span><span class="sxs-lookup"><span data-stu-id="a7c60-149">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="a7c60-150">删除扩展不会删除命名属性。</span><span class="sxs-lookup"><span data-stu-id="a7c60-150">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="a7c60-151">使用开放扩展（针对 Outlook 资源）或扩展属性</span><span class="sxs-lookup"><span data-stu-id="a7c60-151">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="a7c60-152">开放扩展是大部分涉及存储和访问自定义数据的应用场景的推荐解决方案。</span><span class="sxs-lookup"><span data-stu-id="a7c60-152">Open extensions are the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="a7c60-153">不过，如果需要访问尚未通过 [Microsoft Graph API 元数据](../index.md)公开的 Outlook MAPI 属性的自定义数据，则可以使用[扩展属性及其 REST API](extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="a7c60-153">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](../index.md), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="a7c60-154">若要确认元数据公开了哪些属性，请访问 [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata)。</span><span class="sxs-lookup"><span data-stu-id="a7c60-154">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7c60-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7c60-155">JSON representation</span></span>

<span data-ttu-id="a7c60-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7c60-156">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}
```

## <a name="properties"></a><span data-ttu-id="a7c60-157">属性</span><span class="sxs-lookup"><span data-stu-id="a7c60-157">Properties</span></span>

| <span data-ttu-id="a7c60-158">属性</span><span class="sxs-lookup"><span data-stu-id="a7c60-158">Property</span></span> | <span data-ttu-id="a7c60-159">类型</span><span class="sxs-lookup"><span data-stu-id="a7c60-159">Type</span></span> | <span data-ttu-id="a7c60-160">说明</span><span class="sxs-lookup"><span data-stu-id="a7c60-160">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a7c60-161">extensionName</span><span class="sxs-lookup"><span data-stu-id="a7c60-161">extensionName</span></span>|<span data-ttu-id="a7c60-162">String</span><span class="sxs-lookup"><span data-stu-id="a7c60-162">String</span></span>|<span data-ttu-id="a7c60-p106">开放类型数据扩展的唯一文本标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="a7c60-p106">A unique text identifier for an open type data extension. Required.</span></span>|
|<span data-ttu-id="a7c60-165">id</span><span class="sxs-lookup"><span data-stu-id="a7c60-165">id</span></span>|<span data-ttu-id="a7c60-166">String</span><span class="sxs-lookup"><span data-stu-id="a7c60-166">String</span></span>| <span data-ttu-id="a7c60-p107">连接具有 **extensionName** 扩展类型的完全限定的标识符 。只读。</span><span class="sxs-lookup"><span data-stu-id="a7c60-p107">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7c60-169">关系</span><span class="sxs-lookup"><span data-stu-id="a7c60-169">Relationships</span></span>

<span data-ttu-id="a7c60-170">无</span><span class="sxs-lookup"><span data-stu-id="a7c60-170">None</span></span>

## <a name="methods"></a><span data-ttu-id="a7c60-171">方法</span><span class="sxs-lookup"><span data-stu-id="a7c60-171">Methods</span></span>

| <span data-ttu-id="a7c60-172">方法</span><span class="sxs-lookup"><span data-stu-id="a7c60-172">Method</span></span> | <span data-ttu-id="a7c60-173">返回类型</span><span class="sxs-lookup"><span data-stu-id="a7c60-173">Return Type</span></span> | <span data-ttu-id="a7c60-174">说明</span><span class="sxs-lookup"><span data-stu-id="a7c60-174">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="a7c60-175">创建</span><span class="sxs-lookup"><span data-stu-id="a7c60-175">Create</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="a7c60-176">[openTypeExtension](opentypeextension.md) (现有资源实例) ，或包含 openTypeExtension 对象的新联系人[](message.md)[、](contact.md)[事件](event.md)、消息、post、todoTask 或[todoTaskList。](todotasklist.md) [](post.md) [](todotask.md)</span><span class="sxs-lookup"><span data-stu-id="a7c60-176">[openTypeExtension](opentypeextension.md)(in an existing resource instance), or a new [contact](contact.md), [event](event.md), [message](message.md), [post](post.md), [todoTask](todotask.md), or [todoTaskList](todotasklist.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="a7c60-177">在现有的或新的资源实例中创建 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="a7c60-177">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="a7c60-178">获取</span><span class="sxs-lookup"><span data-stu-id="a7c60-178">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="a7c60-179">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="a7c60-179">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="a7c60-180">读取 openTypeExtension 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7c60-180">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="a7c60-181">更新</span><span class="sxs-lookup"><span data-stu-id="a7c60-181">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="a7c60-182">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="a7c60-182">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="a7c60-183">更新 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="a7c60-183">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="a7c60-184">删除</span><span class="sxs-lookup"><span data-stu-id="a7c60-184">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="a7c60-185">无</span><span class="sxs-lookup"><span data-stu-id="a7c60-185">None</span></span> |<span data-ttu-id="a7c60-186">删除 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="a7c60-186">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
