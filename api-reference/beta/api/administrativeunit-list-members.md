---
title: 列出成员
description: 使用此 API 获取成员中一个管理单元的列表 （用户和组）。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7513192986e8df482209c4f8630c8dab8450e614
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917207"
---
# <a name="list-members"></a><span data-ttu-id="3b748-103">列出成员</span><span class="sxs-lookup"><span data-stu-id="3b748-103">List members</span></span>

> <span data-ttu-id="3b748-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3b748-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b748-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3b748-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3b748-106">使用此 API 获取成员中一个管理单元的列表 （用户和组）。</span><span class="sxs-lookup"><span data-stu-id="3b748-106">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b748-107">权限</span><span class="sxs-lookup"><span data-stu-id="3b748-107">Permissions</span></span>
<span data-ttu-id="3b748-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b748-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3b748-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b748-110">Permission type</span></span>      | <span data-ttu-id="3b748-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3b748-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b748-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b748-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3b748-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3b748-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3b748-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b748-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b748-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b748-115">Not supported.</span></span>    |
|<span data-ttu-id="3b748-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b748-116">Application</span></span> | <span data-ttu-id="3b748-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b748-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="3b748-118">注意： 列表中的一个管理单元中的隐藏成员身份的成员，则 Member.Read.Hidden 权限是必需。</span><span class="sxs-lookup"><span data-stu-id="3b748-118">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="3b748-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b748-119">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="3b748-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b748-120">Request headers</span></span>
| <span data-ttu-id="3b748-121">名称</span><span class="sxs-lookup"><span data-stu-id="3b748-121">Name</span></span>      |<span data-ttu-id="3b748-122">说明</span><span class="sxs-lookup"><span data-stu-id="3b748-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3b748-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b748-123">Authorization</span></span>  | <span data-ttu-id="3b748-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3b748-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b748-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b748-126">Request body</span></span>
<span data-ttu-id="3b748-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3b748-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b748-128">响应</span><span class="sxs-lookup"><span data-stu-id="3b748-128">Response</span></span>

<span data-ttu-id="3b748-129">如果成功，此方法返回`200 OK`响应代码和响应正文中的[用户](../resources/user.md)和/或[组](../resources/group.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="3b748-129">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="3b748-130">相反，如果将`$ref`响应将在请求结束时，包含一`@odata.id`成员每 Url 链接。</span><span class="sxs-lookup"><span data-stu-id="3b748-130">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="3b748-131">示例</span><span class="sxs-lookup"><span data-stu-id="3b748-131">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="3b748-132">列表 member 对象</span><span class="sxs-lookup"><span data-stu-id="3b748-132">List member objects</span></span>
<span data-ttu-id="3b748-133">以下请求将列出的管理单元，返回的用户和/或组集合的成员。</span><span class="sxs-lookup"><span data-stu-id="3b748-133">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

<span data-ttu-id="3b748-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b748-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.type":"#microsoft.graph.user",
      "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
      "accountEnabled":true,
      "businessPhones":[],
      "companyName":null,
      "displayName":"Demo User"
    },
    {
      "@odata.type":"#microsoft.graph.group",
      "id":"07eaa5c7-c9b6-45cf-8ff7-3147d5122caa",
      "description":"This group is the best ever",
      "displayName":"Awesome group"
    }
  ]
}
```

##### <a name="list-member-references"></a><span data-ttu-id="3b748-137">列表成员引用</span><span class="sxs-lookup"><span data-stu-id="3b748-137">List member references</span></span>
<span data-ttu-id="3b748-138">以下请求将列表的管理单元，返回的集合的成员引用`@odata.id`成员的引用。</span><span class="sxs-lookup"><span data-stu-id="3b748-138">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="3b748-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b748-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/492c5308-59fd-4740-9c83-4b3db07a6d70"
    },
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/07eaa5c7-c9b6-45cf-8ff7-3147d5122caa"
    }
  ]
}
```
