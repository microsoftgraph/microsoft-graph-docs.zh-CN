---
title: 获取 informationProtectionLabel
description: 检索指定的 informationProtectionLabel 对象的属性和关系。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 89929cbb46de3d70990d0c21abe1fde85848e0b3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001463"
---
# <a name="get-informationprotectionlabel"></a><span data-ttu-id="bda46-103">获取 informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="bda46-103">Get informationProtectionLabel</span></span>

<span data-ttu-id="bda46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bda46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bda46-105">检索 [informationProtectionLabel](../resources/informationprotectionlabel.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bda46-105">Retrieve the properties and relationships of an [informationProtectionLabel](../resources/informationprotectionlabel.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bda46-106">权限</span><span class="sxs-lookup"><span data-stu-id="bda46-106">Permissions</span></span>

<span data-ttu-id="bda46-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bda46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bda46-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bda46-109">Permission type</span></span>                        | <span data-ttu-id="bda46-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bda46-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bda46-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bda46-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bda46-112">InformationProtectionPolicy.Read</span><span class="sxs-lookup"><span data-stu-id="bda46-112">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="bda46-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bda46-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bda46-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bda46-114">Not supported.</span></span>                              |
| <span data-ttu-id="bda46-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bda46-115">Application</span></span>                            | <span data-ttu-id="bda46-116">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="bda46-116">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="bda46-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bda46-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
<span data-ttu-id="bda46-118">若要获取对登录用户或指定用户可用的标签，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="bda46-118">To get a label available to the signed-in user or specified user:</span></span>
```http
GET /me/informationProtection/policy/labels/{id}
GET /users/{id | user-principal-name}/informationProtection/policy/labels/{id}
```

<span data-ttu-id="bda46-119">若要获取组织可使用的标签，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="bda46-119">To get a label available to the organization:</span></span>
```http
GET /informationProtection/policy/labels/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bda46-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bda46-120">Optional query parameters</span></span>

<span data-ttu-id="bda46-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bda46-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bda46-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="bda46-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bda46-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="bda46-123">Request headers</span></span>

| <span data-ttu-id="bda46-124">名称</span><span class="sxs-lookup"><span data-stu-id="bda46-124">Name</span></span>          | <span data-ttu-id="bda46-125">说明</span><span class="sxs-lookup"><span data-stu-id="bda46-125">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="bda46-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bda46-126">Authorization</span></span> | <span data-ttu-id="bda46-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bda46-p103">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="bda46-129">用户代理</span><span class="sxs-lookup"><span data-stu-id="bda46-129">User-Agent</span></span>    | <span data-ttu-id="bda46-130">描述调用应用程序的名称和版本。</span><span class="sxs-lookup"><span data-stu-id="bda46-130">Describes the name and version of the calling application.</span></span> <span data-ttu-id="bda46-131">详细信息将在 Azure 信息保护分析中显现。</span><span class="sxs-lookup"><span data-stu-id="bda46-131">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="bda46-132">建议的格式为 "ApplicationName/版本"。</span><span class="sxs-lookup"><span data-stu-id="bda46-132">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="bda46-133">可选。</span><span class="sxs-lookup"><span data-stu-id="bda46-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bda46-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="bda46-134">Request body</span></span>

<span data-ttu-id="bda46-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bda46-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bda46-136">响应</span><span class="sxs-lookup"><span data-stu-id="bda46-136">Response</span></span>

<span data-ttu-id="bda46-137">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [informationProtectionLabel](../resources/informationprotectionlabel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bda46-137">If successful, this method returns a `200 OK` response code and the requested [informationProtectionLabel](../resources/informationprotectionlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bda46-138">示例</span><span class="sxs-lookup"><span data-stu-id="bda46-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bda46-139">请求</span><span class="sxs-lookup"><span data-stu-id="bda46-139">Request</span></span>

<span data-ttu-id="bda46-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bda46-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bda46-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="bda46-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_informationprotectionlabel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels/{id}
```
# <a name="c"></a>[<span data-ttu-id="bda46-142">C#</span><span class="sxs-lookup"><span data-stu-id="bda46-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-informationprotectionlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bda46-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bda46-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-informationprotectionlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bda46-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bda46-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-informationprotectionlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bda46-145">响应</span><span class="sxs-lookup"><span data-stu-id="bda46-145">Response</span></span>

<span data-ttu-id="bda46-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bda46-146">The following is an example of the response.</span></span>

> <span data-ttu-id="bda46-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bda46-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionLabel"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
User-agent: ContosoLOBApp/1.0

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('1e36d926-d716-4197-ba86-a6e18eb910b9')/informationProtection/policy/labels/$entity",
    "id": "4662f9a3-dd50-4a20-b984-a7be82e0e79c",
    "name": "LabelWithFooterAndHeaderActions_Tests",
    "description": "",
    "color": "",
    "sensitivity": 12,
    "tooltip": "LabelWithFooterAndHeaderActions_Tests",
    "isActive": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get informationProtectionLabel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


