---
title: Outlook 扩展属性概述
description: '扩展属性允许存储自定义数据，并专门用作应用程序访问的回退机制 '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: f534628c32fab68cfcc5816a775b30c6b48aaa23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531465"
---
# <a name="outlook-extended-properties-overview"></a><span data-ttu-id="3c76a-103">Outlook 扩展属性概述</span><span class="sxs-lookup"><span data-stu-id="3c76a-103">Outlook extended properties overview</span></span>

<span data-ttu-id="3c76a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c76a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3c76a-p101">扩展属性允许存储自定义数据，当 Outlook MAPI 属性_尚未在 Microsoft Graph API 元数据中公开_时，扩展属性专门用作应用访问这些属性的自定义数据的回退机制。可以使用扩展属性 REST API 在以下用户资源中存储或获取此类自定义数据：</span><span class="sxs-lookup"><span data-stu-id="3c76a-p101">Extended properties allow storing custom data and specifically serve as a fallback mechanism for apps to access custom data for Outlook MAPI properties when these properties are _not already exposed in the Microsoft Graph API metadata_. You can use extended properties REST API to store or get such custom data in the following user resources:</span></span>

- [<span data-ttu-id="3c76a-107">邮件</span><span class="sxs-lookup"><span data-stu-id="3c76a-107">message</span></span>](../resources/message.md)
- [<span data-ttu-id="3c76a-108">mailFolder</span><span class="sxs-lookup"><span data-stu-id="3c76a-108">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="3c76a-109">事件</span><span class="sxs-lookup"><span data-stu-id="3c76a-109">event</span></span>](../resources/event.md)
- [<span data-ttu-id="3c76a-110">日历</span><span class="sxs-lookup"><span data-stu-id="3c76a-110">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="3c76a-111">联系人</span><span class="sxs-lookup"><span data-stu-id="3c76a-111">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="3c76a-112">contactFolder</span><span class="sxs-lookup"><span data-stu-id="3c76a-112">contactFolder</span></span>](../resources/contactfolder.md)

<span data-ttu-id="3c76a-113">或者，在以下 Office 365 组资源中：</span><span class="sxs-lookup"><span data-stu-id="3c76a-113">Or, in the following Office 365 group resources:</span></span>

- <span data-ttu-id="3c76a-114">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="3c76a-114">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="3c76a-115">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="3c76a-115">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="3c76a-116">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="3c76a-116">group [post](../resources/post.md)</span></span>

## <a name="use-extended-properties-or-open-extensions"></a><span data-ttu-id="3c76a-117">使用扩展属性还是开放扩展？</span><span class="sxs-lookup"><span data-stu-id="3c76a-117">Use extended properties or open extensions?</span></span>

<span data-ttu-id="3c76a-p102">在大多数的常见情况下，你应该能够使用开放扩展（用 [openTypeExtension](../resources/opentypeextension.md) 表示，以前被称为 Office 365 数据扩展）来存储和访问用户邮箱中资源实例的自定义数据。仅当需要访问尚未通过 [Microsoft Graph API 元数据](https://developer.microsoft.com/graph/docs/overview/call_api)公开的 Outlook MAPI 属性的自定义数据时使用扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3c76a-p102">In most common scenarios, you should be able to use open extensions (represented by [openTypeExtension](../resources/opentypeextension.md), formerly known as Office 365 data extensions) to store and access custom data for resource instances in a user's mailbox. Use extended properties only if you need to access custom data for Outlook MAPI properties that are not already exposed in the [Microsoft Graph API metadata](https://developer.microsoft.com/graph/docs/overview/call_api).</span></span>

## <a name="types-of-extended-properties"></a><span data-ttu-id="3c76a-120">扩展属性的类型</span><span class="sxs-lookup"><span data-stu-id="3c76a-120">Types of extended properties</span></span>

<span data-ttu-id="3c76a-121">根据是否打算将单个值或多个值（相同类型）存储在一个扩展属性中，可以将扩展属性创建为 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 或 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)。</span><span class="sxs-lookup"><span data-stu-id="3c76a-121">Depending on whether you intend to store a single or multiple values (of the same type) in an extended property, you can create an extended property as a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md), or [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).</span></span>

