---
title: educationOrganization 资源类型
description: '用于模型之间的教育扇区中的不同组织类型通用性抽象实体。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 122717952781cd8effe415fb01b07ec9bf71143d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507472"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="ca4d8-103">educationOrganization 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca4d8-103">educationOrganization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca4d8-104">用于模型之间的教育扇区中的不同组织类型通用性抽象实体。</span><span class="sxs-lookup"><span data-stu-id="ca4d8-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>  

## <a name="properties"></a><span data-ttu-id="ca4d8-105">属性</span><span class="sxs-lookup"><span data-stu-id="ca4d8-105">Properties</span></span>
| <span data-ttu-id="ca4d8-106">属性</span><span class="sxs-lookup"><span data-stu-id="ca4d8-106">Property</span></span>     | <span data-ttu-id="ca4d8-107">类型</span><span class="sxs-lookup"><span data-stu-id="ca4d8-107">Type</span></span>   |<span data-ttu-id="ca4d8-108">说明</span><span class="sxs-lookup"><span data-stu-id="ca4d8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca4d8-109">说明</span><span class="sxs-lookup"><span data-stu-id="ca4d8-109">description</span></span>|<span data-ttu-id="ca4d8-110">String</span><span class="sxs-lookup"><span data-stu-id="ca4d8-110">String</span></span>| <span data-ttu-id="ca4d8-111">组织说明。</span><span class="sxs-lookup"><span data-stu-id="ca4d8-111">Organization description.</span></span>|
|<span data-ttu-id="ca4d8-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ca4d8-112">displayName</span></span>|<span data-ttu-id="ca4d8-113">String</span><span class="sxs-lookup"><span data-stu-id="ca4d8-113">String</span></span>| <span data-ttu-id="ca4d8-114">组织的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ca4d8-114">Organization display name.</span></span>|
|<span data-ttu-id="ca4d8-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="ca4d8-115">externalSource</span></span>|<span data-ttu-id="ca4d8-116">string</span><span class="sxs-lookup"><span data-stu-id="ca4d8-116">string</span></span>| <span data-ttu-id="ca4d8-117">从在其中创建此组织的源。</span><span class="sxs-lookup"><span data-stu-id="ca4d8-117">Source where this organization was created from.</span></span> <span data-ttu-id="ca4d8-118">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ca4d8-118">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca4d8-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="ca4d8-119">Relationships</span></span>
<span data-ttu-id="ca4d8-120">无。</span><span class="sxs-lookup"><span data-stu-id="ca4d8-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ca4d8-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca4d8-121">JSON representation</span></span>

<span data-ttu-id="ca4d8-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca4d8-122">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationorganization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
