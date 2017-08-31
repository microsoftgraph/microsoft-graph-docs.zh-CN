# <a name="opentypeextension-resource-type-open-extensions"></a><span data-ttu-id="a81ee-101">openTypeExtension 资源类型（开放扩展）</span><span class="sxs-lookup"><span data-stu-id="a81ee-101">openTypeExtension resource type (open extensions)</span></span>

<span data-ttu-id="a81ee-p101">开放扩展（以前被称为 Office 365 数据扩展）提供了一种简单方法，可直接将非类型化属性添加到 Microsoft Graph 中的资源。开放扩展由 **openTypeExtension** 资源表示。添加到资源的任何开放扩展都会显示在 **extensions** 导航属性中，该属性派生自 [extension](extension.md) 抽象类型。每个扩展都有一个 **extensionName** 属性，它是所有扩展以及自定义数据的唯一一个可预定义、可写入的属性。帮助确保扩展名称唯一性的一种方法是使用反向域名名称系统 (DNS) 格式，该格式取决于你拥有的域，例如 `Com.Contoso.ContactInfo`。请勿在扩展名中使用 Microsoft 域（`Com.Microsoft` 或 `Com.OnMicrosoft`）。</span><span class="sxs-lookup"><span data-stu-id="a81ee-p101">Open extensions (formerly known as Office 365 data extensions) gives you an easy way to directly add untyped properties to a resource in Microsoft Graph. Open extensions are represented by the **openTypeExtension** resource. Any open extension added to a resource shows up in the **extensions** navigation property, which is derived from the [extension](extension.md) abstract type.  Each extension has an **extensionName** property which is the only pre-defined, writable property for all extensions, along with your custom data. One way to help make sure extension names are unique is to use a reverse domain name system (DNS) format that is dependent on _your own domain_, for example, `Com.Contoso.ContactInfo`. Do not use the Microsoft domain (`Com.Microsoft` or `Com.OnMicrosoft`) in an extension name.</span></span>

<span data-ttu-id="a81ee-108">开放扩展示例：[使用开放扩展向用户添加自定义数据](../../../concepts/extensibility_open_users.md)</span><span class="sxs-lookup"><span data-stu-id="a81ee-108">Open extension example: [Add custom data to users using open extensions](../../../concepts/extensibility_open_users.md)</span></span>

<span data-ttu-id="a81ee-109">一般可用性（GA: /v1.0 和 /beta）或预览版 (/beta) 对应版本中的以下资源支持开放扩展。</span><span class="sxs-lookup"><span data-stu-id="a81ee-109">Open extensions are supported by the following resources in the corresponding versions - general availability (GA: /v1.0 and /beta) or preview (/beta).</span></span>

