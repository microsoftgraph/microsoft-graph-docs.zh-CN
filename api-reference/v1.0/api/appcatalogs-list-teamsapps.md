---
title: 列出 teamsApp
description: 列出租户应用程序目录中发布的团队应用。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fa54d1ac1eec5dfc0a6995f85ced9f46fa8d47ae
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607339"
---
# <a name="list-teamsapp"></a><span data-ttu-id="fa4eb-103">列出 teamsApp</span><span class="sxs-lookup"><span data-stu-id="fa4eb-103">List teamsApp</span></span>

<span data-ttu-id="fa4eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa4eb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fa4eb-105">列出在 Microsoft 团队应用程序目录中发布的 [应用程序](../resources/teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-105">List [apps](../resources/teamsapp.md) published in the Microsoft Teams app catalog.</span></span> <span data-ttu-id="fa4eb-106">这包括 Microsoft 团队存储中的应用程序，以及组织的应用程序目录 (租户应用程序目录) 中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="fa4eb-107">若要仅从组织的应用程序目录中获取应用程序，请 `organization` 在请求中将 **distributionMethod** 指定为 ""。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa4eb-108">权限</span><span class="sxs-lookup"><span data-stu-id="fa4eb-108">Permissions</span></span>

<span data-ttu-id="fa4eb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="fa4eb-111">**注意：** 只有全局管理员才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="fa4eb-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa4eb-112">Permission Type</span></span>                        | <span data-ttu-id="fa4eb-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa4eb-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="fa4eb-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa4eb-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa4eb-115">AppCatalog、AppCatalog、所有的、所有读写的。 all</span><span class="sxs-lookup"><span data-stu-id="fa4eb-115">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="fa4eb-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa4eb-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa4eb-117">不支持</span><span class="sxs-lookup"><span data-stu-id="fa4eb-117">Not supported</span></span>                       |
| <span data-ttu-id="fa4eb-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa4eb-118">Application</span></span>                            | <span data-ttu-id="fa4eb-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa4eb-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa4eb-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa4eb-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fa4eb-121">Optional query parameters</span></span>

<span data-ttu-id="fa4eb-122">此方法支持使用 `$filter`、`$select` 和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="fa4eb-123">使用 `$expand=AppDefinitions` 将返回有关应用状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-123">Using `$expand=AppDefinitions` will return more information about the state of the app.</span></span> 

> <span data-ttu-id="fa4eb-124">**注意：** 您可以对 [teamsApp](../resources/teamsapp.md) 对象的任何字段进行筛选，以缩短结果列表。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-124">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="fa4eb-125">您可以使用以下任何筛选器操作：等于、不等于、和、或，而不是。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-125">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa4eb-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa4eb-126">Request headers</span></span>

| <span data-ttu-id="fa4eb-127">标头</span><span class="sxs-lookup"><span data-stu-id="fa4eb-127">Header</span></span>        | <span data-ttu-id="fa4eb-128">值</span><span class="sxs-lookup"><span data-stu-id="fa4eb-128">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="fa4eb-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa4eb-129">Authorization</span></span> | <span data-ttu-id="fa4eb-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa4eb-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa4eb-132">Request body</span></span>

<span data-ttu-id="fa4eb-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa4eb-134">响应</span><span class="sxs-lookup"><span data-stu-id="fa4eb-134">Response</span></span>

<span data-ttu-id="fa4eb-135">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [teamsApp](../resources/teamsapp.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-135">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa4eb-136">示例</span><span class="sxs-lookup"><span data-stu-id="fa4eb-136">Examples</span></span>

### <a name="example-1-list-all-applications-specific-to-the-tenant"></a><span data-ttu-id="fa4eb-137">示例1：列出特定于租户的所有应用程序</span><span class="sxs-lookup"><span data-stu-id="fa4eb-137">Example 1: List all applications specific to the tenant</span></span>

<span data-ttu-id="fa4eb-138">下面的示例列出了特定于您的租户的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-138">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="fa4eb-139">请求</span><span class="sxs-lookup"><span data-stu-id="fa4eb-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapps_filter_distributionMethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```



<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="fa4eb-140">响应</span><span class="sxs-lookup"><span data-stu-id="fa4eb-140">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="fa4eb-141">示例2：列出具有给定 ID 的应用程序</span><span class="sxs-lookup"><span data-stu-id="fa4eb-141">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="fa4eb-142">下面的示例列出了具有给定 ID 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-142">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="fa4eb-143">请求</span><span class="sxs-lookup"><span data-stu-id="fa4eb-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_id"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="fa4eb-144">响应</span><span class="sxs-lookup"><span data-stu-id="fa4eb-144">Response</span></span>

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
### <a name="example-3-find-application-based-on-the-teams-app-manifest-id"></a><span data-ttu-id="fa4eb-145">示例3：基于团队应用程序清单 ID 查找应用程序。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-145">Example 3: Find application based on the Teams app manifest ID.</span></span>

<span data-ttu-id="fa4eb-146">下面的示例列出与团队应用程序清单中指定的 "id" 匹配的应用程序。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-146">The following example lists applications that match the 'id' specified in the Teams app manifest.</span></span> <span data-ttu-id="fa4eb-147">在此示例中，团队应用程序的清单 ID 为 "cf1ba4c7-f94e-4d80-ba90-5594b641a8ee"。</span><span class="sxs-lookup"><span data-stu-id="fa4eb-147">In the example, the manifest ID of the Teams app is 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span></span>

#### <a name="request"></a><span data-ttu-id="fa4eb-148">请求</span><span class="sxs-lookup"><span data-stu-id="fa4eb-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_externalid"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```

#### <a name="response"></a><span data-ttu-id="fa4eb-149">响应</span><span class="sxs-lookup"><span data-stu-id="fa4eb-149">Response</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appCatalogs/teamsApps",
    "value": [
        {
            "id": "22f73bbe-f67a-4dea-bd54-54cac718cb2b",
            "externalId": "cf1ba4c7-f94e-4d80-ba90-5594b641a8ee",
            "displayName": "YPA",
            "distributionMethod": "organization"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="fa4eb-150">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fa4eb-150">See also</span></span>

- [<span data-ttu-id="fa4eb-151">列出团队中安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="fa4eb-151">List apps installed in a team</span></span>](team-list-installedapps.md)
- [<span data-ttu-id="fa4eb-152">列出在用户的个人范围内安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="fa4eb-152">List apps installed in the personal scope of a user</span></span>](userteamwork-list-installedapps.md)

