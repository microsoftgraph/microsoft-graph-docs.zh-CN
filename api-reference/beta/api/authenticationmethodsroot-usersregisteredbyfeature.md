---
title: authenticationMethodsRoot： usersRegisteredByFeature
description: 获取能够进行多重身份验证、自助服务密码重置和无密码身份验证的用户数量。
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: apiPageType
ms.openlocfilehash: 3006ca1dafc1eda4774879144673cb804be552e5
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052556"
---
# <a name="authenticationmethodsroot-usersregisteredbyfeature"></a><span data-ttu-id="24b18-103">authenticationMethodsRoot： usersRegisteredByFeature</span><span class="sxs-lookup"><span data-stu-id="24b18-103">authenticationMethodsRoot: usersRegisteredByFeature</span></span>
<span data-ttu-id="24b18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24b18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24b18-105">获取能够进行多重身份验证、自助服务密码重置和无密码身份验证的用户数量。</span><span class="sxs-lookup"><span data-stu-id="24b18-105">Get the number of users capable of multi-factor authentication, self-service password reset, and passwordless authentication.</span></span>

## <a name="permissions"></a><span data-ttu-id="24b18-106">权限</span><span class="sxs-lookup"><span data-stu-id="24b18-106">Permissions</span></span>
<span data-ttu-id="24b18-107">调用此 API 需要以下权限。</span><span class="sxs-lookup"><span data-stu-id="24b18-107">The following permissions are required to call this API.</span></span> <span data-ttu-id="24b18-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24b18-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24b18-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="24b18-109">Permission type</span></span>|<span data-ttu-id="24b18-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24b18-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24b18-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24b18-111">Delegated (work or school account)</span></span>|<span data-ttu-id="24b18-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="24b18-112">Reports.Read.All</span></span>|
|<span data-ttu-id="24b18-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24b18-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24b18-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="24b18-114">Not supported.</span></span>|
|<span data-ttu-id="24b18-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="24b18-115">Application</span></span>|<span data-ttu-id="24b18-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="24b18-116">Not supported.</span></span>|

<span data-ttu-id="24b18-117">若要访问 API，需要以下 [角色之](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) 一：</span><span class="sxs-lookup"><span data-stu-id="24b18-117">In order to access the API, [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles) is required:</span></span>

* <span data-ttu-id="24b18-118">报表阅读人员</span><span class="sxs-lookup"><span data-stu-id="24b18-118">Reports reader</span></span>
* <span data-ttu-id="24b18-119">安全读者</span><span class="sxs-lookup"><span data-stu-id="24b18-119">Security reader</span></span>
* <span data-ttu-id="24b18-120">安全管理员</span><span class="sxs-lookup"><span data-stu-id="24b18-120">Security admin</span></span>
* <span data-ttu-id="24b18-121">全局读取者</span><span class="sxs-lookup"><span data-stu-id="24b18-121">Global reader</span></span>
* <span data-ttu-id="24b18-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="24b18-122">Global admin</span></span>

