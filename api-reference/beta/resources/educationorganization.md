---
title: educationOrganization 资源类型
description: '用于对教育部门中不同组织类型之间的通用性进行建模的抽象实体。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8652e6841c39442d8b9875ea48c785a0275073ef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501484"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="10dce-103">educationOrganization 资源类型</span><span class="sxs-lookup"><span data-stu-id="10dce-103">educationOrganization resource type</span></span>

<span data-ttu-id="10dce-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="10dce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10dce-105">用于对教育部门中不同组织类型之间的通用性进行建模的抽象实体。</span><span class="sxs-lookup"><span data-stu-id="10dce-105">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="10dce-106">属性</span><span class="sxs-lookup"><span data-stu-id="10dce-106">Properties</span></span>
| <span data-ttu-id="10dce-107">属性</span><span class="sxs-lookup"><span data-stu-id="10dce-107">Property</span></span>     | <span data-ttu-id="10dce-108">类型</span><span class="sxs-lookup"><span data-stu-id="10dce-108">Type</span></span>   |<span data-ttu-id="10dce-109">说明</span><span class="sxs-lookup"><span data-stu-id="10dce-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10dce-110">说明</span><span class="sxs-lookup"><span data-stu-id="10dce-110">description</span></span>|<span data-ttu-id="10dce-111">String</span><span class="sxs-lookup"><span data-stu-id="10dce-111">String</span></span>| <span data-ttu-id="10dce-112">组织说明。</span><span class="sxs-lookup"><span data-stu-id="10dce-112">Organization description.</span></span>|
|<span data-ttu-id="10dce-113">displayName</span><span class="sxs-lookup"><span data-stu-id="10dce-113">displayName</span></span>|<span data-ttu-id="10dce-114">String</span><span class="sxs-lookup"><span data-stu-id="10dce-114">String</span></span>| <span data-ttu-id="10dce-115">组织显示名称。</span><span class="sxs-lookup"><span data-stu-id="10dce-115">Organization display name.</span></span>|
|<span data-ttu-id="10dce-116">externalSource</span><span class="sxs-lookup"><span data-stu-id="10dce-116">externalSource</span></span>|<span data-ttu-id="10dce-117">string</span><span class="sxs-lookup"><span data-stu-id="10dce-117">string</span></span>| <span data-ttu-id="10dce-118">从中创建此组织的源。</span><span class="sxs-lookup"><span data-stu-id="10dce-118">Source where this organization was created from.</span></span> <span data-ttu-id="10dce-119">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="10dce-119">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10dce-120">关系</span><span class="sxs-lookup"><span data-stu-id="10dce-120">Relationships</span></span>
<span data-ttu-id="10dce-121">无。</span><span class="sxs-lookup"><span data-stu-id="10dce-121">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="10dce-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="10dce-122">JSON representation</span></span>

<span data-ttu-id="10dce-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10dce-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
