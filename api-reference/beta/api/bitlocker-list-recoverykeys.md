---
title: 列出 recoveryKeys
description: 获取 bitlockerRecoveryKey 对象及其属性的列表。
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 7e4fbd5a2a4c1b76ca985cb17e5c6799cb4f41c5
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240971"
---
# <a name="list-recoverykeys"></a><span data-ttu-id="aff02-103">列出 recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="aff02-103">List recoveryKeys</span></span>
<span data-ttu-id="aff02-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aff02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aff02-105">获取 [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="aff02-105">Get a list of the [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects and their properties.</span></span> 

<span data-ttu-id="aff02-106">此操作不会返回 **key** 属性。</span><span class="sxs-lookup"><span data-stu-id="aff02-106">This operation does not return the **key** property.</span></span> <span data-ttu-id="aff02-107">若要了解如何读取 key 属性 **，请参阅** 获取 [bitlockerRecoveryKey](bitlockerrecoverykey-get.md)。</span><span class="sxs-lookup"><span data-stu-id="aff02-107">For information about how to read the **key** property, see [Get bitlockerRecoveryKey](bitlockerrecoverykey-get.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="aff02-108">权限</span><span class="sxs-lookup"><span data-stu-id="aff02-108">Permissions</span></span>
<span data-ttu-id="aff02-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aff02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aff02-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="aff02-111">Permission type</span></span>|<span data-ttu-id="aff02-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aff02-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aff02-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aff02-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aff02-114">BitLockerKey.ReadBasic.All、BitLockerKey.Read.All</span><span class="sxs-lookup"><span data-stu-id="aff02-114">BitLockerKey.ReadBasic.All, BitLockerKey.Read.All</span></span>|
|<span data-ttu-id="aff02-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aff02-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aff02-116">不支持</span><span class="sxs-lookup"><span data-stu-id="aff02-116">Not supported</span></span>|
|<span data-ttu-id="aff02-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="aff02-117">Application</span></span>|<span data-ttu-id="aff02-118">不支持</span><span class="sxs-lookup"><span data-stu-id="aff02-118">Not supported</span></span>|

><span data-ttu-id="aff02-119">**注意**：对于允许应用代表登录用户获取 BitLockerRecoveryKey 资源的委派权限，租户管理员必须已向用户分配以下角色之一，或者用户必须是最初备份 BitLocker 恢复密钥的设备注册所有者：</span><span class="sxs-lookup"><span data-stu-id="aff02-119">**Note**: For delegated permissions to allow apps to get BitLockerRecoveryKey resources on behalf of the signed-in user, the tenant administrator must have assigned the user one of the following roles, or the user must be the registered owner of the device that the BitLocker recovery key was originally backed up from:</span></span> 
* <span data-ttu-id="aff02-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="aff02-120">Global administrator</span></span>
* <span data-ttu-id="aff02-121">云设备管理员</span><span class="sxs-lookup"><span data-stu-id="aff02-121">Cloud device administrator</span></span>
* <span data-ttu-id="aff02-122">支持人员管理员</span><span class="sxs-lookup"><span data-stu-id="aff02-122">Helpdesk administrator</span></span>
* <span data-ttu-id="aff02-123">Intune 服务管理员</span><span class="sxs-lookup"><span data-stu-id="aff02-123">Intune service administrator</span></span>
* <span data-ttu-id="aff02-124">安全管理员</span><span class="sxs-lookup"><span data-stu-id="aff02-124">Security administrator</span></span>
* <span data-ttu-id="aff02-125">安全读者</span><span class="sxs-lookup"><span data-stu-id="aff02-125">Security reader</span></span>
* <span data-ttu-id="aff02-126">全局读取者</span><span class="sxs-lookup"><span data-stu-id="aff02-126">Global reader</span></span>

## <a name="http-request"></a><span data-ttu-id="aff02-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aff02-127">HTTP request</span></span>
<span data-ttu-id="aff02-128">若要获取租户内BitLocker密钥的列表：</span><span class="sxs-lookup"><span data-stu-id="aff02-128">To get a list of BitLocker keys within the tenant:</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys
```

<span data-ttu-id="aff02-129">若要获取租户中BitLocker设备 ID 筛选的密钥 **列表**：</span><span class="sxs-lookup"><span data-stu-id="aff02-129">To get a list of BitLocker keys within the tenant filtered by the **device id**:</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /informationProtection/bitlocker/recoveryKeys?$filter=deviceId eq '{deviceId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aff02-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aff02-130">Optional query parameters</span></span>
<span data-ttu-id="aff02-131">此方法支持 OData 查询参数按最近备份密钥的设备 `$filter` **ID** 筛选结果。</span><span class="sxs-lookup"><span data-stu-id="aff02-131">This method supports the `$filter` OData query parameter to filter results by the **device id** the key was most recently backed up to.</span></span> <span data-ttu-id="aff02-132">此方法不支持 `$top` 筛选器。</span><span class="sxs-lookup"><span data-stu-id="aff02-132">This method does not support the `$top` filter.</span></span> <span data-ttu-id="aff02-133">有关详细信息，请参阅示例[2。](#example-2)</span><span class="sxs-lookup"><span data-stu-id="aff02-133">For details, see [Example 2](#example-2).</span></span> <span data-ttu-id="aff02-134">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="aff02-134">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="aff02-135">该响应可能还包含 `odata.nextLink` ，您可以使用 它分页浏览结果集。</span><span class="sxs-lookup"><span data-stu-id="aff02-135">The response might also contain an `odata.nextLink`, which you can use to page through the result set.</span></span> <span data-ttu-id="aff02-136">有关详细信息，请参阅[分页 Microsoft Graph数据](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="aff02-136">For details, see [Paging Microsoft Graph data](/graph/paging).</span></span>

## <a name="request-headers"></a><span data-ttu-id="aff02-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="aff02-137">Request headers</span></span>
|<span data-ttu-id="aff02-138">名称</span><span class="sxs-lookup"><span data-stu-id="aff02-138">Name</span></span>|<span data-ttu-id="aff02-139">说明</span><span class="sxs-lookup"><span data-stu-id="aff02-139">Description</span></span>|
|:---|:---|
|<span data-ttu-id="aff02-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="aff02-140">Authorization</span></span>|<span data-ttu-id="aff02-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aff02-p105">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="aff02-143">ocp-client-name</span><span class="sxs-lookup"><span data-stu-id="aff02-143">ocp-client-name</span></span>|<span data-ttu-id="aff02-144">执行 API 调用的客户端应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="aff02-144">Name of the client application performing the API call.</span></span> <span data-ttu-id="aff02-145">必需。</span><span class="sxs-lookup"><span data-stu-id="aff02-145">Required.</span></span>|
|<span data-ttu-id="aff02-146">ocp-client-version</span><span class="sxs-lookup"><span data-stu-id="aff02-146">ocp-client-version</span></span>|<span data-ttu-id="aff02-147">执行 API 调用的客户端应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="aff02-147">Version of the client application performing the API call.</span></span> <span data-ttu-id="aff02-148">必需。</span><span class="sxs-lookup"><span data-stu-id="aff02-148">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aff02-149">请求正文</span><span class="sxs-lookup"><span data-stu-id="aff02-149">Request body</span></span>
<span data-ttu-id="aff02-150">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aff02-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aff02-151">响应</span><span class="sxs-lookup"><span data-stu-id="aff02-151">Response</span></span>

<span data-ttu-id="aff02-152">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="aff02-152">If successful, this method returns a `200 OK` response code and a collection of [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aff02-153">示例</span><span class="sxs-lookup"><span data-stu-id="aff02-153">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="aff02-154">示例 1</span><span class="sxs-lookup"><span data-stu-id="aff02-154">Example 1</span></span>
<span data-ttu-id="aff02-155">检索租户BitLocker密钥的列表。</span><span class="sxs-lookup"><span data-stu-id="aff02-155">Retrieve a list of BitLocker keys in the tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="aff02-156">请求</span><span class="sxs-lookup"><span data-stu-id="aff02-156">Request</span></span>
<span data-ttu-id="aff02-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aff02-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aff02-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="aff02-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bitlockerrecoverykey_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/bitlocker/recoveryKeys
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[<span data-ttu-id="aff02-159">C#</span><span class="sxs-lookup"><span data-stu-id="aff02-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aff02-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aff02-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aff02-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aff02-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aff02-162">Java</span><span class="sxs-lookup"><span data-stu-id="aff02-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="aff02-163">响应</span><span class="sxs-lookup"><span data-stu-id="aff02-163">Response</span></span>
<span data-ttu-id="aff02-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aff02-164">The following is an example of the response.</span></span>

<span data-ttu-id="aff02-165">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aff02-165">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.bitlockerRecoveryKey)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": 1,
      "deviceId": "2ef04ef1-23b0-2e00-a3a5-ab345e567ab6"
    },
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "6a30ed7b-247b-4d26-86b5-2f405e55ea42",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": 1,
      "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
    }
  ]
}
```
### <a name="example-2"></a><span data-ttu-id="aff02-166">示例 2</span><span class="sxs-lookup"><span data-stu-id="aff02-166">Example 2</span></span>
<span data-ttu-id="aff02-167">检索按设备BitLocker筛选的密钥 **列表**。</span><span class="sxs-lookup"><span data-stu-id="aff02-167">Retrieve a list of BitLocker keys filtered by **device id**.</span></span>

#### <a name="request"></a><span data-ttu-id="aff02-168">请求</span><span class="sxs-lookup"><span data-stu-id="aff02-168">Request</span></span>
<span data-ttu-id="aff02-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="aff02-169">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aff02-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="aff02-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleIds": ["1ab40ab2-32a8-4b00-b6b5-ba724e407de9"],
  "name": "get_bitlockerrecoverykey_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/informationProtection/bitlocker/recoveryKeys?$filter=deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```
# <a name="c"></a>[<span data-ttu-id="aff02-171">C#</span><span class="sxs-lookup"><span data-stu-id="aff02-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bitlockerrecoverykey-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aff02-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aff02-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bitlockerrecoverykey-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aff02-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aff02-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bitlockerrecoverykey-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aff02-174">Java</span><span class="sxs-lookup"><span data-stu-id="aff02-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bitlockerrecoverykey-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="aff02-175">响应</span><span class="sxs-lookup"><span data-stu-id="aff02-175">Response</span></span>
<span data-ttu-id="aff02-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aff02-176">The following is an example of the response.</span></span>

<span data-ttu-id="aff02-177">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aff02-177">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.bitlockerRecoveryKey)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
      "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
      "createdDateTime": "2020-06-15T13:45:30.0000000Z",
      "volumeType": 1,
      "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9"
    }
  ]
}
```
