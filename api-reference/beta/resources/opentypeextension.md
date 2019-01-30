---
title: openTypeExtension 资源类型（开放扩展）
description: 打开扩展 （之前被称为 Office 365 数据扩展） 提供轻松直接将非类型化的属性添加到 Microsoft Graph 中的资源。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: ba5dbcd6c5ae1705ffe7e89ca6f529280d98adf5
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643837"
---
# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="a5381-103">openTypeExtension 资源类型（开放扩展）</span><span class="sxs-lookup"><span data-stu-id="a5381-103">openTypeExtension resource type (open extensions)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5381-104">打开扩展 （之前被称为 Office 365 数据扩展） 提供轻松直接将非类型化的属性添加到 Microsoft Graph 中的资源。</span><span class="sxs-lookup"><span data-stu-id="a5381-104">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>
<span data-ttu-id="a5381-105">开放扩展由 **openTypeExtension** 资源表示。</span><span class="sxs-lookup"><span data-stu-id="a5381-105">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="a5381-106">添加到资源的所有开放扩展都会显示在派生自 [extension](extension.md) 抽象类型的 **extensions** 导航属性中。</span><span class="sxs-lookup"><span data-stu-id="a5381-106">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span>  <span data-ttu-id="a5381-107">每个扩展都有 **extensionName** 属性（这是所有扩展的预定义唯一可写属性）和自定义数据。</span><span class="sxs-lookup"><span data-stu-id="a5381-107">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span> <span data-ttu-id="a5381-108">一种有助于确保扩展名称唯一性的方法是，使用反向域名系统 (DNS) 格式，此格式依赖_用户自己的域_。例如，`Com.Contoso.ContactInfo`。</span><span class="sxs-lookup"><span data-stu-id="a5381-108">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="a5381-109">请勿在扩展名称中使用 Microsoft 域（`Com.Microsoft` 或 `Com.OnMicrosoft`）。</span><span class="sxs-lookup"><span data-stu-id="a5381-109">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="a5381-110">开放扩展示例：[使用开放扩展向用户添加自定义数据](/graph/extensibility-open-users)</span><span class="sxs-lookup"><span data-stu-id="a5381-110">Open extension example: [Add custom data to users using open extensions](/graph/extensibility-open-users)</span></span>

<span data-ttu-id="a5381-111">一般可用性（GA: /v1.0 和 /beta）或预览版 (/beta) 对应版本中的以下资源支持开放扩展。</span><span class="sxs-lookup"><span data-stu-id="a5381-111">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

