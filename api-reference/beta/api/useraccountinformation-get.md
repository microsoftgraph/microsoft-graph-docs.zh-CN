---
title: 获取 userAccountInformation
description: 检索 userAccountInformation 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: Profile
doc_type: apiPageType
ms.openlocfilehash: 5f56163db9ea7a13cc03d7199f371cdc070891fd
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228357"
---
# <a name="get-useraccountinformation"></a><span data-ttu-id="155df-103">获取 userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="155df-103">Get userAccountInformation</span></span>

<span data-ttu-id="155df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="155df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="155df-105">检索[userAccountInformation](../resources/useraccountinformation.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="155df-105">Retrieve the properties and relationships of a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="155df-106">权限</span><span class="sxs-lookup"><span data-stu-id="155df-106">Permissions</span></span>

<span data-ttu-id="155df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="155df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="155df-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="155df-109">Permission type</span></span>                        | <span data-ttu-id="155df-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="155df-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="155df-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="155df-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="155df-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="155df-112">Not supported.</span></span>                              |
| <span data-ttu-id="155df-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="155df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="155df-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="155df-114">Not supported.</span></span>                              |
| <span data-ttu-id="155df-115">Application</span><span class="sxs-lookup"><span data-stu-id="155df-115">Application</span></span>                            | <span data-ttu-id="155df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="155df-116">Not supported.</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="155df-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="155df-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /user/profile/account
```

## <a name="optional-query-parameters"></a><span data-ttu-id="155df-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="155df-118">Optional query parameters</span></span>

<span data-ttu-id="155df-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="155df-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="155df-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="155df-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="155df-121">请求头</span><span class="sxs-lookup"><span data-stu-id="155df-121">Request headers</span></span>

| <span data-ttu-id="155df-122">名称</span><span class="sxs-lookup"><span data-stu-id="155df-122">Name</span></span>          |<span data-ttu-id="155df-123">说明</span><span class="sxs-lookup"><span data-stu-id="155df-123">Description</span></span>                |
|:--------------|:--------------------------|
| <span data-ttu-id="155df-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="155df-124">Authorization</span></span> | <span data-ttu-id="155df-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="155df-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="155df-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="155df-127">Request body</span></span>

<span data-ttu-id="155df-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="155df-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="155df-129">响应</span><span class="sxs-lookup"><span data-stu-id="155df-129">Response</span></span>

<span data-ttu-id="155df-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[userAccountInformation](../resources/useraccountinformation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="155df-130">If successful, this method returns a `200 OK` response code and the requested [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="155df-131">示例</span><span class="sxs-lookup"><span data-stu-id="155df-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="155df-132">请求</span><span class="sxs-lookup"><span data-stu-id="155df-132">Request</span></span>

<span data-ttu-id="155df-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="155df-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_useraccountinformation"
}-->

```http
GET https://graph.microsoft.com/Beta/user/profile/account
```

### <a name="response"></a><span data-ttu-id="155df-134">响应</span><span class="sxs-lookup"><span data-stu-id="155df-134">Response</span></span>

<span data-ttu-id="155df-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="155df-135">The following is an example of the response.</span></span>

> <span data-ttu-id="155df-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="155df-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "ageGroup": "ageGroup-value",
  "countryCode": "countryCode-value",
  "preferredLanguageTag": {
    "locale": "locale-value",
    "displayName": "displayName-value"
  },
  "userPrincipalName": "userPrincipalName-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get userAccountInformation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
