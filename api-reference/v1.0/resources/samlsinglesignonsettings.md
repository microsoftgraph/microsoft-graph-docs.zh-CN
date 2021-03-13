---
title: samlSingleSignOnSettings 资源类型
description: 表示 SAML 单一登录设置。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: c923c4c5b7294abb78e7fe93f852f14304601de6
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761084"
---
# <a name="samlsinglesignonsettings-resource-type"></a><span data-ttu-id="ab555-103">samlSingleSignOnSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab555-103">samlSingleSignOnSettings resource type</span></span>

<span data-ttu-id="ab555-104">表示与 SAML 单一登录相关的设置的容器。</span><span class="sxs-lookup"><span data-stu-id="ab555-104">Represents a container for settings related to SAML single sign-on.</span></span>

## <a name="properties"></a><span data-ttu-id="ab555-105">属性</span><span class="sxs-lookup"><span data-stu-id="ab555-105">Properties</span></span>

| <span data-ttu-id="ab555-106">属性</span><span class="sxs-lookup"><span data-stu-id="ab555-106">Property</span></span> | <span data-ttu-id="ab555-107">类型</span><span class="sxs-lookup"><span data-stu-id="ab555-107">Type</span></span> | <span data-ttu-id="ab555-108">说明</span><span class="sxs-lookup"><span data-stu-id="ab555-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ab555-109">relayState</span><span class="sxs-lookup"><span data-stu-id="ab555-109">relayState</span></span>|<span data-ttu-id="ab555-110">字符串</span><span class="sxs-lookup"><span data-stu-id="ab555-110">String</span></span>| <span data-ttu-id="ab555-111">完成单一登录流后，服务提供商将重定向到的相对 URI。</span><span class="sxs-lookup"><span data-stu-id="ab555-111">The relative URI the service provider would redirect to after completion of the single sign-on flow.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="ab555-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab555-112">JSON representation</span></span>
<span data-ttu-id="ab555-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab555-113">Here is a JSON representation of the resource.</span></span>

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
