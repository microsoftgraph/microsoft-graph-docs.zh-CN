---
title: 'informationProtectionLabel: extractLabel'
description: 使用来自带标签的对象的元数据检索 informationProtectionContentLabel。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 043b82820418915f4e38aab1839fee6113b423ec
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994408"
---
# <a name="informationprotectionlabel-extractlabel"></a><span data-ttu-id="c9ed9-103">informationProtectionLabel: extractLabel</span><span class="sxs-lookup"><span data-stu-id="c9ed9-103">informationProtectionLabel: extractLabel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9ed9-104">使用已标记的信息中存在的元数据，将元数据解析为特定的敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-104">Using the metadata that exists on an already-labeled piece of information, resolve the metadata to a specific sensitivity label.</span></span> <span data-ttu-id="c9ed9-105">将[contentInfo](../resources/contentinfo.md)输入解析为[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-105">The [contentInfo](../resources/contentinfo.md) input is resolved to [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md).</span></span>

>[!NOTE]
><span data-ttu-id="c9ed9-106">**[InformationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** 资源表示已应用于一条信息的敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-106">The **[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** resource represents a sensitivity label that has been applied to a piece of information.</span></span> <span data-ttu-id="c9ed9-107">[informationProtectionLabel](../resources/informationprotectionlabel.md)对象是组织标记策略的一部分的抽象标签，可应用于信息。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-107">[informationProtectionLabel](../resources/informationprotectionlabel.md) objects are the abstract labels that are part of the organizational labeling policy and can be applied to information.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9ed9-108">权限</span><span class="sxs-lookup"><span data-stu-id="c9ed9-108">Permissions</span></span>

<span data-ttu-id="c9ed9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c9ed9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9ed9-111">Permission type</span></span>                        | <span data-ttu-id="c9ed9-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c9ed9-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c9ed9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9ed9-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9ed9-114">InformationProtectionPolicy。请阅读</span><span class="sxs-lookup"><span data-stu-id="c9ed9-114">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="c9ed9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9ed9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9ed9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-116">Not supported.</span></span>                              |
| <span data-ttu-id="c9ed9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9ed9-117">Application</span></span>                            | <span data-ttu-id="c9ed9-118">InformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c9ed9-118">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="c9ed9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9ed9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/extractLabel
```

## <a name="request-headers"></a><span data-ttu-id="c9ed9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c9ed9-120">Request headers</span></span>

| <span data-ttu-id="c9ed9-121">名称</span><span class="sxs-lookup"><span data-stu-id="c9ed9-121">Name</span></span>          | <span data-ttu-id="c9ed9-122">说明</span><span class="sxs-lookup"><span data-stu-id="c9ed9-122">Description</span></span>                    |
| :------------ | :----------------------------- |
| <span data-ttu-id="c9ed9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9ed9-123">Authorization</span></span> | <span data-ttu-id="c9ed9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-p104">Bearer {token}. Required.</span></span>                 |
| <span data-ttu-id="c9ed9-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="c9ed9-126">Content-type</span></span>  | <span data-ttu-id="c9ed9-127">Content-type： application/json。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-127">Content-type: application/json.</span></span> <span data-ttu-id="c9ed9-128">必填。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9ed9-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9ed9-129">Request body</span></span>

<span data-ttu-id="c9ed9-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c9ed9-131">参数</span><span class="sxs-lookup"><span data-stu-id="c9ed9-131">Parameter</span></span>   | <span data-ttu-id="c9ed9-132">类型</span><span class="sxs-lookup"><span data-stu-id="c9ed9-132">Type</span></span>                                       | <span data-ttu-id="c9ed9-133">说明</span><span class="sxs-lookup"><span data-stu-id="c9ed9-133">Description</span></span>                                                                                                                                                                                                   |
| :---------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="c9ed9-134">contentInfo</span><span class="sxs-lookup"><span data-stu-id="c9ed9-134">contentInfo</span></span> | [<span data-ttu-id="c9ed9-135">contentInfo</span><span class="sxs-lookup"><span data-stu-id="c9ed9-135">contentInfo</span></span>](../resources/contentinfo.md) | <span data-ttu-id="c9ed9-136">提供有关内容格式、内容状态和现有[元数据](../resources/keyvaluepair.md)的详细信息，作为键/值对。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-136">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |

## <a name="response"></a><span data-ttu-id="c9ed9-137">响应</span><span class="sxs-lookup"><span data-stu-id="c9ed9-137">Response</span></span>

<span data-ttu-id="c9ed9-138">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-138">If successful, this method returns a `200 OK` response code and a new [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c9ed9-139">示例</span><span class="sxs-lookup"><span data-stu-id="c9ed9-139">Examples</span></span>

<span data-ttu-id="c9ed9-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="c9ed9-141">请求</span><span class="sxs-lookup"><span data-stu-id="c9ed9-141">Request</span></span>

<span data-ttu-id="c9ed9-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c9ed9-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9ed9-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_extractlabel"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/extractLabel
Content-type: application/json

{
    "contentInfo": {
        "@odata.type": "#microsoft.graph.contentInfo",
        "format@odata.type": "#microsoft.graph.contentFormat",
        "format": "default",
        "identifier": null,
        "state@odata.type": "#microsoft.graph.contentState",
        "state": "rest",
        "metadata@odata.type": "#Collection(microsoft.graph.keyValuePair)",
        "metadata": [
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
                "value": "True"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
                "value": "Standard"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
                "value": "1/1/0001 12:00:00 AM"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
                "value": "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
                "value": "Top Secret"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
                "value": "0"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId",
                "value": "00000000-0000-0000-0000-000000000000"
            }
        ]
    }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c9ed9-144">C#</span><span class="sxs-lookup"><span data-stu-id="c9ed9-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-extractlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c9ed9-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9ed9-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-extractlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c9ed9-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9ed9-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-extractlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c9ed9-147">响应</span><span class="sxs-lookup"><span data-stu-id="c9ed9-147">Response</span></span>

<span data-ttu-id="c9ed9-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-148">The following is an example of the response.</span></span>

> <span data-ttu-id="c9ed9-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c9ed9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionContentLabel"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.informationProtectionContentLabel",
    "creationDateTime": "1970-01-01T00:00:00Z",
    "assignmentMethod": "standard",
    "label": {
        "id": "722a5300-ac39-4c9a-88e3-f54c46676417",
        "name": "Top Secret",
        "description": "",
        "color": "#000000",
        "sensitivity": 13,
        "tooltip": "This information is top secret.",
        "isActive": true
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel: extractLabel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
