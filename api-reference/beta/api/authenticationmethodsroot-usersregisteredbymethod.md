---
title: authenticationMethodsRoot： usersRegisteredByMethod
description: 获取针对每个身份验证方法注册的用户数。
author: danielwood95
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 5cccef1ba35edbb3eb947cee90fb70c05ff19389
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473470"
---
# <a name="authenticationmethodsroot-usersregisteredbymethod"></a><span data-ttu-id="65d23-103">authenticationMethodsRoot： usersRegisteredByMethod</span><span class="sxs-lookup"><span data-stu-id="65d23-103">authenticationMethodsRoot: usersRegisteredByMethod</span></span>
<span data-ttu-id="65d23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65d23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65d23-105">获取针对每个身份验证方法注册的用户数。</span><span class="sxs-lookup"><span data-stu-id="65d23-105">Get the number of users registered for each authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="65d23-106">权限</span><span class="sxs-lookup"><span data-stu-id="65d23-106">Permissions</span></span>
<span data-ttu-id="65d23-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65d23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65d23-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="65d23-109">Permission type</span></span>|<span data-ttu-id="65d23-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65d23-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65d23-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65d23-111">Delegated (work or school account)</span></span>|<span data-ttu-id="65d23-112">AuditLogs.Read.All</span><span class="sxs-lookup"><span data-stu-id="65d23-112">AuditLogs.Read.All</span></span>|
|<span data-ttu-id="65d23-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65d23-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65d23-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="65d23-114">Not supported.</span></span>|
|<span data-ttu-id="65d23-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="65d23-115">Application</span></span>|<span data-ttu-id="65d23-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="65d23-116">Not supported.</span></span>|

<span data-ttu-id="65d23-117">若要访问 API， [需要以下角色之](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) 一：</span><span class="sxs-lookup"><span data-stu-id="65d23-117">In order to access the API, [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) is required:</span></span>

