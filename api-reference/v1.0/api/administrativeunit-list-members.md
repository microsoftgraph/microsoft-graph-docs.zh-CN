---
title: 列出成员
description: 使用此 API 获取管理单元 (组) 成员列表。
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 538b9c5448cfe2c7cd6eae1b0d9d78825fdf10ef
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433010"
---
# <a name="list-members"></a><span data-ttu-id="1346b-103">列出成员</span><span class="sxs-lookup"><span data-stu-id="1346b-103">List members</span></span>

<span data-ttu-id="1346b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1346b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1346b-105">使用此 API 获取管理单元 (组) 成员列表。</span><span class="sxs-lookup"><span data-stu-id="1346b-105">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="1346b-106">权限</span><span class="sxs-lookup"><span data-stu-id="1346b-106">Permissions</span></span>
<span data-ttu-id="1346b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1346b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1346b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1346b-109">Permission type</span></span>      | <span data-ttu-id="1346b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1346b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1346b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1346b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1346b-112">AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1346b-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1346b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1346b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1346b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1346b-114">Not supported.</span></span>    |
|<span data-ttu-id="1346b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1346b-115">Application</span></span> | <span data-ttu-id="1346b-116">AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1346b-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="1346b-117">注意：若要列出管理单元中隐藏成员身份的成员，需要 Member.Read.Hidden 权限。</span><span class="sxs-lookup"><span data-stu-id="1346b-117">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="1346b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1346b-118">HTTP request</span></span>

```http
GET /directory/administrativeUnits/{id}/members
GET /directory/administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="1346b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1346b-119">Request headers</span></span>
| <span data-ttu-id="1346b-120">名称</span><span class="sxs-lookup"><span data-stu-id="1346b-120">Name</span></span>      |<span data-ttu-id="1346b-121">说明</span><span class="sxs-lookup"><span data-stu-id="1346b-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1346b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1346b-122">Authorization</span></span>  | <span data-ttu-id="1346b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1346b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1346b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1346b-125">Request body</span></span>
<span data-ttu-id="1346b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1346b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1346b-127">响应</span><span class="sxs-lookup"><span data-stu-id="1346b-127">Response</span></span>

<span data-ttu-id="1346b-128">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [用户](../resources/user.md) 和/或 [组](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1346b-128">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="1346b-129">相反，如果放在请求末尾，响应将包含指向成员的链接 `$ref` `@odata.id` /URL 集合。</span><span class="sxs-lookup"><span data-stu-id="1346b-129">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="1346b-130">示例</span><span class="sxs-lookup"><span data-stu-id="1346b-130">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="1346b-131">列出成员对象</span><span class="sxs-lookup"><span data-stu-id="1346b-131">List member objects</span></span>
<span data-ttu-id="1346b-132">以下请求将列出管理单元的成员，并返回用户和/或组的集合。</span><span class="sxs-lookup"><span data-stu-id="1346b-132">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members
```

<span data-ttu-id="1346b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1346b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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

##### <a name="list-member-references"></a><span data-ttu-id="1346b-136">列出成员引用</span><span class="sxs-lookup"><span data-stu-id="1346b-136">List member references</span></span>
<span data-ttu-id="1346b-137">以下请求将列出管理单元的成员引用，并返回对 `@odata.id` 成员的引用集合。</span><span class="sxs-lookup"><span data-stu-id="1346b-137">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="1346b-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1346b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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
