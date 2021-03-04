---
title: 创建帐户
description: 创建新的帐户对象。
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 308f2a1e4087fcbb07efb08be8fc1e4cba7d819f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441006"
---
# <a name="create-account"></a><span data-ttu-id="3377f-103">创建帐户</span><span class="sxs-lookup"><span data-stu-id="3377f-103">Create account</span></span>
<span data-ttu-id="3377f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3377f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3377f-105">在用户配置文件中创建新的 [userAccountInformation](../resources/useraccountinformation.md) [对象](../resources/profile.md)。</span><span class="sxs-lookup"><span data-stu-id="3377f-105">Create a new [userAccountInformation](../resources/useraccountinformation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3377f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="3377f-106">Permissions</span></span>

<span data-ttu-id="3377f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3377f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3377f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3377f-109">Permission type</span></span>                        | <span data-ttu-id="3377f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3377f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3377f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3377f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3377f-112">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3377f-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3377f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3377f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3377f-114">User.ReadWrite、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3377f-114">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="3377f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3377f-115">Application</span></span>                            | <span data-ttu-id="3377f-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3377f-116">User.ReadWrite.All</span></span>                          |

## <a name="http-request"></a><span data-ttu-id="3377f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3377f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/account
POST /users/{id | userPrincipalName}/profile/account
```

## <a name="request-headers"></a><span data-ttu-id="3377f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3377f-118">Request headers</span></span>
|<span data-ttu-id="3377f-119">名称</span><span class="sxs-lookup"><span data-stu-id="3377f-119">Name</span></span>|<span data-ttu-id="3377f-120">说明</span><span class="sxs-lookup"><span data-stu-id="3377f-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3377f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3377f-121">Authorization</span></span>|<span data-ttu-id="3377f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3377f-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3377f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3377f-124">Content-Type</span></span>|<span data-ttu-id="3377f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3377f-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3377f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3377f-127">Request body</span></span>
<span data-ttu-id="3377f-128">在请求正文中，提供 [userAccountInformation](../resources/useraccountinformation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3377f-128">In the request body, supply a JSON representation of the [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

<span data-ttu-id="3377f-129">下表显示创建新的 [userAccountInformation](../resources/useraccountinformation.md) 对象时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3377f-129">The following table shows the properties that are required when you create a new [userAccountInformation](../resources/useraccountinformation.md) object.</span></span>

|<span data-ttu-id="3377f-130">属性</span><span class="sxs-lookup"><span data-stu-id="3377f-130">Property</span></span>|<span data-ttu-id="3377f-131">类型</span><span class="sxs-lookup"><span data-stu-id="3377f-131">Type</span></span>|<span data-ttu-id="3377f-132">说明</span><span class="sxs-lookup"><span data-stu-id="3377f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3377f-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="3377f-133">allowedAudiences</span></span>|<span data-ttu-id="3377f-134">String</span><span class="sxs-lookup"><span data-stu-id="3377f-134">String</span></span>|<span data-ttu-id="3377f-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="3377f-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="3377f-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="3377f-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="3377f-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="3377f-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3377f-138">countryCode</span><span class="sxs-lookup"><span data-stu-id="3377f-138">countryCode</span></span>|<span data-ttu-id="3377f-139">String</span><span class="sxs-lookup"><span data-stu-id="3377f-139">String</span></span>|<span data-ttu-id="3377f-140">包含与用户帐户关联的两个字符的国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="3377f-140">Contains the two-character country code associated with the users account.</span></span>  |
|<span data-ttu-id="3377f-141">推断</span><span class="sxs-lookup"><span data-stu-id="3377f-141">inference</span></span>|[<span data-ttu-id="3377f-142">inferenceData</span><span class="sxs-lookup"><span data-stu-id="3377f-142">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="3377f-143">如果实体是由创建或修改应用程序推断的，则包含推断详细信息。</span><span class="sxs-lookup"><span data-stu-id="3377f-143">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="3377f-144">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="3377f-144">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="3377f-145">preferredLanguageTag</span><span class="sxs-lookup"><span data-stu-id="3377f-145">preferredLanguageTag</span></span>|[<span data-ttu-id="3377f-146">localeInfo</span><span class="sxs-lookup"><span data-stu-id="3377f-146">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="3377f-147">包含用户关联为帐户首选的语言。</span><span class="sxs-lookup"><span data-stu-id="3377f-147">Contains the language the user has associated as preferred for the account.</span></span>   |
|<span data-ttu-id="3377f-148">source</span><span class="sxs-lookup"><span data-stu-id="3377f-148">source</span></span>|[<span data-ttu-id="3377f-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="3377f-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="3377f-150">如果从另一个服务同步，则值的来源。</span><span class="sxs-lookup"><span data-stu-id="3377f-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="3377f-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="3377f-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="3377f-152">响应</span><span class="sxs-lookup"><span data-stu-id="3377f-152">Response</span></span>

<span data-ttu-id="3377f-153">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [userAccountInformation](../resources/useraccountinformation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3377f-153">If successful, this method returns a `201 Created` response code and a [userAccountInformation](../resources/useraccountinformation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3377f-154">示例</span><span class="sxs-lookup"><span data-stu-id="3377f-154">Examples</span></span>


# <a name="http"></a>[<span data-ttu-id="3377f-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="3377f-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_useraccountinformation_from_profile"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/account
Content-Type: application/json
Content-length: 494

{
  "allowedAudiences": "organization",
  "countryCode": "NO",
}
```
# <a name="c"></a>[<span data-ttu-id="3377f-156">C#</span><span class="sxs-lookup"><span data-stu-id="3377f-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-useraccountinformation-from-profile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3377f-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3377f-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-useraccountinformation-from-profile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3377f-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3377f-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-useraccountinformation-from-profile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3377f-159">Java</span><span class="sxs-lookup"><span data-stu-id="3377f-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-useraccountinformation-from-profile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3377f-160">响应</span><span class="sxs-lookup"><span data-stu-id="3377f-160">Response</span></span>
<span data-ttu-id="3377f-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3377f-161">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "source": null,
  "ageGroup": "adult",
  "countryCode": "NO",
  "preferredLanguageTag": null,
  "userPrincipalName": "innocenty.popov@adventureworks.com"
}
```


