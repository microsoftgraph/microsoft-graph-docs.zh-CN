---
title: 创建 emailAuthenticationMethod
description: 创建新的 emailAuthenticationMethod 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9d00dd6d8197be3817f1129d7a8e83522eb71634
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418257"
---
# <a name="create-emailauthenticationmethod"></a><span data-ttu-id="51b68-103">创建 emailAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="51b68-103">Create emailAuthenticationMethod</span></span>
<span data-ttu-id="51b68-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51b68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51b68-105">设置用户的 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51b68-105">Set a user's [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object.</span></span> <span data-ttu-id="51b68-106">电子邮件身份验证是一种自助密码重置方法。</span><span class="sxs-lookup"><span data-stu-id="51b68-106">Email authentication is a self-service password reset method.</span></span> <span data-ttu-id="51b68-107">一个用户可能只有一种电子邮件身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="51b68-107">A user may only have one email authentication method.</span></span>

## <a name="permissions"></a><span data-ttu-id="51b68-108">权限</span><span class="sxs-lookup"><span data-stu-id="51b68-108">Permissions</span></span>
<span data-ttu-id="51b68-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51b68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51b68-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="51b68-111">Permission type</span></span>|<span data-ttu-id="51b68-112">从最高特权到最少特权) 对自己 (的权限</span><span class="sxs-lookup"><span data-stu-id="51b68-112">Permissions acting on self (from most to least privileged)</span></span>|<span data-ttu-id="51b68-113">对其他人进行操作的权限 (从至少到最高特权) </span><span class="sxs-lookup"><span data-stu-id="51b68-113">Permissions acting on others (from least to most privileged)</span></span>|
|:---|:---|:--|
|<span data-ttu-id="51b68-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51b68-114">Delegated (work or school account)</span></span>|<span data-ttu-id="51b68-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="51b68-115">Not supported.</span></span>|<span data-ttu-id="51b68-116">UserAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="51b68-116">UserAuthenticationMethod.ReadWrite.All</span></span>
|<span data-ttu-id="51b68-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51b68-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51b68-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="51b68-118">Not supported.</span></span>|<span data-ttu-id="51b68-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="51b68-119">Not supported.</span></span>
|<span data-ttu-id="51b68-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="51b68-120">Application</span></span>|<span data-ttu-id="51b68-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="51b68-121">Not supported.</span></span>|<span data-ttu-id="51b68-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="51b68-122">Not supported.</span></span>

<span data-ttu-id="51b68-123">对于在其他用户上执行管理的委派方案，管理员需要以下 [角色](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)之一：</span><span class="sxs-lookup"><span data-stu-id="51b68-123">For delegated scenarios where an admin is acting on another user, the admin needs one of the following [roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>

* <span data-ttu-id="51b68-124">全局管理员</span><span class="sxs-lookup"><span data-stu-id="51b68-124">Global admin</span></span>
* <span data-ttu-id="51b68-125">全局读取者</span><span class="sxs-lookup"><span data-stu-id="51b68-125">Global reader</span></span>
* <span data-ttu-id="51b68-126">特权身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="51b68-126">Privileged authentication admin</span></span>
* <span data-ttu-id="51b68-127">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="51b68-127">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="51b68-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51b68-128">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{id | userPrincipalName}/authentication/emailMethods
```

## <a name="request-headers"></a><span data-ttu-id="51b68-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="51b68-129">Request headers</span></span>
|<span data-ttu-id="51b68-130">名称</span><span class="sxs-lookup"><span data-stu-id="51b68-130">Name</span></span>|<span data-ttu-id="51b68-131">说明</span><span class="sxs-lookup"><span data-stu-id="51b68-131">Description</span></span>|
|:---|:---|
|<span data-ttu-id="51b68-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="51b68-132">Authorization</span></span>|<span data-ttu-id="51b68-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="51b68-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="51b68-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51b68-135">Content-Type</span></span>|<span data-ttu-id="51b68-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="51b68-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="51b68-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="51b68-138">Request body</span></span>
<span data-ttu-id="51b68-139">在请求正文中，提供具有所需电子邮件地址的 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51b68-139">In the request body, supply a JSON representation of the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object with the desired email address.</span></span>

<span data-ttu-id="51b68-140">下表显示创建 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="51b68-140">The following table shows the properties that are required when you create the [emailAuthenticationMethod](../resources/emailauthenticationmethod.md).</span></span>

|<span data-ttu-id="51b68-141">属性</span><span class="sxs-lookup"><span data-stu-id="51b68-141">Property</span></span>|<span data-ttu-id="51b68-142">类型</span><span class="sxs-lookup"><span data-stu-id="51b68-142">Type</span></span>|<span data-ttu-id="51b68-143">说明</span><span class="sxs-lookup"><span data-stu-id="51b68-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51b68-144">emailAddress</span><span class="sxs-lookup"><span data-stu-id="51b68-144">emailAddress</span></span>|<span data-ttu-id="51b68-145">String</span><span class="sxs-lookup"><span data-stu-id="51b68-145">String</span></span>|<span data-ttu-id="51b68-146">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="51b68-146">Email address</span></span>|



## <a name="response"></a><span data-ttu-id="51b68-147">响应</span><span class="sxs-lookup"><span data-stu-id="51b68-147">Response</span></span>

<span data-ttu-id="51b68-148">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的 [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51b68-148">If successful, this method returns a `201 Created` response code and a new [emailAuthenticationMethod](../resources/emailauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51b68-149">示例</span><span class="sxs-lookup"><span data-stu-id="51b68-149">Examples</span></span>

### <a name="request"></a><span data-ttu-id="51b68-150">请求</span><span class="sxs-lookup"><span data-stu-id="51b68-150">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_emailauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/emailMethods
Content-Type: application/json

{
  "emailAddress": "kim@contoso.com"
}
```


### <a name="response"></a><span data-ttu-id="51b68-151">响应</span><span class="sxs-lookup"><span data-stu-id="51b68-151">Response</span></span>
<span data-ttu-id="51b68-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="51b68-152">The following is an example of the response.</span></span>

<span data-ttu-id="51b68-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="51b68-153">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "id": "3ddfcfc8-9383-446f-83cc-3ab9be4be18f",
  "emailAddress": "kim@contoso.com"
}
```
