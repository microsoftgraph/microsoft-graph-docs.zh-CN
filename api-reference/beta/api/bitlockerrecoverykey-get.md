---
title: 获取 bitlockerRecoveryKey
description: 检索 bitlockerRecoveryKey 对象的属性和关系。
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d55f1889a8134196760b133827bee2ec8c82b20e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944361"
---
# <a name="get-bitlockerrecoverykey"></a><span data-ttu-id="63d52-103">获取 bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="63d52-103">Get bitlockerRecoveryKey</span></span>
<span data-ttu-id="63d52-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63d52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63d52-105">检索 [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="63d52-105">Retrieve the properties and relationships of a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object.</span></span> 

<span data-ttu-id="63d52-106">默认情况下，此操作不会返回表示实际恢复密钥的 key 属性。</span><span class="sxs-lookup"><span data-stu-id="63d52-106">By default, this operation does not return the **key** property that represents the actual recovery key.</span></span> <span data-ttu-id="63d52-107">若要在 **响应中包括 key** 属性，请使用 `$select` OData 查询参数。</span><span class="sxs-lookup"><span data-stu-id="63d52-107">To include the **key** property in the response, use the `$select` OData query parameter.</span></span> <span data-ttu-id="63d52-108">包含 `$select` 查询参数将触发操作 Azure AD 审核，并生成审核日志。</span><span class="sxs-lookup"><span data-stu-id="63d52-108">Including the `$select` query parameter triggers an Azure AD audit of the operation and generates an audit log.</span></span> <span data-ttu-id="63d52-109">可以在"KeyManagement"类别下的 [Azure AD](/azure/active-directory/reports-monitoring/concept-audit-logs) 审核日志中找到日志。</span><span class="sxs-lookup"><span data-stu-id="63d52-109">You can find the log in [Azure AD audit logs](/azure/active-directory/reports-monitoring/concept-audit-logs) under the KeyManagement category.</span></span>

## <a name="permissions"></a><span data-ttu-id="63d52-110">权限</span><span class="sxs-lookup"><span data-stu-id="63d52-110">Permissions</span></span>
<span data-ttu-id="63d52-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63d52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63d52-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="63d52-113">Permission type</span></span>|<span data-ttu-id="63d52-114">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="63d52-114">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63d52-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63d52-115">Delegated (work or school account)</span></span>|<span data-ttu-id="63d52-116">BitLocker.ReadBasic.All、BitLocker.Read.All</span><span class="sxs-lookup"><span data-stu-id="63d52-116">BitLocker.ReadBasic.All, BitLocker.Read.All</span></span>|
|<span data-ttu-id="63d52-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63d52-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63d52-118">不支持</span><span class="sxs-lookup"><span data-stu-id="63d52-118">Not supported</span></span>|
|<span data-ttu-id="63d52-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="63d52-119">Application</span></span>|<span data-ttu-id="63d52-120">不支持</span><span class="sxs-lookup"><span data-stu-id="63d52-120">Not supported</span></span>|

><span data-ttu-id="63d52-121">**注意：** 对于允许应用代表登录用户获取 BitLockerRecoveryKey 资源的委派权限，租户管理员必须为用户分配以下角色之一，或者用户必须是最初备份 BitLocker 密钥的设备注册所有者： </span><span class="sxs-lookup"><span data-stu-id="63d52-121">**Note:** For delegated permissions to allow apps to get BitLockerRecoveryKey resources on behalf of the signed-in user, the tenant administrator must have assigned the user one of the following roles, or the user must be the **registered owner** of the device that the BitLocker key was originally backed up from:</span></span> 
* <span data-ttu-id="63d52-122">全局管理员</span><span class="sxs-lookup"><span data-stu-id="63d52-122">Global administrator</span></span>
* <span data-ttu-id="63d52-123">云设备管理员</span><span class="sxs-lookup"><span data-stu-id="63d52-123">Cloud device administrator</span></span>
* <span data-ttu-id="63d52-124">支持人员管理员</span><span class="sxs-lookup"><span data-stu-id="63d52-124">Helpdesk administrator</span></span>
* <span data-ttu-id="63d52-125">Intune 服务管理员</span><span class="sxs-lookup"><span data-stu-id="63d52-125">Intune service administrator</span></span>
* <span data-ttu-id="63d52-126">安全管理员</span><span class="sxs-lookup"><span data-stu-id="63d52-126">Security administrator</span></span>
* <span data-ttu-id="63d52-127">安全读者</span><span class="sxs-lookup"><span data-stu-id="63d52-127">Security reader</span></span>
* <span data-ttu-id="63d52-128">全局读取者</span><span class="sxs-lookup"><span data-stu-id="63d52-128">Global reader</span></span>

## <a name="http-request"></a><span data-ttu-id="63d52-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63d52-129">HTTP request</span></span>
<span data-ttu-id="63d52-130">在不返回 key 属性的情况下获取指定的 BitLocker **密钥：**</span><span class="sxs-lookup"><span data-stu-id="63d52-130">To get the specified BitLocker key without returning the **key** property:</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys/'{bitlockeryRecoveryKeyId}'
```

<span data-ttu-id="63d52-131">若要获取指定的 BitLocker 密钥（包括其 **key** 属性）：</span><span class="sxs-lookup"><span data-stu-id="63d52-131">To get the specified BitLocker key including its **key** property:</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys/'{bitlockeryRecoveryKeyId}'?$select=key
```

## <a name="optional-query-parameters"></a><span data-ttu-id="63d52-132">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="63d52-132">Optional query parameters</span></span>
<span data-ttu-id="63d52-133">此方法支持 `$select` OData 查询参数返回 **key** 属性。</span><span class="sxs-lookup"><span data-stu-id="63d52-133">This method supports the `$select` OData query parameter to return the **key** property.</span></span> <span data-ttu-id="63d52-134">有关详细信息，请参阅示例[2。](#example-2)</span><span class="sxs-lookup"><span data-stu-id="63d52-134">For details, see [Example 2](#example-2).</span></span> <span data-ttu-id="63d52-135">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="63d52-135">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="63d52-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="63d52-136">Request headers</span></span>
|<span data-ttu-id="63d52-137">名称</span><span class="sxs-lookup"><span data-stu-id="63d52-137">Name</span></span>|<span data-ttu-id="63d52-138">说明</span><span class="sxs-lookup"><span data-stu-id="63d52-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="63d52-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="63d52-139">Authorization</span></span>|<span data-ttu-id="63d52-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63d52-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="63d52-142">ocp-client-name</span><span class="sxs-lookup"><span data-stu-id="63d52-142">ocp-client-name</span></span>|<span data-ttu-id="63d52-143">执行 API 调用的客户端应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="63d52-143">Name of the client application performing the API call.</span></span> <span data-ttu-id="63d52-144">必填。</span><span class="sxs-lookup"><span data-stu-id="63d52-144">Required.</span></span>|
|<span data-ttu-id="63d52-145">ocp-client-version</span><span class="sxs-lookup"><span data-stu-id="63d52-145">ocp-client-version</span></span>|<span data-ttu-id="63d52-146">执行 API 调用的客户端应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="63d52-146">Version of the client application performing the API call.</span></span> <span data-ttu-id="63d52-147">必填。</span><span class="sxs-lookup"><span data-stu-id="63d52-147">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="63d52-148">请求正文</span><span class="sxs-lookup"><span data-stu-id="63d52-148">Request body</span></span>
<span data-ttu-id="63d52-149">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="63d52-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63d52-150">响应</span><span class="sxs-lookup"><span data-stu-id="63d52-150">Response</span></span>

<span data-ttu-id="63d52-151">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="63d52-151">If successful, this method returns a `200 OK` response code and a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="63d52-152">示例</span><span class="sxs-lookup"><span data-stu-id="63d52-152">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="63d52-153">示例 1</span><span class="sxs-lookup"><span data-stu-id="63d52-153">Example 1</span></span>
<span data-ttu-id="63d52-154">通过指定密钥 ID 获取 BitLocker **密钥**。本示例不返回 **key** 属性。</span><span class="sxs-lookup"><span data-stu-id="63d52-154">Get the BitLocker key by specifying the **key id**. This example does not return the **key** property.</span></span>

#### <a name="request"></a><span data-ttu-id="63d52-155">请求</span><span class="sxs-lookup"><span data-stu-id="63d52-155">Request</span></span>
<span data-ttu-id="63d52-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="63d52-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63d52-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="63d52-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"],
  "name": "get_bitlockerrecoverykey_3"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[<span data-ttu-id="63d52-158">C#</span><span class="sxs-lookup"><span data-stu-id="63d52-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63d52-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63d52-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63d52-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63d52-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63d52-161">Java</span><span class="sxs-lookup"><span data-stu-id="63d52-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="63d52-162">响应</span><span class="sxs-lookup"><span data-stu-id="63d52-162">Response</span></span>
<span data-ttu-id="63d52-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63d52-163">The following is an example of the response.</span></span>

<span data-ttu-id="63d52-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="63d52-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
    "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
    "createdDateTime": "2020-06-15T13:45:30.0000000Z",
    "volumeType": 1,
    "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
  }
}
```

### <a name="example-2"></a><span data-ttu-id="63d52-165">示例 2</span><span class="sxs-lookup"><span data-stu-id="63d52-165">Example 2</span></span>
<span data-ttu-id="63d52-166">通过指定密钥 ID 获取 **具有 key** 属性的 BitLocker **密钥**。</span><span class="sxs-lookup"><span data-stu-id="63d52-166">Get the BitLocker key with the **key** property by specifying the **key id**.</span></span>

#### <a name="request"></a><span data-ttu-id="63d52-167">请求</span><span class="sxs-lookup"><span data-stu-id="63d52-167">Request</span></span>
<span data-ttu-id="63d52-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="63d52-168">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63d52-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="63d52-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"],
  "name": "get_bitlockerrecoverykey_4"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/bitlocker/recoveryKeys/b465e4e8-e4e8-b465-e8e4-65b4e8e465b4?$select=key
```
# <a name="c"></a>[<span data-ttu-id="63d52-170">C#</span><span class="sxs-lookup"><span data-stu-id="63d52-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63d52-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63d52-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63d52-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63d52-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="63d52-173">Java</span><span class="sxs-lookup"><span data-stu-id="63d52-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="63d52-174">响应</span><span class="sxs-lookup"><span data-stu-id="63d52-174">Response</span></span>
<span data-ttu-id="63d52-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63d52-175">The following is an example of the response.</span></span>

<span data-ttu-id="63d52-176">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="63d52-176">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey"
}
-->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
    "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
    "createdDateTime": "String (timestamp)",
    "volumeType": 1,
    "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9",
    "key": "123456-231453-873456-213546-654678-765689-123456-324565"
  }
}
```
