---
title: 'informationProtectionLabel: evaluateRemoval'
description: 评估要删除的标签以及如何根据现有内容信息将其删除。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: acea1f8ba7021e76d069f8da60c7b5cb9bbe9604
ms.sourcegitcommit: 844c6d552a8a60fcda5ef65148570a32fd1004bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/17/2020
ms.locfileid: "41216713"
---
# <a name="informationprotectionlabel-evaluateremoval"></a><span data-ttu-id="b7a95-103">informationProtectionLabel: evaluateRemoval</span><span class="sxs-lookup"><span data-stu-id="b7a95-103">informationProtectionLabel: evaluateRemoval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7a95-104">向正在使用的应用程序指示删除标签信息应采取的操作。</span><span class="sxs-lookup"><span data-stu-id="b7a95-104">Indicate to the consuming application what actions it should take to remove the label information.</span></span>

<span data-ttu-id="b7a95-105">给定[contentInfo](../resources/contentinfo.md)作为输入（其中包括现有的内容元数据[密钥/值对](../resources/keyvaluepair.md)），API 将返回一个[informationProtectionAction](../resources/informationprotectionaction.md) ，其中包含以下一个或多个部分的组合：</span><span class="sxs-lookup"><span data-stu-id="b7a95-105">Given [contentInfo](../resources/contentinfo.md) as an input, which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), the API returns an [informationProtectionAction](../resources/informationprotectionaction.md) that contains some combination of one of more of the following:</span></span> 

* [<span data-ttu-id="b7a95-106">justifyAction</span><span class="sxs-lookup"><span data-stu-id="b7a95-106">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="b7a95-107">metadataAction</span><span class="sxs-lookup"><span data-stu-id="b7a95-107">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="b7a95-108">removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="b7a95-108">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="b7a95-109">removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="b7a95-109">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="b7a95-110">removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="b7a95-110">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="b7a95-111">removeWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="b7a95-111">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="b7a95-112">权限</span><span class="sxs-lookup"><span data-stu-id="b7a95-112">Permissions</span></span>

<span data-ttu-id="b7a95-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7a95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b7a95-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7a95-115">Permission type</span></span>                        | <span data-ttu-id="b7a95-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b7a95-116">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="b7a95-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7a95-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="b7a95-118">InformationProtectionPolicy。请阅读</span><span class="sxs-lookup"><span data-stu-id="b7a95-118">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="b7a95-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7a95-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7a95-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7a95-120">Not supported.</span></span>                              |
| <span data-ttu-id="b7a95-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7a95-121">Application</span></span>                            | <span data-ttu-id="b7a95-122">InformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="b7a95-122">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="b7a95-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7a95-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/evaluateRemoval
```

## <a name="request-headers"></a><span data-ttu-id="b7a95-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7a95-124">Request headers</span></span>

| <span data-ttu-id="b7a95-125">名称</span><span class="sxs-lookup"><span data-stu-id="b7a95-125">Name</span></span>          | <span data-ttu-id="b7a95-126">说明</span><span class="sxs-lookup"><span data-stu-id="b7a95-126">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b7a95-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7a95-127">Authorization</span></span> | <span data-ttu-id="b7a95-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b7a95-p102">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="b7a95-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="b7a95-130">Content-type</span></span>  | <span data-ttu-id="b7a95-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b7a95-p103">application/json. Required.</span></span>                                                                                                                                                       |
| <span data-ttu-id="b7a95-133">用户代理</span><span class="sxs-lookup"><span data-stu-id="b7a95-133">User-Agent</span></span>    | <span data-ttu-id="b7a95-134">描述调用应用程序的名称和版本。</span><span class="sxs-lookup"><span data-stu-id="b7a95-134">Describes the name and version of the calling application.</span></span> <span data-ttu-id="b7a95-135">详细信息将在 Azure 信息保护分析中显现。</span><span class="sxs-lookup"><span data-stu-id="b7a95-135">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="b7a95-136">建议的格式为 "ApplicationName/版本"。</span><span class="sxs-lookup"><span data-stu-id="b7a95-136">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="b7a95-137">可选。</span><span class="sxs-lookup"><span data-stu-id="b7a95-137">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b7a95-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7a95-138">Request body</span></span>

<span data-ttu-id="b7a95-139">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="b7a95-139">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b7a95-140">参数</span><span class="sxs-lookup"><span data-stu-id="b7a95-140">Parameter</span></span>              | <span data-ttu-id="b7a95-141">类型</span><span class="sxs-lookup"><span data-stu-id="b7a95-141">Type</span></span>                                                             | <span data-ttu-id="b7a95-142">说明</span><span class="sxs-lookup"><span data-stu-id="b7a95-142">Description</span></span>                                                                                                                         |
| :--------------------- | :--------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b7a95-143">contentInfo</span><span class="sxs-lookup"><span data-stu-id="b7a95-143">contentInfo</span></span>            | [<span data-ttu-id="b7a95-144">contentInfo</span><span class="sxs-lookup"><span data-stu-id="b7a95-144">contentInfo</span></span>](../resources/contentinfo.md)                       | <span data-ttu-id="b7a95-145">提供有关内容格式、内容状态和现有[元数据](../resources/keyvaluepair.md)的详细信息，作为键/值对。</span><span class="sxs-lookup"><span data-stu-id="b7a95-145">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |
| <span data-ttu-id="b7a95-146">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="b7a95-146">downgradeJustification</span></span> | [<span data-ttu-id="b7a95-147">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="b7a95-147">downgradeJustification</span></span>](../resources/downgradejustification.md) | <span data-ttu-id="b7a95-148">必须由用户或应用程序逻辑提供的理由。</span><span class="sxs-lookup"><span data-stu-id="b7a95-148">Justification that must be provided by the user or application logic.</span></span>                                                               |


## <a name="response"></a><span data-ttu-id="b7a95-149">响应</span><span class="sxs-lookup"><span data-stu-id="b7a95-149">Response</span></span>

<span data-ttu-id="b7a95-150">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[informationProtectionAction](../resources/informationprotectionaction.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="b7a95-150">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span> <span data-ttu-id="b7a95-151">[InformationProtectionAction 对象](../resources/informationprotectionaction.md)将包含一个[metadataAction](../resources/metadataaction.md)对象，该对象通知应用程序要删除的元数据。</span><span class="sxs-lookup"><span data-stu-id="b7a95-151">The [informationProtectionAction object](../resources/informationprotectionaction.md) will contain a [metadataAction](../resources/metadataaction.md) object that informs the application which metadata to remove.</span></span> 

## <a name="examples"></a><span data-ttu-id="b7a95-152">示例</span><span class="sxs-lookup"><span data-stu-id="b7a95-152">Examples</span></span>

<span data-ttu-id="b7a95-153">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="b7a95-153">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b7a95-154">请求</span><span class="sxs-lookup"><span data-stu-id="b7a95-154">Request</span></span>

<span data-ttu-id="b7a95-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b7a95-155">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b7a95-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="b7a95-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateremoval"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/evaluateRemoval
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b7a95-157">C#</span><span class="sxs-lookup"><span data-stu-id="b7a95-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateremoval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b7a95-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b7a95-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateremoval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b7a95-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b7a95-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateremoval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b7a95-160">响应</span><span class="sxs-lookup"><span data-stu-id="b7a95-160">Response</span></span>

<span data-ttu-id="b7a95-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b7a95-161">The following is an example of the response.</span></span>

> <span data-ttu-id="b7a95-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b7a95-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
