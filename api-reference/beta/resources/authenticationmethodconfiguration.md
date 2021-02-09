---
title: authenticationMethodConfigurations
description: authenticationMethodConfigurations 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cda2cda7756bb795c93e10dddbd344e5a4a92ed2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159134"
---
# <a name="authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="b1980-103">authenticationMethodConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1980-103">authenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="b1980-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1980-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1980-105">表示身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="b1980-105">Represents an authentication method policy.</span></span>

## <a name="properties"></a><span data-ttu-id="b1980-106">属性</span><span class="sxs-lookup"><span data-stu-id="b1980-106">Properties</span></span>
|<span data-ttu-id="b1980-107">属性</span><span class="sxs-lookup"><span data-stu-id="b1980-107">Property</span></span>|<span data-ttu-id="b1980-108">类型</span><span class="sxs-lookup"><span data-stu-id="b1980-108">Type</span></span>|<span data-ttu-id="b1980-109">说明</span><span class="sxs-lookup"><span data-stu-id="b1980-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1980-110">id</span><span class="sxs-lookup"><span data-stu-id="b1980-110">id</span></span>|<span data-ttu-id="b1980-111">String</span><span class="sxs-lookup"><span data-stu-id="b1980-111">String</span></span>|<span data-ttu-id="b1980-112">策略名称。</span><span class="sxs-lookup"><span data-stu-id="b1980-112">The policy name.</span></span>|
|<span data-ttu-id="b1980-113">state</span><span class="sxs-lookup"><span data-stu-id="b1980-113">state</span></span>|<span data-ttu-id="b1980-114">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="b1980-114">authenticationMethodState</span></span>|<span data-ttu-id="b1980-115">策略的状态。</span><span class="sxs-lookup"><span data-stu-id="b1980-115">The state of the policy.</span></span> <span data-ttu-id="b1980-116">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b1980-116">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1980-117">关系</span><span class="sxs-lookup"><span data-stu-id="b1980-117">Relationships</span></span>
<span data-ttu-id="b1980-118">无。</span><span class="sxs-lookup"><span data-stu-id="b1980-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1980-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1980-119">JSON representation</span></span>
<span data-ttu-id="b1980-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1980-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodConfiguration",
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