<span data-ttu-id="3c76a-122">其中的每种类型都通过其 **id** 进行标识并将数据存储在 **value** 中。</span><span class="sxs-lookup"><span data-stu-id="3c76a-122">Each of these types identifies the property by its **id** and stores data in **value**.</span></span>

<span data-ttu-id="3c76a-123">可以使用 **id** 获取特定的资源实例以及该扩展属性，或筛选单值扩展属性以获取拥有该属性的所有实例。</span><span class="sxs-lookup"><span data-stu-id="3c76a-123">You can use **id** to get a specific resource instance together with that extended property, or filter on a single-value extended property to get all the instances that have that property.</span></span>

<span data-ttu-id="3c76a-124">**注意** 不能使用 REST API 在一个调用中获取特定实例的所有扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3c76a-124">**Note** You cannot use the REST API to get all the extended properties of a specific instance in one call.</span></span>


### <a name="id-formats"></a><span data-ttu-id="3c76a-125">id 格式</span><span class="sxs-lookup"><span data-stu-id="3c76a-125">id formats</span></span>

<span data-ttu-id="3c76a-126">可以使用以下三种格式之一指定扩展属性的 **id**：</span><span class="sxs-lookup"><span data-stu-id="3c76a-126">You can specify **id** of an extended property in one of three formats:</span></span>

- <span data-ttu-id="3c76a-127">作为命名属性，由扩展属性类型、名称空间和字符串名称标识。</span><span class="sxs-lookup"><span data-stu-id="3c76a-127">As a named property, identified by the extended property type, namespace, and a string name.</span></span>
- <span data-ttu-id="3c76a-128">作为命名属性，由扩展属性类型、名称空间和数字标识符标识。</span><span class="sxs-lookup"><span data-stu-id="3c76a-128">As a named property, identified by the extended property type, namespace, and a numeric identifier.</span></span>
- <span data-ttu-id="3c76a-129">采用属性标记格式，由扩展属性类型和 [MAPI 属性标记](/office/client-developer/outlook/mapi/mapi-property-tags)标识。</span><span class="sxs-lookup"><span data-stu-id="3c76a-129">In a proptag format, identified by the extended property type and a [MAPI property tag](/office/client-developer/outlook/mapi/mapi-property-tags).</span></span>

<span data-ttu-id="3c76a-130">接下来的两个表描述了应用于单值和多值扩展属性的这些格式。</span><span class="sxs-lookup"><span data-stu-id="3c76a-130">The next 2 tables describe these formats as applied to single and multi-value extended properties.</span></span> <span data-ttu-id="3c76a-131">{_type_} 表示一个或多个扩展属性值的类型。</span><span class="sxs-lookup"><span data-stu-id="3c76a-131">{_type_} represents the type of the value or values of the extended property.</span></span> <span data-ttu-id="3c76a-132">示例中使用的是 string、integer 和这些类型的数组。</span><span class="sxs-lookup"><span data-stu-id="3c76a-132">Shown in the examples are string, integer, and arrays of these types.</span></span>

<span data-ttu-id="3c76a-133">**单值扩展属性的有效 id 格式**</span><span class="sxs-lookup"><span data-stu-id="3c76a-133">**Valid id formats for single-value extended properties**</span></span>

