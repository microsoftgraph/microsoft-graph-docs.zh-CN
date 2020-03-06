---
title: 获取 multiValueLegacyExtendedProperty
description: 展开 "。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 6a2642a0c93218020dfb001eca2578a1946453c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511437"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="72e28-103">获取 multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="72e28-103">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="72e28-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72e28-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72e28-105">使用 `$expand` 获取包含多值扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="72e28-105">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="72e28-106">使用查询参数 `$expand`，可以获取使用指明的扩展属性扩展的指定实例。</span><span class="sxs-lookup"><span data-stu-id="72e28-106">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="72e28-107">这是当前获取 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 对象（表示扩展属性）的唯一方式。</span><span class="sxs-lookup"><span data-stu-id="72e28-107">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="72e28-108">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="72e28-108">The following user resources are supported:</span></span>

- [<span data-ttu-id="72e28-109">日历</span><span class="sxs-lookup"><span data-stu-id="72e28-109">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="72e28-110">联系人</span><span class="sxs-lookup"><span data-stu-id="72e28-110">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="72e28-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="72e28-111">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="72e28-112">事件</span><span class="sxs-lookup"><span data-stu-id="72e28-112">event</span></span>](../resources/event.md)
- [<span data-ttu-id="72e28-113">mailFolder</span><span class="sxs-lookup"><span data-stu-id="72e28-113">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="72e28-114">邮件</span><span class="sxs-lookup"><span data-stu-id="72e28-114">message</span></span>](../resources/message.md) 

<span data-ttu-id="72e28-115">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="72e28-115">As well as the following group resources:</span></span>

- <span data-ttu-id="72e28-116">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="72e28-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="72e28-117">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="72e28-117">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="72e28-118">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="72e28-118">group [post](../resources/post.md)</span></span>

<span data-ttu-id="72e28-119">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="72e28-119">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="72e28-120">权限</span><span class="sxs-lookup"><span data-stu-id="72e28-120">Permissions</span></span>
<span data-ttu-id="72e28-121">根据您要获取的扩展属性的资源以及所请求的权限类型（委派或应用程序），必须至少调用下表中指定的权限，才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="72e28-121">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="72e28-122">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72e28-122">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72e28-123">支持的资源</span><span class="sxs-lookup"><span data-stu-id="72e28-123">Supported resource</span></span> | <span data-ttu-id="72e28-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72e28-124">Delegated (work or school account)</span></span> | <span data-ttu-id="72e28-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72e28-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72e28-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="72e28-126">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="72e28-127">日历</span><span class="sxs-lookup"><span data-stu-id="72e28-127">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="72e28-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-128">Calendars.Read</span></span> | <span data-ttu-id="72e28-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-129">Calendars.Read</span></span> | <span data-ttu-id="72e28-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-130">Calendars.Read</span></span> |
| [<span data-ttu-id="72e28-131">联系人</span><span class="sxs-lookup"><span data-stu-id="72e28-131">contact</span></span>](../resources/contact.md) | <span data-ttu-id="72e28-132">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-132">Contacts.Read</span></span> | <span data-ttu-id="72e28-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-133">Contacts.Read</span></span> | <span data-ttu-id="72e28-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-134">Contacts.Read</span></span> |
| [<span data-ttu-id="72e28-135">contactFolder</span><span class="sxs-lookup"><span data-stu-id="72e28-135">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="72e28-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-136">Contacts.Read</span></span> | <span data-ttu-id="72e28-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-137">Contacts.Read</span></span> | <span data-ttu-id="72e28-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-138">Contacts.Read</span></span> |
| [<span data-ttu-id="72e28-139">事件</span><span class="sxs-lookup"><span data-stu-id="72e28-139">event</span></span>](../resources/event.md) | <span data-ttu-id="72e28-140">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-140">Calendars.Read</span></span> | <span data-ttu-id="72e28-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-141">Calendars.Read</span></span> |  <span data-ttu-id="72e28-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-142">Calendars.Read</span></span>|
| <span data-ttu-id="72e28-143">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="72e28-143">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="72e28-144">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="72e28-144">Group.Read.All</span></span> | <span data-ttu-id="72e28-145">不支持</span><span class="sxs-lookup"><span data-stu-id="72e28-145">Not supported</span></span> | <span data-ttu-id="72e28-146">不支持</span><span class="sxs-lookup"><span data-stu-id="72e28-146">Not supported</span></span> |
| <span data-ttu-id="72e28-147">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="72e28-147">group [event](../resources/event.md)</span></span> | <span data-ttu-id="72e28-148">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="72e28-148">Group.Read.All</span></span> | <span data-ttu-id="72e28-149">不支持</span><span class="sxs-lookup"><span data-stu-id="72e28-149">Not supported</span></span> | <span data-ttu-id="72e28-150">不支持</span><span class="sxs-lookup"><span data-stu-id="72e28-150">Not supported</span></span> |
| <span data-ttu-id="72e28-151">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="72e28-151">group [post](../resources/post.md)</span></span> | <span data-ttu-id="72e28-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="72e28-152">Group.Read.All</span></span> | <span data-ttu-id="72e28-153">不支持</span><span class="sxs-lookup"><span data-stu-id="72e28-153">Not supported</span></span> | <span data-ttu-id="72e28-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="72e28-154">Group.Read.All</span></span> |
| [<span data-ttu-id="72e28-155">mailFolder</span><span class="sxs-lookup"><span data-stu-id="72e28-155">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="72e28-156">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-156">Mail.Read</span></span> | <span data-ttu-id="72e28-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-157">Mail.Read</span></span> | <span data-ttu-id="72e28-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-158">Mail.Read</span></span> |
| [<span data-ttu-id="72e28-159">邮件</span><span class="sxs-lookup"><span data-stu-id="72e28-159">message</span></span>](../resources/message.md) | <span data-ttu-id="72e28-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-160">Mail.Read</span></span> | <span data-ttu-id="72e28-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-161">Mail.Read</span></span> | <span data-ttu-id="72e28-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="72e28-162">Mail.Read</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="72e28-163">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72e28-163">HTTP request</span></span>

<span data-ttu-id="72e28-p103">获取通过与 **id** 属性中的筛选器匹配的扩展属性扩展的资源实例。请确保对筛选器字符串中的空白字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)。</span><span class="sxs-lookup"><span data-stu-id="72e28-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="72e28-166">获取**邮件**实例：</span><span class="sxs-lookup"><span data-stu-id="72e28-166">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="72e28-167">获取 **mailFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="72e28-167">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="72e28-168">获取**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="72e28-168">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="72e28-169">获取**日历**实例：</span><span class="sxs-lookup"><span data-stu-id="72e28-169">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="72e28-170">获取**联系人**实例：</span><span class="sxs-lookup"><span data-stu-id="72e28-170">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="72e28-171">获取 **contactFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="72e28-171">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="72e28-172">获取组**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="72e28-172">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="72e28-173">获取组 **post** 实例：</span><span class="sxs-lookup"><span data-stu-id="72e28-173">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="72e28-174">路径参数</span><span class="sxs-lookup"><span data-stu-id="72e28-174">Path parameters</span></span>
|<span data-ttu-id="72e28-175">参数</span><span class="sxs-lookup"><span data-stu-id="72e28-175">Parameter</span></span>|<span data-ttu-id="72e28-176">类型</span><span class="sxs-lookup"><span data-stu-id="72e28-176">Type</span></span>|<span data-ttu-id="72e28-177">说明</span><span class="sxs-lookup"><span data-stu-id="72e28-177">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="72e28-178">id_value</span><span class="sxs-lookup"><span data-stu-id="72e28-178">id_value</span></span>|<span data-ttu-id="72e28-179">String</span><span class="sxs-lookup"><span data-stu-id="72e28-179">String</span></span>|<span data-ttu-id="72e28-p104">要匹配的扩展属性的 ID。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="72e28-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="72e28-184">请求头</span><span class="sxs-lookup"><span data-stu-id="72e28-184">Request headers</span></span>
| <span data-ttu-id="72e28-185">名称</span><span class="sxs-lookup"><span data-stu-id="72e28-185">Name</span></span>      |<span data-ttu-id="72e28-186">说明</span><span class="sxs-lookup"><span data-stu-id="72e28-186">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72e28-187">Authorization</span><span class="sxs-lookup"><span data-stu-id="72e28-187">Authorization</span></span>  | <span data-ttu-id="72e28-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="72e28-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72e28-190">请求正文</span><span class="sxs-lookup"><span data-stu-id="72e28-190">Request body</span></span>
<span data-ttu-id="72e28-191">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="72e28-191">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72e28-192">响应</span><span class="sxs-lookup"><span data-stu-id="72e28-192">Response</span></span>

<span data-ttu-id="72e28-193">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="72e28-193">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="72e28-194">响应正文包括通过匹配的 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 对象扩展的对象，此对象表示请求的资源实例。</span><span class="sxs-lookup"><span data-stu-id="72e28-194">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="72e28-195">示例</span><span class="sxs-lookup"><span data-stu-id="72e28-195">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72e28-196">请求</span><span class="sxs-lookup"><span data-stu-id="72e28-196">Request</span></span>
<span data-ttu-id="72e28-p106">此示例通过包含一个多值扩展属性获取并扩展指定的事件。此筛选器返回其 **id** 与字符串 `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation`（包含 URL 编码，此处为了便于阅读，已将其删除）匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="72e28-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="72e28-199">响应</span><span class="sxs-lookup"><span data-stu-id="72e28-199">Response</span></span>

<span data-ttu-id="72e28-200">响应正文包括指定事件的所有属性以及此筛选器返回的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="72e28-200">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="72e28-p107">注意：为了简单起见，会将此处所示的 **event** 对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="72e28-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
    "@odata.etag": "W/\"mODEKWhc/Um6lA3uPm7PPAAAm8k15A==\"",
    "id": "AAMkAGE1M2_bs88AACbuFiiAAA=",
    "start": {
        "dateTime": "2015-11-26T17:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2015-11-30T05:00:00.0000000",
        "timeZone": "UTC"
    },
    "organizer": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
    "multiValueExtendedProperties": [
        {
            "id": "StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
            "value": [
                "Food",
                "Hiking",
                "Swimming"
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
