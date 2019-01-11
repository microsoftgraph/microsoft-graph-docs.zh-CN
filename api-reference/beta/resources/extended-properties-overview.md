---
title: Outlook 扩展属性概述
description: '扩展的属性允许存储自定义数据和专门用作应用程序访问的回退机制 '
localization_priority: Normal
ms.openlocfilehash: e78b70dc4978cbee05215cffd7a2af1205ba5c69
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846198"
---
# <a name="outlook-extended-properties-overview"></a><span data-ttu-id="723cb-103">Outlook 扩展属性概述</span><span class="sxs-lookup"><span data-stu-id="723cb-103">Outlook extended properties overview</span></span>

> <span data-ttu-id="723cb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="723cb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="723cb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="723cb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="723cb-p102">扩展属性允许存储自定义数据，当 Outlook MAPI 属性_尚未在 Microsoft Graph API 元数据中公开_时，扩展属性专门用作应用访问这些属性的自定义数据的回退机制。可以使用扩展属性 REST API 在以下用户资源中存储或获取此类自定义数据：</span><span class="sxs-lookup"><span data-stu-id="723cb-p102">Extended properties allow storing custom data and specifically serve as a fallback mechanism for apps to access custom data for Outlook MAPI properties when these properties are _not already exposed in the Microsoft Graph API metadata_. You can use extended properties REST API to store or get such custom data in the following user resources:</span></span>

- [<span data-ttu-id="723cb-108">邮件</span><span class="sxs-lookup"><span data-stu-id="723cb-108">message</span></span>](../resources/message.md)
- [<span data-ttu-id="723cb-109">mailFolder</span><span class="sxs-lookup"><span data-stu-id="723cb-109">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="723cb-110">事件</span><span class="sxs-lookup"><span data-stu-id="723cb-110">event</span></span>](../resources/event.md)
- [<span data-ttu-id="723cb-111">日历</span><span class="sxs-lookup"><span data-stu-id="723cb-111">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="723cb-112">联系人</span><span class="sxs-lookup"><span data-stu-id="723cb-112">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="723cb-113">contactFolder</span><span class="sxs-lookup"><span data-stu-id="723cb-113">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="723cb-114">Outlook 任务</span><span class="sxs-lookup"><span data-stu-id="723cb-114">Outlook task</span></span>](../resources/outlooktask.md)
- [<span data-ttu-id="723cb-115">Outlook 任务文件夹</span><span class="sxs-lookup"><span data-stu-id="723cb-115">Outlook task folder</span></span>](../resources/outlooktaskfolder.md) 

<span data-ttu-id="723cb-116">或者，在以下 Office 365 组资源中：</span><span class="sxs-lookup"><span data-stu-id="723cb-116">Or, in the following Office 365 group resources:</span></span>

- <span data-ttu-id="723cb-117">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="723cb-117">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="723cb-118">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="723cb-118">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="723cb-119">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="723cb-119">group [post](../resources/post.md)</span></span> 

## <a name="use-extended-properties-or-open-extensions"></a><span data-ttu-id="723cb-120">使用扩展属性还是开放扩展？</span><span class="sxs-lookup"><span data-stu-id="723cb-120">Use extended properties or open extensions?</span></span>

