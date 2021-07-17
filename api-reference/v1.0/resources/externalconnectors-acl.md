---
title: acl 资源类型
description: 由 externalConnection 索引的项的访问控制Microsoft 搜索项。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 171b53adc815638546bbdf71411c58d293c05de4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467278"
---
# <a name="acl-resource-type"></a><span data-ttu-id="81623-103">acl 资源类型</span><span class="sxs-lookup"><span data-stu-id="81623-103">acl resource type</span></span>

<span data-ttu-id="81623-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="81623-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="81623-105">由 externalConnection 索引的项的访问控制Microsoft 搜索项。</span><span class="sxs-lookup"><span data-stu-id="81623-105">An access control entry for an item indexed by a Microsoft Search externalConnection.</span></span>

## <a name="properties"></a><span data-ttu-id="81623-106">属性</span><span class="sxs-lookup"><span data-stu-id="81623-106">Properties</span></span>
|<span data-ttu-id="81623-107">属性</span><span class="sxs-lookup"><span data-stu-id="81623-107">Property</span></span>|<span data-ttu-id="81623-108">类型</span><span class="sxs-lookup"><span data-stu-id="81623-108">Type</span></span>|<span data-ttu-id="81623-109">说明</span><span class="sxs-lookup"><span data-stu-id="81623-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81623-110">accessType</span><span class="sxs-lookup"><span data-stu-id="81623-110">accessType</span></span>|<span data-ttu-id="81623-111">microsoft.graph.externalConnectors.accessType</span><span class="sxs-lookup"><span data-stu-id="81623-111">microsoft.graph.externalConnectors.accessType</span></span>|<span data-ttu-id="81623-112">授予标识的访问权限。</span><span class="sxs-lookup"><span data-stu-id="81623-112">The access granted to the identity.</span></span> <span data-ttu-id="81623-113">可取值为：`grant`、`deny`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="81623-113">Possible values are: `grant`, `deny`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="81623-114">type</span><span class="sxs-lookup"><span data-stu-id="81623-114">type</span></span>|<span data-ttu-id="81623-115">microsoft.graph.externalConnectors.aclType</span><span class="sxs-lookup"><span data-stu-id="81623-115">microsoft.graph.externalConnectors.aclType</span></span>|<span data-ttu-id="81623-116">标识的类型。</span><span class="sxs-lookup"><span data-stu-id="81623-116">The type of identity.</span></span> <span data-ttu-id="81623-117">可取值为：`user`、`group`、`everyone`、`everyoneExceptGuests`、`externalGroup`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="81623-117">Possible values are: `user`, `group`, `everyone`, `everyoneExceptGuests`, `externalGroup`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="81623-118">value</span><span class="sxs-lookup"><span data-stu-id="81623-118">value</span></span>|<span data-ttu-id="81623-119">String</span><span class="sxs-lookup"><span data-stu-id="81623-119">String</span></span>|<span data-ttu-id="81623-120">标识的唯一标识。</span><span class="sxs-lookup"><span data-stu-id="81623-120">The unique identifer of the identity.</span></span> <span data-ttu-id="81623-121">如果Azure Active Directory，则分别设置为类型为 user、group 和 everyone (和 everyoneExceptGuests 的用户、组或租户) `value` 标识符。</span><span class="sxs-lookup"><span data-stu-id="81623-121">In case of Azure Active Directory identities, `value` is set to the object identifier of the user, group or tenant for types user, group and everyone (and everyoneExceptGuests) respectively.</span></span> <span data-ttu-id="81623-122">如果外部组设置为 `value` externalGroup 的 ID</span><span class="sxs-lookup"><span data-stu-id="81623-122">In case of external groups `value` is set to the ID of the externalGroup</span></span> |

## <a name="relationships"></a><span data-ttu-id="81623-123">关系</span><span class="sxs-lookup"><span data-stu-id="81623-123">Relationships</span></span>
<span data-ttu-id="81623-124">无。</span><span class="sxs-lookup"><span data-stu-id="81623-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="81623-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81623-125">JSON representation</span></span>
<span data-ttu-id="81623-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81623-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.acl"
}
-->
``` json
{
  "type": "String",
  "value": "String",
  "accessType": "String"
}
```

