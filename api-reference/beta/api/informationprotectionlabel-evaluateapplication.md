---
title: informationProtectionLabel：evaluateApplication
description: 根据现有内容信息和所需内容状态评估要应用的标签。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: b48fd3e0137e90232b484acd142224a9a8cdc70c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960956"
---
# <a name="informationprotectionlabel-evaluateapplication"></a><span data-ttu-id="2657d-103">informationProtectionLabel：evaluateApplication</span><span class="sxs-lookup"><span data-stu-id="2657d-103">informationProtectionLabel: evaluateApplication</span></span>

<span data-ttu-id="2657d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2657d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2657d-105">计算 [应应用](../resources/informationprotectionlabel.md) 的信息保护标签，并返回正确标记信息所必须采取的一组操作。</span><span class="sxs-lookup"><span data-stu-id="2657d-105">Compute the [information protection label](../resources/informationprotectionlabel.md) that should be applied and return the set of actions that must be taken to correctly label the information.</span></span> <span data-ttu-id="2657d-106">当用户或服务应手动或显式设置标签，而不是基于文件内容自动设置标签时，此 API 非常有用。</span><span class="sxs-lookup"><span data-stu-id="2657d-106">This API is useful when a label should be set manually or explicitly by a user or service, rather than automatically based on file contents.</span></span> 

<span data-ttu-id="2657d-107">在 [给定 contentInfo](../resources/contentInfo.md)（包括现有内容元数据键 [/](../resources/keyvaluepair.md)值对 ）和 [labelingOptions](../resources/labelingoptions.md) 作为输入时，API 将返回一个 [informationProtectionAction](../resources/informationprotectionaction.md) 对象，该对象包含以下项之一：</span><span class="sxs-lookup"><span data-stu-id="2657d-107">Given [contentInfo](../resources/contentInfo.md), which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), and [labelingOptions](../resources/labelingoptions.md) as an input, the API returns an [informationProtectionAction](../resources/informationprotectionaction.md) object that contains one of more of the following:</span></span> 

