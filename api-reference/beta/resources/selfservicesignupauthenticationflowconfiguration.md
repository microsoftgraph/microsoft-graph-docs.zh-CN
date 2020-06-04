---
title: selfServiceSignUpAuthenticationFlowConfiguration 资源类型
description: 表示与自助注册相关的配置。
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8c75b3a90a7e9de01234bb53ed8346c40eef932f
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556393"
---
# <a name="selfservicesignupauthenticationflowconfiguration-resource-type"></a><span data-ttu-id="b2b1b-103">selfServiceSignUpAuthenticationFlowConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2b1b-103">selfServiceSignUpAuthenticationFlowConfiguration resource type</span></span>


<span data-ttu-id="b2b1b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2b1b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2b1b-105">表示与自助注册相关的配置。</span><span class="sxs-lookup"><span data-stu-id="b2b1b-105">Represents the configurations related to self-service sign up.</span></span>

## <a name="properties"></a><span data-ttu-id="b2b1b-106">属性</span><span class="sxs-lookup"><span data-stu-id="b2b1b-106">Properties</span></span>
|<span data-ttu-id="b2b1b-107">属性</span><span class="sxs-lookup"><span data-stu-id="b2b1b-107">Property</span></span>|<span data-ttu-id="b2b1b-108">类型</span><span class="sxs-lookup"><span data-stu-id="b2b1b-108">Type</span></span>|<span data-ttu-id="b2b1b-109">说明</span><span class="sxs-lookup"><span data-stu-id="b2b1b-109">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="b2b1b-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b2b1b-110">isEnabled</span></span>|<span data-ttu-id="b2b1b-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2b1b-111">Boolean</span></span>|<span data-ttu-id="b2b1b-112">指示是否启用或禁用自助注册流。</span><span class="sxs-lookup"><span data-stu-id="b2b1b-112">Indicates whether self-service sign-up flow is enabled or disabled.</span></span> <span data-ttu-id="b2b1b-113">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="b2b1b-113">The default value is `false`.</span></span> <span data-ttu-id="b2b1b-114">此属性不是键。</span><span class="sxs-lookup"><span data-stu-id="b2b1b-114">This property is not a key.</span></span> <span data-ttu-id="b2b1b-115">必填。</span><span class="sxs-lookup"><span data-stu-id="b2b1b-115">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b2b1b-116">关系</span><span class="sxs-lookup"><span data-stu-id="b2b1b-116">Relationships</span></span>
<span data-ttu-id="b2b1b-117">无。</span><span class="sxs-lookup"><span data-stu-id="b2b1b-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2b1b-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2b1b-118">JSON representation</span></span>
<span data-ttu-id="b2b1b-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2b1b-119">The following is a JSON representation of the resource.</span></span>
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
