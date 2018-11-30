---
title: openTypeExtension 资源类型（开放扩展）
description: 打开扩展 （之前被称为 Office 365 数据扩展） 提供轻松直接将非类型化的属性添加到 Microsoft Graph 中的资源。
ms.openlocfilehash: f28ab43ddb3fd55efbca6738a0369fde37c906db
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044137"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="fe948-103">openTypeExtension 资源类型（开放扩展）</span><span class="sxs-lookup"><span data-stu-id="fe948-103">openTypeExtension resource type (open extensions)</span></span>

> <span data-ttu-id="fe948-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fe948-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe948-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fe948-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe948-106">打开扩展 （之前被称为 Office 365 数据扩展） 提供轻松直接将非类型化的属性添加到 Microsoft Graph 中的资源。</span><span class="sxs-lookup"><span data-stu-id="fe948-106">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>
<span data-ttu-id="fe948-107">开放扩展由 **openTypeExtension** 资源表示。</span><span class="sxs-lookup"><span data-stu-id="fe948-107">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="fe948-108">添加到资源的所有开放扩展都会显示在派生自 [extension](extension.md) 抽象类型的 **extensions** 导航属性中。</span><span class="sxs-lookup"><span data-stu-id="fe948-108">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span>  <span data-ttu-id="fe948-109">每个扩展都有 **extensionName** 属性（这是所有扩展的预定义唯一可写属性）和自定义数据。</span><span class="sxs-lookup"><span data-stu-id="fe948-109">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span> <span data-ttu-id="fe948-110">一种有助于确保扩展名称唯一性的方法是，使用反向域名系统 (DNS) 格式，此格式依赖_用户自己的域_。例如，`Com.Contoso.ContactInfo`。</span><span class="sxs-lookup"><span data-stu-id="fe948-110">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="fe948-111">请勿在扩展名称中使用 Microsoft 域（`Com.Microsoft` 或 `Com.OnMicrosoft`）。</span><span class="sxs-lookup"><span data-stu-id="fe948-111">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="fe948-112">开放扩展示例：[使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)</span><span class="sxs-lookup"><span data-stu-id="fe948-112">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="fe948-113">一般可用性（GA: /v1.0 和 /beta）或预览版 (/beta) 对应版本中的以下资源支持开放扩展。</span><span class="sxs-lookup"><span data-stu-id="fe948-113">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

