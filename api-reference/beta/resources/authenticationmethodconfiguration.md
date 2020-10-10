---
title: authenticationMethodConfigurations
description: authenticationMethodConfigurations 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 856db11063c3f766f07ff725fe172270449d272d
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418281"
---
# <a name="authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="07ab6-103">authenticationMethodConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="07ab6-103">authenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="07ab6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07ab6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07ab6-105">表示身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="07ab6-105">Represents an authentication method policy.</span></span>

## <a name="properties"></a><span data-ttu-id="07ab6-106">属性</span><span class="sxs-lookup"><span data-stu-id="07ab6-106">Properties</span></span>
|<span data-ttu-id="07ab6-107">属性</span><span class="sxs-lookup"><span data-stu-id="07ab6-107">Property</span></span>|<span data-ttu-id="07ab6-108">类型</span><span class="sxs-lookup"><span data-stu-id="07ab6-108">Type</span></span>|<span data-ttu-id="07ab6-109">说明</span><span class="sxs-lookup"><span data-stu-id="07ab6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07ab6-110">id</span><span class="sxs-lookup"><span data-stu-id="07ab6-110">id</span></span>|<span data-ttu-id="07ab6-111">字符串</span><span class="sxs-lookup"><span data-stu-id="07ab6-111">String</span></span>|<span data-ttu-id="07ab6-112">策略名称。</span><span class="sxs-lookup"><span data-stu-id="07ab6-112">The policy name.</span></span>|
|<span data-ttu-id="07ab6-113">state</span><span class="sxs-lookup"><span data-stu-id="07ab6-113">state</span></span>|<span data-ttu-id="07ab6-114">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="07ab6-114">authenticationMethodState</span></span>|<span data-ttu-id="07ab6-115">策略的状态。</span><span class="sxs-lookup"><span data-stu-id="07ab6-115">The state of the policy.</span></span> <span data-ttu-id="07ab6-116">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="07ab6-116">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07ab6-117">关系</span><span class="sxs-lookup"><span data-stu-id="07ab6-117">Relationships</span></span>
<span data-ttu-id="07ab6-118">无。</span><span class="sxs-lookup"><span data-stu-id="07ab6-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="07ab6-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07ab6-119">JSON representation</span></span>
<span data-ttu-id="07ab6-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07ab6-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodConfiguration",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String"
}
```
