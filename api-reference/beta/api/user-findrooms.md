---
title: 用户： findRooms
description: '获取所有会议房间或特定的会议室列表中用户的租户。 '
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0be6034056b20473b65e9a04c70419b3e4e1ba95
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934007"
---
# <a name="user-findrooms"></a><span data-ttu-id="67f3d-103">用户： findRooms</span><span class="sxs-lookup"><span data-stu-id="67f3d-103">user: findRooms</span></span>

> <span data-ttu-id="67f3d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="67f3d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67f3d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="67f3d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="67f3d-106">获取所有会议房间或特定的会议室列表中用户的租户。</span><span class="sxs-lookup"><span data-stu-id="67f3d-106">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="67f3d-107">租户可以将会议房间组织为会议室列表。</span><span class="sxs-lookup"><span data-stu-id="67f3d-107">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="67f3d-108">[EmailAddress](../resources/emailaddress.md)实例表示每个会议室和会议室列表。</span><span class="sxs-lookup"><span data-stu-id="67f3d-108">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="67f3d-109">您可以[获取所有会议室列表](user-findroomlists.md)中的租户，请都获取租户中的所有聊天室或都都获取特定会议室列表中的所有聊天室。</span><span class="sxs-lookup"><span data-stu-id="67f3d-109">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="67f3d-110">您可以获得多租户中的前 100 个聊天室。</span><span class="sxs-lookup"><span data-stu-id="67f3d-110">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="67f3d-111">权限</span><span class="sxs-lookup"><span data-stu-id="67f3d-111">Permissions</span></span>
<span data-ttu-id="67f3d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67f3d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="67f3d-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="67f3d-114">Permission type</span></span>      | <span data-ttu-id="67f3d-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67f3d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67f3d-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67f3d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="67f3d-117">User.ReadBasic.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="67f3d-117">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="67f3d-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67f3d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67f3d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="67f3d-119">Not supported.</span></span>    |
|<span data-ttu-id="67f3d-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="67f3d-120">Application</span></span> | <span data-ttu-id="67f3d-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="67f3d-121">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="67f3d-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67f3d-122">HTTP request</span></span>

<span data-ttu-id="67f3d-123">若要获取租户中的所有聊天室：</span><span class="sxs-lookup"><span data-stu-id="67f3d-123">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/<id>/findRooms
```

<span data-ttu-id="67f3d-124">若要获取的租户特定的会议室列表中的所有聊天室：</span><span class="sxs-lookup"><span data-stu-id="67f3d-124">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list}')
GET /users/<id>/findRooms(RoomList='{room_list}')
```

## <a name="query-parameters"></a><span data-ttu-id="67f3d-125">查询参数</span><span class="sxs-lookup"><span data-stu-id="67f3d-125">Query parameters</span></span>

| <span data-ttu-id="67f3d-126">查询参数</span><span class="sxs-lookup"><span data-stu-id="67f3d-126">Query parameter</span></span>       | <span data-ttu-id="67f3d-127">类型</span><span class="sxs-lookup"><span data-stu-id="67f3d-127">Type</span></span> | <span data-ttu-id="67f3d-128">说明</span><span class="sxs-lookup"><span data-stu-id="67f3d-128">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="67f3d-129">RoomList</span><span class="sxs-lookup"><span data-stu-id="67f3d-129">RoomList</span></span> | <span data-ttu-id="67f3d-130">string</span><span class="sxs-lookup"><span data-stu-id="67f3d-130">string</span></span> | <span data-ttu-id="67f3d-131">与会议室列表关联的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="67f3d-131">The SMTP address associated with the room list.</span></span> <span data-ttu-id="67f3d-132">由包括 SMTP 地址的[电子邮件地址](../resources/emailaddress.md)实例表示每个会议室列表。</span><span class="sxs-lookup"><span data-stu-id="67f3d-132">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="67f3d-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="67f3d-133">Request headers</span></span>
| <span data-ttu-id="67f3d-134">名称</span><span class="sxs-lookup"><span data-stu-id="67f3d-134">Name</span></span>       | <span data-ttu-id="67f3d-135">类型</span><span class="sxs-lookup"><span data-stu-id="67f3d-135">Type</span></span> | <span data-ttu-id="67f3d-136">说明</span><span class="sxs-lookup"><span data-stu-id="67f3d-136">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="67f3d-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="67f3d-137">Authorization</span></span>  | <span data-ttu-id="67f3d-138">string</span><span class="sxs-lookup"><span data-stu-id="67f3d-138">string</span></span>  | <span data-ttu-id="67f3d-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="67f3d-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="67f3d-141">Content-Type</span><span class="sxs-lookup"><span data-stu-id="67f3d-141">Content-Type</span></span>  | <span data-ttu-id="67f3d-142">string</span><span class="sxs-lookup"><span data-stu-id="67f3d-142">string</span></span>  | <span data-ttu-id="67f3d-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="67f3d-p106">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="67f3d-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="67f3d-145">Request body</span></span>
<span data-ttu-id="67f3d-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="67f3d-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67f3d-147">响应</span><span class="sxs-lookup"><span data-stu-id="67f3d-147">Response</span></span>

<span data-ttu-id="67f3d-148">如果成功，此方法返回`200 OK`响应正文中的响应代码和[emailAddress](../resources/emailaddress.md)集合的对象。</span><span class="sxs-lookup"><span data-stu-id="67f3d-148">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="67f3d-149">示例</span><span class="sxs-lookup"><span data-stu-id="67f3d-149">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="67f3d-150">请求 1</span><span class="sxs-lookup"><span data-stu-id="67f3d-150">Request 1</span></span>

<span data-ttu-id="67f3d-151">第一个示例获取在登录用户的租户中定义的所有聊天室。</span><span class="sxs-lookup"><span data-stu-id="67f3d-151">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```

##### <a name="response-1"></a><span data-ttu-id="67f3d-152">响应 1</span><span class="sxs-lookup"><span data-stu-id="67f3d-152">Response 1</span></span>
<span data-ttu-id="67f3d-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="67f3d-153">Here is an example of the response.</span></span> 

<span data-ttu-id="67f3d-p107">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="67f3d-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_rooms_in_tenant",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAddress",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAddress)",
    "value": [
        {
            "name": "Conf Room Adams",
            "address": "Adams@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Baker",
            "address": "Baker@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Crystal",
            "address": "Crystal@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Hood",
            "address": "Hood@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Rainier",
            "address": "Rainier@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Stevens",
            "address": "Stevens@contoso.onmicrosoft.com"
        }
    ]
}
```

##### <a name="request-2"></a><span data-ttu-id="67f3d-156">请求 2</span><span class="sxs-lookup"><span data-stu-id="67f3d-156">Request 2</span></span>

<span data-ttu-id="67f3d-157">第二个示例获取标识的电子邮件地址 Building2Rooms@contoso.onmicrosoft.com 的指定的会议室列表中的聊天室。</span><span class="sxs-lookup"><span data-stu-id="67f3d-157">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```

##### <a name="response-2"></a><span data-ttu-id="67f3d-158">响应 2</span><span class="sxs-lookup"><span data-stu-id="67f3d-158">Response 2</span></span>
<span data-ttu-id="67f3d-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="67f3d-159">Here is an example of the response.</span></span> 

<span data-ttu-id="67f3d-p108">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="67f3d-p108">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_rooms_from_specific_list",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAddress",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAddress)",
    "value": [
        {
            "name": "Conf Room Baker",
            "address": "Baker@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Hood",
            "address": "Hood@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Rainier",
            "address": "Rainier@contoso.onmicrosoft.com"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: findRooms",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
