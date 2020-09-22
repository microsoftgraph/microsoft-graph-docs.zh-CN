---
title: 列出 recoveryKeys
description: 获取 bitlockerRecoveryKey 对象及其属性的列表。
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0ceadccb9ce4fbfcfffab42d403054b95c90ae50
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47992620"
---
# <a name="list-recoverykeys"></a><span data-ttu-id="a4951-103">列出 recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="a4951-103">List recoveryKeys</span></span>
<span data-ttu-id="a4951-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4951-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4951-105">获取 [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="a4951-105">Get a list of the [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects and their properties.</span></span> 

<span data-ttu-id="a4951-106">此操作不会返回 **key** 属性。</span><span class="sxs-lookup"><span data-stu-id="a4951-106">This operation does not return the **key** property.</span></span> <span data-ttu-id="a4951-107">有关如何读取 **key** 属性的信息，请参阅 [Get bitlockerRecoveryKey](bitlockerrecoverykey-get.md)。</span><span class="sxs-lookup"><span data-stu-id="a4951-107">For information about how to read the **key** property, see [Get bitlockerRecoveryKey](bitlockerrecoverykey-get.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a4951-108">权限</span><span class="sxs-lookup"><span data-stu-id="a4951-108">Permissions</span></span>
<span data-ttu-id="a4951-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4951-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4951-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4951-111">Permission type</span></span>|<span data-ttu-id="a4951-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a4951-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4951-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4951-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4951-114">User.readbasic.all、所有 BitLocker。</span><span class="sxs-lookup"><span data-stu-id="a4951-114">BitLocker.ReadBasic.All, BitLocker.Read.All</span></span>|
|<span data-ttu-id="a4951-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4951-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4951-116">不支持</span><span class="sxs-lookup"><span data-stu-id="a4951-116">Not supported</span></span>|
|<span data-ttu-id="a4951-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4951-117">Application</span></span>|<span data-ttu-id="a4951-118">不支持</span><span class="sxs-lookup"><span data-stu-id="a4951-118">Not supported</span></span>|

><span data-ttu-id="a4951-119">**注意**：对于允许应用程序代表登录用户获取 BitLockerRecoveryKey 资源的委派权限，租户管理员必须已为用户分配以下角色之一，或者用户必须是上次备份 BitLocker 恢复密钥的设备的已注册所有者：</span><span class="sxs-lookup"><span data-stu-id="a4951-119">**Note**: For delegated permissions to allow apps to get BitLockerRecoveryKey resources on behalf of the signed-in user, the tenant administrator must have assigned the user one of the following roles, or the user must be the registered owner of the device that the BitLocker recovery key was originally backed up from:</span></span> 
* <span data-ttu-id="a4951-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a4951-120">Global administrator</span></span>
* <span data-ttu-id="a4951-121">云设备管理员</span><span class="sxs-lookup"><span data-stu-id="a4951-121">Cloud device administrator</span></span>
* <span data-ttu-id="a4951-122">支持人员管理员</span><span class="sxs-lookup"><span data-stu-id="a4951-122">Helpdesk administrator</span></span>
* <span data-ttu-id="a4951-123">Intune 服务管理员</span><span class="sxs-lookup"><span data-stu-id="a4951-123">Intune service administrator</span></span>
* <span data-ttu-id="a4951-124">安全管理员</span><span class="sxs-lookup"><span data-stu-id="a4951-124">Security administrator</span></span>
* <span data-ttu-id="a4951-125">安全读者</span><span class="sxs-lookup"><span data-stu-id="a4951-125">Security reader</span></span>
* <span data-ttu-id="a4951-126">全局读取者</span><span class="sxs-lookup"><span data-stu-id="a4951-126">Global reader</span></span>

## <a name="http-request"></a><span data-ttu-id="a4951-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4951-127">HTTP request</span></span>
<span data-ttu-id="a4951-128">若要获取租户中的 BitLocker 密钥列表，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="a4951-128">To get a list of BitLocker keys within the tenant:</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys
```

<span data-ttu-id="a4951-129">若要获取由 **设备 id**筛选的租户中的 BitLocker 密钥列表，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="a4951-129">To get a list of BitLocker keys within the tenant filtered by the **device id**:</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bitlocker/recoveryKeys?$filter=deviceId eq '{deviceId}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4951-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a4951-130">Optional query parameters</span></span>
<span data-ttu-id="a4951-131">此方法支持 `$filter` OData 查询参数按密钥最近备份到的 **设备 id** 筛选结果。</span><span class="sxs-lookup"><span data-stu-id="a4951-131">This method supports the `$filter` OData query parameter to filter results by the **device id** the key was most recently backed up to.</span></span> <span data-ttu-id="a4951-132">有关详细信息，请参阅 [示例 2](#example-2)。</span><span class="sxs-lookup"><span data-stu-id="a4951-132">For details, see [Example 2](#example-2).</span></span> <span data-ttu-id="a4951-133">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a4951-133">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="a4951-134">响应还可能包含 `odata.nextLink` ，可用于对结果集进行分页。</span><span class="sxs-lookup"><span data-stu-id="a4951-134">The response might also contain an `odata.nextLink`, which you can use to page through the result set.</span></span> <span data-ttu-id="a4951-135">有关详细信息，请参阅 [分页 Microsoft Graph 数据](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="a4951-135">For details, see [Paging Microsoft Graph data](/graph/paging).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4951-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4951-136">Request headers</span></span>
|<span data-ttu-id="a4951-137">名称</span><span class="sxs-lookup"><span data-stu-id="a4951-137">Name</span></span>|<span data-ttu-id="a4951-138">说明</span><span class="sxs-lookup"><span data-stu-id="a4951-138">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a4951-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4951-139">Authorization</span></span>|<span data-ttu-id="a4951-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4951-p105">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a4951-142">ocp-客户端-名称</span><span class="sxs-lookup"><span data-stu-id="a4951-142">ocp-client-name</span></span>|<span data-ttu-id="a4951-143">执行 API 调用的客户端应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="a4951-143">Name of the client application performing the API call.</span></span> <span data-ttu-id="a4951-144">必需。</span><span class="sxs-lookup"><span data-stu-id="a4951-144">Required.</span></span>|
|<span data-ttu-id="a4951-145">ocp-客户端-版本</span><span class="sxs-lookup"><span data-stu-id="a4951-145">ocp-client-version</span></span>|<span data-ttu-id="a4951-146">执行 API 调用的客户端应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="a4951-146">Version of the client application performing the API call.</span></span> <span data-ttu-id="a4951-147">必需。</span><span class="sxs-lookup"><span data-stu-id="a4951-147">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4951-148">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4951-148">Request body</span></span>
<span data-ttu-id="a4951-149">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a4951-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4951-150">响应</span><span class="sxs-lookup"><span data-stu-id="a4951-150">Response</span></span>

<span data-ttu-id="a4951-151">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a4951-151">If successful, this method returns a `200 OK` response code and a collection of [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4951-152">示例</span><span class="sxs-lookup"><span data-stu-id="a4951-152">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="a4951-153">示例 1</span><span class="sxs-lookup"><span data-stu-id="a4951-153">Example 1</span></span>
<span data-ttu-id="a4951-154">检索租户中的 BitLocker 密钥列表。</span><span class="sxs-lookup"><span data-stu-id="a4951-154">Retrieve a list of BitLocker keys in the tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="a4951-155">请求</span><span class="sxs-lookup"><span data-stu-id="a4951-155">Request</span></span>
<span data-ttu-id="a4951-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a4951-156">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```


#### <a name="response"></a><span data-ttu-id="a4951-157">响应</span><span class="sxs-lookup"><span data-stu-id="a4951-157">Response</span></span>
<span data-ttu-id="a4951-158">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="a4951-158">The following is an example of the response.</span></span>

<span data-ttu-id="a4951-159">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a4951-159">**Note:** The response object shown here might be shortened for readability.</span></span>
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
### <a name="example-2"></a><span data-ttu-id="a4951-160">示例 2</span><span class="sxs-lookup"><span data-stu-id="a4951-160">Example 2</span></span>
<span data-ttu-id="a4951-161">检索按 **设备 id**筛选的 BitLocker 密钥列表。</span><span class="sxs-lookup"><span data-stu-id="a4951-161">Retrieve a list of BitLocker keys filtered by **device id**.</span></span>

#### <a name="request"></a><span data-ttu-id="a4951-162">请求</span><span class="sxs-lookup"><span data-stu-id="a4951-162">Request</span></span>
<span data-ttu-id="a4951-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a4951-163">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleIds": ["1ab40ab2-32a8-4b00-b6b5-ba724e407de9"],
  "name": "get_bitlockerrecoverykey"
}
-->
``` http
GET https://graph.microsoft.com/beta/bitlocker/recoveryKeys?$filter=deviceId eq '1ab40ab2-32a8-4b00-b6b5-ba724e407de9'
ocp-client-name: "My Friendly Client"
ocp-client-version: "1.2"
```


#### <a name="response"></a><span data-ttu-id="a4951-164">响应</span><span class="sxs-lookup"><span data-stu-id="a4951-164">Response</span></span>
<span data-ttu-id="a4951-165">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="a4951-165">The following is an example of the response.</span></span>

<span data-ttu-id="a4951-166">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a4951-166">**Note:** The response object shown here might be shortened for readability.</span></span>
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
