---
title: 获取 multiValueLegacyExtendedProperty
description: 展开 "。
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 8b014ea576f08b19f10d8943350dfc25983cf1d5
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812377"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="fca8b-103">获取 multiValueLegacyExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="fca8b-103">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="fca8b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fca8b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fca8b-105">使用 `$expand` 获取包含多值扩展属性的资源实例。</span><span class="sxs-lookup"><span data-stu-id="fca8b-105">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="fca8b-106">使用查询参数 `$expand`，可以获取使用指明的扩展属性扩展的指定实例。</span><span class="sxs-lookup"><span data-stu-id="fca8b-106">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="fca8b-107">这是当前获取 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 对象（表示扩展属性）的唯一方式。</span><span class="sxs-lookup"><span data-stu-id="fca8b-107">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="fca8b-108">支持以下用户资源：</span><span class="sxs-lookup"><span data-stu-id="fca8b-108">The following user resources are supported:</span></span>

- [<span data-ttu-id="fca8b-109">日历</span><span class="sxs-lookup"><span data-stu-id="fca8b-109">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="fca8b-110">联系人</span><span class="sxs-lookup"><span data-stu-id="fca8b-110">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="fca8b-111">contactFolder</span><span class="sxs-lookup"><span data-stu-id="fca8b-111">contactFolder</span></span>](../resources/contactfolder.md)
- [<span data-ttu-id="fca8b-112">事件</span><span class="sxs-lookup"><span data-stu-id="fca8b-112">event</span></span>](../resources/event.md)
- [<span data-ttu-id="fca8b-113">mailFolder</span><span class="sxs-lookup"><span data-stu-id="fca8b-113">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="fca8b-114">邮件</span><span class="sxs-lookup"><span data-stu-id="fca8b-114">message</span></span>](../resources/message.md)

<span data-ttu-id="fca8b-115">以及以下组资源：</span><span class="sxs-lookup"><span data-stu-id="fca8b-115">As well as the following group resources:</span></span>

- <span data-ttu-id="fca8b-116">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="fca8b-116">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="fca8b-117">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="fca8b-117">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="fca8b-118">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="fca8b-118">group [post](../resources/post.md)</span></span>

