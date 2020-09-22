---
title: samlSingleSignOnSettings 资源类型
description: 表示 SAML 单一登录设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 6c07e9c0284ef111a3032ec729c3b741be65f920
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016028"
---
# <a name="samlsinglesignonsettings-resource-type"></a><span data-ttu-id="4da0b-103">samlSingleSignOnSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="4da0b-103">samlSingleSignOnSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4da0b-104">表示与 SAML single sign-on 相关的设置的容器。</span><span class="sxs-lookup"><span data-stu-id="4da0b-104">Represents a container for settings related to SAML single sign-on.</span></span>

## <a name="properties"></a><span data-ttu-id="4da0b-105">属性</span><span class="sxs-lookup"><span data-stu-id="4da0b-105">Properties</span></span>

| <span data-ttu-id="4da0b-106">属性</span><span class="sxs-lookup"><span data-stu-id="4da0b-106">Property</span></span> | <span data-ttu-id="4da0b-107">类型</span><span class="sxs-lookup"><span data-stu-id="4da0b-107">Type</span></span> | <span data-ttu-id="4da0b-108">说明</span><span class="sxs-lookup"><span data-stu-id="4da0b-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4da0b-109">relayState</span><span class="sxs-lookup"><span data-stu-id="4da0b-109">relayState</span></span>|<span data-ttu-id="4da0b-110">String</span><span class="sxs-lookup"><span data-stu-id="4da0b-110">String</span></span>| <span data-ttu-id="4da0b-111">单一登录流完成后，服务提供程序将重定向到的相对 URI。</span><span class="sxs-lookup"><span data-stu-id="4da0b-111">The relative URI the service provider would redirect to after completion of the single sign-on flow.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="4da0b-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4da0b-112">JSON representation</span></span>
<span data-ttu-id="4da0b-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4da0b-113">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.samlSingleSignOnSettings"
}-->

```json
{
    "relayState": "string",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "samlSingleSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


