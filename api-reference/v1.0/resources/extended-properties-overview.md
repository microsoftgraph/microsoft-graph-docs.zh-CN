# <a name="outlook-extended-properties-overview"></a><span data-ttu-id="83c93-101">Outlook 扩展属性概述</span><span class="sxs-lookup"><span data-stu-id="83c93-101">Outlook extended properties overview</span></span>

<span data-ttu-id="83c93-p101">扩展属性允许存储自定义数据，当 Outlook MAPI 属性_尚未在 Microsoft Graph API 元数据中公开_时，扩展属性专门用作应用访问这些属性的自定义数据的回退机制。可以使用扩展属性 REST API 在以下用户资源中存储或获取此类自定义数据：</span><span class="sxs-lookup"><span data-stu-id="83c93-p101">Extended properties allow storing custom data and specifically serve as a fallback mechanism for apps to access custom data for Outlook MAPI properties when these properties are _not already exposed in the Microsoft Graph API metadata_. You can use extended properties REST API to store or get such custom data in the following user resources:</span></span>

- [<span data-ttu-id="83c93-104">邮件</span><span class="sxs-lookup"><span data-stu-id="83c93-104">message</span></span>](../resources/message.md)
- [<span data-ttu-id="83c93-105">mailFolder</span><span class="sxs-lookup"><span data-stu-id="83c93-105">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="83c93-106">事件</span><span class="sxs-lookup"><span data-stu-id="83c93-106">event</span></span>](../resources/event.md)
- [<span data-ttu-id="83c93-107">日历</span><span class="sxs-lookup"><span data-stu-id="83c93-107">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="83c93-108">联系人</span><span class="sxs-lookup"><span data-stu-id="83c93-108">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="83c93-109">contactFolder</span><span class="sxs-lookup"><span data-stu-id="83c93-109">contactFolder</span></span>](../resources/contactfolder.md) 

<span data-ttu-id="83c93-110">或者，在以下 Office 365 组资源中：</span><span class="sxs-lookup"><span data-stu-id="83c93-110">Or, in the following Office 365 group resources:</span></span>

- <span data-ttu-id="83c93-111">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="83c93-111">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="83c93-112">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="83c93-112">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="83c93-113">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="83c93-113">group [post](../resources/post.md)</span></span> 

## <a name="use-extended-properties-or-open-extensions"></a><span data-ttu-id="83c93-114">使用扩展属性还是开放扩展？</span><span class="sxs-lookup"><span data-stu-id="83c93-114">Use extended properties or open extensions?</span></span>

