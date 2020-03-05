---
title: 列出成员
description: 使用此 API 获取管理单元中的成员列表（用户和组）。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b5e2c8b25a81f3ae23e33270e17e0303bbad4940
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441707"
---
# <a name="list-members"></a><span data-ttu-id="eb93d-103">列出成员</span><span class="sxs-lookup"><span data-stu-id="eb93d-103">List members</span></span>

<span data-ttu-id="eb93d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="eb93d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb93d-105">使用此 API 获取管理单元中的成员列表（用户和组）。</span><span class="sxs-lookup"><span data-stu-id="eb93d-105">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb93d-106">权限</span><span class="sxs-lookup"><span data-stu-id="eb93d-106">Permissions</span></span>
<span data-ttu-id="eb93d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb93d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb93d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb93d-109">Permission type</span></span>      | <span data-ttu-id="eb93d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb93d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb93d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb93d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eb93d-112">AdministrativeUnit、AdministrativeUnit、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="eb93d-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eb93d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb93d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb93d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb93d-114">Not supported.</span></span>    |
|<span data-ttu-id="eb93d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb93d-115">Application</span></span> | <span data-ttu-id="eb93d-116">AdministrativeUnit、AdministrativeUnit、all、all、all、All 和所有的</span><span class="sxs-lookup"><span data-stu-id="eb93d-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="eb93d-117">注意：若要在管理单元中列出隐藏成员身份的成员，则需要使用 Read. Hidden 权限是必需的。</span><span class="sxs-lookup"><span data-stu-id="eb93d-117">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="eb93d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb93d-118">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="eb93d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb93d-119">Request headers</span></span>
| <span data-ttu-id="eb93d-120">名称</span><span class="sxs-lookup"><span data-stu-id="eb93d-120">Name</span></span>      |<span data-ttu-id="eb93d-121">说明</span><span class="sxs-lookup"><span data-stu-id="eb93d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="eb93d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb93d-122">Authorization</span></span>  | <span data-ttu-id="eb93d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb93d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb93d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb93d-125">Request body</span></span>
<span data-ttu-id="eb93d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eb93d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb93d-127">响应</span><span class="sxs-lookup"><span data-stu-id="eb93d-127">Response</span></span>

<span data-ttu-id="eb93d-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[user](../resources/user.md)和/或[group](../resources/group.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="eb93d-128">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="eb93d-129">相反，如果放`$ref`在请求的末尾，则响应将包含成员的链接/url 的`@odata.id`集合。</span><span class="sxs-lookup"><span data-stu-id="eb93d-129">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="eb93d-130">示例</span><span class="sxs-lookup"><span data-stu-id="eb93d-130">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="eb93d-131">列出成员对象</span><span class="sxs-lookup"><span data-stu-id="eb93d-131">List member objects</span></span>
<span data-ttu-id="eb93d-132">以下请求将列出管理单元的成员，并返回用户和/或组的集合。</span><span class="sxs-lookup"><span data-stu-id="eb93d-132">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

<span data-ttu-id="eb93d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eb93d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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

##### <a name="list-member-references"></a><span data-ttu-id="eb93d-136">列出成员引用</span><span class="sxs-lookup"><span data-stu-id="eb93d-136">List member references</span></span>
<span data-ttu-id="eb93d-137">下面的请求将列出管理单元的成员引用，并返回对成员的`@odata.id`引用集合。</span><span class="sxs-lookup"><span data-stu-id="eb93d-137">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="eb93d-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eb93d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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
