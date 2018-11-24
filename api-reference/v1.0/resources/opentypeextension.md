# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="20ffb-101">openTypeExtension 资源类型（开放扩展）</span><span class="sxs-lookup"><span data-stu-id="20ffb-101">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="20ffb-102">打开扩展 （之前被称为 Office 365 数据扩展） 提供轻松直接将非类型化的属性添加到 Microsoft Graph 中的资源。</span><span class="sxs-lookup"><span data-stu-id="20ffb-102">Open extensions (formerly known as Office 365 data extensions) provide an easy way to directly add untyped properties to a resource in Microsoft Graph.</span></span>

<span data-ttu-id="20ffb-103">开放扩展由 **openTypeExtension** 资源表示。</span><span class="sxs-lookup"><span data-stu-id="20ffb-103">Open extensions are represented by the **openTypeExtension** resource.</span></span> <span data-ttu-id="20ffb-104">添加到资源的所有开放扩展都会显示在派生自 [extension](extension.md) 抽象类型的 **extensions** 导航属性中。</span><span class="sxs-lookup"><span data-stu-id="20ffb-104">Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.</span></span> <span data-ttu-id="20ffb-105">每个扩展都有 **extensionName** 属性（这是所有扩展的预定义唯一可写属性）和自定义数据。</span><span class="sxs-lookup"><span data-stu-id="20ffb-105">Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data.</span></span>

