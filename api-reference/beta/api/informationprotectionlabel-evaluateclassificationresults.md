---
title: 'informationProtectionLabel: evaluateClassificationResults'
description: 根据现有内容信息和分类结果评估要应用的标签。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 22fb19a5d44ff9bed091c1cbd84183470a3490ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001464"
---
# <a name="informationprotectionlabel-evaluateclassificationresults"></a><span data-ttu-id="5b3c2-103">informationProtectionLabel: evaluateClassificationResults</span><span class="sxs-lookup"><span data-stu-id="5b3c2-103">informationProtectionLabel: evaluateClassificationResults</span></span>

<span data-ttu-id="5b3c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b3c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b3c2-105">使用 [分类结果](../resources/classificationresult.md)，计算应应用的 [信息保护标签](../resources/informationprotectionlabel.md) ，并返回为正确标记信息而必须采取的一组操作。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-105">Using [classification results](../resources/classificationresult.md), compute the [information protection label](../resources/informationprotectionlabel.md) that should be applied and return the set of actions that must be taken to correctly label the information.</span></span> <span data-ttu-id="5b3c2-106">如果标签应根据文件内容的分类自动设置，而不是由用户或服务直接标记，则此 API 非常有用。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-106">This API is useful when a label should be set automatically based on classification of the file contents, rather than labeled directly by a user or service.</span></span> 

<span data-ttu-id="5b3c2-107">若要基于分类结果进行评估，请提供 [contentInfo](../resources/contentinfo.md)，其中包括现有的内容元数据 [密钥/值对](../resources/keyvaluepair.md)和 [分类结果](../resources/classificationresult.md)。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-107">To evaluate based on classification results, provide [contentInfo](../resources/contentinfo.md), which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), and [classification results](../resources/classificationresult.md).</span></span> <span data-ttu-id="5b3c2-108">API 返回一个 [informationProtectionAction](../resources/informationprotectionaction.md) ，其中包含以下一个或多个内容：</span><span class="sxs-lookup"><span data-stu-id="5b3c2-108">The API returns an [informationProtectionAction](../resources/informationprotectionaction.md) that contains one of more of the following:</span></span> 

