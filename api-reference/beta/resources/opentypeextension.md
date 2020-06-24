---
title: openTypeExtension 资源类型（开放扩展）
description: 借助开放扩展（旧称为“Office 365 数据扩展”），可以直接将泛型属性轻松添加到 Microsoft Graph 中的资源。
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: 297055a6edb4eb4d094406e03b9e4136f1df68c4
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864103"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="682a2-103">openTypeExtension 资源类型（开放扩展）</span><span class="sxs-lookup"><span data-stu-id="682a2-103">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="682a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="682a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="682a2-105">借助开放扩展（旧称为“Office 365 数据扩展”），可以直接将泛型属性轻松添加到 Microsoft Graph 中的资源。</span><span class="sxs-lookup"><span data-stu-id="682a2-105">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>
<span data-ttu-id="682a2-106">开放扩展由 **openTypeExtension** 资源表示。</span><span class="sxs-lookup"><span data-stu-id="682a2-106">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="682a2-107">添加到资源的所有开放扩展都会显示在派生自 [extension](extension.md) 抽象类型的 **extensions** 导航属性中。</span><span class="sxs-lookup"><span data-stu-id="682a2-107">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span>  <span data-ttu-id="682a2-108">每个扩展都有 **extensionName** 属性（这是所有扩展的预定义唯一可写属性）和自定义数据。</span><span class="sxs-lookup"><span data-stu-id="682a2-108">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span> <span data-ttu-id="682a2-109">一种有助于确保扩展名称唯一性的方法是，使用反向域名系统 (DNS) 格式，此格式依赖_用户自己的域_。例如，`Com.Contoso.ContactInfo`。</span><span class="sxs-lookup"><span data-stu-id="682a2-109">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="682a2-110">请勿在扩展名称中使用 Microsoft 域（`Com.Microsoft` 或 `Com.OnMicrosoft`）。</span><span class="sxs-lookup"><span data-stu-id="682a2-110">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="682a2-111">开放扩展示例：[使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)</span><span class="sxs-lookup"><span data-stu-id="682a2-111">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="682a2-112">一般可用性（GA: /v1.0 和 /beta）或预览版 (/beta) 对应版本中的以下资源支持开放扩展。</span><span class="sxs-lookup"><span data-stu-id="682a2-112">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

| <span data-ttu-id="682a2-113">资源</span><span class="sxs-lookup"><span data-stu-id="682a2-113">Resource</span></span> | <span data-ttu-id="682a2-114">版本</span><span class="sxs-lookup"><span data-stu-id="682a2-114">Version</span></span> |
|---------------|-------|
| [<span data-ttu-id="682a2-115">管理单元</span><span class="sxs-lookup"><span data-stu-id="682a2-115">Administrative unit</span></span>](administrativeunit.md)  | <span data-ttu-id="682a2-116">仅供预览</span><span class="sxs-lookup"><span data-stu-id="682a2-116">Preview only</span></span> |
| [<span data-ttu-id="682a2-117">日历事件</span><span class="sxs-lookup"><span data-stu-id="682a2-117">Calendar event</span></span>](event.md) | <span data-ttu-id="682a2-118">GA</span><span class="sxs-lookup"><span data-stu-id="682a2-118">GA</span></span> |
| <span data-ttu-id="682a2-119">组[日历事件](event.md)</span><span class="sxs-lookup"><span data-stu-id="682a2-119">Group [calendar event](event.md)</span></span> | <span data-ttu-id="682a2-120">GA</span><span class="sxs-lookup"><span data-stu-id="682a2-120">GA</span></span> |
| <span data-ttu-id="682a2-121">组对话线程[帖子](post.md)</span><span class="sxs-lookup"><span data-stu-id="682a2-121">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="682a2-122">GA</span><span class="sxs-lookup"><span data-stu-id="682a2-122">GA</span></span> |
| [<span data-ttu-id="682a2-123">设备</span><span class="sxs-lookup"><span data-stu-id="682a2-123">device</span></span>](device.md) | <span data-ttu-id="682a2-124">GA</span><span class="sxs-lookup"><span data-stu-id="682a2-124">GA</span></span> |
| [<span data-ttu-id="682a2-125">组</span><span class="sxs-lookup"><span data-stu-id="682a2-125">group</span></span>](group.md) | <span data-ttu-id="682a2-126">GA</span><span class="sxs-lookup"><span data-stu-id="682a2-126">GA</span></span> |
| [<span data-ttu-id="682a2-127">邮件</span><span class="sxs-lookup"><span data-stu-id="682a2-127">message</span></span>](message.md) | <span data-ttu-id="682a2-128">GA</span><span class="sxs-lookup"><span data-stu-id="682a2-128">GA</span></span> |
| [<span data-ttu-id="682a2-129">组织</span><span class="sxs-lookup"><span data-stu-id="682a2-129">organization</span></span>](organization.md) | <span data-ttu-id="682a2-130">GA</span><span class="sxs-lookup"><span data-stu-id="682a2-130">GA</span></span> |
| [<span data-ttu-id="682a2-131">个人联系人</span><span class="sxs-lookup"><span data-stu-id="682a2-131">Personal contact</span></span>](contact.md) | <span data-ttu-id="682a2-132">GA</span><span class="sxs-lookup"><span data-stu-id="682a2-132">GA</span></span> |
| [<span data-ttu-id="682a2-133">用户</span><span class="sxs-lookup"><span data-stu-id="682a2-133">user</span></span>](user.md) | <span data-ttu-id="682a2-134">GA</span><span class="sxs-lookup"><span data-stu-id="682a2-134">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="682a2-135">Outlook 特定注意事项</span><span class="sxs-lookup"><span data-stu-id="682a2-135">Outlook-specific considerations</span></span>

