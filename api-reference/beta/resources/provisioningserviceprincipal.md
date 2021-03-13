---
title: provisioningServicePrincipal 资源类型
description: 表示用于设置的服务主体。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 5af9dc46de889eea780ca45eb25463ffafcf1260
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760993"
---
# <a name="provisioningserviceprincipal-resource-type"></a><span data-ttu-id="e2c56-103">provisioningServicePrincipal 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2c56-103">provisioningServicePrincipal resource type</span></span>

<span data-ttu-id="e2c56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2c56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2c56-105">表示用于设置的服务主体。</span><span class="sxs-lookup"><span data-stu-id="e2c56-105">Represents the service principal used for provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="e2c56-106">属性</span><span class="sxs-lookup"><span data-stu-id="e2c56-106">Properties</span></span>

| <span data-ttu-id="e2c56-107">属性</span><span class="sxs-lookup"><span data-stu-id="e2c56-107">Property</span></span>     | <span data-ttu-id="e2c56-108">类型</span><span class="sxs-lookup"><span data-stu-id="e2c56-108">Type</span></span>        | <span data-ttu-id="e2c56-109">说明</span><span class="sxs-lookup"><span data-stu-id="e2c56-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e2c56-110">id</span><span class="sxs-lookup"><span data-stu-id="e2c56-110">id</span></span>|<span data-ttu-id="e2c56-111">String</span><span class="sxs-lookup"><span data-stu-id="e2c56-111">String</span></span>|<span data-ttu-id="e2c56-112">唯一标识 **用于预配的 servicePrincipal。**</span><span class="sxs-lookup"><span data-stu-id="e2c56-112">Uniquely identifies the **servicePrincipal** used for provisioning.</span></span>|
|<span data-ttu-id="e2c56-113">name</span><span class="sxs-lookup"><span data-stu-id="e2c56-113">name</span></span>|<span data-ttu-id="e2c56-114">String</span><span class="sxs-lookup"><span data-stu-id="e2c56-114">String</span></span>| <span data-ttu-id="e2c56-115">**servicePrincipal 的客户定义名称**。</span><span class="sxs-lookup"><span data-stu-id="e2c56-115">Customer-defined name for the **servicePrincipal**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2c56-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2c56-116">JSON representation</span></span>

<span data-ttu-id="e2c56-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2c56-117">The following is a JSON representation of the resource.</span></span>

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