## <a name="http-request"></a><span data-ttu-id="24b18-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24b18-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/authenticationMethods/usersRegisteredByFeature
```

## <a name="function-parameters"></a><span data-ttu-id="24b18-124">函数参数</span><span class="sxs-lookup"><span data-stu-id="24b18-124">Function parameters</span></span>
<span data-ttu-id="24b18-125">下表显示了可用于此函数的参数。</span><span class="sxs-lookup"><span data-stu-id="24b18-125">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="24b18-126">参数</span><span class="sxs-lookup"><span data-stu-id="24b18-126">Parameter</span></span>|<span data-ttu-id="24b18-127">类型</span><span class="sxs-lookup"><span data-stu-id="24b18-127">Type</span></span>|<span data-ttu-id="24b18-128">说明</span><span class="sxs-lookup"><span data-stu-id="24b18-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24b18-129">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="24b18-129">includedUserTypes</span></span>|<span data-ttu-id="24b18-130">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="24b18-130">includedUserTypes</span></span>|<span data-ttu-id="24b18-131">用户类型。</span><span class="sxs-lookup"><span data-stu-id="24b18-131">User type.</span></span> <span data-ttu-id="24b18-132">可取值为：`all`、`member`、`guest`。</span><span class="sxs-lookup"><span data-stu-id="24b18-132">Possible values are: `all`, `member`, `guest`.</span></span>|
|<span data-ttu-id="24b18-133">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="24b18-133">includedUserRoles</span></span>|<span data-ttu-id="24b18-134">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="24b18-134">includedUserRoles</span></span>|<span data-ttu-id="24b18-135">用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="24b18-135">User role type.</span></span> <span data-ttu-id="24b18-136">可取值为：`all`、`privilegedAdmin`、`admin`、`user`。</span><span class="sxs-lookup"><span data-stu-id="24b18-136">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|

<span data-ttu-id="24b18-137">该值 `privilegedAdmin` 由以下特权管理员角色组成：</span><span class="sxs-lookup"><span data-stu-id="24b18-137">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="24b18-138">全局管理员</span><span class="sxs-lookup"><span data-stu-id="24b18-138">Global admin</span></span>
* <span data-ttu-id="24b18-139">安全管理员</span><span class="sxs-lookup"><span data-stu-id="24b18-139">Security admin</span></span>
* <span data-ttu-id="24b18-140">条件访问管理员</span><span class="sxs-lookup"><span data-stu-id="24b18-140">Conditional Access admin</span></span>
* <span data-ttu-id="24b18-141">Exchange 管理员</span><span class="sxs-lookup"><span data-stu-id="24b18-141">Exchange admin</span></span>
* <span data-ttu-id="24b18-142">SharePoint 管理员</span><span class="sxs-lookup"><span data-stu-id="24b18-142">SharePoint admin</span></span>
* <span data-ttu-id="24b18-143">支持管理员</span><span class="sxs-lookup"><span data-stu-id="24b18-143">Helpdesk admin</span></span>
* <span data-ttu-id="24b18-144">帐务管理员</span><span class="sxs-lookup"><span data-stu-id="24b18-144">Billing admin</span></span>
* <span data-ttu-id="24b18-145">用户管理员</span><span class="sxs-lookup"><span data-stu-id="24b18-145">User admin</span></span>
* <span data-ttu-id="24b18-146">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="24b18-146">Authentication admin</span></span>

<span data-ttu-id="24b18-147">该值 `admin` 包括所有 Azure AD 管理员角色。</span><span class="sxs-lookup"><span data-stu-id="24b18-147">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="24b18-148">请求标头</span><span class="sxs-lookup"><span data-stu-id="24b18-148">Request headers</span></span>
|<span data-ttu-id="24b18-149">名称</span><span class="sxs-lookup"><span data-stu-id="24b18-149">Name</span></span>|<span data-ttu-id="24b18-150">说明</span><span class="sxs-lookup"><span data-stu-id="24b18-150">Description</span></span>|
|:---|:---|
|<span data-ttu-id="24b18-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="24b18-151">Authorization</span></span>|<span data-ttu-id="24b18-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="24b18-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24b18-154">请求正文</span><span class="sxs-lookup"><span data-stu-id="24b18-154">Request body</span></span>
<span data-ttu-id="24b18-155">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="24b18-155">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24b18-156">响应</span><span class="sxs-lookup"><span data-stu-id="24b18-156">Response</span></span>

<span data-ttu-id="24b18-157">如果成功，此函数在响应正文中返回响应代码和 `200 OK` [userRegistrationFeatureSummary。](../resources/userregistrationfeaturesummary.md)</span><span class="sxs-lookup"><span data-stu-id="24b18-157">If successful, this function returns a `200 OK` response code and a [userRegistrationFeatureSummary](../resources/userregistrationfeaturesummary.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24b18-158">示例</span><span class="sxs-lookup"><span data-stu-id="24b18-158">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24b18-159">请求</span><span class="sxs-lookup"><span data-stu-id="24b18-159">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "authenticationmethodsroot_usersregisteredbyfeature"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')
```


### <a name="response"></a><span data-ttu-id="24b18-160">响应</span><span class="sxs-lookup"><span data-stu-id="24b18-160">Response</span></span>
<span data-ttu-id="24b18-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="24b18-161">**Note:** The response object shown here might be shortened for readability.</span></span>
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
            "feature": "passwordlessRegistered",
            "userCount": 323
        },
        {
            "feature": "mfaCapable",
            "userCount": 3345
        }
    ]
}
```