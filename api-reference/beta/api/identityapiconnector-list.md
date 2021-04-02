---
title: 列出 identityApiConnectors
description: 获取 identityApiConnector 对象及其属性的列表
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6aa2d3a4a5c45dc7b9e0b168eac7402404fcb982
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507845"
---
# <a name="list-identityapiconnectors"></a><span data-ttu-id="f7bbc-103">列出 identityApiConnectors</span><span class="sxs-lookup"><span data-stu-id="f7bbc-103">List identityApiConnectors</span></span>

<span data-ttu-id="f7bbc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7bbc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7bbc-105">读取 [identityApiConnector 对象](../resources/identityapiconnector.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f7bbc-105">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7bbc-106">权限</span><span class="sxs-lookup"><span data-stu-id="f7bbc-106">Permissions</span></span>

<span data-ttu-id="f7bbc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7bbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7bbc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7bbc-109">Permission type</span></span>                        | <span data-ttu-id="f7bbc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7bbc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f7bbc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7bbc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7bbc-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7bbc-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="f7bbc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7bbc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7bbc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7bbc-114">Not supported.</span></span>  |
| <span data-ttu-id="f7bbc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7bbc-115">Application</span></span>                            | <span data-ttu-id="f7bbc-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7bbc-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="f7bbc-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="f7bbc-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="f7bbc-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="f7bbc-118">Global administrator</span></span>
* <span data-ttu-id="f7bbc-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="f7bbc-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="f7bbc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7bbc-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identity/apiConnectors/
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7bbc-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f7bbc-121">Optional query parameters</span></span>
<span data-ttu-id="f7bbc-122">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f7bbc-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f7bbc-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f7bbc-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7bbc-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7bbc-124">Request headers</span></span>
|<span data-ttu-id="f7bbc-125">名称</span><span class="sxs-lookup"><span data-stu-id="f7bbc-125">Name</span></span>|<span data-ttu-id="f7bbc-126">说明</span><span class="sxs-lookup"><span data-stu-id="f7bbc-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f7bbc-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7bbc-127">Authorization</span></span>|<span data-ttu-id="f7bbc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7bbc-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7bbc-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7bbc-130">Request body</span></span>
<span data-ttu-id="f7bbc-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7bbc-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7bbc-132">响应</span><span class="sxs-lookup"><span data-stu-id="f7bbc-132">Response</span></span>

<span data-ttu-id="f7bbc-133">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [identityApiConnector](../resources/identityapiconnector.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f7bbc-133">If successful, this method returns a `200 OK` response code and a collection of [identityApiConnector](../resources/identityapiconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7bbc-134">示例</span><span class="sxs-lookup"><span data-stu-id="f7bbc-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7bbc-135">请求</span><span class="sxs-lookup"><span data-stu-id="f7bbc-135">Request</span></span>

<span data-ttu-id="f7bbc-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f7bbc-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f7bbc-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7bbc-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_identityApiConnectors"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/apiConnectors
```
# <a name="c"></a>[<span data-ttu-id="f7bbc-138">C#</span><span class="sxs-lookup"><span data-stu-id="f7bbc-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-identityapiconnectors-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7bbc-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7bbc-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-identityapiconnectors-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7bbc-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7bbc-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-identityapiconnectors-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7bbc-141">Java</span><span class="sxs-lookup"><span data-stu-id="f7bbc-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-identityapiconnectors-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7bbc-142">响应</span><span class="sxs-lookup"><span data-stu-id="f7bbc-142">Response</span></span>

<span data-ttu-id="f7bbc-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f7bbc-143">The following is an example of the response.</span></span>

<span data-ttu-id="f7bbc-144">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f7bbc-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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
        },
        {
            "id": "<guid>",
            "displayName": "My API connector",
            "targetUrl": "https://someotherapi.com/api/endpoint",
            "authenticationConfiguration": {
                "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
                "certificateList": [
                    {
                        "thumbprint": "0EB255CC895477798BA418B378255204304897AD",
                        "notAfter": 1666350522,
                        "notBefore": 1508670522,
                        "isActive": true
                    },
                    {
                        "thumbprint": "1AB255CC895477798BA418B378255204304897BC",
                        "notAfter": 1766350522,
                        "notBefore": 1608670522,
                        "isActive": false
                    }
                ]
            }
        }
  ]
}
```
