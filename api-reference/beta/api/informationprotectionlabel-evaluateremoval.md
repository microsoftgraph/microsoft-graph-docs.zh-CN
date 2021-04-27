---
title: informationProtectionLabel：evaluateRemoval
description: 评估要删除的标签以及如何根据现有内容信息删除它。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 92a7c4fc26cc647b141bdd3253f8ecd21bad9479
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040362"
---
# <a name="informationprotectionlabel-evaluateremoval"></a><span data-ttu-id="deefb-103">informationProtectionLabel：evaluateRemoval</span><span class="sxs-lookup"><span data-stu-id="deefb-103">informationProtectionLabel: evaluateRemoval</span></span>

<span data-ttu-id="deefb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deefb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deefb-105">向使用应用程序指示删除标签信息应采取的操作。</span><span class="sxs-lookup"><span data-stu-id="deefb-105">Indicate to the consuming application what actions it should take to remove the label information.</span></span>

<span data-ttu-id="deefb-106">将 [contentInfo](../resources/contentinfo.md) 作为输入（包括现有内容元数据键 [/](../resources/keyvaluepair.md)值对）后，API 将返回 [一个 informationProtectionAction，](../resources/informationprotectionaction.md) 其中包含以下各项之一的某种组合：</span><span class="sxs-lookup"><span data-stu-id="deefb-106">Given [contentInfo](../resources/contentinfo.md) as an input, which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), the API returns an [informationProtectionAction](../resources/informationprotectionaction.md) that contains some combination of one of more of the following:</span></span> 

