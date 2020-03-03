---
title: provisioningServicePrincipal 资源类型
description: 表示用于设置的服务主体。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 59dd514ff818ee37b462d8f21f3dce02d213eb20
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394681"
---
# <a name="provisioningserviceprincipal-resource-type"></a><span data-ttu-id="a50b2-103">provisioningServicePrincipal 资源类型</span><span class="sxs-lookup"><span data-stu-id="a50b2-103">provisioningServicePrincipal resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a50b2-104">表示用于设置的服务主体。</span><span class="sxs-lookup"><span data-stu-id="a50b2-104">Represents the service principal used for provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="a50b2-105">属性</span><span class="sxs-lookup"><span data-stu-id="a50b2-105">Properties</span></span>

| <span data-ttu-id="a50b2-106">属性</span><span class="sxs-lookup"><span data-stu-id="a50b2-106">Property</span></span>     | <span data-ttu-id="a50b2-107">类型</span><span class="sxs-lookup"><span data-stu-id="a50b2-107">Type</span></span>        | <span data-ttu-id="a50b2-108">说明</span><span class="sxs-lookup"><span data-stu-id="a50b2-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a50b2-109">id</span><span class="sxs-lookup"><span data-stu-id="a50b2-109">id</span></span>|<span data-ttu-id="a50b2-110">String</span><span class="sxs-lookup"><span data-stu-id="a50b2-110">String</span></span>|<span data-ttu-id="a50b2-111">唯一标识用于设置的**servicePrincipal** 。</span><span class="sxs-lookup"><span data-stu-id="a50b2-111">Uniquely identifies the **servicePrincipal** used for provisioning.</span></span>|
|<span data-ttu-id="a50b2-112">name</span><span class="sxs-lookup"><span data-stu-id="a50b2-112">name</span></span>|<span data-ttu-id="a50b2-113">String</span><span class="sxs-lookup"><span data-stu-id="a50b2-113">String</span></span>| <span data-ttu-id="a50b2-114">客户为**servicePrincipal**定义的名称。</span><span class="sxs-lookup"><span data-stu-id="a50b2-114">Customer-defined name for the **servicePrincipal**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a50b2-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a50b2-115">JSON representation</span></span>

<span data-ttu-id="a50b2-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a50b2-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningServicePrincipal",
  "baseType": null
}-->

```json
{
  "id": "String",
  "name": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
