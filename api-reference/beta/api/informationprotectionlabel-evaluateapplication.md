---
title: 'informationProtectionLabel: evaluateApplication'
description: 根据现有内容信息和所需内容状态评估要应用的标签。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 92de4d75e93be416b255dfc43400b304938a9759
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994436"
---
# <a name="informationprotectionlabel-evaluateapplication"></a><span data-ttu-id="2ff86-103">informationProtectionLabel: evaluateApplication</span><span class="sxs-lookup"><span data-stu-id="2ff86-103">informationProtectionLabel: evaluateApplication</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ff86-104">计算应应用的[信息保护标签](../resources/informationprotectionlabel.md)，并返回正确标记信息所需采取的一组操作。</span><span class="sxs-lookup"><span data-stu-id="2ff86-104">Compute the [information protection label](../resources/informationprotectionlabel.md) that should be applied and return the set of actions that must be taken to correctly label the information.</span></span> <span data-ttu-id="2ff86-105">如果标签应手动设置或由用户或服务显式设置，而不是基于文件内容自动设置，则此 API 非常有用。</span><span class="sxs-lookup"><span data-stu-id="2ff86-105">This API is useful when a label should be set manually or explicitly by a user or service, rather than automatically based on file contents.</span></span> 

<span data-ttu-id="2ff86-106">给定[contentInfo](../resources/contentInfo.md)（包括现有内容元数据[密钥/值对](../resources/keyvaluepair.md)）和[labelingOptions](../resources/labelingoptions.md)作为输入，API 将返回一个[informationProtectionAction](../resources/informationprotectionaction.md)对象，其中包含以下一个或多个内容：</span><span class="sxs-lookup"><span data-stu-id="2ff86-106">Given [contentInfo](../resources/contentInfo.md), which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), and [labelingOptions](../resources/labelingoptions.md) as an input, the API returns an [informationProtectionAction](../resources/informationprotectionaction.md) object that contains one of more of the following:</span></span> 

