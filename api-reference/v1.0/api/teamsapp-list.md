---
title: 列出 teamsApp
description: 列出租户应用程序目录中发布的团队应用。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 613011ce44b05b1743a8d297fc63450d4eed7dee
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790740"
---
# <a name="list-teamsapp"></a><span data-ttu-id="b26d5-103">列出 teamsApp</span><span class="sxs-lookup"><span data-stu-id="b26d5-103">List teamsApp</span></span>

<span data-ttu-id="b26d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b26d5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b26d5-105">列出在 Microsoft 团队应用程序目录中发布的 [应用程序](../resources/teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="b26d5-105">List [apps](../resources/teamsapp.md) published in the Microsoft Teams app catalog.</span></span> <span data-ttu-id="b26d5-106">这包括 Microsoft 团队存储中的应用程序，以及组织的应用程序目录 (租户应用程序目录) 中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="b26d5-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="b26d5-107">若要仅从组织的应用程序目录中获取应用程序，请 `organization` 在请求中将 **distributionMethod** 指定为 ""。</span><span class="sxs-lookup"><span data-stu-id="b26d5-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="b26d5-108">权限</span><span class="sxs-lookup"><span data-stu-id="b26d5-108">Permissions</span></span>

<span data-ttu-id="b26d5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b26d5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="b26d5-111">**注意：** 只有全局管理员才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b26d5-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="b26d5-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="b26d5-112">Permission Type</span></span>                        | <span data-ttu-id="b26d5-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b26d5-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="b26d5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b26d5-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="b26d5-115">AppCatalog、AppCatalog、所有的、所有读写的。 all</span><span class="sxs-lookup"><span data-stu-id="b26d5-115">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="b26d5-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b26d5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b26d5-117">不支持</span><span class="sxs-lookup"><span data-stu-id="b26d5-117">Not supported</span></span>                       |
| <span data-ttu-id="b26d5-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b26d5-118">Application</span></span>                            | <span data-ttu-id="b26d5-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b26d5-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b26d5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b26d5-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b26d5-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b26d5-121">Optional query parameters</span></span>

<span data-ttu-id="b26d5-122">此方法支持使用 `$filter`、`$select` 和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b26d5-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

> <span data-ttu-id="b26d5-123">**注意：** 您可以对 [teamsApp](../resources/teamsapp.md) 对象的任何字段进行筛选，以缩短结果列表。</span><span class="sxs-lookup"><span data-stu-id="b26d5-123">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="b26d5-124">您可以使用以下任何筛选器操作：等于、不等于、和、或，而不是。</span><span class="sxs-lookup"><span data-stu-id="b26d5-124">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b26d5-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="b26d5-125">Request headers</span></span>

| <span data-ttu-id="b26d5-126">标头</span><span class="sxs-lookup"><span data-stu-id="b26d5-126">Header</span></span>        | <span data-ttu-id="b26d5-127">值</span><span class="sxs-lookup"><span data-stu-id="b26d5-127">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="b26d5-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b26d5-128">Authorization</span></span> | <span data-ttu-id="b26d5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b26d5-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b26d5-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="b26d5-131">Request body</span></span>

<span data-ttu-id="b26d5-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b26d5-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b26d5-133">响应</span><span class="sxs-lookup"><span data-stu-id="b26d5-133">Response</span></span>

<span data-ttu-id="b26d5-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [teamsApp](../resources/teamsapp.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="b26d5-134">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b26d5-135">示例</span><span class="sxs-lookup"><span data-stu-id="b26d5-135">Examples</span></span>

### <a name="example-1-list-all-applications-in-your-tenant"></a><span data-ttu-id="b26d5-136">示例1：列出租户中的所有应用程序</span><span class="sxs-lookup"><span data-stu-id="b26d5-136">Example 1: List all applications in your tenant</span></span>

<span data-ttu-id="b26d5-137">下面的示例列出了特定于您的租户的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="b26d5-137">The following example lists all apps that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="b26d5-138">请求</span><span class="sxs-lookup"><span data-stu-id="b26d5-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApp?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="b26d5-139">响应</span><span class="sxs-lookup"><span data-stu-id="b26d5-139">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="b26d5-140">示例2：列出具有给定 ID 的应用程序</span><span class="sxs-lookup"><span data-stu-id="b26d5-140">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="b26d5-141">下面的示例列出了具有给定 ID 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="b26d5-141">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="b26d5-142">请求</span><span class="sxs-lookup"><span data-stu-id="b26d5-142">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="b26d5-143">响应</span><span class="sxs-lookup"><span data-stu-id="b26d5-143">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```
