---
title: informationProtectionLabel： extractLabel
description: 使用标记对象的元数据检索 informationProtectionContentLabel。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 9a69ae380f0a2bcdcad486c3d78a89cb2023cf4f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040348"
---
# <a name="informationprotectionlabel-extractlabel"></a><span data-ttu-id="80bd3-103">informationProtectionLabel： extractLabel</span><span class="sxs-lookup"><span data-stu-id="80bd3-103">informationProtectionLabel: extractLabel</span></span>

<span data-ttu-id="80bd3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80bd3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80bd3-105">使用已有标签的一条信息上的元数据，将元数据解析为特定的敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="80bd3-105">Using the metadata that exists on an already-labeled piece of information, resolve the metadata to a specific sensitivity label.</span></span> <span data-ttu-id="80bd3-106">[contentInfo](../resources/contentinfo.md)输入解析为[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)。</span><span class="sxs-lookup"><span data-stu-id="80bd3-106">The [contentInfo](../resources/contentinfo.md) input is resolved to [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md).</span></span>

>[!NOTE]
><span data-ttu-id="80bd3-107">**[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** 资源表示已应用于一条信息的敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="80bd3-107">The **[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** resource represents a sensitivity label that has been applied to a piece of information.</span></span> <span data-ttu-id="80bd3-108">[informationProtectionLabel](../resources/informationprotectionlabel.md) 对象是抽象标签，属于组织标签策略的一部分，可应用于信息。</span><span class="sxs-lookup"><span data-stu-id="80bd3-108">[informationProtectionLabel](../resources/informationprotectionlabel.md) objects are the abstract labels that are part of the organizational labeling policy and can be applied to information.</span></span>

## <a name="permissions"></a><span data-ttu-id="80bd3-109">权限</span><span class="sxs-lookup"><span data-stu-id="80bd3-109">Permissions</span></span>

<span data-ttu-id="80bd3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="80bd3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="80bd3-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="80bd3-112">Permission type</span></span>                        | <span data-ttu-id="80bd3-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="80bd3-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="80bd3-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80bd3-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="80bd3-115">InformationProtectionPolicy.Read</span><span class="sxs-lookup"><span data-stu-id="80bd3-115">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="80bd3-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80bd3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80bd3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="80bd3-117">Not supported.</span></span>                              |
| <span data-ttu-id="80bd3-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="80bd3-118">Application</span></span>                            | <span data-ttu-id="80bd3-119">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="80bd3-119">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="80bd3-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80bd3-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/extractLabel
```

## <a name="request-headers"></a><span data-ttu-id="80bd3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="80bd3-121">Request headers</span></span>

| <span data-ttu-id="80bd3-122">名称</span><span class="sxs-lookup"><span data-stu-id="80bd3-122">Name</span></span>          | <span data-ttu-id="80bd3-123">说明</span><span class="sxs-lookup"><span data-stu-id="80bd3-123">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="80bd3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="80bd3-124">Authorization</span></span> | <span data-ttu-id="80bd3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="80bd3-p104">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="80bd3-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="80bd3-127">Content-type</span></span>  | <span data-ttu-id="80bd3-128">内容类型：application/json。</span><span class="sxs-lookup"><span data-stu-id="80bd3-128">Content-type: application/json.</span></span> <span data-ttu-id="80bd3-129">必需。</span><span class="sxs-lookup"><span data-stu-id="80bd3-129">Required.</span></span>                                                                                                                                         |
| <span data-ttu-id="80bd3-130">User-Agent</span><span class="sxs-lookup"><span data-stu-id="80bd3-130">User-Agent</span></span>    | <span data-ttu-id="80bd3-131">描述调用应用程序的名称和版本。</span><span class="sxs-lookup"><span data-stu-id="80bd3-131">Describes the name and version of the calling application.</span></span> <span data-ttu-id="80bd3-132">详细信息将显示于 Azure 信息保护分析中。</span><span class="sxs-lookup"><span data-stu-id="80bd3-132">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="80bd3-133">建议的格式为 ApplicationName/Version。</span><span class="sxs-lookup"><span data-stu-id="80bd3-133">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="80bd3-134">可选。</span><span class="sxs-lookup"><span data-stu-id="80bd3-134">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80bd3-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="80bd3-135">Request body</span></span>

<span data-ttu-id="80bd3-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="80bd3-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="80bd3-137">参数</span><span class="sxs-lookup"><span data-stu-id="80bd3-137">Parameter</span></span>   | <span data-ttu-id="80bd3-138">类型</span><span class="sxs-lookup"><span data-stu-id="80bd3-138">Type</span></span>                                       | <span data-ttu-id="80bd3-139">说明</span><span class="sxs-lookup"><span data-stu-id="80bd3-139">Description</span></span>                                                                                                                         |
| :---------- | :----------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="80bd3-140">contentInfo</span><span class="sxs-lookup"><span data-stu-id="80bd3-140">contentInfo</span></span> | [<span data-ttu-id="80bd3-141">contentInfo</span><span class="sxs-lookup"><span data-stu-id="80bd3-141">contentInfo</span></span>](../resources/contentinfo.md) | <span data-ttu-id="80bd3-142">提供有关内容格式、内容状态和作为键/值对[](../resources/keyvaluepair.md)的现有元数据的详细信息。</span><span class="sxs-lookup"><span data-stu-id="80bd3-142">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |

## <a name="response"></a><span data-ttu-id="80bd3-143">响应</span><span class="sxs-lookup"><span data-stu-id="80bd3-143">Response</span></span>

<span data-ttu-id="80bd3-144">如果成功，此方法在响应正文中返回 响应代码和新 `200 OK` [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80bd3-144">If successful, this method returns a `200 OK` response code and a new [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="80bd3-145">示例</span><span class="sxs-lookup"><span data-stu-id="80bd3-145">Examples</span></span>

<span data-ttu-id="80bd3-146">下面是如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="80bd3-146">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="80bd3-147">请求</span><span class="sxs-lookup"><span data-stu-id="80bd3-147">Request</span></span>

<span data-ttu-id="80bd3-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="80bd3-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="80bd3-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="80bd3-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_extractlabel"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/policy/labels/extractLabel
Content-type: application/json
User-agent: ContosoLOBApp/1.0

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
# <a name="c"></a>[<span data-ttu-id="80bd3-150">C#</span><span class="sxs-lookup"><span data-stu-id="80bd3-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-extractlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80bd3-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80bd3-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-extractlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80bd3-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80bd3-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-extractlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80bd3-153">Java</span><span class="sxs-lookup"><span data-stu-id="80bd3-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/informationprotectionlabel-extractlabel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="80bd3-154">响应</span><span class="sxs-lookup"><span data-stu-id="80bd3-154">Response</span></span>

<span data-ttu-id="80bd3-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="80bd3-155">The following is an example of the response.</span></span>

> <span data-ttu-id="80bd3-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="80bd3-156">**Note:** The response object shown here might be shortened for readability.</span></span>

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


