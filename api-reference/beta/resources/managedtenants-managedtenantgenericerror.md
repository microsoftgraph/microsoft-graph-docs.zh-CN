---
title: managedTenantGenericError 资源类型
description: 表示托管租户的一般错误。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d9cb6ac80bb48e7d8afc91db2cf386a21c7318e9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402025"
---
# <a name="managedtenantgenericerror-resource-type"></a><span data-ttu-id="21326-103">managedTenantGenericError 资源类型</span><span class="sxs-lookup"><span data-stu-id="21326-103">managedTenantGenericError resource type</span></span>

<span data-ttu-id="21326-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="21326-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21326-105">表示托管租户的一般错误。</span><span class="sxs-lookup"><span data-stu-id="21326-105">Represents a generic error for a managed tenant.</span></span>

<span data-ttu-id="21326-106">继承自 [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md)。</span><span class="sxs-lookup"><span data-stu-id="21326-106">Inherits from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span>

## <a name="properties"></a><span data-ttu-id="21326-107">属性</span><span class="sxs-lookup"><span data-stu-id="21326-107">Properties</span></span>
|<span data-ttu-id="21326-108">属性</span><span class="sxs-lookup"><span data-stu-id="21326-108">Property</span></span>|<span data-ttu-id="21326-109">类型</span><span class="sxs-lookup"><span data-stu-id="21326-109">Type</span></span>|<span data-ttu-id="21326-110">说明</span><span class="sxs-lookup"><span data-stu-id="21326-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21326-111">error</span><span class="sxs-lookup"><span data-stu-id="21326-111">error</span></span>|<span data-ttu-id="21326-112">String</span><span class="sxs-lookup"><span data-stu-id="21326-112">String</span></span>|<span data-ttu-id="21326-113">异常的错误消息。</span><span class="sxs-lookup"><span data-stu-id="21326-113">The error message for the exception.</span></span> <span data-ttu-id="21326-114">继承自 [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md)。</span><span class="sxs-lookup"><span data-stu-id="21326-114">Inherited from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span> <span data-ttu-id="21326-115">必填。</span><span class="sxs-lookup"><span data-stu-id="21326-115">Required.</span></span> <span data-ttu-id="21326-116">只读。</span><span class="sxs-lookup"><span data-stu-id="21326-116">Read-only.</span></span>|
|<span data-ttu-id="21326-117">tenantId</span><span class="sxs-lookup"><span data-stu-id="21326-117">tenantId</span></span>|<span data-ttu-id="21326-118">String</span><span class="sxs-lookup"><span data-stu-id="21326-118">String</span></span>|<span data-ttu-id="21326-119">托管Azure Active Directory租户的租户标识符。</span><span class="sxs-lookup"><span data-stu-id="21326-119">The Azure Active Directory tenant identifier for the managed tenant.</span></span> <span data-ttu-id="21326-120">继承自 [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md)。</span><span class="sxs-lookup"><span data-stu-id="21326-120">Inherited from [managedTenantOperationError](../resources/managedtenants-managedtenantoperationerror.md).</span></span> <span data-ttu-id="21326-121">可选。</span><span class="sxs-lookup"><span data-stu-id="21326-121">Optional.</span></span> <span data-ttu-id="21326-122">只读。</span><span class="sxs-lookup"><span data-stu-id="21326-122">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21326-123">关系</span><span class="sxs-lookup"><span data-stu-id="21326-123">Relationships</span></span>
<span data-ttu-id="21326-124">无。</span><span class="sxs-lookup"><span data-stu-id="21326-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="21326-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21326-125">JSON representation</span></span>
<span data-ttu-id="21326-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21326-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantGenericError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantGenericError",
  "tenantId": "String",
  "error": "String"
}
```