* [<span data-ttu-id="2ff86-107">addContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="2ff86-107">addContentFooterAction</span></span>](../resources/addcontentfooteraction.md)
* [<span data-ttu-id="2ff86-108">addContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="2ff86-108">addContentHeaderAction</span></span>](../resources/addcontentheaderaction.md)
* [<span data-ttu-id="2ff86-109">addWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="2ff86-109">addWatermarkAction</span></span>](../resources/addWatermarkaction.md)
* [<span data-ttu-id="2ff86-110">applyLabelAction</span><span class="sxs-lookup"><span data-stu-id="2ff86-110">applyLabelAction</span></span>](../resources/applylabelaction.md)
* [<span data-ttu-id="2ff86-111">customAction</span><span class="sxs-lookup"><span data-stu-id="2ff86-111">customAction</span></span>](../resources/customaction.md)
* [<span data-ttu-id="2ff86-112">justifyAction</span><span class="sxs-lookup"><span data-stu-id="2ff86-112">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="2ff86-113">metadataAction</span><span class="sxs-lookup"><span data-stu-id="2ff86-113">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="2ff86-114">protectAdhocAction</span><span class="sxs-lookup"><span data-stu-id="2ff86-114">protectAdhocAction</span></span>](../resources/protectadhocaction.md)
* [<span data-ttu-id="2ff86-115">protectByTemplateAction</span><span class="sxs-lookup"><span data-stu-id="2ff86-115">protectByTemplateAction</span></span>](../resources/protectBytemplateaction.md)
* [<span data-ttu-id="2ff86-116">protectionDoNotForwardAction</span><span class="sxs-lookup"><span data-stu-id="2ff86-116">protectionDoNotForwardAction</span></span>](../resources/protectdonotforwardaction.md)
* [<span data-ttu-id="2ff86-117">recommendLabelAction</span><span class="sxs-lookup"><span data-stu-id="2ff86-117">recommendLabelAction</span></span>](../resources/recommendlabelaction.md)
* [<span data-ttu-id="2ff86-118">removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="2ff86-118">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="2ff86-119">removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="2ff86-119">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="2ff86-120">removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="2ff86-120">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="2ff86-121">removeWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="2ff86-121">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="2ff86-122">权限</span><span class="sxs-lookup"><span data-stu-id="2ff86-122">Permissions</span></span>

<span data-ttu-id="2ff86-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ff86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ff86-125">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ff86-125">Permission type</span></span>                        | <span data-ttu-id="2ff86-126">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ff86-126">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2ff86-127">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ff86-127">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ff86-128">InformationProtectionPolicy。请阅读</span><span class="sxs-lookup"><span data-stu-id="2ff86-128">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="2ff86-129">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ff86-129">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ff86-130">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ff86-130">Not supported.</span></span>                              |
| <span data-ttu-id="2ff86-131">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ff86-131">Application</span></span>                            | <span data-ttu-id="2ff86-132">InformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="2ff86-132">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="2ff86-133">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ff86-133">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST me/informationprotection/policy/labels/evaluateApplication
POST /users/{id}/informationProtection/policy/labels/evaluateApplication
```

## <a name="request-headers"></a><span data-ttu-id="2ff86-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ff86-134">Request headers</span></span>

| <span data-ttu-id="2ff86-135">名称</span><span class="sxs-lookup"><span data-stu-id="2ff86-135">Name</span></span>          | <span data-ttu-id="2ff86-136">说明</span><span class="sxs-lookup"><span data-stu-id="2ff86-136">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="2ff86-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ff86-137">Authorization</span></span> | <span data-ttu-id="2ff86-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ff86-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="2ff86-140">Content-type</span><span class="sxs-lookup"><span data-stu-id="2ff86-140">Content-type</span></span>  | <span data-ttu-id="2ff86-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2ff86-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ff86-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ff86-143">Request body</span></span>

<span data-ttu-id="2ff86-144">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2ff86-144">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2ff86-145">参数</span><span class="sxs-lookup"><span data-stu-id="2ff86-145">Parameter</span></span>       | <span data-ttu-id="2ff86-146">类型</span><span class="sxs-lookup"><span data-stu-id="2ff86-146">Type</span></span>                                               | <span data-ttu-id="2ff86-147">说明</span><span class="sxs-lookup"><span data-stu-id="2ff86-147">Description</span></span>                                                                                                                                                                                                   |
| :-------------- | :------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="2ff86-148">contentInfo</span><span class="sxs-lookup"><span data-stu-id="2ff86-148">contentInfo</span></span>     | [<span data-ttu-id="2ff86-149">contentInfo</span><span class="sxs-lookup"><span data-stu-id="2ff86-149">contentInfo</span></span>](../resources/contentinfo.md)         | <span data-ttu-id="2ff86-150">提供有关内容格式、内容状态和现有[元数据](../resources/keyvaluepair.md)的详细信息，作为键/值对。</span><span class="sxs-lookup"><span data-stu-id="2ff86-150">Provides details on the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |
| <span data-ttu-id="2ff86-151">labelingOptions</span><span class="sxs-lookup"><span data-stu-id="2ff86-151">labelingOptions</span></span> | [<span data-ttu-id="2ff86-152">labelingOptions</span><span class="sxs-lookup"><span data-stu-id="2ff86-152">labelingOptions</span></span>](../resources/labelingoptions.md) | <span data-ttu-id="2ff86-153">提供有关内容的所需状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2ff86-153">Provides details about the desired state of the content.</span></span>                                                                                                                                                      |

## <a name="response"></a><span data-ttu-id="2ff86-154">响应</span><span class="sxs-lookup"><span data-stu-id="2ff86-154">Response</span></span>

<span data-ttu-id="2ff86-155">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[informationProtectionAction](../resources/informationprotectionaction.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="2ff86-155">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ff86-156">示例</span><span class="sxs-lookup"><span data-stu-id="2ff86-156">Examples</span></span>

<span data-ttu-id="2ff86-157">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="2ff86-157">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2ff86-158">请求</span><span class="sxs-lookup"><span data-stu-id="2ff86-158">Request</span></span>

<span data-ttu-id="2ff86-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2ff86-159">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2ff86-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ff86-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateapplication"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/evaluateApplication
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2ff86-161">C#</span><span class="sxs-lookup"><span data-stu-id="2ff86-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateapplication-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ff86-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ff86-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateapplication-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2ff86-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ff86-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateapplication-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ff86-164">响应</span><span class="sxs-lookup"><span data-stu-id="2ff86-164">Response</span></span>

<span data-ttu-id="2ff86-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2ff86-165">The following is an example of the response.</span></span>

> <span data-ttu-id="2ff86-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2ff86-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
