---
title: cloudPcConnection 资源类型
description: 表示给定托管租户的云电脑连接。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 75af7be7633e43bc594f7185f196f40abca39883
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402072"
---
# <a name="cloudpcconnection-resource-type"></a><span data-ttu-id="81ddd-103">cloudPcConnection 资源类型</span><span class="sxs-lookup"><span data-stu-id="81ddd-103">cloudPcConnection resource type</span></span>

<span data-ttu-id="81ddd-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="81ddd-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81ddd-105">表示给定托管租户的云电脑连接。</span><span class="sxs-lookup"><span data-stu-id="81ddd-105">Represents a cloud PC connection for a given managed tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="81ddd-106">方法</span><span class="sxs-lookup"><span data-stu-id="81ddd-106">Methods</span></span>
|<span data-ttu-id="81ddd-107">方法</span><span class="sxs-lookup"><span data-stu-id="81ddd-107">Method</span></span>|<span data-ttu-id="81ddd-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="81ddd-108">Return type</span></span>|<span data-ttu-id="81ddd-109">说明</span><span class="sxs-lookup"><span data-stu-id="81ddd-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="81ddd-110">列出 cloudPcConnections</span><span class="sxs-lookup"><span data-stu-id="81ddd-110">List cloudPcConnections</span></span>](../api/managedtenants-managedtenant-list-cloudpcconnections.md)|<span data-ttu-id="81ddd-111">[microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) 集合</span><span class="sxs-lookup"><span data-stu-id="81ddd-111">[microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) collection</span></span>|<span data-ttu-id="81ddd-112">获取 [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="81ddd-112">Get a list of the [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) objects and their properties.</span></span>|
|[<span data-ttu-id="81ddd-113">获取 cloudPcConnection</span><span class="sxs-lookup"><span data-stu-id="81ddd-113">Get cloudPcConnection</span></span>](../api/managedtenants-cloudpcconnection-get.md)|[<span data-ttu-id="81ddd-114">microsoft.graph.managedTenants.cloudPcConnection</span><span class="sxs-lookup"><span data-stu-id="81ddd-114">microsoft.graph.managedTenants.cloudPcConnection</span></span>](../resources/managedtenants-cloudpcconnection.md)|<span data-ttu-id="81ddd-115">读取 [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="81ddd-115">Read the properties and relationships of a [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="81ddd-116">属性</span><span class="sxs-lookup"><span data-stu-id="81ddd-116">Properties</span></span>
|<span data-ttu-id="81ddd-117">属性</span><span class="sxs-lookup"><span data-stu-id="81ddd-117">Property</span></span>|<span data-ttu-id="81ddd-118">类型</span><span class="sxs-lookup"><span data-stu-id="81ddd-118">Type</span></span>|<span data-ttu-id="81ddd-119">说明</span><span class="sxs-lookup"><span data-stu-id="81ddd-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81ddd-120">displayName</span><span class="sxs-lookup"><span data-stu-id="81ddd-120">displayName</span></span>|<span data-ttu-id="81ddd-121">String</span><span class="sxs-lookup"><span data-stu-id="81ddd-121">String</span></span>|<span data-ttu-id="81ddd-122">云显示名称连接数。</span><span class="sxs-lookup"><span data-stu-id="81ddd-122">The display name of the cloud PC connection.</span></span> <span data-ttu-id="81ddd-123">必填。</span><span class="sxs-lookup"><span data-stu-id="81ddd-123">Required.</span></span> <span data-ttu-id="81ddd-124">只读。</span><span class="sxs-lookup"><span data-stu-id="81ddd-124">Read-only.</span></span>|
|<span data-ttu-id="81ddd-125">healthCheckStatus</span><span class="sxs-lookup"><span data-stu-id="81ddd-125">healthCheckStatus</span></span>|<span data-ttu-id="81ddd-126">String</span><span class="sxs-lookup"><span data-stu-id="81ddd-126">String</span></span>|<span data-ttu-id="81ddd-127">云电脑连接的运行状况。</span><span class="sxs-lookup"><span data-stu-id="81ddd-127">The health status of the cloud PC connection.</span></span> <span data-ttu-id="81ddd-128">可取值为：`pending`、`running`、`passed`、`failed`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="81ddd-128">Possible values are: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`.</span></span>  <span data-ttu-id="81ddd-129">必需。</span><span class="sxs-lookup"><span data-stu-id="81ddd-129">Required.</span></span> <span data-ttu-id="81ddd-130">只读。</span><span class="sxs-lookup"><span data-stu-id="81ddd-130">Read-only.</span></span>|
|<span data-ttu-id="81ddd-131">id</span><span class="sxs-lookup"><span data-stu-id="81ddd-131">id</span></span>|<span data-ttu-id="81ddd-132">String</span><span class="sxs-lookup"><span data-stu-id="81ddd-132">String</span></span>|<span data-ttu-id="81ddd-133">云电脑连接的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="81ddd-133">The unique identifier for the cloud PC connection.</span></span> <span data-ttu-id="81ddd-134">必填。</span><span class="sxs-lookup"><span data-stu-id="81ddd-134">Required.</span></span> <span data-ttu-id="81ddd-135">只读。</span><span class="sxs-lookup"><span data-stu-id="81ddd-135">Read-only.</span></span>|
|<span data-ttu-id="81ddd-136">lastRefreshedDateTime</span><span class="sxs-lookup"><span data-stu-id="81ddd-136">lastRefreshedDateTime</span></span>|<span data-ttu-id="81ddd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81ddd-137">DateTimeOffset</span></span>|<span data-ttu-id="81ddd-138">实体上次在多租户管理平台中更新的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="81ddd-138">Date and time the entity was last updated in the multi-tenant management platform.</span></span> <span data-ttu-id="81ddd-139">必填。</span><span class="sxs-lookup"><span data-stu-id="81ddd-139">Required.</span></span> <span data-ttu-id="81ddd-140">只读。</span><span class="sxs-lookup"><span data-stu-id="81ddd-140">Read-only.</span></span>|
|<span data-ttu-id="81ddd-141">tenantDisplayName</span><span class="sxs-lookup"><span data-stu-id="81ddd-141">tenantDisplayName</span></span>|<span data-ttu-id="81ddd-142">String</span><span class="sxs-lookup"><span data-stu-id="81ddd-142">String</span></span>|<span data-ttu-id="81ddd-143">托管显示名称租户的租户。</span><span class="sxs-lookup"><span data-stu-id="81ddd-143">The display name for the managed tenant.</span></span> <span data-ttu-id="81ddd-144">必填。</span><span class="sxs-lookup"><span data-stu-id="81ddd-144">Required.</span></span> <span data-ttu-id="81ddd-145">只读。</span><span class="sxs-lookup"><span data-stu-id="81ddd-145">Read-only.</span></span>|
|<span data-ttu-id="81ddd-146">tenantId</span><span class="sxs-lookup"><span data-stu-id="81ddd-146">tenantId</span></span>|<span data-ttu-id="81ddd-147">String</span><span class="sxs-lookup"><span data-stu-id="81ddd-147">String</span></span>|<span data-ttu-id="81ddd-148">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="81ddd-148">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span> <span data-ttu-id="81ddd-149">必填。</span><span class="sxs-lookup"><span data-stu-id="81ddd-149">Required.</span></span> <span data-ttu-id="81ddd-150">只读。</span><span class="sxs-lookup"><span data-stu-id="81ddd-150">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81ddd-151">关系</span><span class="sxs-lookup"><span data-stu-id="81ddd-151">Relationships</span></span>
<span data-ttu-id="81ddd-152">无。</span><span class="sxs-lookup"><span data-stu-id="81ddd-152">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="81ddd-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81ddd-153">JSON representation</span></span>
<span data-ttu-id="81ddd-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81ddd-154">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.cloudPcConnection",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcConnection",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "healthCheckStatus": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
