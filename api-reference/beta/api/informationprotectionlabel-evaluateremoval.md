---
title: 'informationProtectionLabel: evaluateRemoval'
description: 评估要删除的标签以及如何根据现有内容信息将其删除。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ca1a27b30152debe51add8f0b418d3983c13b746
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995933"
---
# <a name="informationprotectionlabel-evaluateremoval"></a><span data-ttu-id="fc500-103">informationProtectionLabel: evaluateRemoval</span><span class="sxs-lookup"><span data-stu-id="fc500-103">informationProtectionLabel: evaluateRemoval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc500-104">向正在使用的应用程序指示删除标签信息应采取的操作。</span><span class="sxs-lookup"><span data-stu-id="fc500-104">Indicate to the consuming application what actions it should take to remove the label information.</span></span>

<span data-ttu-id="fc500-105">给定[contentInfo](../resources/contentinfo.md)作为输入（其中包括现有的内容元数据[密钥/值对](../resources/keyvaluepair.md)），API 将返回一个[informationProtectionAction](../resources/informationprotectionaction.md) ，其中包含以下一个或多个部分的组合：</span><span class="sxs-lookup"><span data-stu-id="fc500-105">Given [contentInfo](../resources/contentinfo.md) as an input, which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), the API returns an [informationProtectionAction](../resources/informationprotectionaction.md) that contains some combination of one of more of the following:</span></span> 

* [<span data-ttu-id="fc500-106">justifyAction</span><span class="sxs-lookup"><span data-stu-id="fc500-106">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="fc500-107">metadataAction</span><span class="sxs-lookup"><span data-stu-id="fc500-107">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="fc500-108">removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="fc500-108">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="fc500-109">removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="fc500-109">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="fc500-110">removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="fc500-110">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="fc500-111">removeWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="fc500-111">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="fc500-112">权限</span><span class="sxs-lookup"><span data-stu-id="fc500-112">Permissions</span></span>

<span data-ttu-id="fc500-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc500-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc500-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc500-115">Permission type</span></span>                        | <span data-ttu-id="fc500-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc500-116">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="fc500-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc500-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc500-118">InformationProtectionPolicy。请阅读</span><span class="sxs-lookup"><span data-stu-id="fc500-118">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="fc500-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc500-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc500-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc500-120">Not supported.</span></span>                              |
| <span data-ttu-id="fc500-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc500-121">Application</span></span>                            | <span data-ttu-id="fc500-122">InformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="fc500-122">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="fc500-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc500-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/evaluateRemoval
```

## <a name="request-headers"></a><span data-ttu-id="fc500-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc500-124">Request headers</span></span>

| <span data-ttu-id="fc500-125">名称</span><span class="sxs-lookup"><span data-stu-id="fc500-125">Name</span></span>          | <span data-ttu-id="fc500-126">说明</span><span class="sxs-lookup"><span data-stu-id="fc500-126">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="fc500-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc500-127">Authorization</span></span> | <span data-ttu-id="fc500-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fc500-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="fc500-130">Content-type</span><span class="sxs-lookup"><span data-stu-id="fc500-130">Content-type</span></span>  | <span data-ttu-id="fc500-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="fc500-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc500-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc500-133">Request body</span></span>

<span data-ttu-id="fc500-134">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="fc500-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fc500-135">参数</span><span class="sxs-lookup"><span data-stu-id="fc500-135">Parameter</span></span>              | <span data-ttu-id="fc500-136">类型</span><span class="sxs-lookup"><span data-stu-id="fc500-136">Type</span></span>                                                             | <span data-ttu-id="fc500-137">说明</span><span class="sxs-lookup"><span data-stu-id="fc500-137">Description</span></span>                                                                                                                                                                                                   |
| :--------------------- | :--------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="fc500-138">contentInfo</span><span class="sxs-lookup"><span data-stu-id="fc500-138">contentInfo</span></span>            | [<span data-ttu-id="fc500-139">contentInfo</span><span class="sxs-lookup"><span data-stu-id="fc500-139">contentInfo</span></span>](../resources/contentinfo.md)                       | <span data-ttu-id="fc500-140">提供有关内容格式、内容状态和现有[元数据](../resources/keyvaluepair.md)的详细信息，作为键/值对。</span><span class="sxs-lookup"><span data-stu-id="fc500-140">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |
| <span data-ttu-id="fc500-141">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="fc500-141">downgradeJustification</span></span> | [<span data-ttu-id="fc500-142">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="fc500-142">downgradeJustification</span></span>](../resources/downgradejustification.md) | <span data-ttu-id="fc500-143">必须由用户或应用程序逻辑提供的理由。</span><span class="sxs-lookup"><span data-stu-id="fc500-143">Justification that must be provided by the user or application logic.</span></span>                                                                                                                                         |


## <a name="response"></a><span data-ttu-id="fc500-144">响应</span><span class="sxs-lookup"><span data-stu-id="fc500-144">Response</span></span>

<span data-ttu-id="fc500-145">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[informationProtectionAction](../resources/informationprotectionaction.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="fc500-145">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span> <span data-ttu-id="fc500-146">[InformationProtectionAction 对象](../resources/informationprotectionaction.md)将包含一个[metadataAction](../resources/metadataaction.md)对象，该对象通知应用程序要删除的元数据。</span><span class="sxs-lookup"><span data-stu-id="fc500-146">The [informationProtectionAction object](../resources/informationprotectionaction.md) will contain a [metadataAction](../resources/metadataaction.md) object that informs the application which metadata to remove.</span></span> 

## <a name="examples"></a><span data-ttu-id="fc500-147">示例</span><span class="sxs-lookup"><span data-stu-id="fc500-147">Examples</span></span>

<span data-ttu-id="fc500-148">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="fc500-148">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="fc500-149">请求</span><span class="sxs-lookup"><span data-stu-id="fc500-149">Request</span></span>

<span data-ttu-id="fc500-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fc500-150">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fc500-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc500-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateremoval"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/evaluateRemoval
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fc500-152">C#</span><span class="sxs-lookup"><span data-stu-id="fc500-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateremoval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc500-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc500-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateremoval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc500-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc500-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateremoval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fc500-155">响应</span><span class="sxs-lookup"><span data-stu-id="fc500-155">Response</span></span>

<span data-ttu-id="fc500-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fc500-156">The following is an example of the response.</span></span>

> <span data-ttu-id="fc500-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fc500-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
