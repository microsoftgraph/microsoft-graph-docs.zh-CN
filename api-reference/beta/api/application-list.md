---
title: 列出应用程序
description: 检索该组织中应用程序的列表。
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 802bf9197ad7574dbf2480fb7c0631e3fd212d9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459001"
---
# <a name="list-applications"></a><span data-ttu-id="c0898-103">列出应用程序</span><span class="sxs-lookup"><span data-stu-id="c0898-103">List applications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0898-104">检索该组织中应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="c0898-104">Retrieve the list of applications in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0898-105">权限</span><span class="sxs-lookup"><span data-stu-id="c0898-105">Permissions</span></span>
<span data-ttu-id="c0898-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0898-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c0898-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0898-108">Permission type</span></span>      | <span data-ttu-id="c0898-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0898-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0898-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0898-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c0898-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c0898-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c0898-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0898-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0898-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0898-113">Not supported.</span></span>    |
|<span data-ttu-id="c0898-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0898-114">Application</span></span> | <span data-ttu-id="c0898-115">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0898-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0898-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0898-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c0898-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c0898-117">Optional query parameters</span></span>
<span data-ttu-id="c0898-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c0898-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0898-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0898-119">Request headers</span></span>
| <span data-ttu-id="c0898-120">名称</span><span class="sxs-lookup"><span data-stu-id="c0898-120">Name</span></span>       | <span data-ttu-id="c0898-121">类型</span><span class="sxs-lookup"><span data-stu-id="c0898-121">Type</span></span> | <span data-ttu-id="c0898-122">说明</span><span class="sxs-lookup"><span data-stu-id="c0898-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c0898-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0898-123">Authorization</span></span>  | <span data-ttu-id="c0898-124">string</span><span class="sxs-lookup"><span data-stu-id="c0898-124">string</span></span>  | <span data-ttu-id="c0898-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c0898-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0898-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0898-127">Request body</span></span>
<span data-ttu-id="c0898-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c0898-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0898-129">响应</span><span class="sxs-lookup"><span data-stu-id="c0898-129">Response</span></span>

<span data-ttu-id="c0898-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [application](../resources/application.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c0898-130">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0898-131">示例</span><span class="sxs-lookup"><span data-stu-id="c0898-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0898-132">请求</span><span class="sxs-lookup"><span data-stu-id="c0898-132">Request</span></span>
<span data-ttu-id="c0898-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c0898-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```http
GET https://graph.microsoft.com/beta/applications
```
##### <a name="response"></a><span data-ttu-id="c0898-134">响应</span><span class="sxs-lookup"><span data-stu-id="c0898-134">Response</span></span>
<span data-ttu-id="c0898-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c0898-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
