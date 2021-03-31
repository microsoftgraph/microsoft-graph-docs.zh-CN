---
title: authenticationMethodConfigurations
description: authenticationMethodConfigurations 对象。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 26d0cd948a69968a7d45b3406b3da7109ffc3f18
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469127"
---
# <a name="authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="d5306-103">authenticationMethodConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5306-103">authenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="d5306-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5306-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5306-105">表示身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="d5306-105">Represents an authentication method policy.</span></span>

## <a name="properties"></a><span data-ttu-id="d5306-106">属性</span><span class="sxs-lookup"><span data-stu-id="d5306-106">Properties</span></span>
|<span data-ttu-id="d5306-107">属性</span><span class="sxs-lookup"><span data-stu-id="d5306-107">Property</span></span>|<span data-ttu-id="d5306-108">类型</span><span class="sxs-lookup"><span data-stu-id="d5306-108">Type</span></span>|<span data-ttu-id="d5306-109">说明</span><span class="sxs-lookup"><span data-stu-id="d5306-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5306-110">id</span><span class="sxs-lookup"><span data-stu-id="d5306-110">id</span></span>|<span data-ttu-id="d5306-111">String</span><span class="sxs-lookup"><span data-stu-id="d5306-111">String</span></span>|<span data-ttu-id="d5306-112">策略名称。</span><span class="sxs-lookup"><span data-stu-id="d5306-112">The policy name.</span></span>|
|<span data-ttu-id="d5306-113">state</span><span class="sxs-lookup"><span data-stu-id="d5306-113">state</span></span>|<span data-ttu-id="d5306-114">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="d5306-114">authenticationMethodState</span></span>|<span data-ttu-id="d5306-115">策略的状态。</span><span class="sxs-lookup"><span data-stu-id="d5306-115">The state of the policy.</span></span> <span data-ttu-id="d5306-116">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="d5306-116">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5306-117">关系</span><span class="sxs-lookup"><span data-stu-id="d5306-117">Relationships</span></span>
<span data-ttu-id="d5306-118">无。</span><span class="sxs-lookup"><span data-stu-id="d5306-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5306-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5306-119">JSON representation</span></span>
<span data-ttu-id="d5306-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5306-120">The following is a JSON representation of the resource.</span></span>
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
