---
title: targetResourceGroup 资源类型
description: '指示由于审核活动受影响的组的类型。 包括与 Azure AD 的统一组类似的值 '
ms.openlocfilehash: 3427f2401a0e93767f0c563842be323f66d9f21b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044754"
---
# <a name="targetresourcegroup-resource-type"></a><span data-ttu-id="4a733-104">targetResourceGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a733-104">targetResourceGroup resource type</span></span>
<span data-ttu-id="4a733-105">指示由于审核活动受影响的组的类型。</span><span class="sxs-lookup"><span data-stu-id="4a733-105">Indicates the type of group that was impacted due to the audit activity.</span></span> <span data-ttu-id="4a733-106">包括与 Azure AD 的统一组类似的值</span><span class="sxs-lookup"><span data-stu-id="4a733-106">Includes values like unified groups versus Azure AD</span></span> 



## <a name="properties"></a><span data-ttu-id="4a733-107">属性</span><span class="sxs-lookup"><span data-stu-id="4a733-107">Properties</span></span>
| <span data-ttu-id="4a733-108">属性</span><span class="sxs-lookup"><span data-stu-id="4a733-108">Property</span></span>     | <span data-ttu-id="4a733-109">类型</span><span class="sxs-lookup"><span data-stu-id="4a733-109">Type</span></span>   |<span data-ttu-id="4a733-110">说明</span><span class="sxs-lookup"><span data-stu-id="4a733-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a733-111">groupType</span><span class="sxs-lookup"><span data-stu-id="4a733-111">groupType</span></span>|<span data-ttu-id="4a733-112">字符串</span><span class="sxs-lookup"><span data-stu-id="4a733-112">String</span></span>| <span data-ttu-id="4a733-113">可取值为：`unifiedGroups`、`azureAD`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4a733-113">Possible values are: `unifiedGroups`, `azureAD`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4a733-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a733-114">JSON representation</span></span>

<span data-ttu-id="4a733-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a733-115">Here is a JSON representation of the resource.</span></span>

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