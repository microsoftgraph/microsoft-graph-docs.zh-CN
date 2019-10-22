---
title: 列出 memberOf
description: 列出此 organizaitonal 联系人所属的组。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1607fec5a1e329d3d6e472bd4c258bc483a1c5a1
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2019
ms.locfileid: "37622596"
---
# <a name="list-memberof"></a><span data-ttu-id="4ac9c-103">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="4ac9c-103">List memberOf</span></span>

<span data-ttu-id="4ac9c-104">列出此[组织联系人](../resources/orgcontact.md)所属的组。</span><span class="sxs-lookup"><span data-stu-id="4ac9c-104">List the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ac9c-105">权限</span><span class="sxs-lookup"><span data-stu-id="4ac9c-105">Permissions</span></span>
<span data-ttu-id="4ac9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ac9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ac9c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ac9c-108">Permission type</span></span>      | <span data-ttu-id="4ac9c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4ac9c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ac9c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ac9c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4ac9c-111">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="4ac9c-111">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="4ac9c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ac9c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ac9c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ac9c-113">Not supported.</span></span>    |
|<span data-ttu-id="4ac9c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ac9c-114">Application</span></span> | <span data-ttu-id="4ac9c-115">OrgContact 和 Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="4ac9c-115">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ac9c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ac9c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4ac9c-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4ac9c-117">Optional query parameters</span></span>
<span data-ttu-id="4ac9c-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `$select` 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4ac9c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `$select` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ac9c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ac9c-119">Request headers</span></span>
| <span data-ttu-id="4ac9c-120">标头</span><span class="sxs-lookup"><span data-stu-id="4ac9c-120">Header</span></span>       | <span data-ttu-id="4ac9c-121">值</span><span class="sxs-lookup"><span data-stu-id="4ac9c-121">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4ac9c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ac9c-122">Authorization</span></span>  | <span data-ttu-id="4ac9c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4ac9c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ac9c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ac9c-125">Request body</span></span>
<span data-ttu-id="4ac9c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4ac9c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ac9c-127">响应</span><span class="sxs-lookup"><span data-stu-id="4ac9c-127">Response</span></span>

<span data-ttu-id="4ac9c-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="4ac9c-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4ac9c-129">示例</span><span class="sxs-lookup"><span data-stu-id="4ac9c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ac9c-130">请求</span><span class="sxs-lookup"><span data-stu-id="4ac9c-130">Request</span></span>
<span data-ttu-id="4ac9c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4ac9c-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "contact_get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/contacts/{id}/memberOf
```

##### <a name="response"></a><span data-ttu-id="4ac9c-132">响应</span><span class="sxs-lookup"><span data-stu-id="4ac9c-132">Response</span></span>
<span data-ttu-id="4ac9c-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4ac9c-133">The following is an example of the response.</span></span>
><span data-ttu-id="4ac9c-134">**注意**：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4ac9c-134">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4ac9c-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4ac9c-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 155

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "024bbfa0-fe5a-4fce-9227-bd6ccf1324bb",
      "createdDateTime": "2018-01-18T18:54:43Z",
      "description": "Best group ever created",
      "displayName": "Best Group",
      "groupTypes": [],
      "isAssignableToRole": null,
      "onPremisesProvisioningErrors": []
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
