---
title: 获取 privilegedApproval
description: 检索的属性和 privilegedapproval 对象的关系。
localization_priority: Normal
ms.openlocfilehash: c718c8d3c9382c5f8af9debf88fd6de5a55b461b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513618"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="8f3a1-103">获取 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="8f3a1-103">Get privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f3a1-104">检索的属性和 privilegedapproval 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="8f3a1-104">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8f3a1-105">权限</span><span class="sxs-lookup"><span data-stu-id="8f3a1-105">Permissions</span></span>
<span data-ttu-id="8f3a1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8f3a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8f3a1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f3a1-108">Permission type</span></span>      | <span data-ttu-id="8f3a1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8f3a1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8f3a1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f3a1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8f3a1-111">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8f3a1-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="8f3a1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f3a1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8f3a1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f3a1-113">Not supported.</span></span>    |
|<span data-ttu-id="8f3a1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f3a1-114">Application</span></span> | <span data-ttu-id="8f3a1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f3a1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8f3a1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f3a1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8f3a1-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8f3a1-117">Optional query parameters</span></span>
<span data-ttu-id="8f3a1-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8f3a1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f3a1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f3a1-119">Request headers</span></span>
| <span data-ttu-id="8f3a1-120">名称</span><span class="sxs-lookup"><span data-stu-id="8f3a1-120">Name</span></span>      |<span data-ttu-id="8f3a1-121">说明</span><span class="sxs-lookup"><span data-stu-id="8f3a1-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8f3a1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f3a1-122">Authorization</span></span>  | <span data-ttu-id="8f3a1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8f3a1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8f3a1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f3a1-125">Request body</span></span>
<span data-ttu-id="8f3a1-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8f3a1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f3a1-127">响应</span><span class="sxs-lookup"><span data-stu-id="8f3a1-127">Response</span></span>

<span data-ttu-id="8f3a1-128">如果成功，此方法返回`200 OK`响应正文中的响应代码和[privilegedApproval](../resources/privilegedapproval.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8f3a1-128">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="8f3a1-129">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="8f3a1-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="8f3a1-130">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="8f3a1-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="8f3a1-131">示例</span><span class="sxs-lookup"><span data-stu-id="8f3a1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8f3a1-132">请求</span><span class="sxs-lookup"><span data-stu-id="8f3a1-132">Request</span></span>
<span data-ttu-id="8f3a1-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f3a1-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/<id>
```
##### <a name="response"></a><span data-ttu-id="8f3a1-134">响应</span><span class="sxs-lookup"><span data-stu-id="8f3a1-134">Response</span></span>
<span data-ttu-id="8f3a1-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f3a1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