<span data-ttu-id="682a2-136">Outlook 资源（事件、邮件或个人联系人）上存在每个开放扩展均存储在 [MAPI 命名属性](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx)中。</span><span class="sxs-lookup"><span data-stu-id="682a2-136">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="682a2-137">为 Outlook 创建开放扩展时，请考虑 MAPI 命名属性为用户邮箱中的有限资源。</span><span class="sxs-lookup"><span data-stu-id="682a2-137">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="682a2-138">当用户的命名属性配额用尽后，无法再为该用户创建任何其他命名属性。</span><span class="sxs-lookup"><span data-stu-id="682a2-138">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="682a2-139">这可能会导致依赖命名属性工作的客户端中出现异常行为。</span><span class="sxs-lookup"><span data-stu-id="682a2-139">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="682a2-140">在 Outlook 资源中创建开放扩展时，请遵循以下指导原则：</span><span class="sxs-lookup"><span data-stu-id="682a2-140">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="682a2-141">创建所需的最少数量的扩展。</span><span class="sxs-lookup"><span data-stu-id="682a2-141">Create the minimum number of extensions required.</span></span> <span data-ttu-id="682a2-142">大多数应用程序只需要一个扩展。</span><span class="sxs-lookup"><span data-stu-id="682a2-142">Most applications should require no more than one extension.</span></span> <span data-ttu-id="682a2-143">扩展未设定定义的属性或结构，因此，可以在一个扩展中存储多个值。</span><span class="sxs-lookup"><span data-stu-id="682a2-143">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="682a2-144">避免以可变方式命名扩展，如基于用户输入等。</span><span class="sxs-lookup"><span data-stu-id="682a2-144">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="682a2-145">每次使用用户邮箱中先前未使用过的新名称创建开放扩展时，将会创建新的 MAP 命名属性。</span><span class="sxs-lookup"><span data-stu-id="682a2-145">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="682a2-146">删除扩展不会删除命名属性。</span><span class="sxs-lookup"><span data-stu-id="682a2-146">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="682a2-147">使用开放扩展（针对 Outlook 资源）或扩展属性</span><span class="sxs-lookup"><span data-stu-id="682a2-147">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="682a2-148">开放扩展是大部分涉及存储和访问自定义数据的应用场景的推荐解决方案。</span><span class="sxs-lookup"><span data-stu-id="682a2-148">Open extensions is the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="682a2-149">不过，如果需要访问尚未通过 [Microsoft Graph API 元数据](https://developer.microsoft.com/graph/docs/overview/call_api)公开的 Outlook MAPI 属性的自定义数据，则可以使用[扩展属性及其 REST API](extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="682a2-149">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="682a2-150">若要确认元数据公开了哪些属性，请访问 [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata)。</span><span class="sxs-lookup"><span data-stu-id="682a2-150">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="682a2-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="682a2-151">JSON representation</span></span>

<span data-ttu-id="682a2-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="682a2-152">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="682a2-153">属性</span><span class="sxs-lookup"><span data-stu-id="682a2-153">Properties</span></span>

| <span data-ttu-id="682a2-154">属性</span><span class="sxs-lookup"><span data-stu-id="682a2-154">Property</span></span> | <span data-ttu-id="682a2-155">类型</span><span class="sxs-lookup"><span data-stu-id="682a2-155">Type</span></span> | <span data-ttu-id="682a2-156">Description</span><span class="sxs-lookup"><span data-stu-id="682a2-156">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="682a2-157">extensionName</span><span class="sxs-lookup"><span data-stu-id="682a2-157">extensionName</span></span>|<span data-ttu-id="682a2-158">String</span><span class="sxs-lookup"><span data-stu-id="682a2-158">String</span></span>|<span data-ttu-id="682a2-159">A unique text identifier for an open type data extension.</span><span class="sxs-lookup"><span data-stu-id="682a2-159">A unique text identifier for an open type data extension.</span></span> <span data-ttu-id="682a2-160">Required.</span><span class="sxs-lookup"><span data-stu-id="682a2-160">Required.</span></span>|
|<span data-ttu-id="682a2-161">id</span><span class="sxs-lookup"><span data-stu-id="682a2-161">id</span></span>|<span data-ttu-id="682a2-162">String</span><span class="sxs-lookup"><span data-stu-id="682a2-162">String</span></span>| <span data-ttu-id="682a2-163">A fully qualified identifier that concatenates the extension type with the **extensionName**.</span><span class="sxs-lookup"><span data-stu-id="682a2-163">A fully qualified identifier that concatenates the extension type with the **extensionName**.</span></span> <span data-ttu-id="682a2-164">Read-only.</span><span class="sxs-lookup"><span data-stu-id="682a2-164">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="682a2-165">关系</span><span class="sxs-lookup"><span data-stu-id="682a2-165">Relationships</span></span>

<span data-ttu-id="682a2-166">无</span><span class="sxs-lookup"><span data-stu-id="682a2-166">None</span></span>

## <a name="methods"></a><span data-ttu-id="682a2-167">方法</span><span class="sxs-lookup"><span data-stu-id="682a2-167">Methods</span></span>

| <span data-ttu-id="682a2-168">方法</span><span class="sxs-lookup"><span data-stu-id="682a2-168">Method</span></span> | <span data-ttu-id="682a2-169">返回类型</span><span class="sxs-lookup"><span data-stu-id="682a2-169">Return Type</span></span> | <span data-ttu-id="682a2-170">说明</span><span class="sxs-lookup"><span data-stu-id="682a2-170">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="682a2-171">Create</span><span class="sxs-lookup"><span data-stu-id="682a2-171">Create</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="682a2-172">[openTypeExtension](opentypeextension.md)（在现有资源实例中）或包含 openTypeExtension 对象的新[联系人](../resources/contact.md)、[事件](../resources/event.md)或[邮件](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="682a2-172">[openTypeExtension](opentypeextension.md)(in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="682a2-173">在现有的或新的资源实例中创建 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="682a2-173">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="682a2-174">获取</span><span class="sxs-lookup"><span data-stu-id="682a2-174">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="682a2-175">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="682a2-175">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="682a2-176">读取 openTypeExtension 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="682a2-176">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="682a2-177">更新</span><span class="sxs-lookup"><span data-stu-id="682a2-177">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="682a2-178">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="682a2-178">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="682a2-179">更新 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="682a2-179">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="682a2-180">删除</span><span class="sxs-lookup"><span data-stu-id="682a2-180">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="682a2-181">无</span><span class="sxs-lookup"><span data-stu-id="682a2-181">None</span></span> |<span data-ttu-id="682a2-182">删除 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="682a2-182">Delete openTypeExtension object.</span></span> |

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
