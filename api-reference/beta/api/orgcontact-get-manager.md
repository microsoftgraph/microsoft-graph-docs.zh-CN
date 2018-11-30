---
title: orgContact： 获取管理器
description: 获取联系人的经理
ms.openlocfilehash: 7fe4c61422eb83bb4501fbb521f301ec6f9afaa5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042629"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="303af-103">orgContact： 获取管理器</span><span class="sxs-lookup"><span data-stu-id="303af-103">orgContact: Get manager</span></span>

> <span data-ttu-id="303af-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="303af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="303af-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="303af-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="303af-106">获取联系人的经理</span><span class="sxs-lookup"><span data-stu-id="303af-106">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="303af-107">权限</span><span class="sxs-lookup"><span data-stu-id="303af-107">Permissions</span></span>
<span data-ttu-id="303af-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="303af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="303af-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="303af-110">Permission type</span></span>      | <span data-ttu-id="303af-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="303af-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="303af-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="303af-112">Delegated (work or school account)</span></span> | <span data-ttu-id="303af-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="303af-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="303af-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="303af-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="303af-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="303af-115">Not supported.</span></span>    |
|<span data-ttu-id="303af-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="303af-116">Application</span></span> | <span data-ttu-id="303af-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="303af-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="303af-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="303af-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="303af-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="303af-119">Optional query parameters</span></span>
<span data-ttu-id="303af-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="303af-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="303af-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="303af-121">Request headers</span></span>
| <span data-ttu-id="303af-122">名称</span><span class="sxs-lookup"><span data-stu-id="303af-122">Name</span></span>       | <span data-ttu-id="303af-123">类型</span><span class="sxs-lookup"><span data-stu-id="303af-123">Type</span></span> | <span data-ttu-id="303af-124">说明</span><span class="sxs-lookup"><span data-stu-id="303af-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="303af-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="303af-125">Authorization</span></span>  | <span data-ttu-id="303af-126">string</span><span class="sxs-lookup"><span data-stu-id="303af-126">string</span></span>  | <span data-ttu-id="303af-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="303af-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="303af-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="303af-129">Request body</span></span>
<span data-ttu-id="303af-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="303af-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="303af-131">响应</span><span class="sxs-lookup"><span data-stu-id="303af-131">Response</span></span>

<span data-ttu-id="303af-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="303af-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="303af-133">示例</span><span class="sxs-lookup"><span data-stu-id="303af-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="303af-134">请求</span><span class="sxs-lookup"><span data-stu-id="303af-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```http
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```

#### <a name="response"></a><span data-ttu-id="303af-135">响应</span><span class="sxs-lookup"><span data-stu-id="303af-135">Response</span></span>

<span data-ttu-id="303af-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="303af-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get manager",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->