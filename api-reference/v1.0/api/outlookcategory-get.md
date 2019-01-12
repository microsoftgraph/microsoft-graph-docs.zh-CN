---
title: 获取 Outlook category
description: 获取指定的 outlookCategory 对象的属性和关系。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4359c3bd87a5eecc3d8b153538b15039ab8be7c6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934903"
---
# <a name="get-outlook-category"></a><span data-ttu-id="35fc6-103">获取 Outlook category</span><span class="sxs-lookup"><span data-stu-id="35fc6-103">Get Outlook category</span></span>


<span data-ttu-id="35fc6-104">获取指定的 [outlookCategory](../resources/outlookcategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="35fc6-104">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="35fc6-105">权限</span><span class="sxs-lookup"><span data-stu-id="35fc6-105">Permissions</span></span>
<span data-ttu-id="35fc6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35fc6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35fc6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="35fc6-108">Permission type</span></span>      | <span data-ttu-id="35fc6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="35fc6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35fc6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35fc6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="35fc6-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="35fc6-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="35fc6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35fc6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35fc6-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="35fc6-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="35fc6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="35fc6-114">Application</span></span> | <span data-ttu-id="35fc6-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="35fc6-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="35fc6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35fc6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="35fc6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="35fc6-117">Optional query parameters</span></span>
<span data-ttu-id="35fc6-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="35fc6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35fc6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="35fc6-119">Request headers</span></span>
| <span data-ttu-id="35fc6-120">名称</span><span class="sxs-lookup"><span data-stu-id="35fc6-120">Name</span></span>      |<span data-ttu-id="35fc6-121">说明</span><span class="sxs-lookup"><span data-stu-id="35fc6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="35fc6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="35fc6-122">Authorization</span></span>  | <span data-ttu-id="35fc6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="35fc6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35fc6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="35fc6-125">Request body</span></span>
<span data-ttu-id="35fc6-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="35fc6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35fc6-127">响应</span><span class="sxs-lookup"><span data-stu-id="35fc6-127">Response</span></span>

<span data-ttu-id="35fc6-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [outlookCategory](../resources/outlookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="35fc6-128">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="35fc6-129">示例</span><span class="sxs-lookup"><span data-stu-id="35fc6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35fc6-130">请求</span><span class="sxs-lookup"><span data-stu-id="35fc6-130">Request</span></span>
<span data-ttu-id="35fc6-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="35fc6-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["de912e4d-c790-4da9-949c-ccd933aaa0f7"],
  "name": "get_outlookcategory"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7
```
##### <a name="response"></a><span data-ttu-id="35fc6-132">响应</span><span class="sxs-lookup"><span data-stu-id="35fc6-132">Response</span></span>
<span data-ttu-id="35fc6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="35fc6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 249

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
  "displayName":"Yellow category",
  "color":"preset3"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