<span data-ttu-id="20ffb-106">一种有助于确保扩展名称唯一性的方法是，使用反向域名系统 (DNS) 格式，此格式依赖_用户自己的域_。例如，`Com.Contoso.ContactInfo`。</span><span class="sxs-lookup"><span data-stu-id="20ffb-106">One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`.</span></span> <span data-ttu-id="20ffb-107">请勿在扩展名称中使用 Microsoft 域（`Com.Microsoft` 或 `Com.OnMicrosoft`）。</span><span class="sxs-lookup"><span data-stu-id="20ffb-107">Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="20ffb-108">开放扩展示例：[使用开放扩展向用户添加自定义数据](../../../concepts/extensibility_open_users.md)</span><span class="sxs-lookup"><span data-stu-id="20ffb-108">Open extension example: [Add custom data to users using open extensions](../../../concepts/extensibility_open_users.md)</span></span>

<span data-ttu-id="20ffb-109">一般可用性（GA: /v1.0 和 /beta）或预览版 (/beta) 对应版本中的以下资源支持开放扩展。</span><span class="sxs-lookup"><span data-stu-id="20ffb-109">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

|<span data-ttu-id="20ffb-110">资源</span><span class="sxs-lookup"><span data-stu-id="20ffb-110">Resource</span></span> |<span data-ttu-id="20ffb-111">版本</span><span class="sxs-lookup"><span data-stu-id="20ffb-111">Version</span></span> |
|:---------------|:-------|
| [<span data-ttu-id="20ffb-112">管理单元</span><span class="sxs-lookup"><span data-stu-id="20ffb-112">Administrative unit</span></span>](../../beta/resources/administrativeunit.md)  | <span data-ttu-id="20ffb-113">仅供预览</span><span class="sxs-lookup"><span data-stu-id="20ffb-113">Preview only</span></span> |
| [<span data-ttu-id="20ffb-114">日历事件</span><span class="sxs-lookup"><span data-stu-id="20ffb-114">Calendar event</span></span>](event.md) | <span data-ttu-id="20ffb-115">GA</span><span class="sxs-lookup"><span data-stu-id="20ffb-115">GA</span></span> |
| <span data-ttu-id="20ffb-116">组[日历事件](event.md)</span><span class="sxs-lookup"><span data-stu-id="20ffb-116">Group [calendar event](event.md)</span></span> | <span data-ttu-id="20ffb-117">GA</span><span class="sxs-lookup"><span data-stu-id="20ffb-117">GA</span></span> |
| <span data-ttu-id="20ffb-118">组对话线程[帖子](post.md)</span><span class="sxs-lookup"><span data-stu-id="20ffb-118">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="20ffb-119">GA</span><span class="sxs-lookup"><span data-stu-id="20ffb-119">GA</span></span> |
| [<span data-ttu-id="20ffb-120">设备</span><span class="sxs-lookup"><span data-stu-id="20ffb-120">device</span></span>](device.md) | <span data-ttu-id="20ffb-121">GA</span><span class="sxs-lookup"><span data-stu-id="20ffb-121">GA</span></span> |
| [<span data-ttu-id="20ffb-122">组</span><span class="sxs-lookup"><span data-stu-id="20ffb-122">group</span></span>](group.md) | <span data-ttu-id="20ffb-123">GA</span><span class="sxs-lookup"><span data-stu-id="20ffb-123">GA</span></span> |
| [<span data-ttu-id="20ffb-124">邮件</span><span class="sxs-lookup"><span data-stu-id="20ffb-124">message</span></span>](message.md) | <span data-ttu-id="20ffb-125">GA</span><span class="sxs-lookup"><span data-stu-id="20ffb-125">GA</span></span> |
| [<span data-ttu-id="20ffb-126">组织</span><span class="sxs-lookup"><span data-stu-id="20ffb-126">organization</span></span>](organization.md) | <span data-ttu-id="20ffb-127">GA</span><span class="sxs-lookup"><span data-stu-id="20ffb-127">GA</span></span> |
| [<span data-ttu-id="20ffb-128">个人联系人</span><span class="sxs-lookup"><span data-stu-id="20ffb-128">Personal contact</span></span>](contact.md) | <span data-ttu-id="20ffb-129">GA</span><span class="sxs-lookup"><span data-stu-id="20ffb-129">GA</span></span> |
| [<span data-ttu-id="20ffb-130">用户</span><span class="sxs-lookup"><span data-stu-id="20ffb-130">user</span></span>](user.md) | <span data-ttu-id="20ffb-131">GA</span><span class="sxs-lookup"><span data-stu-id="20ffb-131">GA</span></span> |

## <a name="outlook-specific-considerations"></a><span data-ttu-id="20ffb-132">特定于 outlook 的注意事项</span><span class="sxs-lookup"><span data-stu-id="20ffb-132">Outlook-specific considerations</span></span>

<span data-ttu-id="20ffb-133">每个打开的扩展名存在于 Outlook 的资源 （事件、 消息或个人联系人） 存储在[MAPI 命名属性](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx)。</span><span class="sxs-lookup"><span data-stu-id="20ffb-133">Each open extension present on an Outlook resource (event, message, or personal contact) is stored in a [MAPI named property](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx).</span></span> <span data-ttu-id="20ffb-134">为 Outlook 创建打开扩展时，请考虑 MAPI 命名属性是用户的邮箱的有限资源。</span><span class="sxs-lookup"><span data-stu-id="20ffb-134">When you create open extensions for Outlook, consider that MAPI named properties are a finite resource in a user's mailbox.</span></span> <span data-ttu-id="20ffb-135">在用尽用户的命名的属性配额时，您无法创建该用户的任何多命名的属性。</span><span class="sxs-lookup"><span data-stu-id="20ffb-135">When a user's named property quota is exhausted, you can't create any more named properties for that user.</span></span> <span data-ttu-id="20ffb-136">这会导致出现异常行为依赖于对函数的命名属性的客户端。</span><span class="sxs-lookup"><span data-stu-id="20ffb-136">This can result in unexpected behavior from clients that rely on named properties to function.</span></span>

<span data-ttu-id="20ffb-137">打开扩展名创建在 Outlook 资源时，请应用以下准则：</span><span class="sxs-lookup"><span data-stu-id="20ffb-137">Apply the following guidelines when you create open extensions on Outlook resources:</span></span>

- <span data-ttu-id="20ffb-138">创建所需的扩展的最小数目。</span><span class="sxs-lookup"><span data-stu-id="20ffb-138">Create the minimum number of extensions required.</span></span> <span data-ttu-id="20ffb-139">大多数应用程序应该要求不多个扩展名。</span><span class="sxs-lookup"><span data-stu-id="20ffb-139">Most applications should require no more than one extension.</span></span> <span data-ttu-id="20ffb-140">扩展具有未定义的设置的属性或结构，因此您可以将多个值存储在一个扩展。</span><span class="sxs-lookup"><span data-stu-id="20ffb-140">Extensions have no set defined properties or structure, so you can store multiple values in a single extension.</span></span>
- <span data-ttu-id="20ffb-141">避免 （例如，基于用户输入等。） 来扩展命名变量的方式。</span><span class="sxs-lookup"><span data-stu-id="20ffb-141">Avoid naming extensions in a variable manner (such as based on user input, etc.).</span></span> <span data-ttu-id="20ffb-142">打开扩展名创建新的名称之前, 的用户的邮箱中未用过的每次创建新的 MAPI 命名属性。</span><span class="sxs-lookup"><span data-stu-id="20ffb-142">Each time an open extension is created with a new name that has not been used in a user's mailbox before, a new MAPI named property is created.</span></span> <span data-ttu-id="20ffb-143">删除扩展不会删除的命名的属性。</span><span class="sxs-lookup"><span data-stu-id="20ffb-143">Removing the extension does not remove the named property.</span></span>

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="20ffb-144">使用打开扩展名 （对于 Outlook 资源） 或扩展的属性</span><span class="sxs-lookup"><span data-stu-id="20ffb-144">Use open extensions (for Outlook resources) or extended properties</span></span>

<span data-ttu-id="20ffb-145">打开扩展是适用于大多数的方案涉及存储和访问自定义数据的建议的解决方案。</span><span class="sxs-lookup"><span data-stu-id="20ffb-145">Open extensions are the recommended solution for most scenarios involving storing and accessing custom data.</span></span> <span data-ttu-id="20ffb-146">但是，您需要通过[Microsoft Graph API 元数据](https://developer.microsoft.com/graph/docs/overview/call_api)访问自定义 Outlook MAPI 属性未已公开的数据，您可以使用[扩展的属性和其 REST API](extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="20ffb-146">If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md).</span></span> <span data-ttu-id="20ffb-147">您可以验证元数据在公开哪些属性[https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata)。</span><span class="sxs-lookup"><span data-stu-id="20ffb-147">You can verify which properties the metadata exposes at [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).</span></span>

## <a name="json-representation"></a><span data-ttu-id="20ffb-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20ffb-148">JSON representation</span></span>

<span data-ttu-id="20ffb-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20ffb-149">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="20ffb-150">属性</span><span class="sxs-lookup"><span data-stu-id="20ffb-150">Properties</span></span>

|<span data-ttu-id="20ffb-151">属性</span><span class="sxs-lookup"><span data-stu-id="20ffb-151">Property</span></span> | <span data-ttu-id="20ffb-152">类型</span><span class="sxs-lookup"><span data-stu-id="20ffb-152">Type</span></span> | <span data-ttu-id="20ffb-153">说明</span><span class="sxs-lookup"><span data-stu-id="20ffb-153">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="20ffb-154">extensionName</span><span class="sxs-lookup"><span data-stu-id="20ffb-154">extensionName</span></span>|<span data-ttu-id="20ffb-155">字符串</span><span class="sxs-lookup"><span data-stu-id="20ffb-155">String</span></span>|<span data-ttu-id="20ffb-p107">开放类型开放扩展的唯一文本标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="20ffb-p107">A unique text identifier for an open type open extension. Required.</span></span>|
|<span data-ttu-id="20ffb-158">id</span><span class="sxs-lookup"><span data-stu-id="20ffb-158">id</span></span>|<span data-ttu-id="20ffb-159">String</span><span class="sxs-lookup"><span data-stu-id="20ffb-159">String</span></span>| <span data-ttu-id="20ffb-p108">连接具有 **extensionName** 扩展类型的完全限定的标识符 。只读。</span><span class="sxs-lookup"><span data-stu-id="20ffb-p108">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20ffb-162">关系</span><span class="sxs-lookup"><span data-stu-id="20ffb-162">Relationships</span></span>

<span data-ttu-id="20ffb-163">无</span><span class="sxs-lookup"><span data-stu-id="20ffb-163">None</span></span>

## <a name="methods"></a><span data-ttu-id="20ffb-164">方法</span><span class="sxs-lookup"><span data-stu-id="20ffb-164">Methods</span></span>

|<span data-ttu-id="20ffb-165">方法</span><span class="sxs-lookup"><span data-stu-id="20ffb-165">Method</span></span> | <span data-ttu-id="20ffb-166">返回类型</span><span class="sxs-lookup"><span data-stu-id="20ffb-166">Return Type</span></span> | <span data-ttu-id="20ffb-167">说明</span><span class="sxs-lookup"><span data-stu-id="20ffb-167">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="20ffb-168">Post</span><span class="sxs-lookup"><span data-stu-id="20ffb-168">Post</span></span>](../api/opentypeextension_post_opentypeextension.md) | <span data-ttu-id="20ffb-169">[openTypeExtension](opentypeextension.md)（在现有资源实例中），或包含 openTypeExtension 对象的新 [contact](../resources/contact.md)、[event](../resources/event.md) 或 [message](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="20ffb-169">[openTypeExtension](opentypeextension.md) (in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object</span></span> | <span data-ttu-id="20ffb-170">在现有的或新的资源实例中创建 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="20ffb-170">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="20ffb-171">获取</span><span class="sxs-lookup"><span data-stu-id="20ffb-171">Get</span></span>](../api/opentypeextension_get.md) | [<span data-ttu-id="20ffb-172">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="20ffb-172">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="20ffb-173">读取 openTypeExtension 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="20ffb-173">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="20ffb-174">更新</span><span class="sxs-lookup"><span data-stu-id="20ffb-174">Update</span></span>](../api/opentypeextension_update.md) | [<span data-ttu-id="20ffb-175">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="20ffb-175">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="20ffb-176">更新 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="20ffb-176">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="20ffb-177">删除</span><span class="sxs-lookup"><span data-stu-id="20ffb-177">Delete</span></span>](../api/opentypeextension_delete.md) | <span data-ttu-id="20ffb-178">无</span><span class="sxs-lookup"><span data-stu-id="20ffb-178">None</span></span> |<span data-ttu-id="20ffb-179">删除 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="20ffb-179">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
