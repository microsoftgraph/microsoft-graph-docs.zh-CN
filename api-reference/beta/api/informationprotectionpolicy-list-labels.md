---
title: 'informationProtectionLabel: listLabels'
description: 检索信息保护标签的列表。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c3e83fd6d7fa19da70010136c3bec85ce17b694a
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216255"
---
# <a name="informationprotectionlabel-listlabels"></a><span data-ttu-id="e8ead-103">informationProtectionLabel: listLabels</span><span class="sxs-lookup"><span data-stu-id="e8ead-103">informationProtectionLabel: listLabels</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8ead-104">获取可供用户或组织使用的[信息保护标签](../resources/informationprotectionlabel.md)的集合。</span><span class="sxs-lookup"><span data-stu-id="e8ead-104">Get a collection of [information protection labels](../resources/informationprotectionlabel.md) available to the user or to the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8ead-105">权限</span><span class="sxs-lookup"><span data-stu-id="e8ead-105">Permissions</span></span>

<span data-ttu-id="e8ead-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8ead-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8ead-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8ead-108">Permission type</span></span>                        | <span data-ttu-id="e8ead-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8ead-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="e8ead-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8ead-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8ead-111">InformationProtectionPolicy。请阅读</span><span class="sxs-lookup"><span data-stu-id="e8ead-111">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="e8ead-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8ead-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8ead-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8ead-113">Not supported.</span></span>                              |
| <span data-ttu-id="e8ead-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8ead-114">Application</span></span>                            | <span data-ttu-id="e8ead-115">InformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e8ead-115">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="e8ead-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8ead-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET me/informationprotection/policy/labels
GET /informationprotection/policy/labels
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8ead-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e8ead-117">Optional query parameters</span></span>

<span data-ttu-id="e8ead-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e8ead-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e8ead-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e8ead-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8ead-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8ead-120">Request headers</span></span>

| <span data-ttu-id="e8ead-121">名称</span><span class="sxs-lookup"><span data-stu-id="e8ead-121">Name</span></span>          | <span data-ttu-id="e8ead-122">说明</span><span class="sxs-lookup"><span data-stu-id="e8ead-122">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e8ead-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8ead-123">Authorization</span></span> | <span data-ttu-id="e8ead-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8ead-p103">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="e8ead-126">用户代理</span><span class="sxs-lookup"><span data-stu-id="e8ead-126">User-Agent</span></span>    | <span data-ttu-id="e8ead-127">描述调用应用程序的名称和版本。</span><span class="sxs-lookup"><span data-stu-id="e8ead-127">Describes the name and version of the calling application.</span></span> <span data-ttu-id="e8ead-128">详细信息将在 Azure 信息保护分析中显现。</span><span class="sxs-lookup"><span data-stu-id="e8ead-128">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="e8ead-129">建议的格式为 "ApplicationName/版本"。</span><span class="sxs-lookup"><span data-stu-id="e8ead-129">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="e8ead-130">可选。</span><span class="sxs-lookup"><span data-stu-id="e8ead-130">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8ead-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8ead-131">Request body</span></span>

<span data-ttu-id="e8ead-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e8ead-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8ead-133">响应</span><span class="sxs-lookup"><span data-stu-id="e8ead-133">Response</span></span>

<span data-ttu-id="e8ead-134">如果成功，此方法在响应`200 OK`正文中返回响应代码和[informationProtectionLabel](../resources/informationprotectionlabel.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="e8ead-134">If successful, this method returns a `200 OK` response code and a collection of [informationProtectionLabel](../resources/informationprotectionlabel.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8ead-135">示例</span><span class="sxs-lookup"><span data-stu-id="e8ead-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8ead-136">请求</span><span class="sxs-lookup"><span data-stu-id="e8ead-136">Request</span></span>

<span data-ttu-id="e8ead-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e8ead-137">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e8ead-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8ead-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_labels"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/informationprotection/policy/labels
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e8ead-139">C#</span><span class="sxs-lookup"><span data-stu-id="e8ead-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-labels-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e8ead-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8ead-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-labels-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e8ead-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8ead-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-labels-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8ead-142">响应</span><span class="sxs-lookup"><span data-stu-id="e8ead-142">Response</span></span>

<span data-ttu-id="e8ead-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e8ead-143">The following is an example of the response.</span></span>

> <span data-ttu-id="e8ead-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e8ead-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
