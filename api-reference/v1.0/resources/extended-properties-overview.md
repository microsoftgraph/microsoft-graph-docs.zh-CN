# <a name="outlook-extended-properties-overview"></a><span data-ttu-id="6c7a1-101">Outlook 扩展属性概述</span><span class="sxs-lookup"><span data-stu-id="6c7a1-101">Outlook extended properties overview</span></span>

<span data-ttu-id="6c7a1-p101">扩展属性允许存储自定义数据，当 Outlook MAPI 属性_尚未在 Microsoft Graph API 元数据中公开_时，扩展属性专门用作应用访问这些属性的自定义数据的回退机制。可以使用扩展属性 REST API 在以下用户资源中存储或获取此类自定义数据：</span><span class="sxs-lookup"><span data-stu-id="6c7a1-p101">Extended properties allow storing custom data and specifically serve as a fallback mechanism for apps to access custom data for Outlook MAPI properties when these properties are _not already exposed in the Microsoft Graph API metadata_. You can use extended properties REST API to store or get such custom data in the following user resources:</span></span>

- [<span data-ttu-id="6c7a1-104">邮件</span><span class="sxs-lookup"><span data-stu-id="6c7a1-104">message</span></span>](../resources/message.md)
- [<span data-ttu-id="6c7a1-105">mailFolder</span><span class="sxs-lookup"><span data-stu-id="6c7a1-105">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="6c7a1-106">事件</span><span class="sxs-lookup"><span data-stu-id="6c7a1-106">event</span></span>](../resources/event.md)
- [<span data-ttu-id="6c7a1-107">日历</span><span class="sxs-lookup"><span data-stu-id="6c7a1-107">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="6c7a1-108">联系人</span><span class="sxs-lookup"><span data-stu-id="6c7a1-108">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="6c7a1-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="6c7a1-109">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="6c7a1-110">或者，在以下 Office 365 组资源中：</span><span class="sxs-lookup"><span data-stu-id="6c7a1-110">Or, in the following Office 365 group resources:</span></span>

- <span data-ttu-id="6c7a1-111">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="6c7a1-111">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="6c7a1-112">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="6c7a1-112">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="6c7a1-113">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="6c7a1-113">group [post](../resources/post.md)</span></span> 

## <a name="use-extended-properties-or-open-extensions"></a><span data-ttu-id="6c7a1-114">使用扩展属性还是开放扩展？</span><span class="sxs-lookup"><span data-stu-id="6c7a1-114">Use extended properties or open extensions?</span></span>

<span data-ttu-id="6c7a1-p102">在大多数的常见情况下，你应该能够使用开放扩展（用 [openTypeExtension](../resources/opentypeextension.md) 表示，以前被称为 Office 365 数据扩展）来存储和访问用户邮箱中资源实例的自定义数据。仅当需要访问尚未通过 [Microsoft Graph API 元数据](http://developer.microsoft.com/en-us/graph/docs/overview/call_api)公开的 Outlook MAPI 属性的自定义数据时使用扩展属性。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-p102">In most common scenarios, you should be able to use open extensions (represented by [openTypeExtension](../resources/opentypeextension.md), formerly known as Office 365 data extensions) to store and access custom data for resource instances in a user's mailbox. Use extended properties only if you need to access custom data for Outlook MAPI properties that are not already exposed in the [Microsoft Graph API metadata](http://developer.microsoft.com/en-us/graph/docs/overview/call_api).</span></span> 

## <a name="types-of-extended-properties"></a><span data-ttu-id="6c7a1-117">扩展属性的类型</span><span class="sxs-lookup"><span data-stu-id="6c7a1-117">Types of extended properties</span></span>

<span data-ttu-id="6c7a1-118">根据是否打算将单个值或多个值（相同类型）存储在一个扩展属性中，可以将扩展属性创建为 [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) 或 [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md)。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-118">Depending on whether you intend to store a single or multiple values (of the same type) in an extended property, you can create an extended property as a [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md), or [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md).</span></span>

<span data-ttu-id="6c7a1-119">其中的每种类型都通过其 **id** 进行标识并将数据存储在 **value** 中。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-119">Each of these types identifies the property by its **id** and stores data in **value**.</span></span> 

<span data-ttu-id="6c7a1-120">可以使用 **id** 获取特定的资源实例以及该扩展属性，或筛选单值扩展属性以获取拥有该属性的所有实例。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-120">You can use **id** to get a specific resource instance together with that extended property, or filter on a single-value extended property to get all the instances that have that property.</span></span> 

<span data-ttu-id="6c7a1-121">**注意**不能使用 REST API 在一个调用中获取特定实例的所有扩展属性。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-121">**Note** You cannot use the REST API to get all the extended properties of a specific instance in one call.</span></span>
  

### <a name="id-formats"></a><span data-ttu-id="6c7a1-122">id 格式</span><span class="sxs-lookup"><span data-stu-id="6c7a1-122">id Formats</span></span>

<span data-ttu-id="6c7a1-123">您可以使用以下三种格式之一指定扩展属性的 **id** :</span><span class="sxs-lookup"><span data-stu-id="6c7a1-123">You can specify **id** of an extended property in one of three formats:</span></span>

- <span data-ttu-id="6c7a1-124">由扩展属性类型、命名空间和字符串名称标识的命名属性。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-124">As a named property, identified by the extended property type, namespace, and a string name.</span></span>
- <span data-ttu-id="6c7a1-125">由扩展属性类型、命名空间和一个数字标识符标识的命名属性。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-125">As a named property, identified by the extended property type, namespace, and a numeric identifier.</span></span>
- <span data-ttu-id="6c7a1-126">由扩展的属性类型和 [MAPI 属性标记](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags)标识的属性标记格式。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-126">In a proptag format, identified by the extended property type and a [MAPI property tag](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).</span></span>

<span data-ttu-id="6c7a1-127">接下来的两个表描述了这些格式应用于单值和多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-127">The next 2 tables below describe the supported formats to specify single and multi-value extended properties.</span></span> <span data-ttu-id="6c7a1-128">{_type_} 表示一个或多个扩展属性值的类型。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-128">{_type_} represents the type of the value or values of the property.</span></span> <span data-ttu-id="6c7a1-129">示例中使用的是 string、integer 和这些类型的数组。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-129">Shown in the examples are string, integer, and arrays of these types.</span></span>

<span data-ttu-id="6c7a1-130">**单值扩展属性的有效 id 格式**</span><span class="sxs-lookup"><span data-stu-id="6c7a1-130">**Valid id formats for single-value extended properties**</span></span>

|<span data-ttu-id="6c7a1-131">**格式**</span><span class="sxs-lookup"><span data-stu-id="6c7a1-131">**Format**</span></span>|<span data-ttu-id="6c7a1-132">**示例**</span><span class="sxs-lookup"><span data-stu-id="6c7a1-132">**Example**</span></span>|<span data-ttu-id="6c7a1-133">**说明**</span><span class="sxs-lookup"><span data-stu-id="6c7a1-133">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="6c7a1-134">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="6c7a1-134">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="6c7a1-135">用所属的命名空间 (GUID) 和字符串名称标识属性。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-135">Identifies a property by the namespace (the GUID) it belongs to, and a name.</span></span>         |
| <span data-ttu-id="6c7a1-136">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="6c7a1-136">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | <span data-ttu-id="6c7a1-137">用所属的命名空间 (GUID) 和数字标识符标识属性。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-137">Identifies a property by the namespace (the GUID) it belongs to, and a name.</span></span>  |
| <span data-ttu-id="6c7a1-138">"{_type_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="6c7a1-138">"{_type_} {_proptag_}"</span></span>                    | ```"String 0x4001001E"```                                           | <span data-ttu-id="6c7a1-139">根据属性标记标识的预定义属性。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-139">Identifies a pre-defined property by its property tag.</span></span> |

<span data-ttu-id="6c7a1-140">**多值扩展属性的有效 id 格式**</span><span class="sxs-lookup"><span data-stu-id="6c7a1-140">**Valid id formats for multi-value extended properties**</span></span>

|<span data-ttu-id="6c7a1-141">**格式**</span><span class="sxs-lookup"><span data-stu-id="6c7a1-141">**Format**</span></span>|<span data-ttu-id="6c7a1-142">**示例**</span><span class="sxs-lookup"><span data-stu-id="6c7a1-142">**Example**</span></span>|<span data-ttu-id="6c7a1-143">**说明**</span><span class="sxs-lookup"><span data-stu-id="6c7a1-143">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="6c7a1-144">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="6c7a1-144">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="6c7a1-145">用命名空间 (GUID) 和字符串名称标识属性。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-145">Identifies a property by the namespace (the GUID) it belongs to, and a name.</span></span>         |
| <span data-ttu-id="6c7a1-146">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="6c7a1-146">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | <span data-ttu-id="6c7a1-147">用命名空间 (GUID) 和数字标识符标识属性。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-147">Identifies a property by the namespace (the GUID) it belongs to, and a name.</span></span>   |
| <span data-ttu-id="6c7a1-148">"{_type_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="6c7a1-148">"{_type_} {_proptag_}"</span></span>                    | ```"StringArray 0x4002101E"```                                           | <span data-ttu-id="6c7a1-149">根据属性标记标识的预定义属性。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-149">Identifies a pre-defined property by its property tag.</span></span> |


<span data-ttu-id="6c7a1-150">使用任一命名属性格式将单值或多值扩展属性定义为自定义属性。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-150">Use either of the named property formats to define a single-value or multi-value extended property as a custom property.</span></span> <span data-ttu-id="6c7a1-151">在这两种格式中，第一种采用字符串名称 (**Name**)，是便于引用的首选格式。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-151">Among the two formats, the first one that takes a string name (**Name**) is the preferred format for ease of reference.</span></span> <span data-ttu-id="6c7a1-152">命名属性在 0x8000 0xfffe 范围内有及其 [属性标识符](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview)。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-152">Named properties have their [property identifiers](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in the 0x8000-0xfffe range.</span></span>

<span data-ttu-id="6c7a1-153">使用属性标记格式访问由 MAPI，或客户端或服务器预定义的属性，以及尚未在 Microsoft Graph 中公开的属性。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-153">Use the proptag format to access properties predefined by MAPI, or by a client or server, and that have not already been exposed in Microsoft Graph.</span></span> <span data-ttu-id="6c7a1-154">这些属性在 0x0001 0x7fff 范围内有属性标识符。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-154">These properties have property identifiers in the 0x0001-0x7fff range.</span></span> <span data-ttu-id="6c7a1-155">不要尝试使用属性标记格式定义自定义属性。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-155">Do not try to define a custom property using the proptag format.</span></span> 

<span data-ttu-id="6c7a1-156">在 \[MS-OXPROPS\] Microsoft Corporation 的[“Exchange Server 协议 Master 属性列表”](https://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx)中，可以了解如何将扩展属性映射到现有 MAPI 属性，如属性标识符和 GUID。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-156">You can find information about mapping an extended property to an existing MAPI property, such as the property identifier and GUID, in \[MS-OXPROPS\] Microsoft Corporation, ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx).</span></span>

<span data-ttu-id="6c7a1-157">**注意**：为 **id** 选择一种格式后，只能按此格式访问扩展属性。</span><span class="sxs-lookup"><span data-stu-id="6c7a1-157">**Note** After you have chosen one format for the **id**, you should access that extended property by only that format.</span></span>

### <a name="rest-api-operations"></a><span data-ttu-id="6c7a1-158">REST API 操作</span><span class="sxs-lookup"><span data-stu-id="6c7a1-158">REST API operations</span></span>
 
<span data-ttu-id="6c7a1-159">单值扩展属性的操作：</span><span class="sxs-lookup"><span data-stu-id="6c7a1-159">Single-value extended property operations:</span></span>

- [<span data-ttu-id="6c7a1-160">在新建或现有的资源实例中创建扩展属性</span><span class="sxs-lookup"><span data-stu-id="6c7a1-160">Create an extended property in a new or existing resource instance</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md)
- [<span data-ttu-id="6c7a1-161">使用 `$expand` 或 `$filter` 获取一个包含扩展属性的资源实例或资源实例集合 `$filter`</span><span class="sxs-lookup"><span data-stu-id="6c7a1-161">Get one or a collection of resource instances with an extended property using `$expand` or `$filter`</span></span>](../api/singlevaluelegacyextendedproperty_get.md)

<span data-ttu-id="6c7a1-162">多值扩展属性的操作：</span><span class="sxs-lookup"><span data-stu-id="6c7a1-162">Multi-value extended property operations:</span></span>

- [<span data-ttu-id="6c7a1-163">在新建或现有的资源实例中创建扩展属性</span><span class="sxs-lookup"><span data-stu-id="6c7a1-163">Create an extended property in a new or existing resource instance</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md)
- [<span data-ttu-id="6c7a1-164">使用 `$expand` 获取一个包含扩展属性的资源实例 `$expand`</span><span class="sxs-lookup"><span data-stu-id="6c7a1-164">Get a resource instance with an extended property using `$expand`</span></span>](../api/multivaluelegacyextendedproperty_get.md)

