---
title: 获取 userAccountInformation
description: 检索 useraccountinformation 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: Profile
doc_type: apiPageType
ms.openlocfilehash: 5d9f276b0fd3677318eb6d9a6701fc77903ba69f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451572"
---
# <a name="get-useraccountinformation"></a><span data-ttu-id="6d1b7-103">获取 userAccountInformation</span><span class="sxs-lookup"><span data-stu-id="6d1b7-103">Get userAccountInformation</span></span>

<span data-ttu-id="6d1b7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6d1b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d1b7-105">检索[userAccountInformation](../resources/useraccountinformation.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6d1b7-105">Retrieve the properties and relationships of a [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d1b7-106">权限</span><span class="sxs-lookup"><span data-stu-id="6d1b7-106">Permissions</span></span>

<span data-ttu-id="6d1b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d1b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d1b7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d1b7-109">Permission type</span></span>                        | <span data-ttu-id="6d1b7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6d1b7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6d1b7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d1b7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d1b7-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d1b7-112">Not supported.</span></span> |
| <span data-ttu-id="6d1b7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d1b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d1b7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d1b7-114">Not supported.</span></span> |
| <span data-ttu-id="6d1b7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d1b7-115">Application</span></span>                            | <span data-ttu-id="6d1b7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d1b7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d1b7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d1b7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /user/profile/account
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d1b7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6d1b7-118">Optional query parameters</span></span>

<span data-ttu-id="6d1b7-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6d1b7-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6d1b7-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6d1b7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d1b7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d1b7-121">Request headers</span></span>

| <span data-ttu-id="6d1b7-122">名称</span><span class="sxs-lookup"><span data-stu-id="6d1b7-122">Name</span></span>      |<span data-ttu-id="6d1b7-123">说明</span><span class="sxs-lookup"><span data-stu-id="6d1b7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6d1b7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d1b7-124">Authorization</span></span> | <span data-ttu-id="6d1b7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6d1b7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d1b7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d1b7-127">Request body</span></span>

<span data-ttu-id="6d1b7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6d1b7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d1b7-129">响应</span><span class="sxs-lookup"><span data-stu-id="6d1b7-129">Response</span></span>

<span data-ttu-id="6d1b7-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[userAccountInformation](../resources/useraccountinformation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6d1b7-130">If successful, this method returns a `200 OK` response code and the requested [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d1b7-131">示例</span><span class="sxs-lookup"><span data-stu-id="6d1b7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d1b7-132">请求</span><span class="sxs-lookup"><span data-stu-id="6d1b7-132">Request</span></span>

<span data-ttu-id="6d1b7-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6d1b7-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_useraccountinformation"
}-->

```http
GET https://graph.microsoft.com/Beta/user/profile/account
```

### <a name="response"></a><span data-ttu-id="6d1b7-134">响应</span><span class="sxs-lookup"><span data-stu-id="6d1b7-134">Response</span></span>

<span data-ttu-id="6d1b7-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6d1b7-135">The following is an example of the response.</span></span>

> <span data-ttu-id="6d1b7-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6d1b7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