<span data-ttu-id="83c93-p102">在大多数的常见情况下，你应该能够使用开放扩展（用 [openTypeExtension](../resources/opentypeextension.md) 表示，以前被称为 Office 365 数据扩展）来存储和访问用户邮箱中资源实例的自定义数据。仅当需要访问尚未通过 [Microsoft Graph API 元数据]((http://developer.microsoft.com/zh-CN/graph/docs/overview/call_api))公开的 Outlook MAPI 属性的自定义数据时使用扩展属性。</span><span class="sxs-lookup"><span data-stu-id="83c93-p102">In most common scenarios, you should be able to use open extensions (represented by [openTypeExtension](../resources/opentypeextension.md), formerly known as Office 365 data extensions) to store and access custom data for resource instances in a user's mailbox. Use extended properties only if you need to access custom data for Outlook MAPI properties that are not already exposed in the [Microsoft Graph API metadata]((http://developer.microsoft.com/zh-CN/graph/docs/overview/call_api)).</span></span> 

## <a name="types-of-extended-properties"></a><span data-ttu-id="83c93-117">扩展属性的类型</span><span class="sxs-lookup"><span data-stu-id="83c93-117">Types of extended properties</span></span>

<span data-ttu-id="83c93-118">根据是否打算将单个值或多个值（相同类型）存储在一个扩展属性中，可以将扩展属性创建为 [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) 或 [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md)。</span><span class="sxs-lookup"><span data-stu-id="83c93-118">Depending on whether you intend to store a single or multiple values (of the same type) in an extended property, you can create an extended property as a [singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md), or [multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md).</span></span>

<span data-ttu-id="83c93-119">其中的每种类型都通过其 **id** 进行标识并将数据存储在 **value** 中。</span><span class="sxs-lookup"><span data-stu-id="83c93-119">Each of these types identifies the property by its **id** and stores data in **value**.</span></span> 

<span data-ttu-id="83c93-120">可以使用 **id** 获取特定的资源实例以及该扩展属性，或筛选单值扩展属性以获取拥有该属性的所有实例。</span><span class="sxs-lookup"><span data-stu-id="83c93-120">You can use **id** to get a specific resource instance together with that extended property, or filter on a single-value extended property to get all the instances that have that property.</span></span> 

<span data-ttu-id="83c93-121">**注意** 不能使用 REST API 在一个调用中获取特定实例的所有扩展属性。</span><span class="sxs-lookup"><span data-stu-id="83c93-121">**Note** You cannot use the REST API to get all the extended properties of a specific instance in one call.</span></span>
  

### <a name="id-formats"></a><span data-ttu-id="83c93-122">id 格式</span><span class="sxs-lookup"><span data-stu-id="83c93-122">id Formats</span></span>

<span data-ttu-id="83c93-123">创建单值或多值扩展属性时，根据字符串名称 (**Name**) 或数字标识符 (**Id**) 以及一个或多个属性值的实际类型，可以按照两种格式中的任一种指定 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="83c93-123">When creating a single-value or multi-value extended property, you can specify the **id** property in one of two formats, based on either a string name (**Name**) or numeric identifier (**Id**), and on the actual type of value or values of the property.</span></span> <span data-ttu-id="83c93-124">接下来的两个表列出了指定单值和多值扩展属性时支持的格式。</span><span class="sxs-lookup"><span data-stu-id="83c93-124">The next 2 tables below describe the supported formats to specify single and multi-value extended properties.</span></span> <span data-ttu-id="83c93-125">{_type_} 表示一个或多个属性值的类型。</span><span class="sxs-lookup"><span data-stu-id="83c93-125">{_type_} represents the type of the value or values of the property.</span></span> <span data-ttu-id="83c93-126">示例中使用的是 string、integer 和这些类型的数组。</span><span class="sxs-lookup"><span data-stu-id="83c93-126">Shown in the examples are string, integer, and arrays of these types.</span></span>

<span data-ttu-id="83c93-127">由于扩展属性在大多数情况下与定义的 MAPI 属性（未在 Microsoft Graph API 元数据中公开）交互操作，为了简单起见，选定格式应反映相应 MAPI 属性在其 [MAPI 属性标识符]((https://msdn.microsoft.com/zh-CN/library/office/cc815528.aspx)) 中使用字符串还是数字值。</span><span class="sxs-lookup"><span data-stu-id="83c93-127">Since extended properties are in most cases inter-operating with defined MAPI properties not exposed in the Microsoft Graph API metadata, for simplicity, the format you choose should reflect whether the corresponding MAPI property uses a character string or numeric value in its [MAPI property identifier]((https://msdn.microsoft.com/zh-CN/library/office/cc815528.aspx)).</span></span>
<span data-ttu-id="83c93-128">在 \[MS-OXPROPS\] Microsoft Corporation 的[“Exchange Server 协议 Master 属性列表”](https://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx)中，可以了解如何将扩展属性映射到现有 MAPI 属性，如属性标识符和 GUID。</span><span class="sxs-lookup"><span data-stu-id="83c93-128">You can find information about mapping an extended property to an existing MAPI property, such as the property identifier and GUID, in \[MS-OXPROPS\] Microsoft Corporation, ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/en-us/library/cc433490%28v=exchg.80%29.aspx).</span></span>

<span data-ttu-id="83c93-129">**注意**：为 **id** 选择一种格式后，只能按此格式访问扩展属性。</span><span class="sxs-lookup"><span data-stu-id="83c93-129">**Note** After you have chosen one format for the **id**, you should access that extended property by only that format.</span></span>


<span data-ttu-id="83c93-130">**单值扩展属性的有效 id 格式**</span><span class="sxs-lookup"><span data-stu-id="83c93-130">**Valid id formats for single-value extended properties**</span></span>

|<span data-ttu-id="83c93-131">**格式**</span><span class="sxs-lookup"><span data-stu-id="83c93-131">**Format**</span></span>|<span data-ttu-id="83c93-132">**示例**</span><span class="sxs-lookup"><span data-stu-id="83c93-132">**Example**</span></span>|<span data-ttu-id="83c93-133">**说明**</span><span class="sxs-lookup"><span data-stu-id="83c93-133">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="83c93-134">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="83c93-134">"{type} {guid} Name {name}"</span></span> | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="83c93-135">用所属的命名空间 (GUID) 和名称标识属性。</span><span class="sxs-lookup"><span data-stu-id="83c93-135">Identifies a property by the namespace (the GUID) it belongs to, and a name.</span></span>         |
| <span data-ttu-id="83c93-136">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="83c93-136">"{type} {guid} Id {id}"</span></span>     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | <span data-ttu-id="83c93-137">用所属的命名空间 (GUID) 和标识符标识属性。</span><span class="sxs-lookup"><span data-stu-id="83c93-137">Identifies a property by the namespace (the GUID) it belongs to, and an identifier.</span></span>  |

<span data-ttu-id="83c93-138">**多值扩展属性的有效 id 格式**</span><span class="sxs-lookup"><span data-stu-id="83c93-138">**Valid id formats for multi-value extended properties**</span></span>

|<span data-ttu-id="83c93-139">**格式**</span><span class="sxs-lookup"><span data-stu-id="83c93-139">**Format**</span></span>|<span data-ttu-id="83c93-140">**示例**</span><span class="sxs-lookup"><span data-stu-id="83c93-140">**Example**</span></span>|<span data-ttu-id="83c93-141">**说明**</span><span class="sxs-lookup"><span data-stu-id="83c93-141">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="83c93-142">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="83c93-142">"{type} {guid} Name {name}"</span></span> | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="83c93-143">用命名空间 (GUID) 和名称标识属性。</span><span class="sxs-lookup"><span data-stu-id="83c93-143">Identifies a property by namespace (the GUID) and name.</span></span>         |
| <span data-ttu-id="83c93-144">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="83c93-144">"{type} {guid} Id {id}"</span></span>     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | <span data-ttu-id="83c93-145">用命名空间 (GUID) 和标识符标识属性。</span><span class="sxs-lookup"><span data-stu-id="83c93-145">Identifies a property by namespace (the GUID) and identifier.</span></span>   |

### <a name="rest-api-operations"></a><span data-ttu-id="83c93-146">REST API 操作</span><span class="sxs-lookup"><span data-stu-id="83c93-146">REST API operations</span></span>
 
<span data-ttu-id="83c93-147">单值扩展属性的操作：</span><span class="sxs-lookup"><span data-stu-id="83c93-147">Single-value extended property operations:</span></span>

- [<span data-ttu-id="83c93-148">在新建或现有的资源实例中创建扩展属性</span><span class="sxs-lookup"><span data-stu-id="83c93-148">Create an extended property in a new or existing resource instance</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md)
- [<span data-ttu-id="83c93-149">使用 `$expand` 或 `$filter` 获取一个包含扩展属性的资源实例或资源实例集合</span><span class="sxs-lookup"><span data-stu-id="83c93-149">Get one or a collection of resource instances with an extended property using `$expand` or `$filter`</span></span>](../api/singlevaluelegacyextendedproperty_get.md)

<span data-ttu-id="83c93-150">多值扩展属性的操作：</span><span class="sxs-lookup"><span data-stu-id="83c93-150">Multi-value extended property operations:</span></span>

- [<span data-ttu-id="83c93-151">在新建或现有的资源实例中创建扩展属性</span><span class="sxs-lookup"><span data-stu-id="83c93-151">Create an extended property in a new or existing resource instance</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md)
- [<span data-ttu-id="83c93-152">使用 `$expand` 获取一个包含扩展属性的资源实例</span><span class="sxs-lookup"><span data-stu-id="83c93-152">Get a resource instance with an extended property using `$expand`</span></span>](../api/multivaluelegacyextendedproperty_get.md)

