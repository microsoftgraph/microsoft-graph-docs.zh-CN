---
title: 应用程序列表
description: 检索此组织中的应用程序的列表。
author: lleonard-msft
ms.openlocfilehash: 138a9e6d238fde44d5b5c47781bbd93cb2b73f98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336692"
---
# <a name="list-applications"></a><span data-ttu-id="0e836-103">应用程序列表</span><span class="sxs-lookup"><span data-stu-id="0e836-103">List applications</span></span>

> <span data-ttu-id="0e836-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0e836-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e836-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0e836-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e836-106">检索此组织中的应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="0e836-106">Retrieve the list of applications in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e836-107">权限</span><span class="sxs-lookup"><span data-stu-id="0e836-107">Permissions</span></span>
<span data-ttu-id="0e836-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0e836-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0e836-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e836-110">Permission type</span></span>      | <span data-ttu-id="0e836-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0e836-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e836-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e836-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0e836-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0e836-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0e836-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e836-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e836-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e836-115">Not supported.</span></span>    |
|<span data-ttu-id="0e836-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e836-116">Application</span></span> | <span data-ttu-id="0e836-117">Application.ReadWrite.All Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e836-117">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e836-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e836-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0e836-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0e836-119">Optional query parameters</span></span>
<span data-ttu-id="0e836-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0e836-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e836-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e836-121">Request headers</span></span>
| <span data-ttu-id="0e836-122">Name</span><span class="sxs-lookup"><span data-stu-id="0e836-122">Name</span></span>       | <span data-ttu-id="0e836-123">类型</span><span class="sxs-lookup"><span data-stu-id="0e836-123">Type</span></span> | <span data-ttu-id="0e836-124">说明</span><span class="sxs-lookup"><span data-stu-id="0e836-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0e836-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e836-125">Authorization</span></span>  | <span data-ttu-id="0e836-126">string</span><span class="sxs-lookup"><span data-stu-id="0e836-126">string</span></span>  | <span data-ttu-id="0e836-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0e836-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e836-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e836-129">Request body</span></span>
<span data-ttu-id="0e836-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e836-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e836-131">响应</span><span class="sxs-lookup"><span data-stu-id="0e836-131">Response</span></span>

<span data-ttu-id="0e836-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[应用程序](../resources/application.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="0e836-132">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0e836-133">示例</span><span class="sxs-lookup"><span data-stu-id="0e836-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e836-134">请求</span><span class="sxs-lookup"><span data-stu-id="0e836-134">Request</span></span>
<span data-ttu-id="0e836-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e836-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```http
GET https://graph.microsoft.com/beta/applications
```
##### <a name="response"></a><span data-ttu-id="0e836-136">响应</span><span class="sxs-lookup"><span data-stu-id="0e836-136">Response</span></span>
<span data-ttu-id="0e836-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e836-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1229

{
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
