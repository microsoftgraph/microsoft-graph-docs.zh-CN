---
title: samlSingleSignOnSettings 资源类型
description: 表示 SAML 单一登录设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 0b82f334196bcd9f7799a3a7a3ef7b5374571ac4
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136128"
---
# <a name="samlsinglesignonsettings-resource-type"></a><span data-ttu-id="93769-103">samlSingleSignOnSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="93769-103">samlSingleSignOnSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93769-104">表示与 SAML 单一登录相关的设置的容器。</span><span class="sxs-lookup"><span data-stu-id="93769-104">Represents a container for settings related to SAML single sign-on.</span></span>

## <a name="properties"></a><span data-ttu-id="93769-105">属性</span><span class="sxs-lookup"><span data-stu-id="93769-105">Properties</span></span>

| <span data-ttu-id="93769-106">属性</span><span class="sxs-lookup"><span data-stu-id="93769-106">Property</span></span> | <span data-ttu-id="93769-107">类型</span><span class="sxs-lookup"><span data-stu-id="93769-107">Type</span></span> | <span data-ttu-id="93769-108">说明</span><span class="sxs-lookup"><span data-stu-id="93769-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="93769-109">relayState</span><span class="sxs-lookup"><span data-stu-id="93769-109">relayState</span></span>|<span data-ttu-id="93769-110">字符串</span><span class="sxs-lookup"><span data-stu-id="93769-110">String</span></span>| <span data-ttu-id="93769-111">完成单一登录流后，服务提供商将重定向到的相对 URI。</span><span class="sxs-lookup"><span data-stu-id="93769-111">The relative URI the service provider would redirect to after completion of the single sign-on flow.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="93769-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93769-112">JSON representation</span></span>
<span data-ttu-id="93769-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93769-113">Here is a JSON representation of the resource.</span></span>

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


