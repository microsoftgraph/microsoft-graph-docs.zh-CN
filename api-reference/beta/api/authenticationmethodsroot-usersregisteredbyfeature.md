---
title: authenticationMethodsRoot： usersRegisteredByFeature
description: 获取能够进行多重身份验证、自助服务密码重置和无密码身份验证的用户数。
author: danielwood95
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 54c1265ebed3eb8a3fe28f091d045b7bfe221b18
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474349"
---
# <a name="authenticationmethodsroot-usersregisteredbyfeature"></a><span data-ttu-id="e4130-103">authenticationMethodsRoot： usersRegisteredByFeature</span><span class="sxs-lookup"><span data-stu-id="e4130-103">authenticationMethodsRoot: usersRegisteredByFeature</span></span>
<span data-ttu-id="e4130-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4130-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4130-105">获取能够进行多重身份验证、自助服务密码重置和无密码身份验证的用户数。</span><span class="sxs-lookup"><span data-stu-id="e4130-105">Get the number of users capable of multi-factor authentication, self-service password reset, and passwordless authentication.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4130-106">权限</span><span class="sxs-lookup"><span data-stu-id="e4130-106">Permissions</span></span>
<span data-ttu-id="e4130-107">调用此 API 需要以下权限。</span><span class="sxs-lookup"><span data-stu-id="e4130-107">The following permissions are required to call this API.</span></span> <span data-ttu-id="e4130-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4130-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4130-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4130-109">Permission type</span></span>|<span data-ttu-id="e4130-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4130-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4130-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4130-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e4130-112">AuditLogs.Read.All</span><span class="sxs-lookup"><span data-stu-id="e4130-112">AuditLogs.Read.All</span></span>|
|<span data-ttu-id="e4130-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4130-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4130-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4130-114">Not supported.</span></span>|
|<span data-ttu-id="e4130-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4130-115">Application</span></span>|<span data-ttu-id="e4130-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4130-116">Not supported.</span></span>|

<span data-ttu-id="e4130-117">若要访问 API， [需要以下角色之](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) 一：</span><span class="sxs-lookup"><span data-stu-id="e4130-117">In order to access the API, [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) is required:</span></span>