* [<span data-ttu-id="2657d-108">addContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="2657d-108">addContentFooterAction</span></span>](../resources/addcontentfooteraction.md)
* [<span data-ttu-id="2657d-109">addContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="2657d-109">addContentHeaderAction</span></span>](../resources/addcontentheaderaction.md)
* [<span data-ttu-id="2657d-110">addActionmarkAction</span><span class="sxs-lookup"><span data-stu-id="2657d-110">addWatermarkAction</span></span>](../resources/addWatermarkaction.md)
* [<span data-ttu-id="2657d-111">applyLabelAction</span><span class="sxs-lookup"><span data-stu-id="2657d-111">applyLabelAction</span></span>](../resources/applylabelaction.md)
* [<span data-ttu-id="2657d-112">customAction</span><span class="sxs-lookup"><span data-stu-id="2657d-112">customAction</span></span>](../resources/customaction.md)
* [<span data-ttu-id="2657d-113">justifyAction</span><span class="sxs-lookup"><span data-stu-id="2657d-113">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="2657d-114">metadataAction</span><span class="sxs-lookup"><span data-stu-id="2657d-114">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="2657d-115">protectAdhocAction</span><span class="sxs-lookup"><span data-stu-id="2657d-115">protectAdhocAction</span></span>](../resources/protectadhocaction.md)
* [<span data-ttu-id="2657d-116">protectByTemplateAction</span><span class="sxs-lookup"><span data-stu-id="2657d-116">protectByTemplateAction</span></span>](../resources/protectBytemplateaction.md)
* [<span data-ttu-id="2657d-117">protectionDoNotForwardAction</span><span class="sxs-lookup"><span data-stu-id="2657d-117">protectionDoNotForwardAction</span></span>](../resources/protectdonotforwardaction.md)
* [<span data-ttu-id="2657d-118">recommendLabelAction</span><span class="sxs-lookup"><span data-stu-id="2657d-118">recommendLabelAction</span></span>](../resources/recommendlabelaction.md)
* [<span data-ttu-id="2657d-119">removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="2657d-119">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="2657d-120">removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="2657d-120">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="2657d-121">removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="2657d-121">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="2657d-122">remove使用markAction</span><span class="sxs-lookup"><span data-stu-id="2657d-122">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="2657d-123">权限</span><span class="sxs-lookup"><span data-stu-id="2657d-123">Permissions</span></span>

<span data-ttu-id="2657d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2657d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2657d-126">权限类型</span><span class="sxs-lookup"><span data-stu-id="2657d-126">Permission type</span></span>                        | <span data-ttu-id="2657d-127">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2657d-127">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2657d-128">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2657d-128">Delegated (work or school account)</span></span>     | <span data-ttu-id="2657d-129">InformationProtectionPolicy.Read</span><span class="sxs-lookup"><span data-stu-id="2657d-129">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="2657d-130">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2657d-130">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2657d-131">不支持。</span><span class="sxs-lookup"><span data-stu-id="2657d-131">Not supported.</span></span>                              |
| <span data-ttu-id="2657d-132">应用程序</span><span class="sxs-lookup"><span data-stu-id="2657d-132">Application</span></span>                            | <span data-ttu-id="2657d-133">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="2657d-133">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="2657d-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2657d-134">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/informationProtection/policy/labels/evaluateApplication
POST /users/{id}/informationProtection/policy/labels/evaluateApplication
```

## <a name="request-headers"></a><span data-ttu-id="2657d-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="2657d-135">Request headers</span></span>

| <span data-ttu-id="2657d-136">名称</span><span class="sxs-lookup"><span data-stu-id="2657d-136">Name</span></span>          | <span data-ttu-id="2657d-137">说明</span><span class="sxs-lookup"><span data-stu-id="2657d-137">Description</span></span>                                                                                                                                                           |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2657d-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="2657d-138">Authorization</span></span> | <span data-ttu-id="2657d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2657d-p103">Bearer {token}. Required.</span></span>                                                                                                                                             |
| <span data-ttu-id="2657d-141">Content-type</span><span class="sxs-lookup"><span data-stu-id="2657d-141">Content-type</span></span>  | <span data-ttu-id="2657d-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2657d-p104">application/json. Required.</span></span>                                                                                                                                           |
| <span data-ttu-id="2657d-144">User-Agent</span><span class="sxs-lookup"><span data-stu-id="2657d-144">User-Agent</span></span>    | <span data-ttu-id="2657d-145">描述调用应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="2657d-145">Describes the name of the calling application.</span></span> <span data-ttu-id="2657d-146">详细信息将显示于 Azure 信息保护分析中。</span><span class="sxs-lookup"><span data-stu-id="2657d-146">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="2657d-147">建议的格式为 ApplicationName/Version。</span><span class="sxs-lookup"><span data-stu-id="2657d-147">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="2657d-148">可选。</span><span class="sxs-lookup"><span data-stu-id="2657d-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2657d-149">请求正文</span><span class="sxs-lookup"><span data-stu-id="2657d-149">Request body</span></span>

<span data-ttu-id="2657d-150">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2657d-150">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2657d-151">参数</span><span class="sxs-lookup"><span data-stu-id="2657d-151">Parameter</span></span>       | <span data-ttu-id="2657d-152">类型</span><span class="sxs-lookup"><span data-stu-id="2657d-152">Type</span></span>                                               | <span data-ttu-id="2657d-153">说明</span><span class="sxs-lookup"><span data-stu-id="2657d-153">Description</span></span>                                                                                                                      |
| :-------------- | :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2657d-154">contentInfo</span><span class="sxs-lookup"><span data-stu-id="2657d-154">contentInfo</span></span>     | [<span data-ttu-id="2657d-155">contentInfo</span><span class="sxs-lookup"><span data-stu-id="2657d-155">contentInfo</span></span>](../resources/contentinfo.md)         | <span data-ttu-id="2657d-156">提供有关内容格式、内容状态和作为键/值对[](../resources/keyvaluepair.md)的现有元数据的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2657d-156">Provides details on the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |
| <span data-ttu-id="2657d-157">labelingOptions</span><span class="sxs-lookup"><span data-stu-id="2657d-157">labelingOptions</span></span> | [<span data-ttu-id="2657d-158">labelingOptions</span><span class="sxs-lookup"><span data-stu-id="2657d-158">labelingOptions</span></span>](../resources/labelingoptions.md) | <span data-ttu-id="2657d-159">提供有关内容所需状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2657d-159">Provides details about the desired state of the content.</span></span>                                                                         |

## <a name="response"></a><span data-ttu-id="2657d-160">响应</span><span class="sxs-lookup"><span data-stu-id="2657d-160">Response</span></span>

<span data-ttu-id="2657d-161">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和新 [informationProtectionAction](../resources/informationprotectionaction.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="2657d-161">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2657d-162">示例</span><span class="sxs-lookup"><span data-stu-id="2657d-162">Examples</span></span>

<span data-ttu-id="2657d-163">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="2657d-163">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2657d-164">请求</span><span class="sxs-lookup"><span data-stu-id="2657d-164">Request</span></span>

<span data-ttu-id="2657d-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2657d-165">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2657d-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="2657d-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateapplication"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/policy/labels/evaluateApplication
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
  "labelingOptions": {
    "@odata.type": "#microsoft.graph.labelingOptions",
    "assignmentMethod@odata.type": "#microsoft.graph.assignmentMethod",
    "assignmentMethod": "standard",
    "labelId@odata.type": "#Guid",
    "labelId": "97309856-9c28-4ac6-9382-5f8bc20c457b",
    "downgradeJustification": null,
    "extendedProperties@odata.type": "#Collection(microsoft.graph.keyValuePair)",
    "extendedProperties": []
  }
}
```
# <a name="c"></a>[<span data-ttu-id="2657d-167">C#</span><span class="sxs-lookup"><span data-stu-id="2657d-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2657d-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2657d-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2657d-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2657d-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2657d-170">Java</span><span class="sxs-lookup"><span data-stu-id="2657d-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/informationprotectionlabel-evaluateapplication-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2657d-171">响应</span><span class="sxs-lookup"><span data-stu-id="2657d-171">Response</span></span>

<span data-ttu-id="2657d-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2657d-172">The following is an example of the response.</span></span>

> <span data-ttu-id="2657d-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2657d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
            "@odata.type": "#microsoft.graph.protectByTemplateAction",
            "templateId": "31f2f3ba-1a56-48b7-ad90-0edc774ccfa2"
        },
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
            "metadataToAdd": [
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_Enabled",
                    "value": "true"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_SetDate",
                    "value": "2019-10-03T21:40:02Z"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_Method",
                    "value": "Standard"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_Name",
                    "value": "Inspire Demo"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_SiteId",
                    "value": "cb46c030-1825-4e81-a295-151c039dbf02"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_ActionId",
                    "value": "987357d3-6512-46b5-b20e-000065400015"
                },
                {
                    "name": "MSIP_Label_97309856-9c28-4ac6-9382-5f8bc20c457b_ContentBits",
                    "value": "8"
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
  "description": "informationProtectionLabel: evaluateApplication",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