| <span data-ttu-id="fe948-114">资源</span><span class="sxs-lookup"><span data-stu-id="fe948-114">Resource</span></span> | <span data-ttu-id="fe948-115">版本</span><span class="sxs-lookup"><span data-stu-id="fe948-115">Version</span></span> |
|---------------|-------|
| [<span data-ttu-id="fe948-116">管理单元</span><span class="sxs-lookup"><span data-stu-id="fe948-116">Administrative unit</span></span>](administrativeunit.md)  | <span data-ttu-id="fe948-117">仅供预览</span><span class="sxs-lookup"><span data-stu-id="fe948-117">Preview only</span></span> |
| [<span data-ttu-id="fe948-118">日历事件</span><span class="sxs-lookup"><span data-stu-id="fe948-118">Calendar event</span></span>](event.md) | <span data-ttu-id="fe948-119">GA</span><span class="sxs-lookup"><span data-stu-id="fe948-119">GA</span></span> |
| <span data-ttu-id="fe948-120">组[日历事件](event.md)</span><span class="sxs-lookup"><span data-stu-id="fe948-120">Group [calendar event](event.md)</span></span> | <span data-ttu-id="fe948-121">GA</span><span class="sxs-lookup"><span data-stu-id="fe948-121">GA</span></span> |
| <span data-ttu-id="fe948-122">组对话线程[帖子](post.md)</span><span class="sxs-lookup"><span data-stu-id="fe948-122">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="fe948-123">GA</span><span class="sxs-lookup"><span data-stu-id="fe948-123">GA</span></span> |
| [<span data-ttu-id="fe948-124">设备</span><span class="sxs-lookup"><span data-stu-id="fe948-124">device</span></span>](device.md) | <span data-ttu-id="fe948-125">GA</span><span class="sxs-lookup"><span data-stu-id="fe948-125">GA</span></span> |
| [<span data-ttu-id="fe948-126">组</span><span class="sxs-lookup"><span data-stu-id="fe948-126">group</span></span>](group.md) | <span data-ttu-id="fe948-127">GA</span><span class="sxs-lookup"><span data-stu-id="fe948-127">GA</span></span> |
| [<span data-ttu-id="fe948-128">邮件</span><span class="sxs-lookup"><span data-stu-id="fe948-128">message</span></span>](message.md) | <span data-ttu-id="fe948-129">GA</span><span class="sxs-lookup"><span data-stu-id="fe948-129">GA</span></span> |
| [<span data-ttu-id="fe948-130">组织</span><span class="sxs-lookup"><span data-stu-id="fe948-130">organization</span></span>](organization.md) | <span data-ttu-id="fe948-131">GA</span><span class="sxs-lookup"><span data-stu-id="fe948-131">GA</span></span> |
| [<span data-ttu-id="fe948-132">个人联系人</span><span class="sxs-lookup"><span data-stu-id="fe948-132">Personal contact</span></span>](contact.md) | <span data-ttu-id="fe948-133">GA</span><span class="sxs-lookup"><span data-stu-id="fe948-133">GA</span></span> |
| [<span data-ttu-id="fe948-134">用户</span><span class="sxs-lookup"><span data-stu-id="fe948-134">user</span></span>](user.md) | <span data-ttu-id="fe948-135">GA</span><span class="sxs-lookup"><span data-stu-id="fe948-135">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="fe948-136">特定于 outlook 的注意事项</span><span class="sxs-lookup"><span data-stu-id="fe948-136">Outlook-specific considerations</span></span>