<span data-ttu-id="fca8b-119">有关何时使用开放扩展或扩展属性，以及如何指定扩展属性的详细信息，请参阅[扩展属性概述](../resources/extended-properties-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="fca8b-119">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="fca8b-120">权限</span><span class="sxs-lookup"><span data-stu-id="fca8b-120">Permissions</span></span>
<span data-ttu-id="fca8b-121">根据要获取扩展属性的资源以及您请求的权限类型 (委派或应用程序) ，在下表中指定的权限是调用此 API 所需的最低权限。</span><span class="sxs-lookup"><span data-stu-id="fca8b-121">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="fca8b-122">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fca8b-122">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fca8b-123">支持的资源</span><span class="sxs-lookup"><span data-stu-id="fca8b-123">Supported resource</span></span> | <span data-ttu-id="fca8b-124">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fca8b-124">Delegated (work or school account)</span></span> | <span data-ttu-id="fca8b-125">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fca8b-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fca8b-126">应用程序</span><span class="sxs-lookup"><span data-stu-id="fca8b-126">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="fca8b-127">calendar</span><span class="sxs-lookup"><span data-stu-id="fca8b-127">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="fca8b-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-128">Calendars.Read</span></span> | <span data-ttu-id="fca8b-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-129">Calendars.Read</span></span> | <span data-ttu-id="fca8b-130">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-130">Calendars.Read</span></span> |
| [<span data-ttu-id="fca8b-131">联系人</span><span class="sxs-lookup"><span data-stu-id="fca8b-131">contact</span></span>](../resources/contact.md) | <span data-ttu-id="fca8b-132">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-132">Contacts.Read</span></span> | <span data-ttu-id="fca8b-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-133">Contacts.Read</span></span> | <span data-ttu-id="fca8b-134">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-134">Contacts.Read</span></span> |
| [<span data-ttu-id="fca8b-135">contactFolder</span><span class="sxs-lookup"><span data-stu-id="fca8b-135">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="fca8b-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-136">Contacts.Read</span></span> | <span data-ttu-id="fca8b-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-137">Contacts.Read</span></span> | <span data-ttu-id="fca8b-138">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-138">Contacts.Read</span></span> |
| [<span data-ttu-id="fca8b-139">事件</span><span class="sxs-lookup"><span data-stu-id="fca8b-139">event</span></span>](../resources/event.md) | <span data-ttu-id="fca8b-140">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-140">Calendars.Read</span></span> | <span data-ttu-id="fca8b-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-141">Calendars.Read</span></span> |  <span data-ttu-id="fca8b-142">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-142">Calendars.Read</span></span>|
| <span data-ttu-id="fca8b-143">组 [日历](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="fca8b-143">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="fca8b-144">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fca8b-144">Group.Read.All</span></span> | <span data-ttu-id="fca8b-145">不支持</span><span class="sxs-lookup"><span data-stu-id="fca8b-145">Not supported</span></span> | <span data-ttu-id="fca8b-146">不支持</span><span class="sxs-lookup"><span data-stu-id="fca8b-146">Not supported</span></span> |
| <span data-ttu-id="fca8b-147">组 [事件](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="fca8b-147">group [event](../resources/event.md)</span></span> | <span data-ttu-id="fca8b-148">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fca8b-148">Group.Read.All</span></span> | <span data-ttu-id="fca8b-149">不支持</span><span class="sxs-lookup"><span data-stu-id="fca8b-149">Not supported</span></span> | <span data-ttu-id="fca8b-150">不支持</span><span class="sxs-lookup"><span data-stu-id="fca8b-150">Not supported</span></span> |
| <span data-ttu-id="fca8b-151">组[帖子](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="fca8b-151">group [post](../resources/post.md)</span></span> | <span data-ttu-id="fca8b-152">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fca8b-152">Group.Read.All</span></span> | <span data-ttu-id="fca8b-153">不支持</span><span class="sxs-lookup"><span data-stu-id="fca8b-153">Not supported</span></span> | <span data-ttu-id="fca8b-154">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="fca8b-154">Group.Read.All</span></span> |
| [<span data-ttu-id="fca8b-155">mailFolder</span><span class="sxs-lookup"><span data-stu-id="fca8b-155">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="fca8b-156">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-156">Mail.Read</span></span> | <span data-ttu-id="fca8b-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-157">Mail.Read</span></span> | <span data-ttu-id="fca8b-158">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-158">Mail.Read</span></span> |
| [<span data-ttu-id="fca8b-159">邮件</span><span class="sxs-lookup"><span data-stu-id="fca8b-159">message</span></span>](../resources/message.md) | <span data-ttu-id="fca8b-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-160">Mail.Read</span></span> | <span data-ttu-id="fca8b-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-161">Mail.Read</span></span> | <span data-ttu-id="fca8b-162">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="fca8b-162">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="fca8b-163">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fca8b-163">HTTP request</span></span>

<span data-ttu-id="fca8b-p103">获取通过与 **id** 属性中的筛选器匹配的扩展属性扩展的资源实例。请确保对筛选器字符串中的空白字符应用 [URL 编码](https://www.w3schools.com/tags/ref_urlencode.asp)。</span><span class="sxs-lookup"><span data-stu-id="fca8b-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="fca8b-166">获取**邮件**实例：</span><span class="sxs-lookup"><span data-stu-id="fca8b-166">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="fca8b-167">获取 **mailFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="fca8b-167">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="fca8b-168">获取**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="fca8b-168">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="fca8b-169">获取**日历**实例：</span><span class="sxs-lookup"><span data-stu-id="fca8b-169">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="fca8b-170">获取**联系人**实例：</span><span class="sxs-lookup"><span data-stu-id="fca8b-170">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="fca8b-171">获取 **contactFolder** 实例：</span><span class="sxs-lookup"><span data-stu-id="fca8b-171">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="fca8b-172">获取组**事件**实例：</span><span class="sxs-lookup"><span data-stu-id="fca8b-172">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="fca8b-173">获取组 **post** 实例：</span><span class="sxs-lookup"><span data-stu-id="fca8b-173">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="fca8b-174">路径参数</span><span class="sxs-lookup"><span data-stu-id="fca8b-174">Path parameters</span></span>
|<span data-ttu-id="fca8b-175">参数</span><span class="sxs-lookup"><span data-stu-id="fca8b-175">Parameter</span></span>|<span data-ttu-id="fca8b-176">类型</span><span class="sxs-lookup"><span data-stu-id="fca8b-176">Type</span></span>|<span data-ttu-id="fca8b-177">说明</span><span class="sxs-lookup"><span data-stu-id="fca8b-177">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fca8b-178">id_value</span><span class="sxs-lookup"><span data-stu-id="fca8b-178">id_value</span></span>|<span data-ttu-id="fca8b-179">String</span><span class="sxs-lookup"><span data-stu-id="fca8b-179">String</span></span>|<span data-ttu-id="fca8b-p104">要匹配的扩展属性的 ID。它必须遵照其中一种支持的格式。有关详细信息，请参阅 [Outlook 扩展属性概述](../resources/extended-properties-overview.md)。必需。</span><span class="sxs-lookup"><span data-stu-id="fca8b-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="fca8b-184">请求标头</span><span class="sxs-lookup"><span data-stu-id="fca8b-184">Request headers</span></span>
| <span data-ttu-id="fca8b-185">名称</span><span class="sxs-lookup"><span data-stu-id="fca8b-185">Name</span></span>      |<span data-ttu-id="fca8b-186">说明</span><span class="sxs-lookup"><span data-stu-id="fca8b-186">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fca8b-187">Authorization</span><span class="sxs-lookup"><span data-stu-id="fca8b-187">Authorization</span></span>  | <span data-ttu-id="fca8b-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fca8b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fca8b-190">请求正文</span><span class="sxs-lookup"><span data-stu-id="fca8b-190">Request body</span></span>
<span data-ttu-id="fca8b-191">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fca8b-191">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fca8b-192">响应</span><span class="sxs-lookup"><span data-stu-id="fca8b-192">Response</span></span>

<span data-ttu-id="fca8b-193">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="fca8b-193">If successful, this method returns a `200 OK` response code.</span></span>

<span data-ttu-id="fca8b-194">响应正文包括通过匹配的 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) 对象扩展的对象，此对象表示请求的资源实例。</span><span class="sxs-lookup"><span data-stu-id="fca8b-194">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="fca8b-195">示例</span><span class="sxs-lookup"><span data-stu-id="fca8b-195">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fca8b-196">请求</span><span class="sxs-lookup"><span data-stu-id="fca8b-196">Request</span></span>
<span data-ttu-id="fca8b-p106">此示例通过包含一个多值扩展属性获取并扩展指定的事件。此筛选器返回其 **id** 与字符串 `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation`（包含 URL 编码，此处为了便于阅读，已将其删除）匹配的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fca8b-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="fca8b-199">响应</span><span class="sxs-lookup"><span data-stu-id="fca8b-199">Response</span></span>

<span data-ttu-id="fca8b-200">响应正文包括指定事件的所有属性以及此筛选器返回的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fca8b-200">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="fca8b-p107">注意：为了简单起见，会将此处所示的 **event** 对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fca8b-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
