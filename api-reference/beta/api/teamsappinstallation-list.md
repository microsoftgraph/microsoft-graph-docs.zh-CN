---
title: 团队中的列表应用程序
description: 检索指定团队中安装的应用程序的列表。
ms.openlocfilehash: 27161394b6f3376d826aa0e156600459c15c0dd1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043057"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="c992f-103">团队中的列表应用程序</span><span class="sxs-lookup"><span data-stu-id="c992f-103">List apps in team</span></span>

> <span data-ttu-id="c992f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c992f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c992f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c992f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c992f-106">检索指定[团队](../resources/team.md)中的[应用程序安装](../resources/teamsappinstallation.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="c992f-106">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c992f-107">权限</span><span class="sxs-lookup"><span data-stu-id="c992f-107">Permissions</span></span>

<span data-ttu-id="c992f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c992f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c992f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c992f-110">Permission type</span></span>      | <span data-ttu-id="c992f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c992f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c992f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c992f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c992f-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c992f-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c992f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c992f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c992f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c992f-115">Not supported.</span></span>    |
|<span data-ttu-id="c992f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c992f-116">Application</span></span> | <span data-ttu-id="c992f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c992f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c992f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c992f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c992f-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c992f-119">Optional query parameters</span></span>

<span data-ttu-id="c992f-120">此方法支持 $filter，$select，和 $expand [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="c992f-120">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c992f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c992f-121">Request headers</span></span>

| <span data-ttu-id="c992f-122">标头</span><span class="sxs-lookup"><span data-stu-id="c992f-122">Header</span></span>       | <span data-ttu-id="c992f-123">值</span><span class="sxs-lookup"><span data-stu-id="c992f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c992f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c992f-124">Authorization</span></span>  | <span data-ttu-id="c992f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c992f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c992f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c992f-127">Request body</span></span>

<span data-ttu-id="c992f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c992f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c992f-129">响应</span><span class="sxs-lookup"><span data-stu-id="c992f-129">Response</span></span>

<span data-ttu-id="c992f-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[teamsApp](../resources/teamsapp.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c992f-130">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c992f-131">示例</span><span class="sxs-lookup"><span data-stu-id="c992f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c992f-132">请求</span><span class="sxs-lookup"><span data-stu-id="c992f-132">Request</span></span>

<span data-ttu-id="c992f-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c992f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="c992f-134">响应</span><span class="sxs-lookup"><span data-stu-id="c992f-134">Response</span></span>

<span data-ttu-id="c992f-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c992f-135">The following is an example of the response.</span></span>
><span data-ttu-id="c992f-136">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c992f-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c992f-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c992f-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="c992f-138">示例--获取已安装的应用程序的名称</span><span class="sxs-lookup"><span data-stu-id="c992f-138">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="c992f-139">请求</span><span class="sxs-lookup"><span data-stu-id="c992f-139">Request</span></span>

<span data-ttu-id="c992f-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c992f-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="c992f-141">响应</span><span class="sxs-lookup"><span data-stu-id="c992f-141">Response</span></span>

<span data-ttu-id="c992f-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c992f-142">The following is an example of the response.</span></span>

><span data-ttu-id="c992f-143">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c992f-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c992f-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c992f-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
    "value": [
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "displayName": "OneNote",
                "version": "1.0.0"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZmQ5MjVhMC0zNTdmLTRkMjUtODQ1Ni1iMzAyMmFhYTQxYTk=",
            "teamsAppDefinition": {
                "id": "MGZkOTI1YTAtMzU3Zi00ZDI1LTg0NTYtYjMwMjJhYWE0MWE5IyMxLjc=",
                "teamsAppId": "0fd925a0-357f-4d25-8456-b3022aaa41a9",
                "displayName": "SurveyMonkey",
                "version": "1.7"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMyYTUyNzcwMy0xZjZmLTQ1NTktYTMzMi1kOGE3ZDI4OGNkODg=",
            "teamsAppDefinition": {
                "id": "MmE1Mjc3MDMtMWY2Zi00NTU5LWEzMzItZDhhN2QyODhjZDg4IyMxLjA=",
                "teamsAppId": "2a527703-1f6f-4559-a332-d8a7d288cd88",
                "displayName": "SharePoint",
                "version": "1.0"
            }
        }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->