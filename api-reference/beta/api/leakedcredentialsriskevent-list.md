---
title: 列表 leakedCredentialsRiskEvents
description: 检索 leakedcredentialsriskevent 对象的列表。
localization_priority: Normal
ms.openlocfilehash: ad34b75117c33014f76464ed85d5f4a644d1de8e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511686"
---
# <a name="list-leakedcredentialsriskevents"></a><span data-ttu-id="46afd-103">列表 leakedCredentialsRiskEvents</span><span class="sxs-lookup"><span data-stu-id="46afd-103">List leakedCredentialsRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46afd-104">检索 leakedcredentialsriskevent 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="46afd-104">Retrieve a list of leakedcredentialsriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="46afd-105">权限</span><span class="sxs-lookup"><span data-stu-id="46afd-105">Permissions</span></span>
<span data-ttu-id="46afd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46afd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46afd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="46afd-108">Permission type</span></span>      | <span data-ttu-id="46afd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46afd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46afd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46afd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="46afd-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="46afd-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="46afd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46afd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46afd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="46afd-113">Not supported.</span></span>    |
|<span data-ttu-id="46afd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="46afd-114">Application</span></span> | <span data-ttu-id="46afd-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="46afd-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46afd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46afd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="46afd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="46afd-117">Request headers</span></span>
| <span data-ttu-id="46afd-118">名称</span><span class="sxs-lookup"><span data-stu-id="46afd-118">Name</span></span>      |<span data-ttu-id="46afd-119">说明</span><span class="sxs-lookup"><span data-stu-id="46afd-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="46afd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="46afd-120">Authorization</span></span>  | <span data-ttu-id="46afd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46afd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46afd-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="46afd-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="46afd-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="46afd-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46afd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="46afd-126">Request body</span></span>
<span data-ttu-id="46afd-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="46afd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46afd-128">响应</span><span class="sxs-lookup"><span data-stu-id="46afd-128">Response</span></span>

<span data-ttu-id="46afd-129">如果成功，此方法返回`200 OK`响应代码和响应正文中的[leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="46afd-129">If successful, this method returns a `200 OK` response code and collection of [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="46afd-130">示例</span><span class="sxs-lookup"><span data-stu-id="46afd-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46afd-131">请求</span><span class="sxs-lookup"><span data-stu-id="46afd-131">Request</span></span>
<span data-ttu-id="46afd-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46afd-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents
```
##### <a name="response"></a><span data-ttu-id="46afd-133">响应</span><span class="sxs-lookup"><span data-stu-id="46afd-133">Response</span></span>
<span data-ttu-id="46afd-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="46afd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "value":
  [
    {
      "closedDateTime": null,
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "active",
      "riskLevel": "high",
      "riskType": "LeakedCredentialsRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "278dc452-4163-dbc6-84eb-a050c37fc931",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List leakedCredentialsRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/leakedcredentialsriskevent-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
