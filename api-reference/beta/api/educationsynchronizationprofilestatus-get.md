---
title: 获取 educationSynchronizationProfile 的状态
description: 获取租户中特定学校数据同步配置文件的状态。 该响应将指示同步的状态。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7bb155d8774ad74f760ed62d94d5f44bb1d07d03
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042938"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="444b8-104">获取 educationSynchronizationProfile 的状态</span><span class="sxs-lookup"><span data-stu-id="444b8-104">Get the status of an educationSynchronizationProfile</span></span>

<span data-ttu-id="444b8-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="444b8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="444b8-106">获取租户中特定学校数据 [同步配置文件](../resources/educationsynchronizationprofile.md) 的状态。</span><span class="sxs-lookup"><span data-stu-id="444b8-106">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="444b8-107">该响应将指示同步的状态。</span><span class="sxs-lookup"><span data-stu-id="444b8-107">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="444b8-108">权限</span><span class="sxs-lookup"><span data-stu-id="444b8-108">Permissions</span></span>

<span data-ttu-id="444b8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="444b8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="444b8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="444b8-111">Permission type</span></span>                       | <span data-ttu-id="444b8-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="444b8-112">Permissions (from least to most privileged)</span></span>                 |
| :------------------------------------ | :---------------------------------------------------------- |
| <span data-ttu-id="444b8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="444b8-113">Delegated (work or school account)</span></span>    | <span data-ttu-id="444b8-114">EduAdministration.Read、EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="444b8-114">EduAdministration.Read, EduAdministration.ReadWrite</span></span>         |
| <span data-ttu-id="444b8-115">委派 (个人 Microsoft 帐户</span><span class="sxs-lookup"><span data-stu-id="444b8-115">Delegated (personal Microsoft account</span></span> | <span data-ttu-id="444b8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="444b8-116">Not supported.</span></span>                                              |
| <span data-ttu-id="444b8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="444b8-117">Application</span></span>                           | <span data-ttu-id="444b8-118">EduAdministration.Read.All、EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="444b8-118">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="444b8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="444b8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="444b8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="444b8-120">Request headers</span></span>

| <span data-ttu-id="444b8-121">名称</span><span class="sxs-lookup"><span data-stu-id="444b8-121">Name</span></span>          | <span data-ttu-id="444b8-122">类型</span><span class="sxs-lookup"><span data-stu-id="444b8-122">Type</span></span>   | <span data-ttu-id="444b8-123">说明</span><span class="sxs-lookup"><span data-stu-id="444b8-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="444b8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="444b8-124">Authorization</span></span> | <span data-ttu-id="444b8-125">string</span><span class="sxs-lookup"><span data-stu-id="444b8-125">string</span></span> | <span data-ttu-id="444b8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="444b8-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="444b8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="444b8-128">Request body</span></span>

<span data-ttu-id="444b8-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="444b8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="444b8-130">响应</span><span class="sxs-lookup"><span data-stu-id="444b8-130">Response</span></span>

<span data-ttu-id="444b8-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="444b8-131">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="444b8-132">示例</span><span class="sxs-lookup"><span data-stu-id="444b8-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="444b8-133">请求</span><span class="sxs-lookup"><span data-stu-id="444b8-133">Request</span></span>

<span data-ttu-id="444b8-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="444b8-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="444b8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="444b8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```
# <a name="c"></a>[<span data-ttu-id="444b8-136">C#</span><span class="sxs-lookup"><span data-stu-id="444b8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-status-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="444b8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="444b8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-status-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="444b8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="444b8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-status-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="444b8-139">Java</span><span class="sxs-lookup"><span data-stu-id="444b8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-status-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="444b8-140">响应</span><span class="sxs-lookup"><span data-stu-id="444b8-140">Response</span></span>

<span data-ttu-id="444b8-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="444b8-141">The following is an example of the response.</span></span>

> <span data-ttu-id="444b8-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="444b8-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/profileStatus/$entity",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
    "status": "inProgress",
    "lastSynchronizationDateTime": "2017-07-04T22:06:37.6472621Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


