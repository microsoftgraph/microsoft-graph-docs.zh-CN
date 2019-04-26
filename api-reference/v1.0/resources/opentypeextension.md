---
title: openTypeExtension 资源类型（开放扩展）
description: 借助开放扩展（旧称为“Office 365 数据扩展”），可以直接将泛型属性轻松添加到 Microsoft Graph 中的资源。
localization_priority: Priority
author: dkershaw10
ms.openlocfilehash: 854897e1cc4d887fc0f4d2f184a4e745e5cdc468
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462632"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="0fedd-103">openTypeExtension 资源类型（开放扩展）</span><span class="sxs-lookup"><span data-stu-id="0fedd-103">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="0fedd-104">借助开放扩展（旧称为“Office 365 数据扩展”），可以直接将泛型属性轻松添加到 Microsoft Graph 中的资源。</span><span class="sxs-lookup"><span data-stu-id="0fedd-104">Open extensions (formerly known as Office 365 data extensions) give you an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>

<span data-ttu-id="0fedd-105">开放扩展由 **openTypeExtension** 资源表示。</span><span class="sxs-lookup"><span data-stu-id="0fedd-105">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="0fedd-106">添加到资源的所有开放扩展都会显示在派生自 [extension](extension.md) 抽象类型的 **extensions** 导航属性中。</span><span class="sxs-lookup"><span data-stu-id="0fedd-106">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span> <span data-ttu-id="0fedd-107">每个扩展都有 **extensionName** 属性（这是所有扩展的预定义唯一可写属性）和自定义数据。</span><span class="sxs-lookup"><span data-stu-id="0fedd-107">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span>

<span data-ttu-id="0fedd-108">一种有助于确保扩展名称唯一性的方法是，使用反向域名系统 (DNS) 格式，此格式依赖_用户自己的域_。例如，`Com.Contoso.ContactInfo`。</span><span class="sxs-lookup"><span data-stu-id="0fedd-108">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="0fedd-109">请勿在扩展名称中使用 Microsoft 域（`Com.Microsoft` 或 `Com.OnMicrosoft`）。</span><span class="sxs-lookup"><span data-stu-id="0fedd-109">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="0fedd-110">开放扩展示例：[使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)</span><span class="sxs-lookup"><span data-stu-id="0fedd-110">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="0fedd-111">一般可用性（GA: /v1.0 和 /beta）或预览版 (/beta) 对应版本中的以下资源支持开放扩展。</span><span class="sxs-lookup"><span data-stu-id="0fedd-111">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

