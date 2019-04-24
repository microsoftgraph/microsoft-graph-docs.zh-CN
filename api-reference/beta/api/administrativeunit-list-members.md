---
title: 列出成员
description: 使用此 API 获取管理单元中的成员列表 (用户和组)。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: aa8d70d72c5d55cac0ff8aea66d3c56b4e9f80ce
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459496"
---
# <a name="list-members"></a><span data-ttu-id="4b217-103">列出成员</span><span class="sxs-lookup"><span data-stu-id="4b217-103">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b217-104">使用此 API 获取管理单元中的成员列表 (用户和组)。</span><span class="sxs-lookup"><span data-stu-id="4b217-104">Use this API to get the members list (user and group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b217-105">权限</span><span class="sxs-lookup"><span data-stu-id="4b217-105">Permissions</span></span>
<span data-ttu-id="4b217-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b217-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4b217-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b217-108">Permission type</span></span>      | <span data-ttu-id="4b217-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4b217-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b217-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b217-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4b217-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4b217-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4b217-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b217-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4b217-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b217-113">Not supported.</span></span>    |
|<span data-ttu-id="4b217-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b217-114">Application</span></span> | <span data-ttu-id="4b217-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b217-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="4b217-116">注意: 若要在管理单元中列出隐藏成员身份的成员, 则需要使用 Read. hidden 权限是必需的。</span><span class="sxs-lookup"><span data-stu-id="4b217-116">Note: To list the members of a hidden membership in an administrative unit, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="4b217-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b217-117">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="4b217-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b217-118">Request headers</span></span>
| <span data-ttu-id="4b217-119">名称</span><span class="sxs-lookup"><span data-stu-id="4b217-119">Name</span></span>      |<span data-ttu-id="4b217-120">说明</span><span class="sxs-lookup"><span data-stu-id="4b217-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4b217-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b217-121">Authorization</span></span>  | <span data-ttu-id="4b217-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4b217-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4b217-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b217-124">Request body</span></span>
<span data-ttu-id="4b217-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4b217-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b217-126">响应</span><span class="sxs-lookup"><span data-stu-id="4b217-126">Response</span></span>

<span data-ttu-id="4b217-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[user](../resources/user.md)和/或[group](../resources/group.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="4b217-127">If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) and/or [group](../resources/group.md) objects in the response body.</span></span>  <span data-ttu-id="4b217-128">相反, 如果放`$ref`在请求的末尾, 则响应将包含成员的链接/url 的`@odata.id`集合。</span><span class="sxs-lookup"><span data-stu-id="4b217-128">Instead, if you put `$ref` at the end of the request, the response will contain a collection of `@odata.id` links/URLs to the members.</span></span>

## <a name="examples"></a><span data-ttu-id="4b217-129">示例</span><span class="sxs-lookup"><span data-stu-id="4b217-129">Examples</span></span>
##### <a name="list-member-objects"></a><span data-ttu-id="4b217-130">列出成员对象</span><span class="sxs-lookup"><span data-stu-id="4b217-130">List member objects</span></span>
<span data-ttu-id="4b217-131">以下请求将列出管理单元的成员, 并返回用户和/或组的集合。</span><span class="sxs-lookup"><span data-stu-id="4b217-131">The following request will list the members of the administrative unit, returning a collection of users and/or groups.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

<span data-ttu-id="4b217-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4b217-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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

##### <a name="list-member-references"></a><span data-ttu-id="4b217-135">列出成员引用</span><span class="sxs-lookup"><span data-stu-id="4b217-135">List member references</span></span>
<span data-ttu-id="4b217-136">下面的请求将列出管理单元的成员引用, 并返回对成员的`@odata.id`引用集合。</span><span class="sxs-lookup"><span data-stu-id="4b217-136">The following request will list the member references of the administrative unit, returning a collection of `@odata.id` references to the members.</span></span>
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
<span data-ttu-id="4b217-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4b217-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
 
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-list-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