|<span data-ttu-id="3c76a-134">**格式**</span><span class="sxs-lookup"><span data-stu-id="3c76a-134">**Format**</span></span>|<span data-ttu-id="3c76a-135">**示例**</span><span class="sxs-lookup"><span data-stu-id="3c76a-135">**Example**</span></span>|<span data-ttu-id="3c76a-136">**说明**</span><span class="sxs-lookup"><span data-stu-id="3c76a-136">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="3c76a-137">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="3c76a-137">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="3c76a-138">用所属的命名空间 (GUID) 和字符串名称标识属性。</span><span class="sxs-lookup"><span data-stu-id="3c76a-138">Identifies a property by the namespace (the GUID) it belongs to, and a string name.</span></span>         |
| <span data-ttu-id="3c76a-139">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="3c76a-139">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | <span data-ttu-id="3c76a-140">用所属的命名空间 (GUID) 和数字标识符标识属性。</span><span class="sxs-lookup"><span data-stu-id="3c76a-140">Identifies a property by the namespace (the GUID) it belongs to, and a numeric identifier.</span></span>  |
| <span data-ttu-id="3c76a-141">"{_type_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="3c76a-141">"{_type_} {_proptag_}"</span></span>                    | ```"String 0x4001001E"```                                           | <span data-ttu-id="3c76a-142">用属性标记标识预定义的属性。</span><span class="sxs-lookup"><span data-stu-id="3c76a-142">Identifies a pre-defined property by its property tag.</span></span> |

<span data-ttu-id="3c76a-143">**多值扩展属性的有效 id 格式**</span><span class="sxs-lookup"><span data-stu-id="3c76a-143">**Valid id formats for multi-value extended properties**</span></span>

|<span data-ttu-id="3c76a-144">**格式**</span><span class="sxs-lookup"><span data-stu-id="3c76a-144">**Format**</span></span>|<span data-ttu-id="3c76a-145">**示例**</span><span class="sxs-lookup"><span data-stu-id="3c76a-145">**Example**</span></span>|<span data-ttu-id="3c76a-146">**说明**</span><span class="sxs-lookup"><span data-stu-id="3c76a-146">**Description**</span></span>|
|:---------|:----------|:--------------|
| <span data-ttu-id="3c76a-147">"{_type_} {_guid_} **Name** {_name_}"</span><span class="sxs-lookup"><span data-stu-id="3c76a-147">"{_type_} {_guid_} **Name** {_name_}"</span></span> | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | <span data-ttu-id="3c76a-148">用命名空间 (GUID) 和字符串名称标识属性。</span><span class="sxs-lookup"><span data-stu-id="3c76a-148">Identifies a property by the namespace (the GUID) and a string name.</span></span>         |
| <span data-ttu-id="3c76a-149">"{_type_} {_guid_} **Id** {_id_}"</span><span class="sxs-lookup"><span data-stu-id="3c76a-149">"{_type_} {_guid_} **Id** {_id_}"</span></span>     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | <span data-ttu-id="3c76a-150">用命名空间 (GUID) 和数字标识符标识属性。</span><span class="sxs-lookup"><span data-stu-id="3c76a-150">Identifies a property by the namespace (the GUID) and a numeric identifier.</span></span>   |
| <span data-ttu-id="3c76a-151">"{_type_} {_proptag_}"</span><span class="sxs-lookup"><span data-stu-id="3c76a-151">"{_type_} {_proptag_}"</span></span>                    | ```"StringArray 0x4002101E"```                                           | <span data-ttu-id="3c76a-152">用属性标记标识预定义的属性。</span><span class="sxs-lookup"><span data-stu-id="3c76a-152">Identifies a pre-defined property by its property tag.</span></span> |


