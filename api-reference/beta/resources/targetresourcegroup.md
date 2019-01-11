---
title: targetResourceGroup 资源类型
description: '指示由于审核活动受影响的组的类型。 包括与 Azure AD 的统一组类似的值 '
localization_priority: Normal
ms.openlocfilehash: 2cc7e0adb1a93394b64375d05dfb6a6e349bac55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851182"
---
# <a name="targetresourcegroup-resource-type"></a><span data-ttu-id="4b0cf-104">targetResourceGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b0cf-104">targetResourceGroup resource type</span></span>
<span data-ttu-id="4b0cf-105">指示由于审核活动受影响的组的类型。</span><span class="sxs-lookup"><span data-stu-id="4b0cf-105">Indicates the type of group that was impacted due to the audit activity.</span></span> <span data-ttu-id="4b0cf-106">包括与 Azure AD 的统一组类似的值</span><span class="sxs-lookup"><span data-stu-id="4b0cf-106">Includes values like unified groups versus Azure AD</span></span> 



## <a name="properties"></a><span data-ttu-id="4b0cf-107">属性</span><span class="sxs-lookup"><span data-stu-id="4b0cf-107">Properties</span></span>
| <span data-ttu-id="4b0cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="4b0cf-108">Property</span></span>     | <span data-ttu-id="4b0cf-109">类型</span><span class="sxs-lookup"><span data-stu-id="4b0cf-109">Type</span></span>   |<span data-ttu-id="4b0cf-110">Description</span><span class="sxs-lookup"><span data-stu-id="4b0cf-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b0cf-111">groupType</span><span class="sxs-lookup"><span data-stu-id="4b0cf-111">groupType</span></span>|<span data-ttu-id="4b0cf-112">字符串</span><span class="sxs-lookup"><span data-stu-id="4b0cf-112">String</span></span>| <span data-ttu-id="4b0cf-113">可取值为：`unifiedGroups`、`azureAD`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4b0cf-113">Possible values are: `unifiedGroups`, `azureAD`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b0cf-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b0cf-114">JSON representation</span></span>

<span data-ttu-id="4b0cf-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b0cf-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceGroup"
}-->

```json
{
  "groupType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
