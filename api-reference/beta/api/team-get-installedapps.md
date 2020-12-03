---
title: 在团队中获取已安装的应用程序
description: 获取团队中安装的应用程序。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 49903514fb6345978d90ca1df7a8ab5279c61410
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564151"
---
# <a name="get-installed-app-in-team"></a><span data-ttu-id="b48c9-103">在团队中获取已安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="b48c9-103">Get installed app in team</span></span>

<span data-ttu-id="b48c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b48c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b48c9-105">检索在指定[团队](../resources/team.md)中安装的[应用程序](../resources/teamsappinstallation.md)。</span><span class="sxs-lookup"><span data-stu-id="b48c9-105">Retrieve the [app](../resources/teamsappinstallation.md) installed in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b48c9-106">权限</span><span class="sxs-lookup"><span data-stu-id="b48c9-106">Permissions</span></span>

<span data-ttu-id="b48c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b48c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b48c9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b48c9-109">Permission type</span></span>      | <span data-ttu-id="b48c9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b48c9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b48c9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b48c9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b48c9-112">TeamsAppInstallation、ReadWriteSelfForTeam、TeamsAppInstallation、、、、、、、all、all、all 和 all 的所有读写。</span><span class="sxs-lookup"><span data-stu-id="b48c9-112">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="b48c9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b48c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b48c9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b48c9-114">Not supported.</span></span>    |
|<span data-ttu-id="b48c9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b48c9-115">Application</span></span> | <span data-ttu-id="b48c9-116">TeamsAppInstallation、ReadWriteSelfForTeam、TeamsAppInstallation、Group. all、、、、all、all、all、all 和 All 的所有读写。</span><span class="sxs-lookup"><span data-stu-id="b48c9-116">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b48c9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b48c9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b48c9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b48c9-118">Request headers</span></span>

| <span data-ttu-id="b48c9-119">标头</span><span class="sxs-lookup"><span data-stu-id="b48c9-119">Header</span></span>       | <span data-ttu-id="b48c9-120">值</span><span class="sxs-lookup"><span data-stu-id="b48c9-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b48c9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b48c9-121">Authorization</span></span>  | <span data-ttu-id="b48c9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b48c9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b48c9-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b48c9-124">Request body</span></span>

<span data-ttu-id="b48c9-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b48c9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b48c9-126">响应</span><span class="sxs-lookup"><span data-stu-id="b48c9-126">Response</span></span>

<span data-ttu-id="b48c9-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [teamsAppInstallation](../resources/teamsappinstallation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b48c9-127">If successful, this method returns a `200 OK` response code and a [teamsAppInstallation](../resources/teamsappinstallation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b48c9-128">示例</span><span class="sxs-lookup"><span data-stu-id="b48c9-128">Examples</span></span>

### <a name="example-1-get-the-installed-app"></a><span data-ttu-id="b48c9-129">示例1：获取已安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="b48c9-129">Example 1: Get the installed app</span></span>
#### <a name="request"></a><span data-ttu-id="b48c9-130">请求</span><span class="sxs-lookup"><span data-stu-id="b48c9-130">Request</span></span>

<span data-ttu-id="b48c9-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b48c9-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->

```msgraph-interactive
GET /teams/{id}/installedApps/{id}
```

---

#### <a name="response"></a><span data-ttu-id="b48c9-132">响应</span><span class="sxs-lookup"><span data-stu-id="b48c9-132">Response</span></span>

<span data-ttu-id="b48c9-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b48c9-133">The following is an example of the response.</span></span>
><span data-ttu-id="b48c9-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b48c9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-the-installed-app"></a><span data-ttu-id="b48c9-136">示例2：获取已安装应用程序的名称和其他详细信息</span><span class="sxs-lookup"><span data-stu-id="b48c9-136">Example 2: Get the names and other details of the installed app</span></span>

#### <a name="request"></a><span data-ttu-id="b48c9-137">请求</span><span class="sxs-lookup"><span data-stu-id="b48c9-137">Request</span></span>

<span data-ttu-id="b48c9-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b48c9-138">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}?$expand=teamsAppDefinition
```

---

#### <a name="response"></a><span data-ttu-id="b48c9-139">响应</span><span class="sxs-lookup"><span data-stu-id="b48c9-139">Response</span></span>

<span data-ttu-id="b48c9-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b48c9-140">The following is an example of the response.</span></span>

><span data-ttu-id="b48c9-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b48c9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps_expand",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "displayName": "OneNote",
                "version": "beta"
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

