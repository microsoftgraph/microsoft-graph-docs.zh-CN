---
title: provisioningServicePrincipal 资源类型
description: 表示用于设置的服务主体。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fde8f4d41c7e2788c306fe0e0591b9ddb8ba031d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521332"
---
# <a name="provisioningserviceprincipal-resource-type"></a><span data-ttu-id="37c53-103">provisioningServicePrincipal 资源类型</span><span class="sxs-lookup"><span data-stu-id="37c53-103">provisioningServicePrincipal resource type</span></span>

<span data-ttu-id="37c53-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="37c53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37c53-105">表示用于设置的服务主体。</span><span class="sxs-lookup"><span data-stu-id="37c53-105">Represents the service principal used for provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="37c53-106">属性</span><span class="sxs-lookup"><span data-stu-id="37c53-106">Properties</span></span>

| <span data-ttu-id="37c53-107">属性</span><span class="sxs-lookup"><span data-stu-id="37c53-107">Property</span></span>     | <span data-ttu-id="37c53-108">类型</span><span class="sxs-lookup"><span data-stu-id="37c53-108">Type</span></span>        | <span data-ttu-id="37c53-109">说明</span><span class="sxs-lookup"><span data-stu-id="37c53-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="37c53-110">id</span><span class="sxs-lookup"><span data-stu-id="37c53-110">id</span></span>|<span data-ttu-id="37c53-111">String</span><span class="sxs-lookup"><span data-stu-id="37c53-111">String</span></span>|<span data-ttu-id="37c53-112">唯一标识用于设置的**servicePrincipal** 。</span><span class="sxs-lookup"><span data-stu-id="37c53-112">Uniquely identifies the **servicePrincipal** used for provisioning.</span></span>|
|<span data-ttu-id="37c53-113">name</span><span class="sxs-lookup"><span data-stu-id="37c53-113">name</span></span>|<span data-ttu-id="37c53-114">String</span><span class="sxs-lookup"><span data-stu-id="37c53-114">String</span></span>| <span data-ttu-id="37c53-115">客户为**servicePrincipal**定义的名称。</span><span class="sxs-lookup"><span data-stu-id="37c53-115">Customer-defined name for the **servicePrincipal**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37c53-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37c53-116">JSON representation</span></span>

<span data-ttu-id="37c53-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37c53-117">The following is a JSON representation of the resource.</span></span>

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
