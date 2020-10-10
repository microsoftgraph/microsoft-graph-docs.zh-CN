---
title: fido2KeyRestrictions 资源类型
description: 表示作为 FIDO2 安全密钥身份验证方法策略的一部分强制实施的主要限制。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c606b1d7bdbf604bd5109379bffb2c1a20f60730
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418196"
---
# <a name="fido2keyrestrictions-resource-type"></a><span data-ttu-id="376e8-103">fido2KeyRestrictions 资源类型</span><span class="sxs-lookup"><span data-stu-id="376e8-103">fido2KeyRestrictions resource type</span></span>

<span data-ttu-id="376e8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="376e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="376e8-105">表示作为 [FIDO2 安全密钥身份验证方法策略](../resources/fido2authenticationmethodconfiguration.md)的一部分强制实施的主要限制。</span><span class="sxs-lookup"><span data-stu-id="376e8-105">Represents the key restrictions that are enforced as part of the [FIDO2 security keys authentication methods policy](../resources/fido2authenticationmethodconfiguration.md).</span></span>

## <a name="properties"></a><span data-ttu-id="376e8-106">属性</span><span class="sxs-lookup"><span data-stu-id="376e8-106">Properties</span></span>
|<span data-ttu-id="376e8-107">属性</span><span class="sxs-lookup"><span data-stu-id="376e8-107">Property</span></span>|<span data-ttu-id="376e8-108">类型</span><span class="sxs-lookup"><span data-stu-id="376e8-108">Type</span></span>|<span data-ttu-id="376e8-109">说明</span><span class="sxs-lookup"><span data-stu-id="376e8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="376e8-110">aaGuids</span><span class="sxs-lookup"><span data-stu-id="376e8-110">aaGuids</span></span>|<span data-ttu-id="376e8-111">字符串集合</span><span class="sxs-lookup"><span data-stu-id="376e8-111">String collection</span></span>|<span data-ttu-id="376e8-112">身份验证器证明 Guid 的集合。</span><span class="sxs-lookup"><span data-stu-id="376e8-112">A collection of Authenticator Attestation GUIDs.</span></span> <span data-ttu-id="376e8-113">AADGUIDs 定义密钥类型和制造商。</span><span class="sxs-lookup"><span data-stu-id="376e8-113">AADGUIDs define key types and manufacturers.</span></span>|
|<span data-ttu-id="376e8-114">enforcementType</span><span class="sxs-lookup"><span data-stu-id="376e8-114">enforcementType</span></span>|<span data-ttu-id="376e8-115">fido2RestrictionEnforcementType</span><span class="sxs-lookup"><span data-stu-id="376e8-115">fido2RestrictionEnforcementType</span></span>|<span data-ttu-id="376e8-116">强制类型。</span><span class="sxs-lookup"><span data-stu-id="376e8-116">Enforcement type.</span></span> <span data-ttu-id="376e8-117">可取值为：`allow`、`block`。</span><span class="sxs-lookup"><span data-stu-id="376e8-117">Possible values are: `allow`, `block`.</span></span>|
|<span data-ttu-id="376e8-118">isEnforced</span><span class="sxs-lookup"><span data-stu-id="376e8-118">isEnforced</span></span>|<span data-ttu-id="376e8-119">布尔</span><span class="sxs-lookup"><span data-stu-id="376e8-119">Boolean</span></span>|<span data-ttu-id="376e8-120">确定是否启用配置的键强制。</span><span class="sxs-lookup"><span data-stu-id="376e8-120">Determines if the configured key enforcement is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="376e8-121">关系</span><span class="sxs-lookup"><span data-stu-id="376e8-121">Relationships</span></span>
<span data-ttu-id="376e8-122">无。</span><span class="sxs-lookup"><span data-stu-id="376e8-122">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="376e8-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="376e8-123">JSON representation</span></span>
<span data-ttu-id="376e8-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="376e8-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fido2KeyRestrictions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2KeyRestrictions",
  "isEnforced": "Boolean",
  "enforcementType": "String",
  "aaGuids": [
    "String"
  ]
}
```
