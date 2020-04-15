---
title: windowsInformationProtectionProxiedDomainCollection 资源类型
description: Windows 信息保护代理域集合
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 500f662b0a610866ac3e637850f5fd6edeffaa5b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459691"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="2702e-103">windowsInformationProtectionProxiedDomainCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="2702e-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="2702e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2702e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2702e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2702e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2702e-106">Windows 信息保护代理域集合</span><span class="sxs-lookup"><span data-stu-id="2702e-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="2702e-107">属性</span><span class="sxs-lookup"><span data-stu-id="2702e-107">Properties</span></span>
|<span data-ttu-id="2702e-108">属性</span><span class="sxs-lookup"><span data-stu-id="2702e-108">Property</span></span>|<span data-ttu-id="2702e-109">类型</span><span class="sxs-lookup"><span data-stu-id="2702e-109">Type</span></span>|<span data-ttu-id="2702e-110">说明</span><span class="sxs-lookup"><span data-stu-id="2702e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2702e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2702e-111">displayName</span></span>|<span data-ttu-id="2702e-112">String</span><span class="sxs-lookup"><span data-stu-id="2702e-112">String</span></span>|<span data-ttu-id="2702e-113">显示名称</span><span class="sxs-lookup"><span data-stu-id="2702e-113">Display name</span></span>|
|<span data-ttu-id="2702e-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="2702e-114">proxiedDomains</span></span>|<span data-ttu-id="2702e-115">[proxiedDomain](../resources/intune-mam-proxieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2702e-115">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="2702e-116">代理域集合</span><span class="sxs-lookup"><span data-stu-id="2702e-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="2702e-117">关系</span><span class="sxs-lookup"><span data-stu-id="2702e-117">Relationships</span></span>
<span data-ttu-id="2702e-118">无</span><span class="sxs-lookup"><span data-stu-id="2702e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2702e-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2702e-119">JSON Representation</span></span>
<span data-ttu-id="2702e-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2702e-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
  "displayName": "String",
  "proxiedDomains": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ]
}
```







