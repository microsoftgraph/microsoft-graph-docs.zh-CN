---
title: 团队中的列表应用程序
description: 检索指定团队中安装的应用程序的列表。
ms.openlocfilehash: 214685302b9c3a09f06cb4d5c13525c222bf658f
ms.sourcegitcommit: ba6b1d1a12dcb54916b4d3e529c856f6514e01e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/12/2018
ms.locfileid: "27241046"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="2458b-103">团队中的列表应用程序</span><span class="sxs-lookup"><span data-stu-id="2458b-103">List apps in team</span></span>



<span data-ttu-id="2458b-104">检索指定[团队](../resources/team.md)中的[应用程序安装](../resources/teamsappinstallation.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="2458b-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2458b-105">权限</span><span class="sxs-lookup"><span data-stu-id="2458b-105">Permissions</span></span>

<span data-ttu-id="2458b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2458b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2458b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2458b-108">Permission type</span></span>      | <span data-ttu-id="2458b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2458b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2458b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2458b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2458b-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2458b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2458b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2458b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2458b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2458b-113">Not supported.</span></span>    |
|<span data-ttu-id="2458b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2458b-114">Application</span></span> | <span data-ttu-id="2458b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2458b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2458b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2458b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2458b-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2458b-117">Optional query parameters</span></span>

<span data-ttu-id="2458b-118">此方法支持 $filter，$select，和 $expand [OData 查询参数](/graph/query-parameters)，以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="2458b-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2458b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2458b-119">Request headers</span></span>

| <span data-ttu-id="2458b-120">标头</span><span class="sxs-lookup"><span data-stu-id="2458b-120">Header</span></span>       | <span data-ttu-id="2458b-121">值</span><span class="sxs-lookup"><span data-stu-id="2458b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2458b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2458b-122">Authorization</span></span>  | <span data-ttu-id="2458b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2458b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2458b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2458b-125">Request body</span></span>

<span data-ttu-id="2458b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2458b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2458b-127">响应</span><span class="sxs-lookup"><span data-stu-id="2458b-127">Response</span></span>

<span data-ttu-id="2458b-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[teamsApp](../resources/teamsapp.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="2458b-128">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2458b-129">示例</span><span class="sxs-lookup"><span data-stu-id="2458b-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="2458b-130">请求</span><span class="sxs-lookup"><span data-stu-id="2458b-130">Request</span></span>

<span data-ttu-id="2458b-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2458b-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET /teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="2458b-132">响应</span><span class="sxs-lookup"><span data-stu-id="2458b-132">Response</span></span>

<span data-ttu-id="2458b-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2458b-133">The following is an example of the response.</span></span>
><span data-ttu-id="2458b-134">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2458b-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2458b-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2458b-135">All the properties will be returned from an actual call.</span></span>
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

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="2458b-136">示例--获取已安装的应用程序的名称</span><span class="sxs-lookup"><span data-stu-id="2458b-136">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="2458b-137">请求</span><span class="sxs-lookup"><span data-stu-id="2458b-137">Request</span></span>

<span data-ttu-id="2458b-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2458b-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/v1.0/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="2458b-139">响应</span><span class="sxs-lookup"><span data-stu-id="2458b-139">Response</span></span>

<span data-ttu-id="2458b-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2458b-140">The following is an example of the response.</span></span>

><span data-ttu-id="2458b-141">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2458b-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2458b-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2458b-142">All the properties will be returned from an actual call.</span></span>
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