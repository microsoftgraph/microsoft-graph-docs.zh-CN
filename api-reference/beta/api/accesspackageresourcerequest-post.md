---
title: 创建 accessPackageResourceRequest
description: 创建新的 accessPackageResourceRequest。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 46b40c4650890db6a506fce0c8422cea07a4f5c1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871745"
---
# <a name="create-accesspackageresourcerequest"></a><span data-ttu-id="88a8a-103">创建 accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="88a8a-103">Create accessPackageResourceRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88a8a-104">创建一个新的[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)对象，以请求将资源添加到访问包目录。</span><span class="sxs-lookup"><span data-stu-id="88a8a-104">Create a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object to request the addition of a resource to an access package catalog.</span></span>

## <a name="permissions"></a><span data-ttu-id="88a8a-105">权限</span><span class="sxs-lookup"><span data-stu-id="88a8a-105">Permissions</span></span>

<span data-ttu-id="88a8a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88a8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="88a8a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="88a8a-108">Permission type</span></span>                        | <span data-ttu-id="88a8a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88a8a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="88a8a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88a8a-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="88a8a-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88a8a-111">EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="88a8a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88a8a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88a8a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="88a8a-113">Not supported.</span></span> |
| <span data-ttu-id="88a8a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="88a8a-114">Application</span></span>                            | <span data-ttu-id="88a8a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="88a8a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="88a8a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88a8a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## <a name="request-headers"></a><span data-ttu-id="88a8a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="88a8a-117">Request headers</span></span>

| <span data-ttu-id="88a8a-118">名称</span><span class="sxs-lookup"><span data-stu-id="88a8a-118">Name</span></span>          | <span data-ttu-id="88a8a-119">说明</span><span class="sxs-lookup"><span data-stu-id="88a8a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="88a8a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="88a8a-120">Authorization</span></span> | <span data-ttu-id="88a8a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88a8a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="88a8a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88a8a-123">Content-Type</span></span>  | <span data-ttu-id="88a8a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="88a8a-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="88a8a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="88a8a-126">Request body</span></span>

<span data-ttu-id="88a8a-127">在请求正文中，提供[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88a8a-127">In the request body, supply a JSON representation of an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.</span></span> <span data-ttu-id="88a8a-128">将`accessPackageResource`与[accessPackageResource](../resources/accesspackageresource.md)对象的关系作为请求的一部分包括在内。</span><span class="sxs-lookup"><span data-stu-id="88a8a-128">Include the `accessPackageResource` relationship with an [accessPackageResource](../resources/accesspackageresource.md) object as part of the request.</span></span>

<span data-ttu-id="88a8a-129">若`accessPackageResource`要将 Azure AD 组作为资源添加到目录，则中的**originSystem**属性的值应为**AadGroup** ， **originId**的值是组的标识符。</span><span class="sxs-lookup"><span data-stu-id="88a8a-129">To add an Azure AD group as a resource to a catalog, the value of the **originSystem** property within the `accessPackageResource` should be **AadGroup** and the value of the **originId** is the identifier of the group.</span></span>


## <a name="response"></a><span data-ttu-id="88a8a-130">响应</span><span class="sxs-lookup"><span data-stu-id="88a8a-130">Response</span></span>

<span data-ttu-id="88a8a-131">如果成功，此方法在响应正文中返回一个200系列响应代码和一个新的[accessPackageResourceRequest](../resources/accesspackageresourcerequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="88a8a-131">If successful, this method returns a 200-series response code and a new [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="88a8a-132">示例</span><span class="sxs-lookup"><span data-stu-id="88a8a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="88a8a-133">请求</span><span class="sxs-lookup"><span data-stu-id="88a8a-133">Request</span></span>

<span data-ttu-id="88a8a-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="88a8a-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-type: application/json

{
  "catalogId":"26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "requestType": "AdminAdd",
  "justification": "",
  "accessPackageResource": {
     "displayName": "Sales",
     "description": "https://contoso.sharepoint.com/sites/Sales",
     "url": "https://contoso.sharepoint.com/sites/Sales",
     "resourceType": "SharePoint Online Site",
     "originId": "https://contoso.sharepoint.com/sites/Sales",
     "originSystem": "SharePointOnline"
  }
}
```

### <a name="response"></a><span data-ttu-id="88a8a-135">响应</span><span class="sxs-lookup"><span data-stu-id="88a8a-135">Response</span></span>

<span data-ttu-id="88a8a-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="88a8a-136">The following is an example of the response.</span></span>

> <span data-ttu-id="88a8a-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="88a8a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResourceRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
  "isValidationOnly": false,
  "justification": "",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "requestType": "AdminAdd"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageResourceRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
