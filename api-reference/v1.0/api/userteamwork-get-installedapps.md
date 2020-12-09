---
title: 为用户获取安装的应用程序
description: 检索在指定用户的个人作用域中安装的应用程序。
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9ac5b4a83528d007e7df49345752b47275b884c1
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607187"
---
# <a name="get-installed-app-for-user"></a><span data-ttu-id="21154-103">为用户获取安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="21154-103">Get installed app for user</span></span>

<span data-ttu-id="21154-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21154-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="21154-105">检索在指定[用户](../resources/user.md)的个人作用域中安装的[应用程序](../resources/teamsappinstallation.md)。</span><span class="sxs-lookup"><span data-stu-id="21154-105">Retrieve the [app](../resources/teamsappinstallation.md) installed in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="21154-106">权限</span><span class="sxs-lookup"><span data-stu-id="21154-106">Permissions</span></span>

<span data-ttu-id="21154-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21154-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21154-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="21154-109">Permission type</span></span>      | <span data-ttu-id="21154-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="21154-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21154-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21154-111">Delegated (work or school account)</span></span> | <span data-ttu-id="21154-112">ReadForUser、TeamsAppInstallation、TeamsAppInstallation TeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="21154-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="21154-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21154-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21154-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="21154-114">Not supported.</span></span>    |
|<span data-ttu-id="21154-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="21154-115">Application</span></span> | <span data-ttu-id="21154-116">TeamsAppInstallation、TeamsAppInstallation、ReadWriteSelfForUser、TeamsAppInstallation。 all</span><span class="sxs-lookup"><span data-stu-id="21154-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="21154-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21154-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{user-id}/teamwork/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="21154-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="21154-118">Request headers</span></span>

| <span data-ttu-id="21154-119">标头</span><span class="sxs-lookup"><span data-stu-id="21154-119">Header</span></span>       | <span data-ttu-id="21154-120">值</span><span class="sxs-lookup"><span data-stu-id="21154-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="21154-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="21154-121">Authorization</span></span>  | <span data-ttu-id="21154-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="21154-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="21154-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="21154-124">Request body</span></span>

<span data-ttu-id="21154-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="21154-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21154-126">响应</span><span class="sxs-lookup"><span data-stu-id="21154-126">Response</span></span>

<span data-ttu-id="21154-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [应用程序](../resources/teamsappinstallation.md) 。</span><span class="sxs-lookup"><span data-stu-id="21154-127">If successful, this method returns a `200 OK` response code and an [app](../resources/teamsappinstallation.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="21154-128">示例</span><span class="sxs-lookup"><span data-stu-id="21154-128">Examples</span></span>

### <a name="example-1-get-an-app-installed-for-the-specified-user"></a><span data-ttu-id="21154-129">示例1：获取为指定用户安装的应用程序</span><span class="sxs-lookup"><span data-stu-id="21154-129">Example 1: Get an app installed for the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="21154-130">请求</span><span class="sxs-lookup"><span data-stu-id="21154-130">Request</span></span>

<span data-ttu-id="21154-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="21154-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk
```

#### <a name="response"></a><span data-ttu-id="21154-132">响应</span><span class="sxs-lookup"><span data-stu-id="21154-132">Response</span></span>

<span data-ttu-id="21154-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="21154-133">The following is an example of the response.</span></span>
><span data-ttu-id="21154-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="21154-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps",
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
      "id": "YTZiNjMzNjUtMzFhNC00ZjQzLTkyZWMtNzEwYjcxNTU3YWY5IyMwLjk"
    }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-the-app-installed-for-the-user"></a><span data-ttu-id="21154-136">示例2：获取为用户安装的应用程序的名称和其他详细信息</span><span class="sxs-lookup"><span data-stu-id="21154-136">Example 2: Get the names and other details of the app installed for the user</span></span>

#### <a name="request"></a><span data-ttu-id="21154-137">请求</span><span class="sxs-lookup"><span data-stu-id="21154-137">Request</span></span>

<span data-ttu-id="21154-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="21154-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "user_list_teamsApps_details"
} -->

```http
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk=?$expand=teamsAppDefinition
```

#### <a name="response"></a><span data-ttu-id="21154-139">响应</span><span class="sxs-lookup"><span data-stu-id="21154-139">Response</span></span>

<span data-ttu-id="21154-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="21154-140">The following is an example of the response.</span></span>

><span data-ttu-id="21154-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="21154-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_details",
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
          "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('5b649834-7412-4cce-9e69-176e95a394f5')/installedApps(teamsAppDefinition())/$entity",
          "id": "NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk=",
          "teamsAppDefinition": {
                                  "id": "YTZiNjMzNjUtMzFhNC00ZjQzLTkyZWMtNzEwYjcxNTU3YWY5IyMwLjk=",
                                  "teamsAppId": "a6b63365-31a4-4f43-92ec-710b71557af9",
                                  "displayName": "Power Apps",
                                  "version": "0.9"
                                }
          }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User get teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
