---
title: 'informationProtectionLabel: extractLabel'
description: 使用来自带标签的对象的元数据检索 informationProtectionContentLabel。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c04849feac987eefef82eb3e069645406218ff1f
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216304"
---
# <a name="informationprotectionlabel-extractlabel"></a><span data-ttu-id="38712-103">informationProtectionLabel: extractLabel</span><span class="sxs-lookup"><span data-stu-id="38712-103">informationProtectionLabel: extractLabel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38712-104">使用已标记的信息中存在的元数据，将元数据解析为特定的敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="38712-104">Using the metadata that exists on an already-labeled piece of information, resolve the metadata to a specific sensitivity label.</span></span> <span data-ttu-id="38712-105">将[contentInfo](../resources/contentinfo.md)输入解析为[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)。</span><span class="sxs-lookup"><span data-stu-id="38712-105">The [contentInfo](../resources/contentinfo.md) input is resolved to [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md).</span></span>

>[!NOTE]
><span data-ttu-id="38712-106">**[InformationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** 资源表示已应用于一条信息的敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="38712-106">The **[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** resource represents a sensitivity label that has been applied to a piece of information.</span></span> <span data-ttu-id="38712-107">[informationProtectionLabel](../resources/informationprotectionlabel.md)对象是组织标记策略的一部分的抽象标签，可应用于信息。</span><span class="sxs-lookup"><span data-stu-id="38712-107">[informationProtectionLabel](../resources/informationprotectionlabel.md) objects are the abstract labels that are part of the organizational labeling policy and can be applied to information.</span></span>

## <a name="permissions"></a><span data-ttu-id="38712-108">权限</span><span class="sxs-lookup"><span data-stu-id="38712-108">Permissions</span></span>

<span data-ttu-id="38712-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38712-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="38712-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="38712-111">Permission type</span></span>                        | <span data-ttu-id="38712-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38712-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="38712-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38712-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="38712-114">InformationProtectionPolicy。请阅读</span><span class="sxs-lookup"><span data-stu-id="38712-114">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="38712-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38712-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="38712-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="38712-116">Not supported.</span></span>                              |
| <span data-ttu-id="38712-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="38712-117">Application</span></span>                            | <span data-ttu-id="38712-118">InformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="38712-118">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="38712-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38712-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/extractLabel
```

## <a name="request-headers"></a><span data-ttu-id="38712-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="38712-120">Request headers</span></span>

| <span data-ttu-id="38712-121">名称</span><span class="sxs-lookup"><span data-stu-id="38712-121">Name</span></span>          | <span data-ttu-id="38712-122">说明</span><span class="sxs-lookup"><span data-stu-id="38712-122">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="38712-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="38712-123">Authorization</span></span> | <span data-ttu-id="38712-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38712-p104">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="38712-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="38712-126">Content-type</span></span>  | <span data-ttu-id="38712-127">Content-type： application/json。</span><span class="sxs-lookup"><span data-stu-id="38712-127">Content-type: application/json.</span></span> <span data-ttu-id="38712-128">必需。</span><span class="sxs-lookup"><span data-stu-id="38712-128">Required.</span></span>                                                                                                                                         |
| <span data-ttu-id="38712-129">用户代理</span><span class="sxs-lookup"><span data-stu-id="38712-129">User-Agent</span></span>    | <span data-ttu-id="38712-130">描述调用应用程序的名称和版本。</span><span class="sxs-lookup"><span data-stu-id="38712-130">Describes the name and version of the calling application.</span></span> <span data-ttu-id="38712-131">详细信息将在 Azure 信息保护分析中显现。</span><span class="sxs-lookup"><span data-stu-id="38712-131">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="38712-132">建议的格式为 "ApplicationName/版本"。</span><span class="sxs-lookup"><span data-stu-id="38712-132">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="38712-133">可选。</span><span class="sxs-lookup"><span data-stu-id="38712-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38712-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="38712-134">Request body</span></span>

<span data-ttu-id="38712-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="38712-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="38712-136">参数</span><span class="sxs-lookup"><span data-stu-id="38712-136">Parameter</span></span>   | <span data-ttu-id="38712-137">类型</span><span class="sxs-lookup"><span data-stu-id="38712-137">Type</span></span>                                       | <span data-ttu-id="38712-138">说明</span><span class="sxs-lookup"><span data-stu-id="38712-138">Description</span></span>                                                                                                                         |
| :---------- | :----------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="38712-139">contentInfo</span><span class="sxs-lookup"><span data-stu-id="38712-139">contentInfo</span></span> | [<span data-ttu-id="38712-140">contentInfo</span><span class="sxs-lookup"><span data-stu-id="38712-140">contentInfo</span></span>](../resources/contentinfo.md) | <span data-ttu-id="38712-141">提供有关内容格式、内容状态和现有[元数据](../resources/keyvaluepair.md)的详细信息，作为键/值对。</span><span class="sxs-lookup"><span data-stu-id="38712-141">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |

## <a name="response"></a><span data-ttu-id="38712-142">响应</span><span class="sxs-lookup"><span data-stu-id="38712-142">Response</span></span>

<span data-ttu-id="38712-143">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)对象。</span><span class="sxs-lookup"><span data-stu-id="38712-143">If successful, this method returns a `200 OK` response code and a new [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="38712-144">示例</span><span class="sxs-lookup"><span data-stu-id="38712-144">Examples</span></span>

<span data-ttu-id="38712-145">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="38712-145">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="38712-146">请求</span><span class="sxs-lookup"><span data-stu-id="38712-146">Request</span></span>

<span data-ttu-id="38712-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="38712-147">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="38712-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="38712-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_extractlabel"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/extractLabel
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="38712-149">C#</span><span class="sxs-lookup"><span data-stu-id="38712-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-extractlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38712-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38712-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-extractlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="38712-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38712-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-extractlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="38712-152">响应</span><span class="sxs-lookup"><span data-stu-id="38712-152">Response</span></span>

<span data-ttu-id="38712-153">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="38712-153">The following is an example of the response.</span></span>

> <span data-ttu-id="38712-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="38712-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
