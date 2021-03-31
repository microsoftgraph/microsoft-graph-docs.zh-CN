---
title: servicePrincipalIdentity 资源类型
description: 为服务主体标识创建模型。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a49adab87ac5ebe7b8eddf106d8d38c4e15acd11
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469738"
---
# <a name="serviceprincipalidentity-resource-type"></a><span data-ttu-id="30df8-103">servicePrincipalIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="30df8-103">servicePrincipalIdentity resource type</span></span>

<span data-ttu-id="30df8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30df8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30df8-105">为服务主体标识创建模型。</span><span class="sxs-lookup"><span data-stu-id="30df8-105">Models a service principal identity.</span></span>

<span data-ttu-id="30df8-106">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="30df8-106">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="30df8-107">属性</span><span class="sxs-lookup"><span data-stu-id="30df8-107">Properties</span></span>
|<span data-ttu-id="30df8-108">属性</span><span class="sxs-lookup"><span data-stu-id="30df8-108">Property</span></span>|<span data-ttu-id="30df8-109">类型</span><span class="sxs-lookup"><span data-stu-id="30df8-109">Type</span></span>|<span data-ttu-id="30df8-110">说明</span><span class="sxs-lookup"><span data-stu-id="30df8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30df8-111">appId</span><span class="sxs-lookup"><span data-stu-id="30df8-111">appId</span></span>|<span data-ttu-id="30df8-112">String</span><span class="sxs-lookup"><span data-stu-id="30df8-112">String</span></span>| <span data-ttu-id="30df8-113">服务主体的应用程序标识符。</span><span class="sxs-lookup"><span data-stu-id="30df8-113">The application identifier of the service principal.</span></span> |
|<span data-ttu-id="30df8-114">displayName</span><span class="sxs-lookup"><span data-stu-id="30df8-114">displayName</span></span>|<span data-ttu-id="30df8-115">String</span><span class="sxs-lookup"><span data-stu-id="30df8-115">String</span></span>| <span data-ttu-id="30df8-116">服务显示名称标识的组。</span><span class="sxs-lookup"><span data-stu-id="30df8-116">The display name of the service principal identity.</span></span> <span data-ttu-id="30df8-117">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="30df8-117">Inherited from [identity](../resources/identity.md).</span></span> |
|<span data-ttu-id="30df8-118">id</span><span class="sxs-lookup"><span data-stu-id="30df8-118">id</span></span>|<span data-ttu-id="30df8-119">String</span><span class="sxs-lookup"><span data-stu-id="30df8-119">String</span></span>| <span data-ttu-id="30df8-120">服务主体标识的标识符。</span><span class="sxs-lookup"><span data-stu-id="30df8-120">The identifier of the service principal identity.</span></span> <span data-ttu-id="30df8-121">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="30df8-121">Inherited from [identity](../resources/identity.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="30df8-122">关系</span><span class="sxs-lookup"><span data-stu-id="30df8-122">Relationships</span></span>
<span data-ttu-id="30df8-123">无。</span><span class="sxs-lookup"><span data-stu-id="30df8-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="30df8-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30df8-124">JSON representation</span></span>
<span data-ttu-id="30df8-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30df8-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.servicePrincipalIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.servicePrincipalIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "appId": "String"
}
```
