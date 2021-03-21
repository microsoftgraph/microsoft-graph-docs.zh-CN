---
title: authenticationMethodConfigurations
description: authenticationMethodConfigurations 对象。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 083ace96234a724fc4c9f6e1cdda0cbd8a99e22a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964680"
---
# <a name="authenticationmethodconfiguration-resource-type"></a><span data-ttu-id="d957f-103">authenticationMethodConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d957f-103">authenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="d957f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d957f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d957f-105">表示身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="d957f-105">Represents an authentication method policy.</span></span>

## <a name="properties"></a><span data-ttu-id="d957f-106">属性</span><span class="sxs-lookup"><span data-stu-id="d957f-106">Properties</span></span>
|<span data-ttu-id="d957f-107">属性</span><span class="sxs-lookup"><span data-stu-id="d957f-107">Property</span></span>|<span data-ttu-id="d957f-108">类型</span><span class="sxs-lookup"><span data-stu-id="d957f-108">Type</span></span>|<span data-ttu-id="d957f-109">说明</span><span class="sxs-lookup"><span data-stu-id="d957f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d957f-110">id</span><span class="sxs-lookup"><span data-stu-id="d957f-110">id</span></span>|<span data-ttu-id="d957f-111">String</span><span class="sxs-lookup"><span data-stu-id="d957f-111">String</span></span>|<span data-ttu-id="d957f-112">策略名称。</span><span class="sxs-lookup"><span data-stu-id="d957f-112">The policy name.</span></span>|
|<span data-ttu-id="d957f-113">state</span><span class="sxs-lookup"><span data-stu-id="d957f-113">state</span></span>|<span data-ttu-id="d957f-114">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="d957f-114">authenticationMethodState</span></span>|<span data-ttu-id="d957f-115">策略的状态。</span><span class="sxs-lookup"><span data-stu-id="d957f-115">The state of the policy.</span></span> <span data-ttu-id="d957f-116">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="d957f-116">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d957f-117">关系</span><span class="sxs-lookup"><span data-stu-id="d957f-117">Relationships</span></span>
<span data-ttu-id="d957f-118">无。</span><span class="sxs-lookup"><span data-stu-id="d957f-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d957f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d957f-119">JSON representation</span></span>
<span data-ttu-id="d957f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d957f-120">The following is a JSON representation of the resource.</span></span>
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
