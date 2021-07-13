---
title: tenantInfo 资源类型
description: 表示托管租户的信息。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: c81df716b74511daab1f713f73bdd872e84e4987
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402269"
---
# <a name="tenantinfo-resource-type"></a><span data-ttu-id="0010e-103">tenantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="0010e-103">tenantInfo resource type</span></span>

<span data-ttu-id="0010e-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="0010e-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0010e-105">表示托管租户的信息。</span><span class="sxs-lookup"><span data-stu-id="0010e-105">Represents information for a managed tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="0010e-106">属性</span><span class="sxs-lookup"><span data-stu-id="0010e-106">Properties</span></span>
|<span data-ttu-id="0010e-107">属性</span><span class="sxs-lookup"><span data-stu-id="0010e-107">Property</span></span>|<span data-ttu-id="0010e-108">类型</span><span class="sxs-lookup"><span data-stu-id="0010e-108">Type</span></span>|<span data-ttu-id="0010e-109">说明</span><span class="sxs-lookup"><span data-stu-id="0010e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0010e-110">tenantId</span><span class="sxs-lookup"><span data-stu-id="0010e-110">tenantId</span></span>|<span data-ttu-id="0010e-111">String</span><span class="sxs-lookup"><span data-stu-id="0010e-111">String</span></span>|<span data-ttu-id="0010e-112">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="0010e-112">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="0010e-113">可选。</span><span class="sxs-lookup"><span data-stu-id="0010e-113">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0010e-114">关系</span><span class="sxs-lookup"><span data-stu-id="0010e-114">Relationships</span></span>
<span data-ttu-id="0010e-115">无。</span><span class="sxs-lookup"><span data-stu-id="0010e-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0010e-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0010e-116">JSON representation</span></span>
<span data-ttu-id="0010e-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0010e-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantInfo",
  "tenantId": "String"
}
```