| <span data-ttu-id="a81ee-110">资源</span><span class="sxs-lookup"><span data-stu-id="a81ee-110">Resource</span></span> | <span data-ttu-id="a81ee-111">版本</span><span class="sxs-lookup"><span data-stu-id="a81ee-111">Version</span></span> |
|---------------|-------|
| [<span data-ttu-id="a81ee-112">管理单元</span><span class="sxs-lookup"><span data-stu-id="a81ee-112">Administrative unit</span></span>](../../beta/resources/administrativeunit.md)  | <span data-ttu-id="a81ee-113">仅供预览</span><span class="sxs-lookup"><span data-stu-id="a81ee-113">Preview only</span></span> |
| [<span data-ttu-id="a81ee-114">日历事件</span><span class="sxs-lookup"><span data-stu-id="a81ee-114">Calendar event</span></span>](event.md) | <span data-ttu-id="a81ee-115">GA</span><span class="sxs-lookup"><span data-stu-id="a81ee-115">GA</span></span> |
| <span data-ttu-id="a81ee-116">组[日历事件](event.md)</span><span class="sxs-lookup"><span data-stu-id="a81ee-116">[Group calendar event](event.md)</span></span> | <span data-ttu-id="a81ee-117">GA</span><span class="sxs-lookup"><span data-stu-id="a81ee-117">GA</span></span> |
| <span data-ttu-id="a81ee-118">组对话线程[帖子](post.md)</span><span class="sxs-lookup"><span data-stu-id="a81ee-118">Group conversation thread [post](post.md)</span></span> | <span data-ttu-id="a81ee-119">GA</span><span class="sxs-lookup"><span data-stu-id="a81ee-119">GA</span></span> |
| [<span data-ttu-id="a81ee-120">设备</span><span class="sxs-lookup"><span data-stu-id="a81ee-120">device</span></span>](device.md) | <span data-ttu-id="a81ee-121">GA</span><span class="sxs-lookup"><span data-stu-id="a81ee-121">GA</span></span> |
| [<span data-ttu-id="a81ee-122">组</span><span class="sxs-lookup"><span data-stu-id="a81ee-122">group</span></span>](group.md) | <span data-ttu-id="a81ee-123">GA</span><span class="sxs-lookup"><span data-stu-id="a81ee-123">GA</span></span> |
| [<span data-ttu-id="a81ee-124">邮件</span><span class="sxs-lookup"><span data-stu-id="a81ee-124">message</span></span>](message.md) | <span data-ttu-id="a81ee-125">GA</span><span class="sxs-lookup"><span data-stu-id="a81ee-125">GA</span></span> |
| [<span data-ttu-id="a81ee-126">组织</span><span class="sxs-lookup"><span data-stu-id="a81ee-126">organization</span></span>](organization.md) | <span data-ttu-id="a81ee-127">GA</span><span class="sxs-lookup"><span data-stu-id="a81ee-127">GA</span></span> |
| [<span data-ttu-id="a81ee-128">个人联系人</span><span class="sxs-lookup"><span data-stu-id="a81ee-128">Personal contact</span></span>](contact.md) | <span data-ttu-id="a81ee-129">GA</span><span class="sxs-lookup"><span data-stu-id="a81ee-129">GA</span></span> |
| [<span data-ttu-id="a81ee-130">用户</span><span class="sxs-lookup"><span data-stu-id="a81ee-130">user</span></span>](user.md) | <span data-ttu-id="a81ee-131">GA</span><span class="sxs-lookup"><span data-stu-id="a81ee-131">GA</span></span> |

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a><span data-ttu-id="a81ee-132">使用开放扩展（针对 Outlook 资源）还是使用扩展属性？</span><span class="sxs-lookup"><span data-stu-id="a81ee-132">Use open extensions (for Outlook resources) or extended properties?</span></span>

