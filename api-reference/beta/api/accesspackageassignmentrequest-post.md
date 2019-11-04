---
title: 创建 accessPackageAssignmentRequest
description: 创建新的 accessPackageAssignmentRequest。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 90530cb12ece487c440fee2f1283dec787cda709
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935239"
---
# <a name="create-accesspackageassignmentrequest"></a><span data-ttu-id="58d1d-103">创建 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="58d1d-103">Create accessPackageAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58d1d-104">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，创建一个新的[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="58d1d-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), create a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="58d1d-105">权限</span><span class="sxs-lookup"><span data-stu-id="58d1d-105">Permissions</span></span>

<span data-ttu-id="58d1d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="58d1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58d1d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="58d1d-108">Permission type</span></span>                        | <span data-ttu-id="58d1d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="58d1d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="58d1d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="58d1d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="58d1d-111">EntitlementManagement</span><span class="sxs-lookup"><span data-stu-id="58d1d-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="58d1d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="58d1d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58d1d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="58d1d-113">Not supported.</span></span> |
| <span data-ttu-id="58d1d-114">Application</span><span class="sxs-lookup"><span data-stu-id="58d1d-114">Application</span></span>                            | <span data-ttu-id="58d1d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="58d1d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="58d1d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="58d1d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="request-headers"></a><span data-ttu-id="58d1d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="58d1d-117">Request headers</span></span>

| <span data-ttu-id="58d1d-118">名称</span><span class="sxs-lookup"><span data-stu-id="58d1d-118">Name</span></span>          | <span data-ttu-id="58d1d-119">说明</span><span class="sxs-lookup"><span data-stu-id="58d1d-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="58d1d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="58d1d-120">Authorization</span></span> | <span data-ttu-id="58d1d-121">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="58d1d-121">Bearer \{token\}.</span></span> <span data-ttu-id="58d1d-122">必填。</span><span class="sxs-lookup"><span data-stu-id="58d1d-122">Required.</span></span> |
| <span data-ttu-id="58d1d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="58d1d-123">Content-Type</span></span>  | <span data-ttu-id="58d1d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="58d1d-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="58d1d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="58d1d-125">Request body</span></span>

<span data-ttu-id="58d1d-126">在请求正文中，提供[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58d1d-126">In the request body, supply a JSON representation of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="58d1d-127">响应</span><span class="sxs-lookup"><span data-stu-id="58d1d-127">Response</span></span>

<span data-ttu-id="58d1d-128">如果成功，此方法在响应正文中返回一个200系列响应代码和一个新的[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="58d1d-128">If successful, this method returns a 200-series response code and a new [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="58d1d-129">示例</span><span class="sxs-lookup"><span data-stu-id="58d1d-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="58d1d-130">请求</span><span class="sxs-lookup"><span data-stu-id="58d1d-130">Request</span></span>

<span data-ttu-id="58d1d-131">下面是一个直接分配请求的示例。</span><span class="sxs-lookup"><span data-stu-id="58d1d-131">The following is an example of the request for a direct assignment.</span></span>  <span data-ttu-id="58d1d-132">的`targetID`值是要分配的用户的对象 ID， `accessPackageId`是所需的访问包的值，并且值`assignmentPolicyId`是该访问包中的直接分配策略。</span><span class="sxs-lookup"><span data-stu-id="58d1d-132">The value of the `targetID` is the object ID of a user being assigned, the value of the `accessPackageId` is the desired access package, and the value of `assignmentPolicyId` is a direct assignment policy in that access package.</span></span>
 
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentrequest_from_accesspackageassignmentrequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
Content-type: application/json

{
  "requestType": "AdminAdd",
  "accessPackageAssignment":{
     "targetId":"46184453-e63b-4f20-86c2-c557ed5d5df9",
     "assignmentPolicyId":"2264bf65-76ba-417b-a27d-54d291f0cbc8",
     "accessPackageId":"a914b616-e04e-476b-aa37-91038f0b165b"
  }
}
```

### <a name="response"></a><span data-ttu-id="58d1d-133">响应</span><span class="sxs-lookup"><span data-stu-id="58d1d-133">Response</span></span>

<span data-ttu-id="58d1d-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="58d1d-134">The following is an example of the response.</span></span>

> <span data-ttu-id="58d1d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="58d1d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{

  "id": "7e382d02-4454-436b-b700-59c7dd77f466",
  "requestType": "AdminAdd",
  "requestState": "Submitted",
  "requestStatus": "Accepted",
  "isValidationOnly": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->