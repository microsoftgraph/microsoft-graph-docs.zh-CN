---
title: orgContact： 获取管理器
description: 获取联系人的经理
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 96833e9b38b2d988a3843e097a11fe38a247c0b6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524854"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="73539-103">orgContact： 获取管理器</span><span class="sxs-lookup"><span data-stu-id="73539-103">orgContact: Get manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73539-104">获取联系人的经理</span><span class="sxs-lookup"><span data-stu-id="73539-104">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="73539-105">权限</span><span class="sxs-lookup"><span data-stu-id="73539-105">Permissions</span></span>
<span data-ttu-id="73539-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73539-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73539-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="73539-108">Permission type</span></span>      | <span data-ttu-id="73539-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73539-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73539-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73539-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73539-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="73539-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="73539-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73539-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73539-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="73539-113">Not supported.</span></span>    |
|<span data-ttu-id="73539-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="73539-114">Application</span></span> | <span data-ttu-id="73539-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73539-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73539-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73539-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73539-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="73539-117">Optional query parameters</span></span>
<span data-ttu-id="73539-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="73539-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73539-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="73539-119">Request headers</span></span>
| <span data-ttu-id="73539-120">名称</span><span class="sxs-lookup"><span data-stu-id="73539-120">Name</span></span>       | <span data-ttu-id="73539-121">类型</span><span class="sxs-lookup"><span data-stu-id="73539-121">Type</span></span> | <span data-ttu-id="73539-122">说明</span><span class="sxs-lookup"><span data-stu-id="73539-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="73539-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="73539-123">Authorization</span></span>  | <span data-ttu-id="73539-124">string</span><span class="sxs-lookup"><span data-stu-id="73539-124">string</span></span>  | <span data-ttu-id="73539-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73539-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73539-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="73539-127">Request body</span></span>
<span data-ttu-id="73539-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73539-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73539-129">响应</span><span class="sxs-lookup"><span data-stu-id="73539-129">Response</span></span>

<span data-ttu-id="73539-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="73539-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="73539-131">示例</span><span class="sxs-lookup"><span data-stu-id="73539-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="73539-132">请求</span><span class="sxs-lookup"><span data-stu-id="73539-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```http
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```

#### <a name="response"></a><span data-ttu-id="73539-133">响应</span><span class="sxs-lookup"><span data-stu-id="73539-133">Response</span></span>

<span data-ttu-id="73539-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73539-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 455

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "24fcbca3-c3e2-48bf-9ffc-c7f81b81483d",
    "businessPhones": [
        "+1 205 555 0108"
    ],
    "displayName": "Diego Siciliani",
    "givenName": "Diego",
    "jobTitle": "CVP Finance",
    "mail": "DiegoS@contoso.com",
    "mobilePhone": null,
    "officeLocation": "14/1108",
    "preferredLanguage": "en-US",
    "surname": "Siciliani",
    "userPrincipalName": "DiegoS@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get manager",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-get-manager.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