| <span data-ttu-id="a5381-112">资源</span><span class="sxs-lookup"><span data-stu-id="a5381-112">Resource</span></span> | <span data-ttu-id="a5381-113">版本</span><span class="sxs-lookup"><span data-stu-id="a5381-113">Version</span></span> |
|---------------|-------|
| [<span data-ttu-id="a5381-114">管理单元</span><span class="sxs-lookup"><span data-stu-id="a5381-114">Administrative unit</span></span>](administrativeunit.md)  | <span data-ttu-id="a5381-115">仅供预览</span><span class="sxs-lookup"><span data-stu-id="a5381-115">Preview only</span></span> |
| [<span data-ttu-id="a5381-116">日历事件</span><span class="sxs-lookup"><span data-stu-id="a5381-116">Calendar event</span></span>](event.md) | <span data-ttu-id="a5381-117">GA</span><span class="sxs-lookup"><span data-stu-id="a5381-117">GA</span></span> |
| <span data-ttu-id="a5381-118">组[日历事件](event.md)</span><span class="sxs-lookup"><span data-stu-id="a5381-118">Group [calendar event](event.md)</span></span> | <span data-ttu-id="a5381-119">GA</span><span class="sxs-lookup"><span data-stu-id="a5381-119">GA</span></span> |
| <span data-ttu-id="a5381-120">组对话线程[帖子](post.md)</span><span class="sxs-lookup"><span data-stu-id="a5381-120">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="a5381-121">GA</span><span class="sxs-lookup"><span data-stu-id="a5381-121">GA</span></span> |
| [<span data-ttu-id="a5381-122">设备</span><span class="sxs-lookup"><span data-stu-id="a5381-122">device</span></span>](device.md) | <span data-ttu-id="a5381-123">GA</span><span class="sxs-lookup"><span data-stu-id="a5381-123">GA</span></span> |
| [<span data-ttu-id="a5381-124">组</span><span class="sxs-lookup"><span data-stu-id="a5381-124">group</span></span>](group.md) | <span data-ttu-id="a5381-125">GA</span><span class="sxs-lookup"><span data-stu-id="a5381-125">GA</span></span> |
| [<span data-ttu-id="a5381-126">邮件</span><span class="sxs-lookup"><span data-stu-id="a5381-126">message</span></span>](message.md) | <span data-ttu-id="a5381-127">GA</span><span class="sxs-lookup"><span data-stu-id="a5381-127">GA</span></span> |
| [<span data-ttu-id="a5381-128">组织</span><span class="sxs-lookup"><span data-stu-id="a5381-128">organization</span></span>](organization.md) | <span data-ttu-id="a5381-129">GA</span><span class="sxs-lookup"><span data-stu-id="a5381-129">GA</span></span> |
| [<span data-ttu-id="a5381-130">个人联系人</span><span class="sxs-lookup"><span data-stu-id="a5381-130">Personal contact</span></span>](contact.md) | <span data-ttu-id="a5381-131">GA</span><span class="sxs-lookup"><span data-stu-id="a5381-131">GA</span></span> |
| [<span data-ttu-id="a5381-132">用户</span><span class="sxs-lookup"><span data-stu-id="a5381-132">user</span></span>](user.md) | <span data-ttu-id="a5381-133">GA</span><span class="sxs-lookup"><span data-stu-id="a5381-133">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="a5381-134">特定于 outlook 的注意事项</span><span class="sxs-lookup"><span data-stu-id="a5381-134">Outlook-specific considerations</span></span>

