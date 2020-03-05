---
title: 列出应用程序
description: 检索与 connectorGroup 相关联的 application 对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 350bc05c94bf177a350ee681e83cc16323f26046
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437467"
---
# <a name="list-applications"></a><span data-ttu-id="bb402-103">列出应用程序</span><span class="sxs-lookup"><span data-stu-id="bb402-103">List applications</span></span>

<span data-ttu-id="bb402-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="bb402-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb402-105">检索与 connectorGroup 相关联的 application 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="bb402-105">Retrieve a list of application objects associated with the connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb402-106">权限</span><span class="sxs-lookup"><span data-stu-id="bb402-106">Permissions</span></span>
<span data-ttu-id="bb402-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb402-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb402-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb402-109">Permission type</span></span>      | <span data-ttu-id="bb402-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb402-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb402-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb402-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bb402-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bb402-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bb402-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb402-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb402-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb402-114">Not supported.</span></span>    |
|<span data-ttu-id="bb402-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb402-115">Application</span></span> | <span data-ttu-id="bb402-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb402-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb402-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb402-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups/{id}/applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bb402-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bb402-118">Optional query parameters</span></span>
<span data-ttu-id="bb402-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bb402-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb402-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb402-120">Request headers</span></span>
| <span data-ttu-id="bb402-121">名称</span><span class="sxs-lookup"><span data-stu-id="bb402-121">Name</span></span>      |<span data-ttu-id="bb402-122">说明</span><span class="sxs-lookup"><span data-stu-id="bb402-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bb402-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb402-123">Authorization</span></span>  | <span data-ttu-id="bb402-124">负载.</span><span class="sxs-lookup"><span data-stu-id="bb402-124">Bearer.</span></span> <span data-ttu-id="bb402-125">必需</span><span class="sxs-lookup"><span data-stu-id="bb402-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb402-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb402-126">Request body</span></span>
<span data-ttu-id="bb402-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb402-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb402-128">响应</span><span class="sxs-lookup"><span data-stu-id="bb402-128">Response</span></span>

<span data-ttu-id="bb402-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[application](../resources/application.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="bb402-129">If successful, this method returns a `200 OK` response code and collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb402-130">示例</span><span class="sxs-lookup"><span data-stu-id="bb402-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb402-131">请求</span><span class="sxs-lookup"><span data-stu-id="bb402-131">Request</span></span>
<span data-ttu-id="bb402-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bb402-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applications"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
```
##### <a name="response"></a><span data-ttu-id="bb402-133">响应</span><span class="sxs-lookup"><span data-stu-id="bb402-133">Response</span></span>
<span data-ttu-id="bb402-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb402-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 420

{
  "value": [
    {
      "appId": "appId-value",
      "onPremisesPublishing": {
        "externalUrl": "externalUrl-value",
        "internalUrl": "internalUrl-value",
        "externalAuthenticationType": "externalAuthenticationType-value",
        "customDomainCertificate": "customDomainCertificate-value",
        "isTranslateHostHeaderEnabled": true,
        "isOnPremPublishingEnabled": true
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
