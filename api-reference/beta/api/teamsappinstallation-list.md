---
title: 列出团队中的应用
description: 检索在指定团队中安装的应用程序的列表。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 749a0c0e0c3a93b54487d9dea8823ad59a2658fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544568"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="f14ea-103">列出团队中的应用</span><span class="sxs-lookup"><span data-stu-id="f14ea-103">List apps in team</span></span>



<span data-ttu-id="f14ea-104">检索在指定[团队](../resources/team.md)中[安装的应用程序](../resources/teamsappinstallation.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="f14ea-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f14ea-105">权限</span><span class="sxs-lookup"><span data-stu-id="f14ea-105">Permissions</span></span>

<span data-ttu-id="f14ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f14ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f14ea-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f14ea-108">Permission type</span></span>      | <span data-ttu-id="f14ea-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f14ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f14ea-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f14ea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f14ea-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f14ea-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f14ea-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f14ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f14ea-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f14ea-113">Not supported.</span></span>    |
|<span data-ttu-id="f14ea-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f14ea-114">Application</span></span> | <span data-ttu-id="f14ea-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f14ea-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="f14ea-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f14ea-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f14ea-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f14ea-117">Optional query parameters</span></span>

<span data-ttu-id="f14ea-118">此方法支持 $filter、$select 和 $expand [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f14ea-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f14ea-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f14ea-119">Request headers</span></span>

| <span data-ttu-id="f14ea-120">标头</span><span class="sxs-lookup"><span data-stu-id="f14ea-120">Header</span></span>       | <span data-ttu-id="f14ea-121">值</span><span class="sxs-lookup"><span data-stu-id="f14ea-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f14ea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f14ea-122">Authorization</span></span>  | <span data-ttu-id="f14ea-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f14ea-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f14ea-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f14ea-125">Request body</span></span>

<span data-ttu-id="f14ea-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f14ea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f14ea-127">响应</span><span class="sxs-lookup"><span data-stu-id="f14ea-127">Response</span></span>

<span data-ttu-id="f14ea-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[teamsApp](../resources/teamsapp.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="f14ea-128">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f14ea-129">示例</span><span class="sxs-lookup"><span data-stu-id="f14ea-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="f14ea-130">请求</span><span class="sxs-lookup"><span data-stu-id="f14ea-130">Request</span></span>

<span data-ttu-id="f14ea-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f14ea-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET /teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="f14ea-132">响应</span><span class="sxs-lookup"><span data-stu-id="f14ea-132">Response</span></span>

<span data-ttu-id="f14ea-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f14ea-133">The following is an example of the response.</span></span>
><span data-ttu-id="f14ea-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f14ea-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f14ea-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f14ea-135">All the properties will be returned from an actual call.</span></span>
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

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="f14ea-136">示例--获取已安装应用程序的名称</span><span class="sxs-lookup"><span data-stu-id="f14ea-136">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="f14ea-137">请求</span><span class="sxs-lookup"><span data-stu-id="f14ea-137">Request</span></span>

<span data-ttu-id="f14ea-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f14ea-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/v1.0/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="f14ea-139">响应</span><span class="sxs-lookup"><span data-stu-id="f14ea-139">Response</span></span>

<span data-ttu-id="f14ea-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f14ea-140">The following is an example of the response.</span></span>

><span data-ttu-id="f14ea-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f14ea-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f14ea-142">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f14ea-142">All the properties will be returned from an actual call.</span></span>
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