* [<span data-ttu-id="deefb-107">justifyAction</span><span class="sxs-lookup"><span data-stu-id="deefb-107">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="deefb-108">metadataAction</span><span class="sxs-lookup"><span data-stu-id="deefb-108">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="deefb-109">removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="deefb-109">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="deefb-110">removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="deefb-110">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="deefb-111">removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="deefb-111">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="deefb-112">remove使用markAction</span><span class="sxs-lookup"><span data-stu-id="deefb-112">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="deefb-113">权限</span><span class="sxs-lookup"><span data-stu-id="deefb-113">Permissions</span></span>

<span data-ttu-id="deefb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="deefb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="deefb-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="deefb-116">Permission type</span></span>                        | <span data-ttu-id="deefb-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="deefb-117">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="deefb-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="deefb-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="deefb-119">InformationProtectionPolicy.Read</span><span class="sxs-lookup"><span data-stu-id="deefb-119">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="deefb-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="deefb-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="deefb-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="deefb-121">Not supported.</span></span>                              |
| <span data-ttu-id="deefb-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="deefb-122">Application</span></span>                            | <span data-ttu-id="deefb-123">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="deefb-123">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="deefb-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="deefb-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/policy/labels/evaluateRemoval
```

## <a name="request-headers"></a><span data-ttu-id="deefb-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="deefb-125">Request headers</span></span>

| <span data-ttu-id="deefb-126">名称</span><span class="sxs-lookup"><span data-stu-id="deefb-126">Name</span></span>          | <span data-ttu-id="deefb-127">说明</span><span class="sxs-lookup"><span data-stu-id="deefb-127">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="deefb-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="deefb-128">Authorization</span></span> | <span data-ttu-id="deefb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="deefb-p102">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="deefb-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="deefb-131">Content-type</span></span>  | <span data-ttu-id="deefb-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="deefb-p103">application/json. Required.</span></span>                                                                                                                                                       |
| <span data-ttu-id="deefb-134">User-Agent</span><span class="sxs-lookup"><span data-stu-id="deefb-134">User-Agent</span></span>    | <span data-ttu-id="deefb-135">描述调用应用程序的名称和版本。</span><span class="sxs-lookup"><span data-stu-id="deefb-135">Describes the name and version of the calling application.</span></span> <span data-ttu-id="deefb-136">详细信息将显示于 Azure 信息保护分析中。</span><span class="sxs-lookup"><span data-stu-id="deefb-136">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="deefb-137">建议的格式为 ApplicationName/Version。</span><span class="sxs-lookup"><span data-stu-id="deefb-137">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="deefb-138">可选。</span><span class="sxs-lookup"><span data-stu-id="deefb-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="deefb-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="deefb-139">Request body</span></span>

<span data-ttu-id="deefb-140">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="deefb-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="deefb-141">参数</span><span class="sxs-lookup"><span data-stu-id="deefb-141">Parameter</span></span>              | <span data-ttu-id="deefb-142">类型</span><span class="sxs-lookup"><span data-stu-id="deefb-142">Type</span></span>                                                             | <span data-ttu-id="deefb-143">说明</span><span class="sxs-lookup"><span data-stu-id="deefb-143">Description</span></span>                                                                                                                         |
| :--------------------- | :--------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="deefb-144">contentInfo</span><span class="sxs-lookup"><span data-stu-id="deefb-144">contentInfo</span></span>            | [<span data-ttu-id="deefb-145">contentInfo</span><span class="sxs-lookup"><span data-stu-id="deefb-145">contentInfo</span></span>](../resources/contentinfo.md)                       | <span data-ttu-id="deefb-146">提供有关内容格式、内容状态和作为键/值对[](../resources/keyvaluepair.md)的现有元数据的详细信息。</span><span class="sxs-lookup"><span data-stu-id="deefb-146">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |
| <span data-ttu-id="deefb-147">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="deefb-147">downgradeJustification</span></span> | [<span data-ttu-id="deefb-148">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="deefb-148">downgradeJustification</span></span>](../resources/downgradejustification.md) | <span data-ttu-id="deefb-149">必须由用户或应用程序逻辑提供的理由。</span><span class="sxs-lookup"><span data-stu-id="deefb-149">Justification that must be provided by the user or application logic.</span></span>                                                               |


## <a name="response"></a><span data-ttu-id="deefb-150">响应</span><span class="sxs-lookup"><span data-stu-id="deefb-150">Response</span></span>

<span data-ttu-id="deefb-151">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和新 [informationProtectionAction](../resources/informationprotectionaction.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="deefb-151">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span> <span data-ttu-id="deefb-152">[informationProtectionAction 对象](../resources/informationprotectionaction.md)将包含一个[metadataAction](../resources/metadataaction.md)对象，该对象通知应用程序要删除的元数据。</span><span class="sxs-lookup"><span data-stu-id="deefb-152">The [informationProtectionAction object](../resources/informationprotectionaction.md) will contain a [metadataAction](../resources/metadataaction.md) object that informs the application which metadata to remove.</span></span> 

## <a name="examples"></a><span data-ttu-id="deefb-153">示例</span><span class="sxs-lookup"><span data-stu-id="deefb-153">Examples</span></span>

<span data-ttu-id="deefb-154">下面是如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="deefb-154">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="deefb-155">请求</span><span class="sxs-lookup"><span data-stu-id="deefb-155">Request</span></span>

<span data-ttu-id="deefb-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="deefb-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="deefb-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="deefb-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateremoval"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/policy/labels/evaluateRemoval
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
        "value": "General"
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
  },
  "downgradeJustification": {
        "justificationMessage": "The information has been declassified.",
        "isDowngradeJustified": true
    }
}
```
# <a name="c"></a>[<span data-ttu-id="deefb-158">C#</span><span class="sxs-lookup"><span data-stu-id="deefb-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateremoval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="deefb-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="deefb-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateremoval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="deefb-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="deefb-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateremoval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="deefb-161">Java</span><span class="sxs-lookup"><span data-stu-id="deefb-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/informationprotectionlabel-evaluateremoval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="deefb-162">响应</span><span class="sxs-lookup"><span data-stu-id="deefb-162">Response</span></span>

<span data-ttu-id="deefb-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="deefb-163">The following is an example of the response.</span></span>

> <span data-ttu-id="deefb-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="deefb-164">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionAction",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.informationProtectionAction)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.metadataAction",
            "metadataToRemove": [
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId"
            ],
            "metadataToAdd": []
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel: evaluateRemoval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