|<span data-ttu-id="0fedd-112">资源</span><span class="sxs-lookup"><span data-stu-id="0fedd-112">Resource</span></span> |<span data-ttu-id="0fedd-113">版本</span><span class="sxs-lookup"><span data-stu-id="0fedd-113">Version</span></span> |
|:---------------|:-------|
| [<span data-ttu-id="0fedd-114">管理单元</span><span class="sxs-lookup"><span data-stu-id="0fedd-114">Administrative unit</span></span>](/graph/api/resources/administrativeunit?view=graph-rest-beta)  | <span data-ttu-id="0fedd-115">仅供预览</span><span class="sxs-lookup"><span data-stu-id="0fedd-115">Preview only</span></span> |
| [<span data-ttu-id="0fedd-116">日历事件</span><span class="sxs-lookup"><span data-stu-id="0fedd-116">Calendar event</span></span>](event.md) | <span data-ttu-id="0fedd-117">GA</span><span class="sxs-lookup"><span data-stu-id="0fedd-117">GA</span></span> |
| <span data-ttu-id="0fedd-118">组[日历事件](event.md)</span><span class="sxs-lookup"><span data-stu-id="0fedd-118">Group [calendar event](event.md)</span></span> | <span data-ttu-id="0fedd-119">GA</span><span class="sxs-lookup"><span data-stu-id="0fedd-119">GA</span></span> |
| <span data-ttu-id="0fedd-120">组对话线程[帖子](post.md)</span><span class="sxs-lookup"><span data-stu-id="0fedd-120">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="0fedd-121">GA</span><span class="sxs-lookup"><span data-stu-id="0fedd-121">GA</span></span> |
| [<span data-ttu-id="0fedd-122">设备</span><span class="sxs-lookup"><span data-stu-id="0fedd-122">device</span></span>](device.md) | <span data-ttu-id="0fedd-123">GA</span><span class="sxs-lookup"><span data-stu-id="0fedd-123">GA</span></span> |
| [<span data-ttu-id="0fedd-124">组</span><span class="sxs-lookup"><span data-stu-id="0fedd-124">group</span></span>](group.md) | <span data-ttu-id="0fedd-125">GA</span><span class="sxs-lookup"><span data-stu-id="0fedd-125">GA</span></span> |
| [<span data-ttu-id="0fedd-126">邮件</span><span class="sxs-lookup"><span data-stu-id="0fedd-126">message</span></span>](message.md) | <span data-ttu-id="0fedd-127">GA</span><span class="sxs-lookup"><span data-stu-id="0fedd-127">GA</span></span> |
| [<span data-ttu-id="0fedd-128">组织</span><span class="sxs-lookup"><span data-stu-id="0fedd-128">organization</span></span>](organization.md) | <span data-ttu-id="0fedd-129">GA</span><span class="sxs-lookup"><span data-stu-id="0fedd-129">GA</span></span> |
| [<span data-ttu-id="0fedd-130">个人联系人</span><span class="sxs-lookup"><span data-stu-id="0fedd-130">Personal contact</span></span>](contact.md) | <span data-ttu-id="0fedd-131">GA</span><span class="sxs-lookup"><span data-stu-id="0fedd-131">GA</span></span> |
| [<span data-ttu-id="0fedd-132">用户</span><span class="sxs-lookup"><span data-stu-id="0fedd-132">user</span></span>](user.md) | <span data-ttu-id="0fedd-133">GA</span><span class="sxs-lookup"><span data-stu-id="0fedd-133">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="0fedd-134">Outlook 特定注意事项</span><span class="sxs-lookup"><span data-stu-id="0fedd-134">Outlook-specific considerations</span></span>

<span data-ttu-id="0fedd-135">Outlook 资源（事件、邮件或个人联系人）上存在每个开放扩展均存储在 [MAPI 命名属性](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx)中。</span><span class="sxs-lookup"><span data-stu-id="0fedd-135">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="0fedd-136">为 Outlook 创建开放扩展时，请考虑 MAPI 命名属性为用户邮箱中的有限资源。</span><span class="sxs-lookup"><span data-stu-id="0fedd-136">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="0fedd-137">当用户的命名属性配额用尽后，无法再为该用户创建任何其他命名属性。</span><span class="sxs-lookup"><span data-stu-id="0fedd-137">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="0fedd-138">这可能会导致依赖命名属性工作的客户端中出现异常行为。</span><span class="sxs-lookup"><span data-stu-id="0fedd-138">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="0fedd-139">在 Outlook 资源中创建开放扩展时，请遵循以下指导原则：</span><span class="sxs-lookup"><span data-stu-id="0fedd-139">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="0fedd-140">创建所需的最少数量的扩展。</span><span class="sxs-lookup"><span data-stu-id="0fedd-140">Create the minimum number of extensions required.</span></span> <span data-ttu-id="0fedd-141">大多数应用程序只需要一个扩展。</span><span class="sxs-lookup"><span data-stu-id="0fedd-141">Most applications should require no more than one extension.</span></span> <span data-ttu-id="0fedd-142">扩展未设定定义的属性或结构，因此，可以在一个扩展中存储多个值。</span><span class="sxs-lookup"><span data-stu-id="0fedd-142">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="0fedd-143">避免以可变方式命名扩展，如基于用户输入等。</span><span class="sxs-lookup"><span data-stu-id="0fedd-143">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="0fedd-144">每次使用用户邮箱中先前未使用过的新名称创建开放扩展时，将会创建新的 MAP 命名属性。</span><span class="sxs-lookup"><span data-stu-id="0fedd-144">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="0fedd-145">删除扩展不会删除命名属性。</span><span class="sxs-lookup"><span data-stu-id="0fedd-145">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="0fedd-146">使用开放扩展（针对 Outlook 资源）或扩展属性</span><span class="sxs-lookup"><span data-stu-id="0fedd-146">Use open extensions (for Outlook resources) or extended properties?</span></span>

