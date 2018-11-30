---
title: 获取应用程序
description: 检索的属性和 application 对象的关系。
ms.openlocfilehash: 0ba50fa0a3fec2c1f9a6adce828e845f0c4d3b2d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044253"
---
# <a name="get-application"></a><span data-ttu-id="3ccd2-103">获取应用程序</span><span class="sxs-lookup"><span data-stu-id="3ccd2-103">Get Application</span></span>

> <span data-ttu-id="3ccd2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3ccd2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ccd2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3ccd2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3ccd2-106">检索的属性和 application 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="3ccd2-106">Retrieve the properties and relationships of application object.</span></span>
## <a name="permissions"></a><span data-ttu-id="3ccd2-107">权限</span><span class="sxs-lookup"><span data-stu-id="3ccd2-107">Permissions</span></span>
<span data-ttu-id="3ccd2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ccd2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ccd2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ccd2-110">Permission type</span></span>      | <span data-ttu-id="3ccd2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ccd2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ccd2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ccd2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3ccd2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ccd2-113">Not supported.</span></span>    |
|<span data-ttu-id="3ccd2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ccd2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ccd2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ccd2-115">Not supported.</span></span>    |
|<span data-ttu-id="3ccd2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ccd2-116">Application</span></span> | <span data-ttu-id="3ccd2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ccd2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ccd2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ccd2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /workbook/application
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3ccd2-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3ccd2-119">Optional query parameters</span></span>
<span data-ttu-id="3ccd2-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3ccd2-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ccd2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ccd2-121">Request headers</span></span>
| <span data-ttu-id="3ccd2-122">名称</span><span class="sxs-lookup"><span data-stu-id="3ccd2-122">Name</span></span>      |<span data-ttu-id="3ccd2-123">说明</span><span class="sxs-lookup"><span data-stu-id="3ccd2-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3ccd2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ccd2-124">Authorization</span></span>  | <span data-ttu-id="3ccd2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ccd2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ccd2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ccd2-127">Request body</span></span>
<span data-ttu-id="3ccd2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3ccd2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ccd2-129">响应</span><span class="sxs-lookup"><span data-stu-id="3ccd2-129">Response</span></span>

<span data-ttu-id="3ccd2-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[应用程序](../resources/application.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3ccd2-130">If successful, this method returns a `200 OK` response code and [Application](../resources/application.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3ccd2-131">示例</span><span class="sxs-lookup"><span data-stu-id="3ccd2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ccd2-132">请求</span><span class="sxs-lookup"><span data-stu-id="3ccd2-132">Request</span></span>
<span data-ttu-id="3ccd2-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ccd2-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```http
GET https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/application
```
##### <a name="response"></a><span data-ttu-id="3ccd2-134">响应</span><span class="sxs-lookup"><span data-stu-id="3ccd2-134">Response</span></span>
<span data-ttu-id="3ccd2-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3ccd2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 48

{
  "calculationMode": "calculationMode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Application",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->