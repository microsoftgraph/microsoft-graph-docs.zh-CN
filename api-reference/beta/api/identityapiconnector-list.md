---
title: 列出 identityApiConnectors
description: 获取 identityApiConnector 对象及其属性的列表
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ca946e80b590926aa8f15b7b790d5bd098838cf
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720141"
---
# <a name="list-identityapiconnectors"></a><span data-ttu-id="5676d-103">列出 identityApiConnectors</span><span class="sxs-lookup"><span data-stu-id="5676d-103">List identityApiConnectors</span></span>

<span data-ttu-id="5676d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5676d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5676d-105">读取 [identityApiConnector 对象](../resources/identityapiconnector.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="5676d-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5676d-106">权限</span><span class="sxs-lookup"><span data-stu-id="5676d-106">Permissions</span></span>

<span data-ttu-id="5676d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5676d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5676d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5676d-109">Permission type</span></span>                        | <span data-ttu-id="5676d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5676d-110">Permissions (from most to least privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5676d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5676d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5676d-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5676d-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="5676d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5676d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5676d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5676d-114">Not supported.</span></span>  |
| <span data-ttu-id="5676d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5676d-115">Application</span></span>                            | <span data-ttu-id="5676d-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5676d-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="5676d-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="5676d-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="5676d-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="5676d-118">Global administrator</span></span>
* <span data-ttu-id="5676d-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="5676d-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="5676d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5676d-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identity/apiConnectors/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5676d-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5676d-121">Optional query parameters</span></span>
<span data-ttu-id="5676d-122">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5676d-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5676d-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5676d-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5676d-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="5676d-124">Request headers</span></span>
|<span data-ttu-id="5676d-125">名称</span><span class="sxs-lookup"><span data-stu-id="5676d-125">Name</span></span>|<span data-ttu-id="5676d-126">说明</span><span class="sxs-lookup"><span data-stu-id="5676d-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5676d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="5676d-127">Authorization</span></span>|<span data-ttu-id="5676d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5676d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5676d-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5676d-130">Request body</span></span>
<span data-ttu-id="5676d-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5676d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5676d-132">响应</span><span class="sxs-lookup"><span data-stu-id="5676d-132">Response</span></span>

<span data-ttu-id="5676d-133">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [identityApiConnector](../resources/identityapiconnector.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5676d-133">If successful, this method returns a `200 OK` response code and a collection of [identityApiConnector](../resources/identityapiconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5676d-134">示例</span><span class="sxs-lookup"><span data-stu-id="5676d-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="5676d-135">请求</span><span class="sxs-lookup"><span data-stu-id="5676d-135">Request</span></span>

<span data-ttu-id="5676d-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5676d-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_identityApiConnectors"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/apiConnectors
```

### <a name="response"></a><span data-ttu-id="5676d-137">响应</span><span class="sxs-lookup"><span data-stu-id="5676d-137">Response</span></span>

<span data-ttu-id="5676d-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5676d-138">The following is an example of the response.</span></span>

<span data-ttu-id="5676d-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5676d-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityApiConnector",
  "isCollection": true
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/apiConnectors",
    "value": [
      {
          "id": "<guid>",
          "displayName": "Test API",
          "targetUrl": "https://someapi.com/api/endpoint",
          "authenticationConfiguration": {
            "@odata.type": "#microsoft.graph.basicAuthentication",
            "username": "<USERNAME>",
            "password": "******"
          }
      }
  ]
}
```
