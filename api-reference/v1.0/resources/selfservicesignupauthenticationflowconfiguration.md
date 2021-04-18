---
title: selfServiceSignUpAuthenticationFlowConfiguration 资源类型
description: 表示与自助注册相关的配置。
author: linkhp
localization_priority: Priority
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a235c9e9869b3e0b0c36b0369ae6163083b3cf20
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882946"
---
# <a name="selfservicesignupauthenticationflowconfiguration-resource-type"></a><span data-ttu-id="7cbed-103">selfServiceSignUpAuthenticationFlowConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="7cbed-103">selfServiceSignUpAuthenticationFlowConfiguration resource type</span></span>

<span data-ttu-id="7cbed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cbed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7cbed-105">表示与自助注册相关的配置。</span><span class="sxs-lookup"><span data-stu-id="7cbed-105">Represents the configurations related to self-service sign-up.</span></span>

## <a name="properties"></a><span data-ttu-id="7cbed-106">属性</span><span class="sxs-lookup"><span data-stu-id="7cbed-106">Properties</span></span>

|<span data-ttu-id="7cbed-107">属性</span><span class="sxs-lookup"><span data-stu-id="7cbed-107">Property</span></span>|<span data-ttu-id="7cbed-108">类型</span><span class="sxs-lookup"><span data-stu-id="7cbed-108">Type</span></span>|<span data-ttu-id="7cbed-109">说明</span><span class="sxs-lookup"><span data-stu-id="7cbed-109">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="7cbed-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7cbed-110">isEnabled</span></span>|<span data-ttu-id="7cbed-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="7cbed-111">Boolean</span></span>|<span data-ttu-id="7cbed-112">指示是启用还是禁用自助注册流。</span><span class="sxs-lookup"><span data-stu-id="7cbed-112">Indicates whether self-service sign-up flow is enabled or disabled.</span></span> <span data-ttu-id="7cbed-113">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="7cbed-113">The default value is `false`.</span></span> <span data-ttu-id="7cbed-114">此属性不是一个注册表项。</span><span class="sxs-lookup"><span data-stu-id="7cbed-114">This property is not a key.</span></span> <span data-ttu-id="7cbed-115">必填。</span><span class="sxs-lookup"><span data-stu-id="7cbed-115">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7cbed-116">关系</span><span class="sxs-lookup"><span data-stu-id="7cbed-116">Relationships</span></span>

<span data-ttu-id="7cbed-117">无。</span><span class="sxs-lookup"><span data-stu-id="7cbed-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7cbed-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7cbed-118">JSON representation</span></span>

<span data-ttu-id="7cbed-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7cbed-119">The following is a JSON representation of the resource.</span></span>
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
