---
title: printUserIdentity 资源类型
description: 代表通用打印服务中的用户标识。 映射到 Azure AD 用户。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: de2899b3ca75660280b797dda62993789f634096
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917608"
---
# <a name="printuseridentity-resource-type"></a><span data-ttu-id="4b116-104">printUserIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b116-104">printUserIdentity resource type</span></span>

<span data-ttu-id="4b116-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b116-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b116-106">代表通用打印服务中的用户标识。</span><span class="sxs-lookup"><span data-stu-id="4b116-106">Represents a user identity within the Universal Print service.</span></span> <span data-ttu-id="4b116-107">映射到[Azure Active Directory （AZURE AD）用户](user.md)。</span><span class="sxs-lookup"><span data-stu-id="4b116-107">Maps to an [Azure Active Directory (Azure AD) user](user.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4b116-108">属性</span><span class="sxs-lookup"><span data-stu-id="4b116-108">Properties</span></span>
| <span data-ttu-id="4b116-109">属性</span><span class="sxs-lookup"><span data-stu-id="4b116-109">Property</span></span>     | <span data-ttu-id="4b116-110">类型</span><span class="sxs-lookup"><span data-stu-id="4b116-110">Type</span></span>        | <span data-ttu-id="4b116-111">说明</span><span class="sxs-lookup"><span data-stu-id="4b116-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4b116-112">id</span><span class="sxs-lookup"><span data-stu-id="4b116-112">id</span></span>|<span data-ttu-id="4b116-113">String</span><span class="sxs-lookup"><span data-stu-id="4b116-113">String</span></span>|<span data-ttu-id="4b116-114">PrintUserIdentity 的标识符。</span><span class="sxs-lookup"><span data-stu-id="4b116-114">The printUserIdentity's identifier.</span></span> <span data-ttu-id="4b116-115">只读。</span><span class="sxs-lookup"><span data-stu-id="4b116-115">Read-only.</span></span>|
|<span data-ttu-id="4b116-116">displayName</span><span class="sxs-lookup"><span data-stu-id="4b116-116">displayName</span></span>|<span data-ttu-id="4b116-117">String</span><span class="sxs-lookup"><span data-stu-id="4b116-117">String</span></span>|<span data-ttu-id="4b116-118">PrintUserIdentity 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4b116-118">The printUserIdentity's display name.</span></span>|
|<span data-ttu-id="4b116-119">ipAddress</span><span class="sxs-lookup"><span data-stu-id="4b116-119">ipAddress</span></span>|<span data-ttu-id="4b116-120">String</span><span class="sxs-lookup"><span data-stu-id="4b116-120">String</span></span>|<span data-ttu-id="4b116-121">PrintUserIdentity 的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="4b116-121">The printUserIdentity' IP address.</span></span> <span data-ttu-id="4b116-122">未填充。</span><span class="sxs-lookup"><span data-stu-id="4b116-122">Not populated.</span></span>|
|<span data-ttu-id="4b116-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4b116-123">userPrincipalName</span></span>|<span data-ttu-id="4b116-124">字符串</span><span class="sxs-lookup"><span data-stu-id="4b116-124">String</span></span>|<span data-ttu-id="4b116-125">PrintUserIdentity 的用户主体名称（UPN）。</span><span class="sxs-lookup"><span data-stu-id="4b116-125">The printUserIdentity's user principal name (UPN).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b116-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b116-126">JSON representation</span></span>

<span data-ttu-id="4b116-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b116-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUserIdentity",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "ipAddress": "String",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUserIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