<span data-ttu-id="fe948-137">每个打开的扩展名存在于 Outlook 的资源 （事件、 消息或个人联系人） 存储在[MAPI 命名属性](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx)。</span><span class="sxs-lookup"><span data-stu-id="fe948-137">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="fe948-138">为 Outlook 创建打开扩展时，请考虑 MAPI 命名属性是用户的邮箱的有限资源。</span><span class="sxs-lookup"><span data-stu-id="fe948-138">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="fe948-139">在用尽用户的命名的属性配额时，您无法创建该用户的任何多命名的属性。</span><span class="sxs-lookup"><span data-stu-id="fe948-139">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="fe948-140">这会导致出现异常行为依赖于对函数的命名属性的客户端。</span><span class="sxs-lookup"><span data-stu-id="fe948-140">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="fe948-141">打开扩展名创建在 Outlook 资源时，请应用以下准则：</span><span class="sxs-lookup"><span data-stu-id="fe948-141">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="fe948-142">创建所需的扩展的最小数目。</span><span class="sxs-lookup"><span data-stu-id="fe948-142">Create the minimum number of extensions required.</span></span> <span data-ttu-id="fe948-143">大多数应用程序应该要求不多个扩展名。</span><span class="sxs-lookup"><span data-stu-id="fe948-143">Most applications should require no more than one extension.</span></span> <span data-ttu-id="fe948-144">扩展具有未定义的设置的属性或结构，因此您可以将多个值存储在一个扩展。</span><span class="sxs-lookup"><span data-stu-id="fe948-144">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="fe948-145">避免 （例如，基于用户输入等。） 来扩展命名变量的方式。</span><span class="sxs-lookup"><span data-stu-id="fe948-145">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="fe948-146">打开扩展名创建新的名称之前, 的用户的邮箱中未用过的每次创建新的 MAPI 命名属性。</span><span class="sxs-lookup"><span data-stu-id="fe948-146">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="fe948-147">删除扩展不会删除的命名的属性。</span><span class="sxs-lookup"><span data-stu-id="fe948-147">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="fe948-148">使用打开扩展名 （对于 Outlook 资源） 或扩展的属性</span><span class="sxs-lookup"><span data-stu-id="fe948-148">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="fe948-149">打开扩展是适用于大多数的方案涉及存储和访问自定义数据的建议的解决方案。</span><span class="sxs-lookup"><span data-stu-id="fe948-149">Open extensions is the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="fe948-150">但是，您需要通过[Microsoft Graph API 元数据](https://developer.microsoft.com/graph/docs/overview/call_api)访问自定义 Outlook MAPI 属性未已公开的数据，您可以使用[扩展的属性和其 REST API](extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="fe948-150">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="fe948-151">您可以验证元数据在公开哪些属性[https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata)。</span><span class="sxs-lookup"><span data-stu-id="fe948-151">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe948-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe948-152">JSON representation</span></span>

<span data-ttu-id="fe948-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe948-153">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.opentypeextension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a><span data-ttu-id="fe948-154">属性</span><span class="sxs-lookup"><span data-stu-id="fe948-154">Properties</span></span>

| <span data-ttu-id="fe948-155">属性</span><span class="sxs-lookup"><span data-stu-id="fe948-155">Property</span></span> | <span data-ttu-id="fe948-156">类型</span><span class="sxs-lookup"><span data-stu-id="fe948-156">Type</span></span> | <span data-ttu-id="fe948-157">说明</span><span class="sxs-lookup"><span data-stu-id="fe948-157">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="fe948-158">extensionName</span><span class="sxs-lookup"><span data-stu-id="fe948-158">extensionName</span></span>|<span data-ttu-id="fe948-159">String</span><span class="sxs-lookup"><span data-stu-id="fe948-159">String</span></span>|<span data-ttu-id="fe948-p107">开放类型数据扩展的唯一文本标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="fe948-p107">A unique text identifier for an open type data extension. Required.</span></span>|
|<span data-ttu-id="fe948-162">id</span><span class="sxs-lookup"><span data-stu-id="fe948-162">id</span></span>|<span data-ttu-id="fe948-163">String</span><span class="sxs-lookup"><span data-stu-id="fe948-163">String</span></span>| <span data-ttu-id="fe948-p108">连接具有 **extensionName** 扩展类型的完全限定的标识符 。只读。</span><span class="sxs-lookup"><span data-stu-id="fe948-p108">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe948-166">关系</span><span class="sxs-lookup"><span data-stu-id="fe948-166">Relationships</span></span>

<span data-ttu-id="fe948-167">无</span><span class="sxs-lookup"><span data-stu-id="fe948-167">None</span></span>

## <a name="methods"></a><span data-ttu-id="fe948-168">方法</span><span class="sxs-lookup"><span data-stu-id="fe948-168">Methods</span></span>

| <span data-ttu-id="fe948-169">方法</span><span class="sxs-lookup"><span data-stu-id="fe948-169">Method</span></span> | <span data-ttu-id="fe948-170">返回类型</span><span class="sxs-lookup"><span data-stu-id="fe948-170">Return Type</span></span> | <span data-ttu-id="fe948-171">说明</span><span class="sxs-lookup"><span data-stu-id="fe948-171">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="fe948-172">Post</span><span class="sxs-lookup"><span data-stu-id="fe948-172">Post</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="fe948-173">[openTypeExtension](opentypeextension.md)（在现有资源实例中），或新[联系人](../resources/contact.md)、[事件](../resources/event.md)或[消息](../resources/message.md)，其中包含一个 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="fe948-173">[openTypeExtension](opentypeextension.md)(in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="fe948-174">在现有的或新的资源实例中创建 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="fe948-174">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="fe948-175">获取</span><span class="sxs-lookup"><span data-stu-id="fe948-175">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="fe948-176">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="fe948-176">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="fe948-177">读取 openTypeExtension 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fe948-177">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="fe948-178">更新</span><span class="sxs-lookup"><span data-stu-id="fe948-178">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="fe948-179">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="fe948-179">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="fe948-180">更新 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="fe948-180">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="fe948-181">删除</span><span class="sxs-lookup"><span data-stu-id="fe948-181">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="fe948-182">无</span><span class="sxs-lookup"><span data-stu-id="fe948-182">None</span></span> |<span data-ttu-id="fe948-183">删除 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="fe948-183">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->