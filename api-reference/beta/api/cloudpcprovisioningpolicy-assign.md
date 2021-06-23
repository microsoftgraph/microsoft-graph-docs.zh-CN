---
title: cloudPcProvisioningPolicy：assign
description: 将云电脑预配策略分配给你的组。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 46d9877b8a17056aee84f1216c4f38227bdc097c
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082193"
---
# <a name="cloudpcprovisioningpolicy-assign"></a><span data-ttu-id="05ff4-103">cloudPcProvisioningPolicy：assign</span><span class="sxs-lookup"><span data-stu-id="05ff4-103">cloudPcProvisioningPolicy: assign</span></span>

<span data-ttu-id="05ff4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05ff4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05ff4-105">将 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 分配给用户组。</span><span class="sxs-lookup"><span data-stu-id="05ff4-105">Assign [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) to user groups.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="05ff4-106">权限</span><span class="sxs-lookup"><span data-stu-id="05ff4-106">Permissions</span></span>

<span data-ttu-id="05ff4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05ff4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05ff4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="05ff4-109">Permission type</span></span>|<span data-ttu-id="05ff4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05ff4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05ff4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05ff4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05ff4-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05ff4-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="05ff4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05ff4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05ff4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="05ff4-114">Not supported.</span></span>|
|<span data-ttu-id="05ff4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="05ff4-115">Application</span></span>|<span data-ttu-id="05ff4-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05ff4-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05ff4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05ff4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="05ff4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="05ff4-118">Request headers</span></span>

|<span data-ttu-id="05ff4-119">名称</span><span class="sxs-lookup"><span data-stu-id="05ff4-119">Name</span></span>|<span data-ttu-id="05ff4-120">说明</span><span class="sxs-lookup"><span data-stu-id="05ff4-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="05ff4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="05ff4-121">Authorization</span></span>|<span data-ttu-id="05ff4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="05ff4-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="05ff4-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05ff4-124">Content-Type</span></span>|<span data-ttu-id="05ff4-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="05ff4-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="05ff4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="05ff4-127">Request body</span></span>

<span data-ttu-id="05ff4-128">在请求正文中，提供 [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05ff4-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) object.</span></span>

|<span data-ttu-id="05ff4-129">参数</span><span class="sxs-lookup"><span data-stu-id="05ff4-129">Parameter</span></span>|<span data-ttu-id="05ff4-130">类型</span><span class="sxs-lookup"><span data-stu-id="05ff4-130">Type</span></span>|<span data-ttu-id="05ff4-131">说明</span><span class="sxs-lookup"><span data-stu-id="05ff4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05ff4-132">assignments</span><span class="sxs-lookup"><span data-stu-id="05ff4-132">assignments</span></span>|<span data-ttu-id="05ff4-133">[cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="05ff4-133">[cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) collection</span></span> | <span data-ttu-id="05ff4-134">要分配给相应目标组的云电脑预配策略资源的集合。</span><span class="sxs-lookup"><span data-stu-id="05ff4-134">The collection of cloud PC provisioning policy resources each to be assigned to the corresponding target group.</span></span> <span data-ttu-id="05ff4-135">目前Microsoft 365 Azure AD 中的安全组和安全组。</span><span class="sxs-lookup"><span data-stu-id="05ff4-135">Only Microsoft 365 groups and security groups in Azure AD are currently supported.</span></span> |

## <a name="response"></a><span data-ttu-id="05ff4-136">响应</span><span class="sxs-lookup"><span data-stu-id="05ff4-136">Response</span></span>

<span data-ttu-id="05ff4-137">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="05ff4-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="05ff4-138">示例</span><span class="sxs-lookup"><span data-stu-id="05ff4-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="05ff4-139">请求</span><span class="sxs-lookup"><span data-stu-id="05ff4-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="05ff4-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="05ff4-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "assign_cloudpcprovisioningpolicy",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicyAssignment",
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}/assign
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicyAssignment",
  "assignments": [
    {
      "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
      "target":{
        "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
        "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
        }
    }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="05ff4-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05ff4-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/assign-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05ff4-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05ff4-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/assign-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="05ff4-143">响应</span><span class="sxs-lookup"><span data-stu-id="05ff4-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
