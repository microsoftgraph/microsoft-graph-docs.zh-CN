---
title: 列出成员
description: 使用此 API 获取管理单元 (组) 成员列表。
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6eca10c34ea8750a356a584aac8c09e2e6006a6b
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991510"
---
# <a name="list-members"></a><span data-ttu-id="e43a9-103">列出成员</span><span class="sxs-lookup"><span data-stu-id="e43a9-103">List members</span></span>

<span data-ttu-id="e43a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e43a9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e43a9-105">使用此 API 获取管理单元 (组) 成员列表。</span><span class="sxs-lookup"><span data-stu-id="e43a9-105">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="e43a9-106">权限</span><span class="sxs-lookup"><span data-stu-id="e43a9-106">Permissions</span></span>
<span data-ttu-id="e43a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e43a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e43a9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e43a9-109">Permission type</span></span>      | <span data-ttu-id="e43a9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e43a9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e43a9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e43a9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e43a9-112">AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e43a9-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e43a9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e43a9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e43a9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e43a9-114">Not supported.</span></span>    |
|<span data-ttu-id="e43a9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e43a9-115">Application</span></span> | <span data-ttu-id="e43a9-116">AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e43a9-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="e43a9-117">注意：若要列出管理单元中隐藏成员身份的成员，需要 Member.Read.Hidden 权限。</span><span class="sxs-lookup"><span data-stu-id="e43a9-117">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="e43a9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e43a9-118">HTTP request</span></span>

```http
GET /directory/administrativeUnits/{id}/members
GET /directory/administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e43a9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e43a9-119">Request headers</span></span>
| <span data-ttu-id="e43a9-120">名称</span><span class="sxs-lookup"><span data-stu-id="e43a9-120">Name</span></span>      |<span data-ttu-id="e43a9-121">说明</span><span class="sxs-lookup"><span data-stu-id="e43a9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e43a9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e43a9-122">Authorization</span></span>  | <span data-ttu-id="e43a9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e43a9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e43a9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e43a9-125">Request body</span></span>
<span data-ttu-id="e43a9-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e43a9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e43a9-127">响应</span><span class="sxs-lookup"><span data-stu-id="e43a9-127">Response</span></span>

<span data-ttu-id="e43a9-128">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [user](../resources/user.md) 和/或 [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e43a9-128">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="e43a9-129">相反，如果放在请求末尾，响应将包含指向成员的链接 `$ref` `@odata.id` /URL 集合。</span><span class="sxs-lookup"><span data-stu-id="e43a9-129">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="e43a9-130">示例</span><span class="sxs-lookup"><span data-stu-id="e43a9-130">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="e43a9-131">列出成员对象</span><span class="sxs-lookup"><span data-stu-id="e43a9-131">List member objects</span></span>
<span data-ttu-id="e43a9-132">以下请求将列出管理单元的成员，并返回用户和/或组的集合。</span><span class="sxs-lookup"><span data-stu-id="e43a9-132">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members
```

<span data-ttu-id="e43a9-p104">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e43a9-p104">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
 
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

##### <a name="list-member-references"></a><span data-ttu-id="e43a9-135">列出成员引用</span><span class="sxs-lookup"><span data-stu-id="e43a9-135">List member references</span></span>
<span data-ttu-id="e43a9-136">以下请求将列出管理单元的成员引用，并返回 `@odata.id` 对成员的引用集合。</span><span class="sxs-lookup"><span data-stu-id="e43a9-136">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="e43a9-p105">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e43a9-p105">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/492c5308-59fd-4740-9c83-4b3db07a6d70"
    },
    {
      "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/07eaa5c7-c9b6-45cf-8ff7-3147d5122caa"
    }
  ]
}
```