<span data-ttu-id="0fedd-147">开放扩展是大部分涉及存储和访问自定义数据的应用场景的推荐解决方案。</span><span class="sxs-lookup"><span data-stu-id="0fedd-147">Open extensions is the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="0fedd-148">不过，如果需要访问尚未通过 [Microsoft Graph API 元数据](https://developer.microsoft.com/graph/docs/overview/call_api)公开的 Outlook MAPI 属性的自定义数据，则可以使用[扩展属性及其 REST API](extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="0fedd-148">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="0fedd-149">若要确认元数据公开了哪些属性，请访问 [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata)。</span><span class="sxs-lookup"><span data-stu-id="0fedd-149">You can verify which properties the metadata exposes at https://graph.microsoft.com/v1.0/$metadata.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fedd-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fedd-150">JSON representation</span></span>

<span data-ttu-id="0fedd-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fedd-151">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.extension",
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a><span data-ttu-id="0fedd-152">属性</span><span class="sxs-lookup"><span data-stu-id="0fedd-152">Properties</span></span>

|<span data-ttu-id="0fedd-153">属性</span><span class="sxs-lookup"><span data-stu-id="0fedd-153">Property</span></span> | <span data-ttu-id="0fedd-154">类型</span><span class="sxs-lookup"><span data-stu-id="0fedd-154">Type</span></span> | <span data-ttu-id="0fedd-155">说明</span><span class="sxs-lookup"><span data-stu-id="0fedd-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0fedd-156">extensionName</span><span class="sxs-lookup"><span data-stu-id="0fedd-156">extensionName</span></span>|<span data-ttu-id="0fedd-157">String</span><span class="sxs-lookup"><span data-stu-id="0fedd-157">String</span></span>|<span data-ttu-id="0fedd-p107">开放类型开放扩展的唯一文本标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="0fedd-p107">A unique text identifier for an open type open extension. Required.</span></span>|
|<span data-ttu-id="0fedd-160">id</span><span class="sxs-lookup"><span data-stu-id="0fedd-160">id</span></span>|<span data-ttu-id="0fedd-161">String</span><span class="sxs-lookup"><span data-stu-id="0fedd-161">String</span></span>| <span data-ttu-id="0fedd-p108">连接具有 **extensionName** 扩展类型的完全限定的标识符 。只读。</span><span class="sxs-lookup"><span data-stu-id="0fedd-p108">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fedd-164">关系</span><span class="sxs-lookup"><span data-stu-id="0fedd-164">Relationships</span></span>

<span data-ttu-id="0fedd-165">无</span><span class="sxs-lookup"><span data-stu-id="0fedd-165">None</span></span>

## <a name="methods"></a><span data-ttu-id="0fedd-166">方法</span><span class="sxs-lookup"><span data-stu-id="0fedd-166">Methods</span></span>

|<span data-ttu-id="0fedd-167">方法</span><span class="sxs-lookup"><span data-stu-id="0fedd-167">Method</span></span> | <span data-ttu-id="0fedd-168">返回类型</span><span class="sxs-lookup"><span data-stu-id="0fedd-168">Return Type</span></span> | <span data-ttu-id="0fedd-169">说明</span><span class="sxs-lookup"><span data-stu-id="0fedd-169">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="0fedd-170">Post</span><span class="sxs-lookup"><span data-stu-id="0fedd-170">Post</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="0fedd-171">[openTypeExtension](opentypeextension.md)（在现有资源实例中），或包含 openTypeExtension 对象的新 [contact](../resources/contact.md)、[event](../resources/event.md) 或 [message](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="0fedd-171">[openTypeExtension](opentypeextension.md) (in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object</span></span> | <span data-ttu-id="0fedd-172">在现有的或新的资源实例中创建 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="0fedd-172">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="0fedd-173">获取</span><span class="sxs-lookup"><span data-stu-id="0fedd-173">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="0fedd-174">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="0fedd-174">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="0fedd-175">读取 openTypeExtension 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fedd-175">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="0fedd-176">更新</span><span class="sxs-lookup"><span data-stu-id="0fedd-176">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="0fedd-177">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="0fedd-177">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="0fedd-178">更新 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="0fedd-178">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="0fedd-179">删除</span><span class="sxs-lookup"><span data-stu-id="0fedd-179">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="0fedd-180">无</span><span class="sxs-lookup"><span data-stu-id="0fedd-180">None</span></span> |<span data-ttu-id="0fedd-181">删除 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="0fedd-181">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
