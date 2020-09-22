---
title: 'informationProtectionLabel: listLabels'
description: 检索信息保护标签的列表。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9cd8fcd909c5c6e952763c6fa09e56c2f57fabe8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990625"
---
# <a name="informationprotectionlabel-listlabels"></a><span data-ttu-id="394ca-103">informationProtectionLabel: listLabels</span><span class="sxs-lookup"><span data-stu-id="394ca-103">informationProtectionLabel: listLabels</span></span>

<span data-ttu-id="394ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="394ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="394ca-105">获取可供用户或组织使用的 [信息保护标签](../resources/informationprotectionlabel.md) 的集合。</span><span class="sxs-lookup"><span data-stu-id="394ca-105">Get a collection of [information protection labels](../resources/informationprotectionlabel.md) available to the user or to the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="394ca-106">权限</span><span class="sxs-lookup"><span data-stu-id="394ca-106">Permissions</span></span>

<span data-ttu-id="394ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="394ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="394ca-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="394ca-109">Permission type</span></span>                        | <span data-ttu-id="394ca-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="394ca-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="394ca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="394ca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="394ca-112">InformationProtectionPolicy.Read</span><span class="sxs-lookup"><span data-stu-id="394ca-112">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="394ca-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="394ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="394ca-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="394ca-114">Not supported.</span></span>                              |
| <span data-ttu-id="394ca-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="394ca-115">Application</span></span>                            | <span data-ttu-id="394ca-116">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="394ca-116">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="394ca-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="394ca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
<span data-ttu-id="394ca-118">若要获取对登录用户或指定用户可用的标签，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="394ca-118">To get labels available to the signed-in user or specified user:</span></span>
```http
GET /me/informationProtection/policy/labels
GET /users/{id | user-principal-name}/informationProtection/policy/labels
```

<span data-ttu-id="394ca-119">若要获取组织可使用的标签，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="394ca-119">To get labels available to the organization:</span></span>
```http
GET /informationProtection/policy/labels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="394ca-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="394ca-120">Optional query parameters</span></span>

<span data-ttu-id="394ca-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="394ca-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="394ca-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="394ca-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="394ca-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="394ca-123">Request headers</span></span>

| <span data-ttu-id="394ca-124">名称</span><span class="sxs-lookup"><span data-stu-id="394ca-124">Name</span></span>          | <span data-ttu-id="394ca-125">说明</span><span class="sxs-lookup"><span data-stu-id="394ca-125">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="394ca-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="394ca-126">Authorization</span></span> | <span data-ttu-id="394ca-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="394ca-p103">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="394ca-129">用户代理</span><span class="sxs-lookup"><span data-stu-id="394ca-129">User-Agent</span></span>    | <span data-ttu-id="394ca-130">描述调用应用程序的名称和版本。</span><span class="sxs-lookup"><span data-stu-id="394ca-130">Describes the name and version of the calling application.</span></span> <span data-ttu-id="394ca-131">详细信息将在 Azure 信息保护分析中显现。</span><span class="sxs-lookup"><span data-stu-id="394ca-131">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="394ca-132">建议的格式为 "ApplicationName/版本"。</span><span class="sxs-lookup"><span data-stu-id="394ca-132">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="394ca-133">可选。</span><span class="sxs-lookup"><span data-stu-id="394ca-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="394ca-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="394ca-134">Request body</span></span>

<span data-ttu-id="394ca-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="394ca-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="394ca-136">响应</span><span class="sxs-lookup"><span data-stu-id="394ca-136">Response</span></span>

<span data-ttu-id="394ca-137">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [informationProtectionLabel](../resources/informationprotectionlabel.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="394ca-137">If successful, this method returns a `200 OK` response code and a collection of [informationProtectionLabel](../resources/informationprotectionlabel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="394ca-138">示例</span><span class="sxs-lookup"><span data-stu-id="394ca-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="394ca-139">请求</span><span class="sxs-lookup"><span data-stu-id="394ca-139">Request</span></span>

<span data-ttu-id="394ca-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="394ca-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="394ca-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="394ca-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_labels"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationProtection/policy/labels
```
# <a name="c"></a>[<span data-ttu-id="394ca-142">C#</span><span class="sxs-lookup"><span data-stu-id="394ca-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-labels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="394ca-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="394ca-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-labels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="394ca-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="394ca-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-labels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="394ca-145">响应</span><span class="sxs-lookup"><span data-stu-id="394ca-145">Response</span></span>

<span data-ttu-id="394ca-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="394ca-146">The following is an example of the response.</span></span>

> <span data-ttu-id="394ca-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="394ca-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionLabel",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
User-agent: ContosoLOBApp/1.0

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('1e36d926-d716-4197-ba86-a6e18eb910b9')/informationProtection/policy/labels",
  "value": [
      {
          "id": "3a80e051-487c-40d4-b491-73ad25d997e6",
          "name": "General",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 1,
          "tooltip": "Data classified as Contoso General.",
          "isActive": true
      },
      {
          "id": "4662f9a3-dd50-4a20-b984-a7be82e0e79c",
          "name": "Confidential",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 2,
          "tooltip": "Data classificed as Contoso Confidential.",
          "isActive": true
      },
      {
          "id": "4b18e8bb-b4a5-4695-85d0-8ae23ef27892",
          "name": "Highly Confidential",
          "description": "Consult Contoso data labeling policy for more details.",
          "color": "",
          "sensitivity": 3,
          "tooltip": "Data classified as Contoso Highly Confidential.",
          "isActive": true
      }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List labels",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


