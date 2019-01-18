---
title: 获取应用程序
description: 检索应用程序对象的属性和关系。
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 444a95d437591bade674b350c67ec349b06f8d8c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941805"
---
# <a name="get-application"></a><span data-ttu-id="8d8fe-103">获取应用程序</span><span class="sxs-lookup"><span data-stu-id="8d8fe-103">Get an application key</span></span>

> <span data-ttu-id="8d8fe-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8d8fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d8fe-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8d8fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d8fe-106">检索应用程序对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8d8fe-106">Retrieve the properties and relationships of calendar object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d8fe-107">权限</span><span class="sxs-lookup"><span data-stu-id="8d8fe-107">Permissions</span></span>
<span data-ttu-id="8d8fe-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d8fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d8fe-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d8fe-110">Permission type</span></span>      | <span data-ttu-id="8d8fe-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d8fe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d8fe-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d8fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8d8fe-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8d8fe-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8d8fe-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d8fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d8fe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d8fe-115">Not supported.</span></span>    |
|<span data-ttu-id="8d8fe-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d8fe-116">Application</span></span> | <span data-ttu-id="8d8fe-117">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="8d8fe-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d8fe-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d8fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8d8fe-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8d8fe-119">Optional query parameters</span></span>
<span data-ttu-id="8d8fe-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8d8fe-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d8fe-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d8fe-121">Request headers</span></span>
| <span data-ttu-id="8d8fe-122">名称</span><span class="sxs-lookup"><span data-stu-id="8d8fe-122">Name</span></span>       | <span data-ttu-id="8d8fe-123">类型</span><span class="sxs-lookup"><span data-stu-id="8d8fe-123">Type</span></span> | <span data-ttu-id="8d8fe-124">说明</span><span class="sxs-lookup"><span data-stu-id="8d8fe-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8d8fe-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d8fe-125">Authorization</span></span>  | <span data-ttu-id="8d8fe-126">string</span><span class="sxs-lookup"><span data-stu-id="8d8fe-126">string</span></span>  | <span data-ttu-id="8d8fe-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8d8fe-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d8fe-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d8fe-129">Request body</span></span>
<span data-ttu-id="8d8fe-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8d8fe-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d8fe-131">响应</span><span class="sxs-lookup"><span data-stu-id="8d8fe-131">Response</span></span>

<span data-ttu-id="8d8fe-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8d8fe-132">If successful, this method returns a `200 OK` response code and a [settingStateDeviceSummary](../resources/application.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8d8fe-133">示例</span><span class="sxs-lookup"><span data-stu-id="8d8fe-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d8fe-134">请求</span><span class="sxs-lookup"><span data-stu-id="8d8fe-134">Request</span></span>
<span data-ttu-id="8d8fe-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8d8fe-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```http
GET https://graph.microsoft.com/beta/applications/{id}
```
##### <a name="response"></a><span data-ttu-id="8d8fe-136">响应</span><span class="sxs-lookup"><span data-stu-id="8d8fe-136">Response</span></span>
<span data-ttu-id="8d8fe-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8d8fe-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1044

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
