---
title: 向组授予的列表 appRoleAssignments
description: 检索已授予组的 appRoleAssignments 的列表。
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 310629a06e911f408b780bdcbfa19c61bc7997e9
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288693"
---
# <a name="list-approleassignments-granted-to-a-group"></a><span data-ttu-id="4f992-103">向组授予的列表 appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="4f992-103">List appRoleAssignments granted to a group</span></span>

<span data-ttu-id="4f992-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f992-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4f992-105">检索已授予组的[appRoleAssignment](../resources/approleassignment.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="4f992-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a group.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f992-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4f992-106">Permissions</span></span>

<span data-ttu-id="4f992-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f992-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f992-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f992-109">Permission type</span></span>      | <span data-ttu-id="4f992-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f992-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f992-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f992-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4f992-112">"AppRoleAssignment"、"全部"、"全部"、"Directory.accessasuser.all"、"全部"、"全部"、"directory"</span><span class="sxs-lookup"><span data-stu-id="4f992-112">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="4f992-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f992-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f992-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f992-114">Not supported.</span></span>    |
|<span data-ttu-id="4f992-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f992-115">Application</span></span> | <span data-ttu-id="4f992-116">"AppRoleAssignment"、"全部"、"全部"、"全部"、"全部"、"目录"</span><span class="sxs-lookup"><span data-stu-id="4f992-116">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f992-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f992-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f992-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4f992-118">Optional query parameters</span></span>

<span data-ttu-id="4f992-119">此方法支持使用 [OData 查询参数](/graph/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4f992-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f992-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f992-120">Request headers</span></span>

| <span data-ttu-id="4f992-121">名称</span><span class="sxs-lookup"><span data-stu-id="4f992-121">Name</span></span>           | <span data-ttu-id="4f992-122">说明</span><span class="sxs-lookup"><span data-stu-id="4f992-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="4f992-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f992-123">Authorization</span></span>  | <span data-ttu-id="4f992-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f992-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4f992-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f992-126">Request body</span></span>

<span data-ttu-id="4f992-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4f992-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f992-128">响应</span><span class="sxs-lookup"><span data-stu-id="4f992-128">Response</span></span>

<span data-ttu-id="4f992-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="4f992-129">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f992-130">示例</span><span class="sxs-lookup"><span data-stu-id="4f992-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f992-131">请求</span><span class="sxs-lookup"><span data-stu-id="4f992-131">Request</span></span>

<span data-ttu-id="4f992-132">下面的示例演示了一个检索已分配给组的应用程序角色的请求。</span><span class="sxs-lookup"><span data-stu-id="4f992-132">The following example shows a request to retrieve the app roles that have been assigned to a group.</span></span>

<!-- {
  "blockType": "request",
  "name": "group_get_approleassignments"
}-->

```http
GET https://graph.microsoft.com/v1.0/groups/{id}/appRoleAssignments
```

### <a name="response"></a><span data-ttu-id="4f992-133">响应</span><span class="sxs-lookup"><span data-stu-id="4f992-133">Response</span></span>

<span data-ttu-id="4f992-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4f992-134">The following is an example of the response.</span></span>

> <span data-ttu-id="4f992-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4f992-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
