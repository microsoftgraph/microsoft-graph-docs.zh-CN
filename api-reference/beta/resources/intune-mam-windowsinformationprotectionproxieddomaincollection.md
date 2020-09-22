---
title: windowsInformationProtectionProxiedDomainCollection 资源类型
description: Windows 信息保护代理域集合
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 044a257810cc3039f2022d948632207f2bb06262
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029923"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="51905-103">windowsInformationProtectionProxiedDomainCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="51905-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="51905-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51905-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51905-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="51905-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51905-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51905-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51905-107">Windows 信息保护代理域集合</span><span class="sxs-lookup"><span data-stu-id="51905-107">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="51905-108">属性</span><span class="sxs-lookup"><span data-stu-id="51905-108">Properties</span></span>
|<span data-ttu-id="51905-109">属性</span><span class="sxs-lookup"><span data-stu-id="51905-109">Property</span></span>|<span data-ttu-id="51905-110">类型</span><span class="sxs-lookup"><span data-stu-id="51905-110">Type</span></span>|<span data-ttu-id="51905-111">说明</span><span class="sxs-lookup"><span data-stu-id="51905-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51905-112">displayName</span><span class="sxs-lookup"><span data-stu-id="51905-112">displayName</span></span>|<span data-ttu-id="51905-113">String</span><span class="sxs-lookup"><span data-stu-id="51905-113">String</span></span>|<span data-ttu-id="51905-114">显示名称</span><span class="sxs-lookup"><span data-stu-id="51905-114">Display name</span></span>|
|<span data-ttu-id="51905-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="51905-115">proxiedDomains</span></span>|<span data-ttu-id="51905-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="51905-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="51905-117">代理域集合</span><span class="sxs-lookup"><span data-stu-id="51905-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="51905-118">关系</span><span class="sxs-lookup"><span data-stu-id="51905-118">Relationships</span></span>
<span data-ttu-id="51905-119">无</span><span class="sxs-lookup"><span data-stu-id="51905-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51905-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51905-120">JSON Representation</span></span>
<span data-ttu-id="51905-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51905-121">Here is a JSON representation of the resource.</span></span>
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






