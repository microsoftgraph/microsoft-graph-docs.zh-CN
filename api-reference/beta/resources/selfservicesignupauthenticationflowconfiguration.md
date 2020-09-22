---
title: selfServiceSignUpAuthenticationFlowConfiguration 资源类型
description: 表示与自助注册相关的配置。
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 658e27e4fe75424f4bd39cc6c3a76255e70c4d92
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988805"
---
# <a name="selfservicesignupauthenticationflowconfiguration-resource-type"></a><span data-ttu-id="01271-103">selfServiceSignUpAuthenticationFlowConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="01271-103">selfServiceSignUpAuthenticationFlowConfiguration resource type</span></span>


<span data-ttu-id="01271-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01271-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="01271-105">表示与自助注册相关的配置。</span><span class="sxs-lookup"><span data-stu-id="01271-105">Represents the configurations related to self-service sign up.</span></span>

## <a name="properties"></a><span data-ttu-id="01271-106">属性</span><span class="sxs-lookup"><span data-stu-id="01271-106">Properties</span></span>
|<span data-ttu-id="01271-107">属性</span><span class="sxs-lookup"><span data-stu-id="01271-107">Property</span></span>|<span data-ttu-id="01271-108">类型</span><span class="sxs-lookup"><span data-stu-id="01271-108">Type</span></span>|<span data-ttu-id="01271-109">说明</span><span class="sxs-lookup"><span data-stu-id="01271-109">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="01271-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="01271-110">isEnabled</span></span>|<span data-ttu-id="01271-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="01271-111">Boolean</span></span>|<span data-ttu-id="01271-112">指示是启用还是禁用自助注册流。</span><span class="sxs-lookup"><span data-stu-id="01271-112">Indicates whether self-service sign-up flow is enabled or disabled.</span></span> <span data-ttu-id="01271-113">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="01271-113">The default value is `false`.</span></span> <span data-ttu-id="01271-114">此属性不是一个注册表项。</span><span class="sxs-lookup"><span data-stu-id="01271-114">This property is not a key.</span></span> <span data-ttu-id="01271-115">必填。</span><span class="sxs-lookup"><span data-stu-id="01271-115">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="01271-116">关系</span><span class="sxs-lookup"><span data-stu-id="01271-116">Relationships</span></span>
<span data-ttu-id="01271-117">无。</span><span class="sxs-lookup"><span data-stu-id="01271-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="01271-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01271-118">JSON representation</span></span>
<span data-ttu-id="01271-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01271-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.selfServiceSignUpAuthenticationFlowConfiguration"
}
-->

``` json
{
  "isEnabled": "Boolean"
}
```