* [<span data-ttu-id="5b3c2-109">addContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="5b3c2-109">addContentFooterAction</span></span>](../resources/addcontentfooteraction.md)
* [<span data-ttu-id="5b3c2-110">addContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="5b3c2-110">addContentHeaderAction</span></span>](../resources/addcontentheaderaction.md)
* [<span data-ttu-id="5b3c2-111">addWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="5b3c2-111">addWatermarkAction</span></span>](../resources/addWatermarkaction.md)
* [<span data-ttu-id="5b3c2-112">applyLabelAction</span><span class="sxs-lookup"><span data-stu-id="5b3c2-112">applyLabelAction</span></span>](../resources/applylabelaction.md)
* [<span data-ttu-id="5b3c2-113">customAction</span><span class="sxs-lookup"><span data-stu-id="5b3c2-113">customAction</span></span>](../resources/customaction.md)
* [<span data-ttu-id="5b3c2-114">justifyAction</span><span class="sxs-lookup"><span data-stu-id="5b3c2-114">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="5b3c2-115">metadataAction</span><span class="sxs-lookup"><span data-stu-id="5b3c2-115">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="5b3c2-116">protectAdhocAction</span><span class="sxs-lookup"><span data-stu-id="5b3c2-116">protectAdhocAction</span></span>](../resources/protectadhocaction.md)
* [<span data-ttu-id="5b3c2-117">protectByTemplateAction</span><span class="sxs-lookup"><span data-stu-id="5b3c2-117">protectByTemplateAction</span></span>](../resources/protectBytemplateaction.md)
* [<span data-ttu-id="5b3c2-118">protectionDoNotForwardAction</span><span class="sxs-lookup"><span data-stu-id="5b3c2-118">protectionDoNotForwardAction</span></span>](../resources/protectdonotforwardaction.md)
* [<span data-ttu-id="5b3c2-119">recommendLabelAction</span><span class="sxs-lookup"><span data-stu-id="5b3c2-119">recommendLabelAction</span></span>](../resources/recommendlabelaction.md)
* [<span data-ttu-id="5b3c2-120">removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="5b3c2-120">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="5b3c2-121">removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="5b3c2-121">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="5b3c2-122">removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="5b3c2-122">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="5b3c2-123">removeWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="5b3c2-123">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="5b3c2-124">权限</span><span class="sxs-lookup"><span data-stu-id="5b3c2-124">Permissions</span></span>

<span data-ttu-id="5b3c2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b3c2-127">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b3c2-127">Permission type</span></span>                        | <span data-ttu-id="5b3c2-128">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b3c2-128">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5b3c2-129">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b3c2-129">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b3c2-130">InformationProtectionPolicy.Read</span><span class="sxs-lookup"><span data-stu-id="5b3c2-130">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="5b3c2-131">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b3c2-131">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b3c2-132">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-132">Not supported.</span></span>                              |
| <span data-ttu-id="5b3c2-133">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b3c2-133">Application</span></span>                            | <span data-ttu-id="5b3c2-134">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b3c2-134">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="5b3c2-135">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b3c2-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/{id}/evaluateClassificationResults
```

## <a name="request-headers"></a><span data-ttu-id="5b3c2-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b3c2-136">Request headers</span></span>

| <span data-ttu-id="5b3c2-137">名称</span><span class="sxs-lookup"><span data-stu-id="5b3c2-137">Name</span></span>          | <span data-ttu-id="5b3c2-138">说明</span><span class="sxs-lookup"><span data-stu-id="5b3c2-138">Description</span></span>                                                                                                                                                           |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5b3c2-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b3c2-139">Authorization</span></span> | <span data-ttu-id="5b3c2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-p104">Bearer {token}. Required.</span></span>                                                                                                                                             |
| <span data-ttu-id="5b3c2-142">Content-type</span><span class="sxs-lookup"><span data-stu-id="5b3c2-142">Content-type</span></span>  | <span data-ttu-id="5b3c2-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5b3c2-p105">application/json. Required.</span></span>                                                                                                                                           |
| <span data-ttu-id="5b3c2-145">用户代理</span><span class="sxs-lookup"><span data-stu-id="5b3c2-145">User-Agent</span></span>    | <span data-ttu-id="5b3c2-146">描述调用应用程序的名称和版本。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-146">Describes the name and version of the calling application.</span></span> <span data-ttu-id="5b3c2-147">详细信息将在 Azure 信息保护分析中显现。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-147">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="5b3c2-148">建议的格式为 "ApplicationName/版本"。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-148">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="5b3c2-149">可选。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-149">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b3c2-150">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b3c2-150">Request body</span></span>

<span data-ttu-id="5b3c2-151">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-151">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="5b3c2-152">参数</span><span class="sxs-lookup"><span data-stu-id="5b3c2-152">Parameter</span></span>             | <span data-ttu-id="5b3c2-153">类型</span><span class="sxs-lookup"><span data-stu-id="5b3c2-153">Type</span></span>                                                                    | <span data-ttu-id="5b3c2-154">说明</span><span class="sxs-lookup"><span data-stu-id="5b3c2-154">Description</span></span>                                                                                                                                                                                                                                                                           |
| :-------------------- | :---------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="5b3c2-155">contentInfo</span><span class="sxs-lookup"><span data-stu-id="5b3c2-155">contentInfo</span></span>           | [<span data-ttu-id="5b3c2-156">contentInfo</span><span class="sxs-lookup"><span data-stu-id="5b3c2-156">contentInfo</span></span>](../resources/contentInfo.md)                              | <span data-ttu-id="5b3c2-157">提供有关内容格式、内容状态和现有 [元数据](../resources/keyvaluepair.md) 的详细信息，作为键/值对。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-157">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span>                                                                                                                                                   |
| <span data-ttu-id="5b3c2-158">classificationResults</span><span class="sxs-lookup"><span data-stu-id="5b3c2-158">classificationResults</span></span> | <span data-ttu-id="5b3c2-159">[classificationResult](../resources/classificationresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5b3c2-159">[classificationResult](../resources/classificationresult.md) collection</span></span> | <span data-ttu-id="5b3c2-160">包含由数据分类终结点返回的一组分类结果。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-160">Contains the set of classification results returned by the data classification endpoint.</span></span> <span data-ttu-id="5b3c2-161">分类信息用于根据 Office 365 安全与合规中心中的 Microsoft 信息保护策略标签配置确定适当的标签。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-161">Classification information is used to determine the appropriate label based on the Microsoft Information Protection policy label configuration in Office 365 Security and Compliance Center.</span></span> |

## <a name="response"></a><span data-ttu-id="5b3c2-162">响应</span><span class="sxs-lookup"><span data-stu-id="5b3c2-162">Response</span></span>

<span data-ttu-id="5b3c2-163">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和新的 [informationProtectionAction](../resources/informationprotectionaction.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-163">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b3c2-164">示例</span><span class="sxs-lookup"><span data-stu-id="5b3c2-164">Examples</span></span>

<span data-ttu-id="5b3c2-165">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-165">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="5b3c2-166">请求</span><span class="sxs-lookup"><span data-stu-id="5b3c2-166">Request</span></span>

<span data-ttu-id="5b3c2-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5b3c2-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b3c2-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateclassificationresults"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/evaluateClassificationResults
Content-type: application/json
User-agent: ContosoLOBApp/1.0

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
# <a name="c"></a>[<span data-ttu-id="5b3c2-169">C#</span><span class="sxs-lookup"><span data-stu-id="5b3c2-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateclassificationresults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5b3c2-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b3c2-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateclassificationresults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5b3c2-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b3c2-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateclassificationresults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5b3c2-172">响应</span><span class="sxs-lookup"><span data-stu-id="5b3c2-172">Response</span></span>

<span data-ttu-id="5b3c2-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-173">The following is an example of the response.</span></span>

> <span data-ttu-id="5b3c2-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5b3c2-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


