---
title: managedTenantOperationError 资源类型
description: 表示托管租户操作的错误的抽象类型。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d8dc51747ac63f6f8a719b0256c398d14d1c4034
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402309"
---
# <a name="managedtenantoperationerror-resource-type"></a><span data-ttu-id="adca1-103">managedTenantOperationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="adca1-103">managedTenantOperationError resource type</span></span>

<span data-ttu-id="adca1-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="adca1-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adca1-105">表示托管租户操作的错误的抽象类型。</span><span class="sxs-lookup"><span data-stu-id="adca1-105">An abstract type that represents an error for a managed tenant operation.</span></span>

## <a name="properties"></a><span data-ttu-id="adca1-106">属性</span><span class="sxs-lookup"><span data-stu-id="adca1-106">Properties</span></span>
|<span data-ttu-id="adca1-107">属性</span><span class="sxs-lookup"><span data-stu-id="adca1-107">Property</span></span>|<span data-ttu-id="adca1-108">类型</span><span class="sxs-lookup"><span data-stu-id="adca1-108">Type</span></span>|<span data-ttu-id="adca1-109">说明</span><span class="sxs-lookup"><span data-stu-id="adca1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adca1-110">error</span><span class="sxs-lookup"><span data-stu-id="adca1-110">error</span></span>|<span data-ttu-id="adca1-111">String</span><span class="sxs-lookup"><span data-stu-id="adca1-111">String</span></span>|<span data-ttu-id="adca1-112">异常的错误消息。</span><span class="sxs-lookup"><span data-stu-id="adca1-112">The error message for the exception.</span></span>|
|<span data-ttu-id="adca1-113">tenantId</span><span class="sxs-lookup"><span data-stu-id="adca1-113">tenantId</span></span>|<span data-ttu-id="adca1-114">String</span><span class="sxs-lookup"><span data-stu-id="adca1-114">String</span></span>|<span data-ttu-id="adca1-115">托管Azure Active Directory租户的租户[标识符](../resources/managedtenants-tenant.md)。</span><span class="sxs-lookup"><span data-stu-id="adca1-115">The Azure Active Directory tenant identifier for the [managed tenant](../resources/managedtenants-tenant.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="adca1-116">关系</span><span class="sxs-lookup"><span data-stu-id="adca1-116">Relationships</span></span>
<span data-ttu-id="adca1-117">无。</span><span class="sxs-lookup"><span data-stu-id="adca1-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="adca1-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="adca1-118">JSON representation</span></span>
<span data-ttu-id="adca1-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adca1-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.managedTenantOperationError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.managedTenantOperationError",
  "tenantId": "String",
  "error": "String"
}
```
