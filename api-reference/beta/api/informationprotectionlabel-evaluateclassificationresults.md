---
title: 'informationProtectionLabel: evaluateClassificationResults'
description: 根据现有内容信息和分类结果评估要应用的标签。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 06031fd4887b417fe12858ca5d3f1622f58a4f96
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995617"
---
# <a name="informationprotectionlabel-evaluateclassificationresults"></a><span data-ttu-id="74930-103">informationProtectionLabel: evaluateClassificationResults</span><span class="sxs-lookup"><span data-stu-id="74930-103">informationProtectionLabel: evaluateClassificationResults</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74930-104">使用[分类结果](../resources/classificationresult.md)，计算应应用的[信息保护标签](../resources/informationprotectionlabel.md)，并返回为正确标记信息而必须采取的一组操作。</span><span class="sxs-lookup"><span data-stu-id="74930-104">Using [classification results](../resources/classificationresult.md), compute the [information protection label](../resources/informationprotectionlabel.md) that should be applied and return the set of actions that must be taken to correctly label the information.</span></span> <span data-ttu-id="74930-105">如果标签应根据文件内容的分类自动设置，而不是由用户或服务直接标记，则此 API 非常有用。</span><span class="sxs-lookup"><span data-stu-id="74930-105">This API is useful when a label should be set automatically based on classification of the file contents, rather than labeled directly by a user or service.</span></span> 

<span data-ttu-id="74930-106">若要基于分类结果进行评估，请提供[contentInfo](../resources/contentinfo.md)，其中包括现有的内容元数据[密钥/值对](../resources/keyvaluepair.md)和[分类结果](../resources/classificationresult.md)。</span><span class="sxs-lookup"><span data-stu-id="74930-106">To evaluate based on classification results, provide [contentInfo](../resources/contentinfo.md), which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), and [classification results](../resources/classificationresult.md).</span></span> <span data-ttu-id="74930-107">API 返回一个[informationProtectionAction](../resources/informationprotectionaction.md) ，其中包含以下一个或多个内容：</span><span class="sxs-lookup"><span data-stu-id="74930-107">The API returns an [informationProtectionAction](../resources/informationprotectionaction.md) that contains one of more of the following:</span></span> 

