---
title: provisioningServicePrincipal 资源类型
description: 表示用于设置的服务主体。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e163be94269ee6a75f148b460f728a36e8945645
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446574"
---
# <a name="provisioningserviceprincipal-resource-type"></a><span data-ttu-id="0df1d-103">provisioningServicePrincipal 资源类型</span><span class="sxs-lookup"><span data-stu-id="0df1d-103">provisioningServicePrincipal resource type</span></span>

<span data-ttu-id="0df1d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0df1d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0df1d-105">表示用于设置的服务主体。</span><span class="sxs-lookup"><span data-stu-id="0df1d-105">Represents the service principal used for provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="0df1d-106">属性</span><span class="sxs-lookup"><span data-stu-id="0df1d-106">Properties</span></span>

| <span data-ttu-id="0df1d-107">属性</span><span class="sxs-lookup"><span data-stu-id="0df1d-107">Property</span></span>     | <span data-ttu-id="0df1d-108">类型</span><span class="sxs-lookup"><span data-stu-id="0df1d-108">Type</span></span>        | <span data-ttu-id="0df1d-109">说明</span><span class="sxs-lookup"><span data-stu-id="0df1d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0df1d-110">id</span><span class="sxs-lookup"><span data-stu-id="0df1d-110">id</span></span>|<span data-ttu-id="0df1d-111">String</span><span class="sxs-lookup"><span data-stu-id="0df1d-111">String</span></span>|<span data-ttu-id="0df1d-112">唯一标识用于设置的**servicePrincipal** 。</span><span class="sxs-lookup"><span data-stu-id="0df1d-112">Uniquely identifies the **servicePrincipal** used for provisioning.</span></span>|
|<span data-ttu-id="0df1d-113">name</span><span class="sxs-lookup"><span data-stu-id="0df1d-113">name</span></span>|<span data-ttu-id="0df1d-114">String</span><span class="sxs-lookup"><span data-stu-id="0df1d-114">String</span></span>| <span data-ttu-id="0df1d-115">客户为**servicePrincipal**定义的名称。</span><span class="sxs-lookup"><span data-stu-id="0df1d-115">Customer-defined name for the **servicePrincipal**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0df1d-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0df1d-116">JSON representation</span></span>

<span data-ttu-id="0df1d-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0df1d-117">The following is a JSON representation of the resource.</span></span>

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
