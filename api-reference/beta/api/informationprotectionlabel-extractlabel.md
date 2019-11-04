---
title: 'informationProtectionLabel: extractLabel'
description: 使用来自带标签的对象的元数据检索 informationProtectionContentLabel。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6fe074f5dfa27dbad6b5415f3c75d5458665d2ea
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938020"
---
# <a name="informationprotectionlabel-extractlabel"></a><span data-ttu-id="d1da4-103">informationProtectionLabel: extractLabel</span><span class="sxs-lookup"><span data-stu-id="d1da4-103">informationProtectionLabel: extractLabel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1da4-104">使用已标记的信息中存在的元数据，将元数据解析为特定的敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="d1da4-104">Using the metadata that exists on an already-labeled piece of information, resolve the metadata to a specific sensitivity label.</span></span> <span data-ttu-id="d1da4-105">将[contentInfo](../resources/contentinfo.md)输入解析为[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)。</span><span class="sxs-lookup"><span data-stu-id="d1da4-105">The [contentInfo](../resources/contentinfo.md) input is resolved to [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md).</span></span>

>[!NOTE]
><span data-ttu-id="d1da4-106">**[InformationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** 资源表示已应用于一条信息的敏感度标签。</span><span class="sxs-lookup"><span data-stu-id="d1da4-106">The **[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** resource represents a sensitivity label that has been applied to a piece of information.</span></span> <span data-ttu-id="d1da4-107">[informationProtectionLabel](../resources/informationprotectionlabel.md)对象是组织标记策略的一部分的抽象标签，可应用于信息。</span><span class="sxs-lookup"><span data-stu-id="d1da4-107">[informationProtectionLabel](../resources/informationprotectionlabel.md) objects are the abstract labels that are part of the organizational labeling policy and can be applied to information.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1da4-108">权限</span><span class="sxs-lookup"><span data-stu-id="d1da4-108">Permissions</span></span>

<span data-ttu-id="d1da4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1da4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d1da4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1da4-111">Permission type</span></span>                        | <span data-ttu-id="d1da4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1da4-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d1da4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1da4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1da4-114">InformationProtectionPolicy。请阅读</span><span class="sxs-lookup"><span data-stu-id="d1da4-114">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="d1da4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1da4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1da4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1da4-116">Not supported.</span></span>                              |
| <span data-ttu-id="d1da4-117">Application</span><span class="sxs-lookup"><span data-stu-id="d1da4-117">Application</span></span>                            | <span data-ttu-id="d1da4-118">InformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="d1da4-118">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="d1da4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1da4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/extractLabel
```

## <a name="request-headers"></a><span data-ttu-id="d1da4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1da4-120">Request headers</span></span>

| <span data-ttu-id="d1da4-121">名称</span><span class="sxs-lookup"><span data-stu-id="d1da4-121">Name</span></span>          | <span data-ttu-id="d1da4-122">说明</span><span class="sxs-lookup"><span data-stu-id="d1da4-122">Description</span></span>                    |
| :------------ | :----------------------------- |
| <span data-ttu-id="d1da4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1da4-123">Authorization</span></span> | <span data-ttu-id="d1da4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d1da4-p104">Bearer {token}. Required.</span></span>                 |
| <span data-ttu-id="d1da4-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="d1da4-126">Content-type</span></span>  | <span data-ttu-id="d1da4-127">Content-type： application/json。</span><span class="sxs-lookup"><span data-stu-id="d1da4-127">Content-type: application/json.</span></span> <span data-ttu-id="d1da4-128">必填。</span><span class="sxs-lookup"><span data-stu-id="d1da4-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1da4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1da4-129">Request body</span></span>

<span data-ttu-id="d1da4-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="d1da4-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d1da4-131">参数</span><span class="sxs-lookup"><span data-stu-id="d1da4-131">Parameter</span></span>   | <span data-ttu-id="d1da4-132">类型</span><span class="sxs-lookup"><span data-stu-id="d1da4-132">Type</span></span>                                       | <span data-ttu-id="d1da4-133">描述</span><span class="sxs-lookup"><span data-stu-id="d1da4-133">Description</span></span>                                                                                                                                                                                                   |
| :---------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="d1da4-134">contentInfo</span><span class="sxs-lookup"><span data-stu-id="d1da4-134">contentInfo</span></span> | [<span data-ttu-id="d1da4-135">contentInfo</span><span class="sxs-lookup"><span data-stu-id="d1da4-135">contentInfo</span></span>](../resources/contentinfo.md) | <span data-ttu-id="d1da4-136">提供有关内容格式、内容状态和现有[元数据](../resources/keyvaluepair.md)的详细信息，作为键/值对。</span><span class="sxs-lookup"><span data-stu-id="d1da4-136">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |

## <a name="response"></a><span data-ttu-id="d1da4-137">响应</span><span class="sxs-lookup"><span data-stu-id="d1da4-137">Response</span></span>

<span data-ttu-id="d1da4-138">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d1da4-138">If successful, this method returns a `200 OK` response code and a new [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d1da4-139">示例</span><span class="sxs-lookup"><span data-stu-id="d1da4-139">Examples</span></span>

<span data-ttu-id="d1da4-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="d1da4-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="d1da4-141">请求</span><span class="sxs-lookup"><span data-stu-id="d1da4-141">Request</span></span>

<span data-ttu-id="d1da4-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d1da4-142">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d1da4-143">响应</span><span class="sxs-lookup"><span data-stu-id="d1da4-143">Response</span></span>

<span data-ttu-id="d1da4-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d1da4-144">The following is an example of the response.</span></span>

> <span data-ttu-id="d1da4-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d1da4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