<span data-ttu-id="723cb-p103">在大多数的常见情况下，你应该能够使用开放扩展（用 [openTypeExtension](../resources/opentypeextension.md) 表示，以前被称为 Office 365 数据扩展）来存储和访问用户邮箱中资源实例的自定义数据。仅当需要访问尚未通过 [Microsoft Graph API 元数据](https://developer.microsoft.com/graph/docs/overview/call_api)公开的 Outlook MAPI 属性的自定义数据时使用扩展属性。</span><span class="sxs-lookup"><span data-stu-id="723cb-p103">In most common scenarios, you should be able to use open extensions (represented by [openTypeExtension](../resources/opentypeextension.md), formerly known as Office 365 data extensions) to store and access custom data for resource instances in a user's mailbox. Use extended properties only if you need to access custom data for Outlook MAPI properties that are not already exposed in the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api).</span></span>

## <a name="types-of-extended-properties"></a><span data-ttu-id="723cb-123">扩展属性的类型</span><span class="sxs-lookup"><span data-stu-id="723cb-123">Types of extended properties</span></span>

<span data-ttu-id="723cb-124">根据是否打算将单个值或多个值（相同类型）存储在一个扩展属性中，可以将扩展属性创建为 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 或 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)。</span><span class="sxs-lookup"><span data-stu-id="723cb-124">Depending on whether you intend to store a single or multiple values (of the same type) in an extended property, you can create an extended property as a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), or [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span></span>

<span data-ttu-id="723cb-125">其中的每种类型都通过其 **id** 进行标识并将数据存储在 **value** 中。</span><span class="sxs-lookup"><span data-stu-id="723cb-125">Each of these types identifies the property by its **id** and stores data in **value**.</span></span> 

<span data-ttu-id="723cb-126">可以使用 **id** 获取特定的资源实例以及该扩展属性，或筛选单值扩展属性以获取拥有该属性的所有实例。</span><span class="sxs-lookup"><span data-stu-id="723cb-126">You can use **id** to get a specific resource instance together with that extended property, or filter on a single-value extended property to get all the instances that have that property.</span></span> 

<span data-ttu-id="723cb-127">**注意** 不能使用 REST API 在一个调用中获取特定实例的所有扩展属性。</span><span class="sxs-lookup"><span data-stu-id="723cb-127">**Note** You cannot use the REST API to get all the extended properties of a specific instance in one call.</span></span>
  

### <a name="id-formats"></a><span data-ttu-id="723cb-128">id 格式</span><span class="sxs-lookup"><span data-stu-id="723cb-128">id formats</span></span>

<span data-ttu-id="723cb-129">您可以在三种格式之一指定的扩展属性的**id** :</span><span class="sxs-lookup"><span data-stu-id="723cb-129">You can specify **id** of an extended property in one of three formats:</span></span>

- <span data-ttu-id="723cb-130">为扩展的属性类型、 命名空间和字符串名称由标识的命名属性。</span><span class="sxs-lookup"><span data-stu-id="723cb-130">As a named property, identified by the extended property type, namespace, and a string name.</span></span>
- <span data-ttu-id="723cb-131">为扩展的属性类型、 命名空间和一个数字标识符标识的命名属性。</span><span class="sxs-lookup"><span data-stu-id="723cb-131">As a named property, identified by the extended property type, namespace, and a numeric identifier.</span></span>
- <span data-ttu-id="723cb-132">在由扩展的属性类型和[MAPI 属性标记](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags)标识属性标记格式。</span><span class="sxs-lookup"><span data-stu-id="723cb-132">In a proptag format, identified by the extended property type and a [MAPI property tag](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags).</span></span>

<span data-ttu-id="723cb-133">接下来的两个表介绍这些格式为单角色和多值应用于的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="723cb-133">The next 2 tables describe these formats as applied to single and multi-value extended properties.</span></span> <span data-ttu-id="723cb-134">{_类型_} 表示的扩展属性的值的类型。</span><span class="sxs-lookup"><span data-stu-id="723cb-134">{_type_} represents the type of the value or values of the extended property.</span></span> <span data-ttu-id="723cb-135">示例中使用的是 string、integer 和这些类型的数组。</span><span class="sxs-lookup"><span data-stu-id="723cb-135">Shown in the examples are string, integer, and arrays of these types.</span></span>

<span data-ttu-id="723cb-136">**单值扩展属性的有效 id 格式**</span><span class="sxs-lookup"><span data-stu-id="723cb-136">**Valid id formats for single-value extended properties**</span></span>

|<span data-ttu-id="723cb-137">**格式**</span><span class="sxs-lookup"><span data-stu-id="723cb-137">**Format**</span></span>|<span data-ttu-id="723cb-138">**示例**</span><span class="sxs-lookup"><span data-stu-id="723cb-138">**Example**</span></span>|<span data-ttu-id="723cb-139">**说明**</span><span class="sxs-lookup"><span data-stu-id="723cb-139">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="723cb-140">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="723cb-140">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="723cb-141">标识属性由其所属的命名空间 (GUID) 和字符串名称。</span><span class="sxs-lookup"><span data-stu-id="723cb-141">Identifies a property by the namespace (the GUID) it belongs to, and a string name.</span></span>         |
| <span data-ttu-id="723cb-142">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="723cb-142">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | <span data-ttu-id="723cb-143">标识通过其所属的命名空间 (GUID) 和一个数字标识符的属性。</span><span class="sxs-lookup"><span data-stu-id="723cb-143">Identifies a property by the namespace (the GUID) it belongs to, and a numeric identifier.</span></span>  |
| <span data-ttu-id="723cb-144">"{_类型_} {_属性标记_}"</span><span class="sxs-lookup"><span data-stu-id="723cb-144">"{_type_} {_proptag_}"</span></span>                    | ```"String 0x4001001E"```                                           | <span data-ttu-id="723cb-145">根据属性标记标识的预定义的属性。</span><span class="sxs-lookup"><span data-stu-id="723cb-145">Identifies a pre-defined property by its property tag.</span></span> |

<span data-ttu-id="723cb-146">**多值扩展属性的有效 id 格式**</span><span class="sxs-lookup"><span data-stu-id="723cb-146">**Valid id formats for multi-value extended properties**</span></span>

|<span data-ttu-id="723cb-147">**格式**</span><span class="sxs-lookup"><span data-stu-id="723cb-147">**Format**</span></span>|<span data-ttu-id="723cb-148">**示例**</span><span class="sxs-lookup"><span data-stu-id="723cb-148">**Example**</span></span>|<span data-ttu-id="723cb-149">**说明**</span><span class="sxs-lookup"><span data-stu-id="723cb-149">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="723cb-150">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="723cb-150">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="723cb-151">标识属性的命名空间 (GUID) 和字符串名称。</span><span class="sxs-lookup"><span data-stu-id="723cb-151">Identifies a property by the namespace (the GUID) and a string name.</span></span>         |
| <span data-ttu-id="723cb-152">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="723cb-152">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | <span data-ttu-id="723cb-153">标识属性的命名空间 (GUID) 和数字的标识符。</span><span class="sxs-lookup"><span data-stu-id="723cb-153">Identifies a property by the namespace (the GUID) and a numeric identifier.</span></span>   |
| <span data-ttu-id="723cb-154">"{_类型_} {_属性标记_}"</span><span class="sxs-lookup"><span data-stu-id="723cb-154">"{_type_} {_proptag_}"</span></span>                    | ```"StringArray 0x4002101E"```                                           | <span data-ttu-id="723cb-155">根据属性标记标识的预定义的属性。</span><span class="sxs-lookup"><span data-stu-id="723cb-155">Identifies a pre-defined property by its property tag.</span></span> |


<span data-ttu-id="723cb-156">使用的命名的属性的格式之一以定义一个或多值单值的扩展的属性为自定义属性。</span><span class="sxs-lookup"><span data-stu-id="723cb-156">Use either of the named property formats to define a single-value or multi-value extended property as a custom property.</span></span> <span data-ttu-id="723cb-157">之间的两个格式，第一个采用字符串名称 （**Name**） 是为了便于引用的首选的格式。</span><span class="sxs-lookup"><span data-stu-id="723cb-157">Among the two formats, the first one that takes a string name (**Name**) is the preferred format for ease of reference.</span></span> <span data-ttu-id="723cb-158">命名的属性中 0x8000 0xfffe 有及其[属性标识符](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview)范围。</span><span class="sxs-lookup"><span data-stu-id="723cb-158">Named properties have their [property identifiers](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in the 0x8000-0xfffe range.</span></span>

<span data-ttu-id="723cb-159">使用属性标记格式访问通过 MAPI，或客户端或服务器，预定义的属性和的具有不已经暴露在 Microsoft Graph 中。</span><span class="sxs-lookup"><span data-stu-id="723cb-159">Use the proptag format to access properties predefined by MAPI, or by a client or server, and that have not already been exposed in Microsoft Graph.</span></span> <span data-ttu-id="723cb-160">这些属性中 0x0001 0x7fff 有属性标识符范围。</span><span class="sxs-lookup"><span data-stu-id="723cb-160">These properties have property identifiers in the 0x0001-0x7fff range.</span></span> <span data-ttu-id="723cb-161">不要尝试定义使用属性标记格式的自定义属性。</span><span class="sxs-lookup"><span data-stu-id="723cb-161">Do not try to define a custom property using the proptag format.</span></span> 

<span data-ttu-id="723cb-162">在 \[MS-OXPROPS\] Microsoft Corporation 的[“Exchange Server 协议 Master 属性列表”](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx)中，可以了解如何将扩展属性映射到现有 MAPI 属性，如属性标识符和 GUID。</span><span class="sxs-lookup"><span data-stu-id="723cb-162">You can find information about mapping an extended property to an existing MAPI property, such as the property identifier and GUID, in \[MS-OXPROPS\] Microsoft Corporation, ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span></span>

<span data-ttu-id="723cb-163">**注意**：为 **id** 选择一种格式后，只能按此格式访问扩展属性。</span><span class="sxs-lookup"><span data-stu-id="723cb-163">**Note** After you have chosen one format for the **id**, you should access that extended property by only that format.</span></span>

## <a name="rest-api-operations"></a><span data-ttu-id="723cb-164">REST API 操作</span><span class="sxs-lookup"><span data-stu-id="723cb-164">REST API operations</span></span>
 
<span data-ttu-id="723cb-165">单值扩展属性的操作：</span><span class="sxs-lookup"><span data-stu-id="723cb-165">Single-value extended property operations:</span></span>

- [<span data-ttu-id="723cb-166">在新建或现有的资源实例中创建扩展属性</span><span class="sxs-lookup"><span data-stu-id="723cb-166">Create an extended property in a new or existing resource instance</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [<span data-ttu-id="723cb-167">使用 `$expand` 或 `$filter` 获取一个包含扩展属性的资源实例或资源实例集合</span><span class="sxs-lookup"><span data-stu-id="723cb-167">Get one or a collection of resource instances with an extended property using `$expand` or `$filter`</span></span>](../api/singlevaluelegacyextendedproperty-get.md)

<span data-ttu-id="723cb-168">多值扩展属性的操作：</span><span class="sxs-lookup"><span data-stu-id="723cb-168">Multi-value extended property operations:</span></span>

- [<span data-ttu-id="723cb-169">在新建或现有的资源实例中创建扩展属性</span><span class="sxs-lookup"><span data-stu-id="723cb-169">Create an extended property in a new or existing resource instance</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [<span data-ttu-id="723cb-170">使用 `$expand` 获取一个包含扩展属性的资源实例</span><span class="sxs-lookup"><span data-stu-id="723cb-170">Get a resource instance with an extended property using `$expand`</span></span>](../api/multivaluelegacyextendedproperty-get.md)

