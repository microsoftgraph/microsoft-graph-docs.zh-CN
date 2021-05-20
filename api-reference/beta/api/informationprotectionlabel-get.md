---
title: 获取 informationProtectionLabel
description: 检索指定 informationProtectionLabel 对象的属性和关系。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 02b1d36a2b4639487b9dd88dcf67c9592bce1aa9
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579618"
---
# <a name="get-informationprotectionlabel"></a><span data-ttu-id="ee9bc-103">获取 informationProtectionLabel</span><span class="sxs-lookup"><span data-stu-id="ee9bc-103">Get informationProtectionLabel</span></span>

<span data-ttu-id="ee9bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee9bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee9bc-105">检索 [informationProtectionLabel 对象的属性和](../resources/informationprotectionlabel.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="ee9bc-105">Retrieve the properties and relationships of an [informationProtectionLabel](../resources/informationprotectionlabel.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee9bc-106">权限</span><span class="sxs-lookup"><span data-stu-id="ee9bc-106">Permissions</span></span>

<span data-ttu-id="ee9bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ee9bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ee9bc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ee9bc-109">Permission type</span></span>                        | <span data-ttu-id="ee9bc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ee9bc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ee9bc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ee9bc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ee9bc-112">InformationProtectionPolicy.Read</span><span class="sxs-lookup"><span data-stu-id="ee9bc-112">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="ee9bc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ee9bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee9bc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ee9bc-114">Not supported.</span></span>                              |
| <span data-ttu-id="ee9bc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ee9bc-115">Application</span></span>                            | <span data-ttu-id="ee9bc-116">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee9bc-116">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="ee9bc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ee9bc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
<span data-ttu-id="ee9bc-118">若要获取登录用户或指定用户可用的标签，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="ee9bc-118">To get a label available to the signed-in user or specified user:</span></span>
```http
GET /me/informationProtection/policy/labels/{id}
GET /users/{id | user-principal-name}/informationProtection/policy/labels/{id}
```

<span data-ttu-id="ee9bc-119">若要获取对组织可用的标签，请：</span><span class="sxs-lookup"><span data-stu-id="ee9bc-119">To get a label available to the organization:</span></span>
```http
GET /informationProtection/policy/labels/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee9bc-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ee9bc-120">Optional query parameters</span></span>

<span data-ttu-id="ee9bc-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ee9bc-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ee9bc-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="ee9bc-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee9bc-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ee9bc-123">Request headers</span></span>

| <span data-ttu-id="ee9bc-124">名称</span><span class="sxs-lookup"><span data-stu-id="ee9bc-124">Name</span></span>          | <span data-ttu-id="ee9bc-125">说明</span><span class="sxs-lookup"><span data-stu-id="ee9bc-125">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ee9bc-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee9bc-126">Authorization</span></span> | <span data-ttu-id="ee9bc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ee9bc-p103">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="ee9bc-129">User-Agent</span><span class="sxs-lookup"><span data-stu-id="ee9bc-129">User-Agent</span></span>    | <span data-ttu-id="ee9bc-130">描述调用应用程序的名称和版本。</span><span class="sxs-lookup"><span data-stu-id="ee9bc-130">Describes the name and version of the calling application.</span></span> <span data-ttu-id="ee9bc-131">详细信息将显示于 Azure 信息保护分析中。</span><span class="sxs-lookup"><span data-stu-id="ee9bc-131">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="ee9bc-132">建议的格式为 ApplicationName/Version。</span><span class="sxs-lookup"><span data-stu-id="ee9bc-132">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="ee9bc-133">可选。</span><span class="sxs-lookup"><span data-stu-id="ee9bc-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee9bc-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="ee9bc-134">Request body</span></span>

<span data-ttu-id="ee9bc-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ee9bc-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee9bc-136">响应</span><span class="sxs-lookup"><span data-stu-id="ee9bc-136">Response</span></span>

<span data-ttu-id="ee9bc-137">如果成功，此方法在响应正文中返回 响应代码和请求的信息 `200 OK` [ProtectionLabel](../resources/informationprotectionlabel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ee9bc-137">If successful, this method returns a `200 OK` response code and the requested [informationProtectionLabel](../resources/informationprotectionlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ee9bc-138">示例</span><span class="sxs-lookup"><span data-stu-id="ee9bc-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ee9bc-139">请求</span><span class="sxs-lookup"><span data-stu-id="ee9bc-139">Request</span></span>

<span data-ttu-id="ee9bc-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ee9bc-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ee9bc-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee9bc-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_informationprotectionlabel"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels/{id}
```
# <a name="c"></a>[<span data-ttu-id="ee9bc-142">C#</span><span class="sxs-lookup"><span data-stu-id="ee9bc-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-informationprotectionlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee9bc-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee9bc-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-informationprotectionlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee9bc-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee9bc-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-informationprotectionlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee9bc-145">Java</span><span class="sxs-lookup"><span data-stu-id="ee9bc-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-informationprotectionlabel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ee9bc-146">响应</span><span class="sxs-lookup"><span data-stu-id="ee9bc-146">Response</span></span>

<span data-ttu-id="ee9bc-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ee9bc-147">The following is an example of the response.</span></span>

> <span data-ttu-id="ee9bc-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ee9bc-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "id": "4b18e8bb-b4a5-4695-85d0-8ae23ef27892",
  "name": "Highly Confidential",
  "description": "Consult Contoso data labeling policy for more details.",
  "color": "",
  "sensitivity": 3,
  "tooltip": "Data classified as Contoso Highly Confidential.",
  "isActive": true,
  "parent": null
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


