---
title: managedTenantExecutionError 资源类型
description: 表示托管租户操作异常。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 5a1fd2d1524cad663ee6acef93ab20cc8e40fd24
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402031"
---
# <a name="managedtenantexecutionerror-resource-type"></a><span data-ttu-id="bf7ea-103">managedTenantExecutionError 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf7ea-103">managedTenantExecutionError resource type</span></span>

<span data-ttu-id="bf7ea-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="bf7ea-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf7ea-105">表示托管租户操作异常。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-105">Represents an exception for a managed tenant operation.</span></span>

<span data-ttu-id="bf7ea-106">继承自 [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md)。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-106">Inherits from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bf7ea-107">属性</span><span class="sxs-lookup"><span data-stu-id="bf7ea-107">Properties</span></span>
|<span data-ttu-id="bf7ea-108">属性</span><span class="sxs-lookup"><span data-stu-id="bf7ea-108">Property</span></span>|<span data-ttu-id="bf7ea-109">类型</span><span class="sxs-lookup"><span data-stu-id="bf7ea-109">Type</span></span>|<span data-ttu-id="bf7ea-110">说明</span><span class="sxs-lookup"><span data-stu-id="bf7ea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf7ea-111">error</span><span class="sxs-lookup"><span data-stu-id="bf7ea-111">error</span></span>|<span data-ttu-id="bf7ea-112">String</span><span class="sxs-lookup"><span data-stu-id="bf7ea-112">String</span></span>|<span data-ttu-id="bf7ea-113">异常的错误消息。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-113">The error message for the exception.</span></span> <span data-ttu-id="bf7ea-114">继承自 [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md)。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-114">Inherited from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span> <span data-ttu-id="bf7ea-115">必填。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-115">Required.</span></span> <span data-ttu-id="bf7ea-116">只读。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-116">Read-only.</span></span>|
|<span data-ttu-id="bf7ea-117">errorDetails</span><span class="sxs-lookup"><span data-stu-id="bf7ea-117">errorDetails</span></span>|<span data-ttu-id="bf7ea-118">String</span><span class="sxs-lookup"><span data-stu-id="bf7ea-118">String</span></span>|<span data-ttu-id="bf7ea-119">异常的其他错误信息。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-119">Additional error information for the exception.</span></span> <span data-ttu-id="bf7ea-120">可选。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-120">Optional.</span></span> <span data-ttu-id="bf7ea-121">只读。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-121">Read-only.</span></span>|
|<span data-ttu-id="bf7ea-122">nodeId</span><span class="sxs-lookup"><span data-stu-id="bf7ea-122">nodeId</span></span>|<span data-ttu-id="bf7ea-123">Int32</span><span class="sxs-lookup"><span data-stu-id="bf7ea-123">Int32</span></span>|<span data-ttu-id="bf7ea-124">发生异常的节点标识符。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-124">The node identifier where the exception occurred.</span></span> <span data-ttu-id="bf7ea-125">必填。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-125">Required.</span></span> <span data-ttu-id="bf7ea-126">只读。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-126">Read-only.</span></span>|
|<span data-ttu-id="bf7ea-127">rawToken</span><span class="sxs-lookup"><span data-stu-id="bf7ea-127">rawToken</span></span>|<span data-ttu-id="bf7ea-128">String</span><span class="sxs-lookup"><span data-stu-id="bf7ea-128">String</span></span>|<span data-ttu-id="bf7ea-129">异常的标记。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-129">The token for the exception.</span></span> <span data-ttu-id="bf7ea-130">可选。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-130">Optional.</span></span> <span data-ttu-id="bf7ea-131">只读。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-131">Read-only.</span></span>|
|<span data-ttu-id="bf7ea-132">statementIndex</span><span class="sxs-lookup"><span data-stu-id="bf7ea-132">statementIndex</span></span>|<span data-ttu-id="bf7ea-133">Int32</span><span class="sxs-lookup"><span data-stu-id="bf7ea-133">Int32</span></span>|<span data-ttu-id="bf7ea-134">异常的语句索引。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-134">The statement index for the exception.</span></span> <span data-ttu-id="bf7ea-135">必填。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-135">Required.</span></span> <span data-ttu-id="bf7ea-136">只读。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-136">Read-only.</span></span>|
|<span data-ttu-id="bf7ea-137">tenantId</span><span class="sxs-lookup"><span data-stu-id="bf7ea-137">tenantId</span></span>|<span data-ttu-id="bf7ea-138">String</span><span class="sxs-lookup"><span data-stu-id="bf7ea-138">String</span></span>|<span data-ttu-id="bf7ea-139">托管Azure Active Directory租户的租户标识符。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-139">The Azure Active Directory tenant identifier for the managed tenant.</span></span> <span data-ttu-id="bf7ea-140">继承自 [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md)。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-140">Inherited from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span> <span data-ttu-id="bf7ea-141">必填。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-141">Required.</span></span> <span data-ttu-id="bf7ea-142">只读。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-142">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf7ea-143">关系</span><span class="sxs-lookup"><span data-stu-id="bf7ea-143">Relationships</span></span>
<span data-ttu-id="bf7ea-144">无。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf7ea-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf7ea-145">JSON representation</span></span>
<span data-ttu-id="bf7ea-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf7ea-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantExecutionError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantExecutionError",
  "tenantId": "String",
  "error": "String",
  "rawToken": "String",
  "statementIndex": "Integer",
  "nodeId": "Integer",
  "errorDetails": "String"
}
```
