---
title: 可传递列表组的成员
description: 获取组的成员的列表。 一组可将用户、 联系人、 设备、 服务主体和其他组作为成员。 此操作可传递，也将返回所有嵌套成员一个平面列表。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 6ed3d4e4a927181f6bf8ea2c90edf337b0f8f32d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576295"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="80596-105">可传递列表组的成员</span><span class="sxs-lookup"><span data-stu-id="80596-105">List group transitive members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80596-106">获取组的成员的列表。</span><span class="sxs-lookup"><span data-stu-id="80596-106">Get a list of the group's members.</span></span> <span data-ttu-id="80596-107">一组可将用户、 联系人、 设备、 服务主体和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="80596-107">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="80596-108">此操作可传递，也将返回所有嵌套成员一个平面列表。</span><span class="sxs-lookup"><span data-stu-id="80596-108">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="80596-109">权限</span><span class="sxs-lookup"><span data-stu-id="80596-109">Permissions</span></span>

<span data-ttu-id="80596-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80596-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80596-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="80596-112">Permission type</span></span>      | <span data-ttu-id="80596-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80596-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80596-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80596-114">Delegated (work or school account)</span></span> | <span data-ttu-id="80596-115">Directory.Read.All，Directory.AccessAsUser.All，User.ReadBasic.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="80596-115">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="80596-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80596-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80596-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="80596-117">Not supported.</span></span>    |
|<span data-ttu-id="80596-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="80596-118">Application</span></span> | <span data-ttu-id="80596-119">Directory.Read.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="80596-119">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="80596-120">注意： 列表中隐藏成员资格组的成员，则 Member.Read.Hidden 权限是必需。</span><span class="sxs-lookup"><span data-stu-id="80596-120">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="80596-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80596-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80596-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="80596-122">Optional query parameters</span></span>

<span data-ttu-id="80596-123">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="80596-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80596-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="80596-124">Request headers</span></span>

| <span data-ttu-id="80596-125">名称</span><span class="sxs-lookup"><span data-stu-id="80596-125">Name</span></span>       | <span data-ttu-id="80596-126">类型</span><span class="sxs-lookup"><span data-stu-id="80596-126">Type</span></span> | <span data-ttu-id="80596-127">说明</span><span class="sxs-lookup"><span data-stu-id="80596-127">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="80596-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="80596-128">Authorization</span></span>  | <span data-ttu-id="80596-129">string</span><span class="sxs-lookup"><span data-stu-id="80596-129">string</span></span>  | <span data-ttu-id="80596-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80596-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80596-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="80596-132">Request body</span></span>

<span data-ttu-id="80596-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="80596-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80596-134">响应</span><span class="sxs-lookup"><span data-stu-id="80596-134">Response</span></span>

<span data-ttu-id="80596-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="80596-135">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80596-136">示例</span><span class="sxs-lookup"><span data-stu-id="80596-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="80596-137">请求</span><span class="sxs-lookup"><span data-stu-id="80596-137">Request</span></span>

<span data-ttu-id="80596-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="80596-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```

### <a name="response"></a><span data-ttu-id="80596-139">响应</span><span class="sxs-lookup"><span data-stu-id="80596-139">Response</span></span>

<span data-ttu-id="80596-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="80596-140">The following is an example of the response.</span></span>
><span data-ttu-id="80596-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="80596-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="80596-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="80596-142">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
    "@odata.type": "#microsoft.graph.user",
    
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-transitivemembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