<span data-ttu-id="3c76a-153">使用任一命名属性格式将单值或多值扩展属性定义为自定义属性。</span><span class="sxs-lookup"><span data-stu-id="3c76a-153">Use either of the named property formats to define a single-value or multi-value extended property as a custom property.</span></span> <span data-ttu-id="3c76a-154">在这两种格式中，第一种采用字符串名称 (**Name**) 的格式是易于参考的首选格式。</span><span class="sxs-lookup"><span data-stu-id="3c76a-154">Among the two formats, the first one that takes a string name (**Name**) is the preferred format for ease of reference.</span></span> <span data-ttu-id="3c76a-155">命名属性的[属性标识符](/office/client-developer/outlook/mapi/mapi-property-identifier-overview)在 0x8000-0xfffe 范围内。</span><span class="sxs-lookup"><span data-stu-id="3c76a-155">Named properties have their [property identifiers](/office/client-developer/outlook/mapi/mapi-property-identifier-overview) in the 0x8000-0xfffe range.</span></span>

<span data-ttu-id="3c76a-156">使用属性标记格式访问由 MAPI 或客户端或服务器预定义的属性，以及尚未在 Microsoft Graph 中公开的属性。</span><span class="sxs-lookup"><span data-stu-id="3c76a-156">Use the proptag format to access properties predefined by MAPI, or by a client or server, and that have not already been exposed in Microsoft Graph.</span></span> <span data-ttu-id="3c76a-157">这些属性的属性标识符在 0x0001-0x7fff 范围内。</span><span class="sxs-lookup"><span data-stu-id="3c76a-157">These properties have property identifiers in the 0x0001-0x7fff range.</span></span> <span data-ttu-id="3c76a-158">不要尝试使用属性标记格式定义自定义属性。</span><span class="sxs-lookup"><span data-stu-id="3c76a-158">Do not try to define a custom property using the proptag format.</span></span>

<span data-ttu-id="3c76a-159">在 \[MS-OXPROPS\] Microsoft Corporation 的[“Exchange Server 协议 Master 属性列表”](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx)中，可以了解如何将扩展属性映射到现有 MAPI 属性，如属性标识符和 GUID。</span><span class="sxs-lookup"><span data-stu-id="3c76a-159">You can find information about mapping an extended property to an existing MAPI property, such as the property identifier and GUID, in \[MS-OXPROPS\] Microsoft Corporation, ["Exchange Server Protocols Master Property List"](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx).</span></span>

<span data-ttu-id="3c76a-160">**注意**：为 **id** 选择一种格式后，只能按此格式访问扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3c76a-160">**Note** After you have chosen one format for the **id**, you should access that extended property by only that format.</span></span>

### <a name="rest-api-operations"></a><span data-ttu-id="3c76a-161">REST API 操作</span><span class="sxs-lookup"><span data-stu-id="3c76a-161">REST API operations</span></span>

<span data-ttu-id="3c76a-162">单值扩展属性的操作：</span><span class="sxs-lookup"><span data-stu-id="3c76a-162">Single-value extended property operations:</span></span>

- [<span data-ttu-id="3c76a-163">在新建或现有的资源实例中创建扩展属性</span><span class="sxs-lookup"><span data-stu-id="3c76a-163">Create an extended property in a new or existing resource instance</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [<span data-ttu-id="3c76a-164">使用 `$expand` 或 `$filter` 获取一个包含扩展属性的资源实例或资源实例集合</span><span class="sxs-lookup"><span data-stu-id="3c76a-164">Get one or a collection of resource instances with an extended property using `$expand` or `$filter`</span></span>](../api/singlevaluelegacyextendedproperty-get.md)

<span data-ttu-id="3c76a-165">多值扩展属性的操作：</span><span class="sxs-lookup"><span data-stu-id="3c76a-165">Multi-value extended property operations:</span></span>

- [<span data-ttu-id="3c76a-166">在新建或现有的资源实例中创建扩展属性</span><span class="sxs-lookup"><span data-stu-id="3c76a-166">Create an extended property in a new or existing resource instance</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [<span data-ttu-id="3c76a-167">使用 `$expand` 获取一个包含扩展属性的资源实例</span><span class="sxs-lookup"><span data-stu-id="3c76a-167">Get a resource instance with an extended property using `$expand`</span></span>](../api/multivaluelegacyextendedproperty-get.md)

