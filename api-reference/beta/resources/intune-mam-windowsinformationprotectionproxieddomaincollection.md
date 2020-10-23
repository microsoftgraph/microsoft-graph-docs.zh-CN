---
title: windowsInformationProtectionProxiedDomainCollection 资源类型
description: Windows 信息保护代理域集合
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aca4ed171834992007017313961a934c47f2e5c6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691237"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="6260e-103">windowsInformationProtectionProxiedDomainCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="6260e-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="6260e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6260e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6260e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6260e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6260e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6260e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6260e-107">Windows 信息保护代理域集合</span><span class="sxs-lookup"><span data-stu-id="6260e-107">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="6260e-108">属性</span><span class="sxs-lookup"><span data-stu-id="6260e-108">Properties</span></span>
|<span data-ttu-id="6260e-109">属性</span><span class="sxs-lookup"><span data-stu-id="6260e-109">Property</span></span>|<span data-ttu-id="6260e-110">类型</span><span class="sxs-lookup"><span data-stu-id="6260e-110">Type</span></span>|<span data-ttu-id="6260e-111">说明</span><span class="sxs-lookup"><span data-stu-id="6260e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6260e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="6260e-112">displayName</span></span>|<span data-ttu-id="6260e-113">String</span><span class="sxs-lookup"><span data-stu-id="6260e-113">String</span></span>|<span data-ttu-id="6260e-114">显示名称</span><span class="sxs-lookup"><span data-stu-id="6260e-114">Display name</span></span>|
|<span data-ttu-id="6260e-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="6260e-115">proxiedDomains</span></span>|<span data-ttu-id="6260e-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6260e-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="6260e-117">代理域集合</span><span class="sxs-lookup"><span data-stu-id="6260e-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="6260e-118">关系</span><span class="sxs-lookup"><span data-stu-id="6260e-118">Relationships</span></span>
<span data-ttu-id="6260e-119">无</span><span class="sxs-lookup"><span data-stu-id="6260e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6260e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6260e-120">JSON Representation</span></span>
<span data-ttu-id="6260e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6260e-121">Here is a JSON representation of the resource.</span></span>
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





