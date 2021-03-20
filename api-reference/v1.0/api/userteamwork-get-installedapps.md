---
title: 获取用户的已安装应用
description: 检索在指定用户的个人范围内安装的应用。
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 609c4081d30e831bca2573d4195e9221e5d42b05
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961133"
---
# <a name="get-installed-app-for-user"></a><span data-ttu-id="7e01a-103">获取用户的已安装应用</span><span class="sxs-lookup"><span data-stu-id="7e01a-103">Get installed app for user</span></span>

<span data-ttu-id="7e01a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e01a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7e01a-105">检索 [在](../resources/teamsappinstallation.md) 指定用户的个人范围内安装 [的应用](../resources/user.md)。</span><span class="sxs-lookup"><span data-stu-id="7e01a-105">Retrieve the [app](../resources/teamsappinstallation.md) installed in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e01a-106">权限</span><span class="sxs-lookup"><span data-stu-id="7e01a-106">Permissions</span></span>

<span data-ttu-id="7e01a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e01a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e01a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e01a-109">Permission type</span></span>      | <span data-ttu-id="7e01a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e01a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e01a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e01a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7e01a-112">TeamsAppInstallation.ReadForUser、TeamsAppInstallation.ReadWriteSelfForUser、TeamsAppInstallation.ReadWriteForUser</span><span class="sxs-lookup"><span data-stu-id="7e01a-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser</span></span> |
|<span data-ttu-id="7e01a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e01a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e01a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e01a-114">Not supported.</span></span>    |
|<span data-ttu-id="7e01a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e01a-115">Application</span></span> | <span data-ttu-id="7e01a-116">TeamsAppInstallation.ReadForUser.All、TeamsAppInstallation.ReadWriteSelfForUser.All、TeamsAppInstallation.ReadWriteForUser.All</span><span class="sxs-lookup"><span data-stu-id="7e01a-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e01a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e01a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{user-id}/teamwork/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="7e01a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e01a-118">Request headers</span></span>

| <span data-ttu-id="7e01a-119">标头</span><span class="sxs-lookup"><span data-stu-id="7e01a-119">Header</span></span>       | <span data-ttu-id="7e01a-120">值</span><span class="sxs-lookup"><span data-stu-id="7e01a-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7e01a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e01a-121">Authorization</span></span>  | <span data-ttu-id="7e01a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e01a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7e01a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e01a-124">Request body</span></span>

<span data-ttu-id="7e01a-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7e01a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e01a-126">响应</span><span class="sxs-lookup"><span data-stu-id="7e01a-126">Response</span></span>

<span data-ttu-id="7e01a-127">如果成功，此方法在响应 `200 OK` 正文中返回 [响应代码](../resources/teamsappinstallation.md) 和应用。</span><span class="sxs-lookup"><span data-stu-id="7e01a-127">If successful, this method returns a `200 OK` response code and an [app](../resources/teamsappinstallation.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7e01a-128">示例</span><span class="sxs-lookup"><span data-stu-id="7e01a-128">Examples</span></span>

### <a name="example-1-get-an-app-installed-for-the-specified-user"></a><span data-ttu-id="7e01a-129">示例 1：为指定用户安装应用</span><span class="sxs-lookup"><span data-stu-id="7e01a-129">Example 1: Get an app installed for the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="7e01a-130">请求</span><span class="sxs-lookup"><span data-stu-id="7e01a-130">Request</span></span>

<span data-ttu-id="7e01a-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e01a-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="7e01a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e01a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk
```
# <a name="c"></a>[<span data-ttu-id="7e01a-133">C#</span><span class="sxs-lookup"><span data-stu-id="7e01a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-teamsapps-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e01a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e01a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-teamsapps-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e01a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e01a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-teamsapps-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e01a-136">Java</span><span class="sxs-lookup"><span data-stu-id="7e01a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-list-teamsapps-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7e01a-137">响应</span><span class="sxs-lookup"><span data-stu-id="7e01a-137">Response</span></span>

<span data-ttu-id="7e01a-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7e01a-138">The following is an example of the response.</span></span>
><span data-ttu-id="7e01a-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7e01a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_1",
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

### <a name="example-2-get-the-names-and-other-details-of-the-app-installed-for-the-user"></a><span data-ttu-id="7e01a-141">示例 2：获取为用户安装的应用的名称和其他详细信息</span><span class="sxs-lookup"><span data-stu-id="7e01a-141">Example 2: Get the names and other details of the app installed for the user</span></span>

#### <a name="request"></a><span data-ttu-id="7e01a-142">请求</span><span class="sxs-lookup"><span data-stu-id="7e01a-142">Request</span></span>

<span data-ttu-id="7e01a-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e01a-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "user_list_teamsApps_details"
} -->

```http
GET https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk=?$expand=teamsAppDefinition
```

#### <a name="response"></a><span data-ttu-id="7e01a-144">响应</span><span class="sxs-lookup"><span data-stu-id="7e01a-144">Response</span></span>

<span data-ttu-id="7e01a-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7e01a-145">The following is an example of the response.</span></span>

><span data-ttu-id="7e01a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7e01a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