* <span data-ttu-id="65d23-118">报表阅读人员</span><span class="sxs-lookup"><span data-stu-id="65d23-118">Reports reader</span></span>
* <span data-ttu-id="65d23-119">安全读者</span><span class="sxs-lookup"><span data-stu-id="65d23-119">Security reader</span></span>
* <span data-ttu-id="65d23-120">安全管理员</span><span class="sxs-lookup"><span data-stu-id="65d23-120">Security admin</span></span>
* <span data-ttu-id="65d23-121">全局读取者</span><span class="sxs-lookup"><span data-stu-id="65d23-121">Global reader</span></span>
* <span data-ttu-id="65d23-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="65d23-122">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="65d23-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65d23-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/authenticationMethods/usersRegisteredByMethod
```

## <a name="function-parameters"></a><span data-ttu-id="65d23-124">函数参数</span><span class="sxs-lookup"><span data-stu-id="65d23-124">Function parameters</span></span>
<span data-ttu-id="65d23-125">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="65d23-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="65d23-126">参数</span><span class="sxs-lookup"><span data-stu-id="65d23-126">Parameter</span></span>|<span data-ttu-id="65d23-127">类型</span><span class="sxs-lookup"><span data-stu-id="65d23-127">Type</span></span>|<span data-ttu-id="65d23-128">说明</span><span class="sxs-lookup"><span data-stu-id="65d23-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65d23-129">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="65d23-129">includedUserTypes</span></span>|<span data-ttu-id="65d23-130">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="65d23-130">includedUserTypes</span></span>|<span data-ttu-id="65d23-131">用户类型。</span><span class="sxs-lookup"><span data-stu-id="65d23-131">User type.</span></span> <span data-ttu-id="65d23-132">可取值为：`all`、`member`、`guest`。</span><span class="sxs-lookup"><span data-stu-id="65d23-132">Possible values are: `all`, `member`, `guest`.</span></span>|
|<span data-ttu-id="65d23-133">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="65d23-133">includedUserRoles</span></span>|<span data-ttu-id="65d23-134">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="65d23-134">includedUserRoles</span></span>|<span data-ttu-id="65d23-135">用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="65d23-135">User role type.</span></span> <span data-ttu-id="65d23-136">可取值为：`all`、`privilegedAdmin`、`admin`、`user`。</span><span class="sxs-lookup"><span data-stu-id="65d23-136">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|

<span data-ttu-id="65d23-137">值 `privilegedAdmin` 由以下特权管理员角色组成：</span><span class="sxs-lookup"><span data-stu-id="65d23-137">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="65d23-138">全局管理员</span><span class="sxs-lookup"><span data-stu-id="65d23-138">Global admin</span></span>
* <span data-ttu-id="65d23-139">安全管理员</span><span class="sxs-lookup"><span data-stu-id="65d23-139">Security admin</span></span>
* <span data-ttu-id="65d23-140">条件访问管理员</span><span class="sxs-lookup"><span data-stu-id="65d23-140">Conditional Access admin</span></span>
* <span data-ttu-id="65d23-141">Exchange 管理员</span><span class="sxs-lookup"><span data-stu-id="65d23-141">Exchange admin</span></span>
* <span data-ttu-id="65d23-142">SharePoint 管理员</span><span class="sxs-lookup"><span data-stu-id="65d23-142">SharePoint admin</span></span>
* <span data-ttu-id="65d23-143">支持管理员</span><span class="sxs-lookup"><span data-stu-id="65d23-143">Helpdesk admin</span></span>
* <span data-ttu-id="65d23-144">帐务管理员</span><span class="sxs-lookup"><span data-stu-id="65d23-144">Billing admin</span></span>
* <span data-ttu-id="65d23-145">用户管理员</span><span class="sxs-lookup"><span data-stu-id="65d23-145">User admin</span></span>
* <span data-ttu-id="65d23-146">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="65d23-146">Authentication admin</span></span>

<span data-ttu-id="65d23-147">值 `admin` 包括所有 Azure AD 管理员角色。</span><span class="sxs-lookup"><span data-stu-id="65d23-147">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="65d23-148">请求标头</span><span class="sxs-lookup"><span data-stu-id="65d23-148">Request headers</span></span>
|<span data-ttu-id="65d23-149">名称</span><span class="sxs-lookup"><span data-stu-id="65d23-149">Name</span></span>|<span data-ttu-id="65d23-150">说明</span><span class="sxs-lookup"><span data-stu-id="65d23-150">Description</span></span>|
|:---|:---|
|<span data-ttu-id="65d23-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="65d23-151">Authorization</span></span>|<span data-ttu-id="65d23-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65d23-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65d23-154">请求正文</span><span class="sxs-lookup"><span data-stu-id="65d23-154">Request body</span></span>
<span data-ttu-id="65d23-155">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="65d23-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65d23-156">响应</span><span class="sxs-lookup"><span data-stu-id="65d23-156">Response</span></span>

<span data-ttu-id="65d23-157">如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [userRegistrationMethodSummary。](../resources/userregistrationmethodsummary.md)</span><span class="sxs-lookup"><span data-stu-id="65d23-157">If successful, this function returns a `200 OK` response code and a [userRegistrationMethodSummary](../resources/userregistrationmethodsummary.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65d23-158">示例</span><span class="sxs-lookup"><span data-stu-id="65d23-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65d23-159">请求</span><span class="sxs-lookup"><span data-stu-id="65d23-159">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="65d23-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="65d23-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "authenticationmethodsroot_usersregisteredbymethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/authenticationMethods/usersRegisteredByMethod(includedUserTypes='all',includedUserRoles='all')
```
# <a name="c"></a>[<span data-ttu-id="65d23-161">C#</span><span class="sxs-lookup"><span data-stu-id="65d23-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/authenticationmethodsroot-usersregisteredbymethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65d23-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65d23-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/authenticationmethodsroot-usersregisteredbymethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65d23-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65d23-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/authenticationmethodsroot-usersregisteredbymethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65d23-164">Java</span><span class="sxs-lookup"><span data-stu-id="65d23-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/authenticationmethodsroot-usersregisteredbymethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="65d23-165">响应</span><span class="sxs-lookup"><span data-stu-id="65d23-165">Response</span></span>
<span data-ttu-id="65d23-166">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="65d23-166">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userRegistrationFeatureSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.userRegistrationMethodSummary",
    "userTypes": "all",
    "userRoles": "all",
    "userRegistrationMethodCounts": [{
            "authenticationMethod": "password",
            "userCount": 12209
        },
        {
            "authenticationMethod": "windowsHelloForBusiness",
            "userCount": 223
        },
        {
            "authenticationMethod": "mobilePhone",
            "userCount": 4234
        }
    ]
}
```