<span data-ttu-id="a5381-135">每个打开的扩展名存在于 Outlook 的资源 （事件、 消息或个人联系人） 存储在[MAPI 命名属性](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx)。</span><span class="sxs-lookup"><span data-stu-id="a5381-135">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="a5381-136">为 Outlook 创建打开扩展时，请考虑 MAPI 命名属性是用户的邮箱的有限资源。</span><span class="sxs-lookup"><span data-stu-id="a5381-136">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="a5381-137">在用尽用户的命名的属性配额时，您无法创建该用户的任何多命名的属性。</span><span class="sxs-lookup"><span data-stu-id="a5381-137">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="a5381-138">这会导致出现异常行为依赖于对函数的命名属性的客户端。</span><span class="sxs-lookup"><span data-stu-id="a5381-138">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="a5381-139">打开扩展名创建在 Outlook 资源时，请应用以下准则：</span><span class="sxs-lookup"><span data-stu-id="a5381-139">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="a5381-140">创建所需的扩展的最小数目。</span><span class="sxs-lookup"><span data-stu-id="a5381-140">Create the minimum number of extensions required.</span></span> <span data-ttu-id="a5381-141">大多数应用程序应该要求不多个扩展名。</span><span class="sxs-lookup"><span data-stu-id="a5381-141">Most applications should require no more than one extension.</span></span> <span data-ttu-id="a5381-142">扩展具有未定义的设置的属性或结构，因此您可以将多个值存储在一个扩展。</span><span class="sxs-lookup"><span data-stu-id="a5381-142">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="a5381-143">避免 （例如，基于用户输入等。） 来扩展命名变量的方式。</span><span class="sxs-lookup"><span data-stu-id="a5381-143">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="a5381-144">打开扩展名创建新的名称之前, 的用户的邮箱中未用过的每次创建新的 MAPI 命名属性。</span><span class="sxs-lookup"><span data-stu-id="a5381-144">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="a5381-145">删除扩展不会删除的命名的属性。</span><span class="sxs-lookup"><span data-stu-id="a5381-145">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="a5381-146">使用打开扩展名 （对于 Outlook 资源） 或扩展的属性</span><span class="sxs-lookup"><span data-stu-id="a5381-146">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="a5381-147">打开扩展是适用于大多数的方案涉及存储和访问自定义数据的建议的解决方案。</span><span class="sxs-lookup"><span data-stu-id="a5381-147">Open extensions is the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="a5381-148">但是，您需要通过[Microsoft Graph API 元数据](https://developer.microsoft.com/graph/docs/overview/call_api)访问自定义 Outlook MAPI 属性未已公开的数据，您可以使用[扩展的属性和其 REST API](extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="a5381-148">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="a5381-149">您可以验证元数据在公开哪些属性[https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata)。</span><span class="sxs-lookup"><span data-stu-id="a5381-149">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5381-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5381-150">JSON representation</span></span>

<span data-ttu-id="a5381-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5381-151">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="a5381-152">属性</span><span class="sxs-lookup"><span data-stu-id="a5381-152">Properties</span></span>

| <span data-ttu-id="a5381-153">属性</span><span class="sxs-lookup"><span data-stu-id="a5381-153">Property</span></span> | <span data-ttu-id="a5381-154">类型</span><span class="sxs-lookup"><span data-stu-id="a5381-154">Type</span></span> | <span data-ttu-id="a5381-155">说明</span><span class="sxs-lookup"><span data-stu-id="a5381-155">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a5381-156">extensionName</span><span class="sxs-lookup"><span data-stu-id="a5381-156">extensionName</span></span>|<span data-ttu-id="a5381-157">String</span><span class="sxs-lookup"><span data-stu-id="a5381-157">String</span></span>|<span data-ttu-id="a5381-p106">开放类型数据扩展的唯一文本标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="a5381-p106">A unique text identifier for an open type data extension. Required.</span></span>|
|<span data-ttu-id="a5381-160">id</span><span class="sxs-lookup"><span data-stu-id="a5381-160">id</span></span>|<span data-ttu-id="a5381-161">String</span><span class="sxs-lookup"><span data-stu-id="a5381-161">String</span></span>| <span data-ttu-id="a5381-p107">连接具有 **extensionName** 扩展类型的完全限定的标识符 。只读。</span><span class="sxs-lookup"><span data-stu-id="a5381-p107">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5381-164">关系</span><span class="sxs-lookup"><span data-stu-id="a5381-164">Relationships</span></span>

<span data-ttu-id="a5381-165">无</span><span class="sxs-lookup"><span data-stu-id="a5381-165">None</span></span>

## <a name="methods"></a><span data-ttu-id="a5381-166">方法</span><span class="sxs-lookup"><span data-stu-id="a5381-166">Methods</span></span>

| <span data-ttu-id="a5381-167">方法</span><span class="sxs-lookup"><span data-stu-id="a5381-167">Method</span></span> | <span data-ttu-id="a5381-168">返回类型</span><span class="sxs-lookup"><span data-stu-id="a5381-168">Return Type</span></span> | <span data-ttu-id="a5381-169">说明</span><span class="sxs-lookup"><span data-stu-id="a5381-169">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="a5381-170">Post</span><span class="sxs-lookup"><span data-stu-id="a5381-170">Post</span></span>](../api/opentypeextension-post-opentypeextension.md) | <span data-ttu-id="a5381-171">[openTypeExtension](opentypeextension.md)（在现有资源实例中），或新[联系人](../resources/contact.md)、[事件](../resources/event.md)或[消息](../resources/message.md)，其中包含一个 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="a5381-171">[openTypeExtension](opentypeextension.md)(in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="a5381-172">在现有的或新的资源实例中创建 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="a5381-172">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="a5381-173">获取</span><span class="sxs-lookup"><span data-stu-id="a5381-173">Get</span></span>](../api/opentypeextension-get.md) | [<span data-ttu-id="a5381-174">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="a5381-174">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="a5381-175">读取 openTypeExtension 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a5381-175">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="a5381-176">更新</span><span class="sxs-lookup"><span data-stu-id="a5381-176">Update</span></span>](../api/opentypeextension-update.md) | [<span data-ttu-id="a5381-177">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="a5381-177">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="a5381-178">更新 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="a5381-178">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="a5381-179">删除</span><span class="sxs-lookup"><span data-stu-id="a5381-179">Delete</span></span>](../api/opentypeextension-delete.md) | <span data-ttu-id="a5381-180">无</span><span class="sxs-lookup"><span data-stu-id="a5381-180">None</span></span> |<span data-ttu-id="a5381-181">删除 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="a5381-181">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/opentypeextension.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
