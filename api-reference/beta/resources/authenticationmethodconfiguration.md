---
title: authenticationMethodConfigurations
description: authenticationMethodConfigurations 对象。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 691184b1dfbf0323204debd70488d232d77b4f7a
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761133"
---
# <a name="authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="dcfbb-103">authenticationMethodConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="dcfbb-103">authenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="dcfbb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcfbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcfbb-105">表示身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="dcfbb-105">Represents an authentication method policy.</span></span>

## <a name="properties"></a><span data-ttu-id="dcfbb-106">属性</span><span class="sxs-lookup"><span data-stu-id="dcfbb-106">Properties</span></span>
|<span data-ttu-id="dcfbb-107">属性</span><span class="sxs-lookup"><span data-stu-id="dcfbb-107">Property</span></span>|<span data-ttu-id="dcfbb-108">类型</span><span class="sxs-lookup"><span data-stu-id="dcfbb-108">Type</span></span>|<span data-ttu-id="dcfbb-109">说明</span><span class="sxs-lookup"><span data-stu-id="dcfbb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcfbb-110">id</span><span class="sxs-lookup"><span data-stu-id="dcfbb-110">id</span></span>|<span data-ttu-id="dcfbb-111">String</span><span class="sxs-lookup"><span data-stu-id="dcfbb-111">String</span></span>|<span data-ttu-id="dcfbb-112">策略名称。</span><span class="sxs-lookup"><span data-stu-id="dcfbb-112">The policy name.</span></span>|
|<span data-ttu-id="dcfbb-113">state</span><span class="sxs-lookup"><span data-stu-id="dcfbb-113">state</span></span>|<span data-ttu-id="dcfbb-114">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="dcfbb-114">authenticationMethodState</span></span>|<span data-ttu-id="dcfbb-115">策略的状态。</span><span class="sxs-lookup"><span data-stu-id="dcfbb-115">The state of the policy.</span></span> <span data-ttu-id="dcfbb-116">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="dcfbb-116">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcfbb-117">关系</span><span class="sxs-lookup"><span data-stu-id="dcfbb-117">Relationships</span></span>
<span data-ttu-id="dcfbb-118">无。</span><span class="sxs-lookup"><span data-stu-id="dcfbb-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dcfbb-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dcfbb-119">JSON representation</span></span>
<span data-ttu-id="dcfbb-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dcfbb-120">The following is a JSON representation of the resource.</span></span>
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