* <span data-ttu-id="e4130-118">报表阅读人员</span><span class="sxs-lookup"><span data-stu-id="e4130-118">Reports reader</span></span>
* <span data-ttu-id="e4130-119">安全读者</span><span class="sxs-lookup"><span data-stu-id="e4130-119">Security reader</span></span>
* <span data-ttu-id="e4130-120">安全管理员</span><span class="sxs-lookup"><span data-stu-id="e4130-120">Security admin</span></span>
* <span data-ttu-id="e4130-121">全局读取者</span><span class="sxs-lookup"><span data-stu-id="e4130-121">Global reader</span></span>
* <span data-ttu-id="e4130-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="e4130-122">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="e4130-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4130-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/authenticationMethods/usersRegisteredByFeature
```

## <a name="function-parameters"></a><span data-ttu-id="e4130-124">函数参数</span><span class="sxs-lookup"><span data-stu-id="e4130-124">Function parameters</span></span>
<span data-ttu-id="e4130-125">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="e4130-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e4130-126">参数</span><span class="sxs-lookup"><span data-stu-id="e4130-126">Parameter</span></span>|<span data-ttu-id="e4130-127">类型</span><span class="sxs-lookup"><span data-stu-id="e4130-127">Type</span></span>|<span data-ttu-id="e4130-128">说明</span><span class="sxs-lookup"><span data-stu-id="e4130-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4130-129">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="e4130-129">includedUserTypes</span></span>|<span data-ttu-id="e4130-130">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="e4130-130">includedUserTypes</span></span>|<span data-ttu-id="e4130-131">用户类型。</span><span class="sxs-lookup"><span data-stu-id="e4130-131">User type.</span></span> <span data-ttu-id="e4130-132">可取值为：`all`、`member`、`guest`。</span><span class="sxs-lookup"><span data-stu-id="e4130-132">Possible values are: `all`, `member`, `guest`.</span></span>|
|<span data-ttu-id="e4130-133">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="e4130-133">includedUserRoles</span></span>|<span data-ttu-id="e4130-134">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="e4130-134">includedUserRoles</span></span>|<span data-ttu-id="e4130-135">用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="e4130-135">User role type.</span></span> <span data-ttu-id="e4130-136">可取值为：`all`、`privilegedAdmin`、`admin`、`user`。</span><span class="sxs-lookup"><span data-stu-id="e4130-136">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|

<span data-ttu-id="e4130-137">值 `privilegedAdmin` 由以下特权管理员角色组成：</span><span class="sxs-lookup"><span data-stu-id="e4130-137">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="e4130-138">全局管理员</span><span class="sxs-lookup"><span data-stu-id="e4130-138">Global admin</span></span>
* <span data-ttu-id="e4130-139">安全管理员</span><span class="sxs-lookup"><span data-stu-id="e4130-139">Security admin</span></span>
* <span data-ttu-id="e4130-140">条件访问管理员</span><span class="sxs-lookup"><span data-stu-id="e4130-140">Conditional Access admin</span></span>
* <span data-ttu-id="e4130-141">Exchange 管理员</span><span class="sxs-lookup"><span data-stu-id="e4130-141">Exchange admin</span></span>
* <span data-ttu-id="e4130-142">SharePoint 管理员</span><span class="sxs-lookup"><span data-stu-id="e4130-142">SharePoint admin</span></span>
* <span data-ttu-id="e4130-143">支持管理员</span><span class="sxs-lookup"><span data-stu-id="e4130-143">Helpdesk admin</span></span>
* <span data-ttu-id="e4130-144">帐务管理员</span><span class="sxs-lookup"><span data-stu-id="e4130-144">Billing admin</span></span>
* <span data-ttu-id="e4130-145">用户管理员</span><span class="sxs-lookup"><span data-stu-id="e4130-145">User admin</span></span>
* <span data-ttu-id="e4130-146">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="e4130-146">Authentication admin</span></span>

<span data-ttu-id="e4130-147">值 `admin` 包括所有 Azure AD 管理员角色。</span><span class="sxs-lookup"><span data-stu-id="e4130-147">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="e4130-148">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4130-148">Request headers</span></span>
|<span data-ttu-id="e4130-149">名称</span><span class="sxs-lookup"><span data-stu-id="e4130-149">Name</span></span>|<span data-ttu-id="e4130-150">说明</span><span class="sxs-lookup"><span data-stu-id="e4130-150">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e4130-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4130-151">Authorization</span></span>|<span data-ttu-id="e4130-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e4130-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4130-154">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4130-154">Request body</span></span>
<span data-ttu-id="e4130-155">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e4130-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4130-156">响应</span><span class="sxs-lookup"><span data-stu-id="e4130-156">Response</span></span>

<span data-ttu-id="e4130-157">如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [userRegistrationFeatureSummary。](../resources/userregistrationfeaturesummary.md)</span><span class="sxs-lookup"><span data-stu-id="e4130-157">If successful, this function returns a `200 OK` response code and a [userRegistrationFeatureSummary](../resources/userregistrationfeaturesummary.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e4130-158">示例</span><span class="sxs-lookup"><span data-stu-id="e4130-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e4130-159">请求</span><span class="sxs-lookup"><span data-stu-id="e4130-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e4130-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4130-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "authenticationmethodsroot_usersregisteredbyfeature"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')
```
# <a name="c"></a>[<span data-ttu-id="e4130-161">C#</span><span class="sxs-lookup"><span data-stu-id="e4130-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/authenticationmethodsroot-usersregisteredbyfeature-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4130-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4130-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/authenticationmethodsroot-usersregisteredbyfeature-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4130-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4130-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/authenticationmethodsroot-usersregisteredbyfeature-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4130-164">Java</span><span class="sxs-lookup"><span data-stu-id="e4130-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/authenticationmethodsroot-usersregisteredbyfeature-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e4130-165">响应</span><span class="sxs-lookup"><span data-stu-id="e4130-165">Response</span></span>
<span data-ttu-id="e4130-166">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e4130-166">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userRegistrationFeatureSummary"
} -->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.userRegistrationFeatureSummary",
    "totalUserCount": 23123,
    "userTypes": "all",
    "userRoles": "all",
    "userRegistrationFeatureCounts": [{
            "feature": "ssprRegistered",
            "userCount": 23423
        },
        {
            "feature": "ssprEnabled",
            "userCount": 4234
        },
        {
            "feature": "ssprCapable",
            "userCount": 4234
        }, {
            "feature": "passwordlessCapable",
            "userCount": 323
        },
        {
            "feature": "mfaCapable",
            "userCount": 3345
        }
    ]
}
```