* [<span data-ttu-id="74930-108">addContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="74930-108">addContentFooterAction</span></span>](../resources/addcontentfooteraction.md)
* [<span data-ttu-id="74930-109">addContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="74930-109">addContentHeaderAction</span></span>](../resources/addcontentheaderaction.md)
* [<span data-ttu-id="74930-110">addWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="74930-110">addWatermarkAction</span></span>](../resources/addWatermarkaction.md)
* [<span data-ttu-id="74930-111">applyLabelAction</span><span class="sxs-lookup"><span data-stu-id="74930-111">applyLabelAction</span></span>](../resources/applylabelaction.md)
* [<span data-ttu-id="74930-112">customAction</span><span class="sxs-lookup"><span data-stu-id="74930-112">customAction</span></span>](../resources/customaction.md)
* [<span data-ttu-id="74930-113">justifyAction</span><span class="sxs-lookup"><span data-stu-id="74930-113">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="74930-114">metadataAction</span><span class="sxs-lookup"><span data-stu-id="74930-114">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="74930-115">protectAdhocAction</span><span class="sxs-lookup"><span data-stu-id="74930-115">protectAdhocAction</span></span>](../resources/protectadhocaction.md)
* [<span data-ttu-id="74930-116">protectByTemplateAction</span><span class="sxs-lookup"><span data-stu-id="74930-116">protectByTemplateAction</span></span>](../resources/protectBytemplateaction.md)
* [<span data-ttu-id="74930-117">protectionDoNotForwardAction</span><span class="sxs-lookup"><span data-stu-id="74930-117">protectionDoNotForwardAction</span></span>](../resources/protectdonotforwardaction.md)
* [<span data-ttu-id="74930-118">recommendLabelAction</span><span class="sxs-lookup"><span data-stu-id="74930-118">recommendLabelAction</span></span>](../resources/recommendlabelaction.md)
* [<span data-ttu-id="74930-119">removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="74930-119">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="74930-120">removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="74930-120">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="74930-121">removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="74930-121">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="74930-122">removeWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="74930-122">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="74930-123">权限</span><span class="sxs-lookup"><span data-stu-id="74930-123">Permissions</span></span>

<span data-ttu-id="74930-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="74930-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="74930-126">权限类型</span><span class="sxs-lookup"><span data-stu-id="74930-126">Permission type</span></span>                        | <span data-ttu-id="74930-127">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="74930-127">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="74930-128">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="74930-128">Delegated (work or school account)</span></span>     | <span data-ttu-id="74930-129">InformationProtectionPolicy。请阅读</span><span class="sxs-lookup"><span data-stu-id="74930-129">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="74930-130">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="74930-130">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="74930-131">不支持。</span><span class="sxs-lookup"><span data-stu-id="74930-131">Not supported.</span></span>                              |
| <span data-ttu-id="74930-132">应用程序</span><span class="sxs-lookup"><span data-stu-id="74930-132">Application</span></span>                            | <span data-ttu-id="74930-133">InformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="74930-133">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="74930-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="74930-134">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/{id}/evaluateClassificationResults
```

## <a name="request-headers"></a><span data-ttu-id="74930-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="74930-135">Request headers</span></span>

| <span data-ttu-id="74930-136">名称</span><span class="sxs-lookup"><span data-stu-id="74930-136">Name</span></span>          | <span data-ttu-id="74930-137">说明</span><span class="sxs-lookup"><span data-stu-id="74930-137">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="74930-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="74930-138">Authorization</span></span> | <span data-ttu-id="74930-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="74930-p104">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="74930-141">Content-type</span><span class="sxs-lookup"><span data-stu-id="74930-141">Content-type</span></span>  | <span data-ttu-id="74930-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="74930-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="74930-144">请求正文</span><span class="sxs-lookup"><span data-stu-id="74930-144">Request body</span></span>

<span data-ttu-id="74930-145">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="74930-145">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="74930-146">参数</span><span class="sxs-lookup"><span data-stu-id="74930-146">Parameter</span></span>             | <span data-ttu-id="74930-147">类型</span><span class="sxs-lookup"><span data-stu-id="74930-147">Type</span></span>                                                                    | <span data-ttu-id="74930-148">说明</span><span class="sxs-lookup"><span data-stu-id="74930-148">Description</span></span>                                                                                                                                                                                                                                                                           |
| :-------------------- | :---------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="74930-149">contentInfo</span><span class="sxs-lookup"><span data-stu-id="74930-149">contentInfo</span></span>           | [<span data-ttu-id="74930-150">contentInfo</span><span class="sxs-lookup"><span data-stu-id="74930-150">contentInfo</span></span>](../resources/contentInfo.md)                              | <span data-ttu-id="74930-151">提供有关内容格式、内容状态和现有[元数据](../resources/keyvaluepair.md)的详细信息，作为键/值对。</span><span class="sxs-lookup"><span data-stu-id="74930-151">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span>                                                                         |
| <span data-ttu-id="74930-152">classificationResults</span><span class="sxs-lookup"><span data-stu-id="74930-152">classificationResults</span></span> | <span data-ttu-id="74930-153">[classificationResult](../resources/classificationresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="74930-153">[classificationResult](../resources/classificationresult.md) collection</span></span> | <span data-ttu-id="74930-154">包含由数据分类终结点返回的一组分类结果。</span><span class="sxs-lookup"><span data-stu-id="74930-154">Contains the set of classification results returned by the data classification endpoint.</span></span> <span data-ttu-id="74930-155">Classificaiton 信息用于根据 Office 365 安全与合规中心中的 Microsoft 信息保护策略标签配置确定适当的标签。</span><span class="sxs-lookup"><span data-stu-id="74930-155">Classificaiton information is used to determine the appropriate label based on the Microsoft Information Protection policy label configuration in Office 365 Security and Compliance Center.</span></span> |

## <a name="response"></a><span data-ttu-id="74930-156">响应</span><span class="sxs-lookup"><span data-stu-id="74930-156">Response</span></span>

<span data-ttu-id="74930-157">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[informationProtectionAction](../resources/informationprotectionaction.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="74930-157">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="74930-158">示例</span><span class="sxs-lookup"><span data-stu-id="74930-158">Examples</span></span>

<span data-ttu-id="74930-159">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="74930-159">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="74930-160">请求</span><span class="sxs-lookup"><span data-stu-id="74930-160">Request</span></span>

<span data-ttu-id="74930-161">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="74930-161">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="74930-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="74930-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateclassificationresults"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/evaluateClassificationResults
Content-type: application/json

{
  "contentInfo": {
    "@odata.type": "#microsoft.graph.contentInfo",
    "format@odata.type": "#microsoft.graph.contentFormat",
    "format": "default",
    "identifier": null,
    "state@odata.type": "#microsoft.graph.contentState",
    "state": "rest"
  },
  "classificationResults": [
    {
      "sensitiveTypeId": "cb353f78-2b72-4c3c-8827-92ebe4f69fdf",
      "count": 4,
      "confidenceLevel": 75
    }
   ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="74930-163">C#</span><span class="sxs-lookup"><span data-stu-id="74930-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateclassificationresults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="74930-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="74930-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateclassificationresults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="74930-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="74930-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateclassificationresults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="74930-166">响应</span><span class="sxs-lookup"><span data-stu-id="74930-166">Response</span></span>

<span data-ttu-id="74930-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="74930-167">The following is an example of the response.</span></span>

> <span data-ttu-id="74930-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="74930-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
            "@odata.type": "#microsoft.graph.applyLabelAction",
            "responsibleSensitiveTypeIds": [
                "cb353f78-2b72-4c3c-8827-92ebe4f69fdf"
            ],
            "actionSource": "automatic",
            "label": {
                "id": "722a5300-ac39-4c9a-88e3-f54c46676417",
                "name": "Top Secret",
                "description": "",
                "color": "#000000",
                "sensitivity": 13,
                "tooltip": "This information is Top Secret.",
                "isActive": true
            },
            "actions": [
                {
                    "@odata.type": "#microsoft.graph.protectByTemplateAction",
                    "templateId": "0e7fea72-7bba-4438-a070-95c292cd6f8c"
                },
                {
                    "@odata.type": "#microsoft.graph.metadataAction",
                    "metadataToRemove": [],
                    "metadataToAdd": [
                        {
                            "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
                            "value": "true"
                        },
                        {
                            "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
                            "value": "2019-10-03T21:50:20Z"
                        },
                        {
                            "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
                            "value": "Standard"
                        },
                        {
                            "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
                            "value": "Top Secret"
                        },
                        {
                            "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
                            "value": "cb46c030-1825-4e81-a295-151c039dbf02"
                        },
                        {
                            "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId",
                            "value": "76dc494e-6c59-43e6-88a1-0000edd58fca"
                        },
                        {
                            "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
                            "value": "8"
                        }
                    ]
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel: evaluateClassificationResults",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
