---
title: windowsInformationProtectionProxiedDomainCollection 资源类型
description: Windows 信息保护代理域集合
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 026a69dc7697a0b779d72dfcab1695cf8c219d83
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264328"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="6bee2-103">windowsInformationProtectionProxiedDomainCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="6bee2-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="6bee2-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6bee2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bee2-105">Windows 信息保护代理域集合</span><span class="sxs-lookup"><span data-stu-id="6bee2-105">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="6bee2-106">属性</span><span class="sxs-lookup"><span data-stu-id="6bee2-106">Properties</span></span>
|<span data-ttu-id="6bee2-107">属性</span><span class="sxs-lookup"><span data-stu-id="6bee2-107">Property</span></span>|<span data-ttu-id="6bee2-108">类型</span><span class="sxs-lookup"><span data-stu-id="6bee2-108">Type</span></span>|<span data-ttu-id="6bee2-109">说明</span><span class="sxs-lookup"><span data-stu-id="6bee2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bee2-110">displayName</span><span class="sxs-lookup"><span data-stu-id="6bee2-110">displayName</span></span>|<span data-ttu-id="6bee2-111">String</span><span class="sxs-lookup"><span data-stu-id="6bee2-111">String</span></span>|<span data-ttu-id="6bee2-112">显示名称</span><span class="sxs-lookup"><span data-stu-id="6bee2-112">Display name</span></span>|
|<span data-ttu-id="6bee2-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="6bee2-113">proxiedDomains</span></span>|<span data-ttu-id="6bee2-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6bee2-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="6bee2-115">代理域集合</span><span class="sxs-lookup"><span data-stu-id="6bee2-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bee2-116">关系</span><span class="sxs-lookup"><span data-stu-id="6bee2-116">Relationships</span></span>
<span data-ttu-id="6bee2-117">无</span><span class="sxs-lookup"><span data-stu-id="6bee2-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6bee2-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6bee2-118">JSON Representation</span></span>
<span data-ttu-id="6bee2-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6bee2-119">Here is a JSON representation of the resource.</span></span>
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