<span data-ttu-id="a81ee-p102">开放扩展是大部分涉及存储和访问自定义数据的应用场景的推荐解决方案。不过，如果需要访问尚未通过 [Microsoft Graph API 元数据](http://developer.microsoft.com/en-us/graph/docs/overview/call_api)公开的 Outlook MAPI 属性的自定义数据，则可以使用[扩展属性及其 REST API](extended-properties-overview.md)。若要确认元数据公开了哪些属性，请访问 https://graph.microsoft.com/v1.0/$metadata。</span><span class="sxs-lookup"><span data-stu-id="a81ee-p102">Open extensions is the recommended solution for most scenarios involving storing and accessing custom data. If, however, you need to access custom data for Outlook MAPI properties that are not already exposed through the [Microsoft Graph API metadata](http://developer.microsoft.com/en-us/graph/docs/overview/call_api), you can use [extended properties and its REST API](extended-properties-overview.md). You can verify which properties the metadata exposes at https://graph.microsoft.com/v1.0/$metadata.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a81ee-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a81ee-136">JSON representation</span></span>

<span data-ttu-id="a81ee-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a81ee-137">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="a81ee-138">属性</span><span class="sxs-lookup"><span data-stu-id="a81ee-138">Properties</span></span>
| <span data-ttu-id="a81ee-139">属性</span><span class="sxs-lookup"><span data-stu-id="a81ee-139">Property</span></span>     | <span data-ttu-id="a81ee-140">类型</span><span class="sxs-lookup"><span data-stu-id="a81ee-140">Type</span></span>   |<span data-ttu-id="a81ee-141">说明</span><span class="sxs-lookup"><span data-stu-id="a81ee-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a81ee-142">extensionName</span><span class="sxs-lookup"><span data-stu-id="a81ee-142">extensionName</span></span>|<span data-ttu-id="a81ee-143">String</span><span class="sxs-lookup"><span data-stu-id="a81ee-143">String</span></span>|<span data-ttu-id="a81ee-p103">开放类型开放扩展的唯一文本标识符。必需。</span><span class="sxs-lookup"><span data-stu-id="a81ee-p103">A unique text identifier for an open type open extension. Required.</span></span>|
|<span data-ttu-id="a81ee-146">id</span><span class="sxs-lookup"><span data-stu-id="a81ee-146">id</span></span>|<span data-ttu-id="a81ee-147">String</span><span class="sxs-lookup"><span data-stu-id="a81ee-147">String</span></span>| <span data-ttu-id="a81ee-p104">连接具有 **extensionName** 扩展类型的完全限定的标识符 。只读。</span><span class="sxs-lookup"><span data-stu-id="a81ee-p104">A fully qualified identifier that concatenates the extension type with the **extensionName**. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a81ee-150">关系</span><span class="sxs-lookup"><span data-stu-id="a81ee-150">Relationships</span></span>
<span data-ttu-id="a81ee-151">无</span><span class="sxs-lookup"><span data-stu-id="a81ee-151">None</span></span>


## <a name="methods"></a><span data-ttu-id="a81ee-152">方法</span><span class="sxs-lookup"><span data-stu-id="a81ee-152">Methods</span></span>

| <span data-ttu-id="a81ee-153">方法</span><span class="sxs-lookup"><span data-stu-id="a81ee-153">Method</span></span>           | <span data-ttu-id="a81ee-154">返回类型</span><span class="sxs-lookup"><span data-stu-id="a81ee-154">Return Type</span></span>    |<span data-ttu-id="a81ee-155">说明</span><span class="sxs-lookup"><span data-stu-id="a81ee-155">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a81ee-156">Post</span><span class="sxs-lookup"><span data-stu-id="a81ee-156">Post</span></span>](../api/opentypeextension_post_opentypeextension.md) | <span data-ttu-id="a81ee-157">现有资源实体中的 [openTypeExtension](opentypeextension.md) 或包含 openTypeExtension 对象的新[联系人](../resources/contact.md)、[事件](../resources/event.md)或[消息](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="a81ee-157">[openTypeExtension](opentypeextension.md) (in an existing resource instance), or a new [contact](../resources/contact.md), [event](../resources/event.md), or [message](../resources/message.md) that contains an openTypeExtension object.</span></span> | <span data-ttu-id="a81ee-158">在现有或新建资源实例中创建 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="a81ee-158">Create an openTypeExtension object in an existing or new resource instance.</span></span>|
|[<span data-ttu-id="a81ee-159">获取</span><span class="sxs-lookup"><span data-stu-id="a81ee-159">Get</span></span>](../api/opentypeextension_get.md) | [<span data-ttu-id="a81ee-160">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="a81ee-160">openTypeExtension</span></span>](opentypeextension.md) |<span data-ttu-id="a81ee-161">读取 openTypeExtension 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a81ee-161">Read properties and relationships of openTypeExtension object.</span></span>|
|[<span data-ttu-id="a81ee-162">更新</span><span class="sxs-lookup"><span data-stu-id="a81ee-162">Update</span></span>](../api/opentypeextension_update.md) | [<span data-ttu-id="a81ee-163">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="a81ee-163">openTypeExtension</span></span>](opentypeextension.md)   |<span data-ttu-id="a81ee-164">更新 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="a81ee-164">Update openTypeExtension object.</span></span> |
|[<span data-ttu-id="a81ee-165">删除</span><span class="sxs-lookup"><span data-stu-id="a81ee-165">Delete</span></span>](../api/opentypeextension_delete.md) | <span data-ttu-id="a81ee-166">无</span><span class="sxs-lookup"><span data-stu-id="a81ee-166">None</span></span> |<span data-ttu-id="a81ee-167">删除 openTypeExtension 对象。</span><span class="sxs-lookup"><span data-stu-id="a81ee-167">Delete openTypeExtension object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->