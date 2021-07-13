---
title: tenantContract 资源类型
description: 表示租户和管理实体之间的关系信息。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 104b475428efe82a2e56f823845b933149aeab18
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402276"
---
# <a name="tenantcontract-resource-type"></a><span data-ttu-id="4f722-103">tenantContract 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f722-103">tenantContract resource type</span></span>

<span data-ttu-id="4f722-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="4f722-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f722-105">表示租户和管理实体之间的关系信息。</span><span class="sxs-lookup"><span data-stu-id="4f722-105">Represents relationship information between a tenant and the managing entity.</span></span>

## <a name="properties"></a><span data-ttu-id="4f722-106">属性</span><span class="sxs-lookup"><span data-stu-id="4f722-106">Properties</span></span>
|<span data-ttu-id="4f722-107">属性</span><span class="sxs-lookup"><span data-stu-id="4f722-107">Property</span></span>|<span data-ttu-id="4f722-108">类型</span><span class="sxs-lookup"><span data-stu-id="4f722-108">Type</span></span>|<span data-ttu-id="4f722-109">说明</span><span class="sxs-lookup"><span data-stu-id="4f722-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f722-110">contractType</span><span class="sxs-lookup"><span data-stu-id="4f722-110">contractType</span></span>|<span data-ttu-id="4f722-111">Int32</span><span class="sxs-lookup"><span data-stu-id="4f722-111">Int32</span></span>|<span data-ttu-id="4f722-112">管理实体和租户之间存在的关系类型。</span><span class="sxs-lookup"><span data-stu-id="4f722-112">The type of relationship that exists between the managing entity and tenant.</span></span> <span data-ttu-id="4f722-113">可选。</span><span class="sxs-lookup"><span data-stu-id="4f722-113">Optional.</span></span> <span data-ttu-id="4f722-114">只读。</span><span class="sxs-lookup"><span data-stu-id="4f722-114">Read-only.</span></span>|
|<span data-ttu-id="4f722-115">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="4f722-115">defaultDomainName</span></span>|<span data-ttu-id="4f722-116">String</span><span class="sxs-lookup"><span data-stu-id="4f722-116">String</span></span>|<span data-ttu-id="4f722-117">租户的默认域名。</span><span class="sxs-lookup"><span data-stu-id="4f722-117">The default domain name for the tenant.</span></span> <span data-ttu-id="4f722-118">必填。</span><span class="sxs-lookup"><span data-stu-id="4f722-118">Required.</span></span> <span data-ttu-id="4f722-119">只读。</span><span class="sxs-lookup"><span data-stu-id="4f722-119">Read-only.</span></span>|
|<span data-ttu-id="4f722-120">displayName</span><span class="sxs-lookup"><span data-stu-id="4f722-120">displayName</span></span>|<span data-ttu-id="4f722-121">String</span><span class="sxs-lookup"><span data-stu-id="4f722-121">String</span></span>|<span data-ttu-id="4f722-122">租户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4f722-122">The display name for the tenant.</span></span> <span data-ttu-id="4f722-123">可选。</span><span class="sxs-lookup"><span data-stu-id="4f722-123">Optional.</span></span> <span data-ttu-id="4f722-124">只读。</span><span class="sxs-lookup"><span data-stu-id="4f722-124">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f722-125">关系</span><span class="sxs-lookup"><span data-stu-id="4f722-125">Relationships</span></span>
<span data-ttu-id="4f722-126">无。</span><span class="sxs-lookup"><span data-stu-id="4f722-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f722-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f722-127">JSON representation</span></span>
<span data-ttu-id="4f722-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f722-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantContract"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantContract",
  "contractType": "Integer",
  "displayName": "String",
  "defaultDomainName": "String"
}
```
