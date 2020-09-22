---
title: windowsInformationProtectionProxiedDomainCollection 资源类型
description: Windows 信息保护代理域集合
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8df7439bec871e8b4c7ea1a8f15829b60f2fa21f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086528"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="47e0f-103">windowsInformationProtectionProxiedDomainCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="47e0f-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="47e0f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47e0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47e0f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="47e0f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47e0f-106">Windows 信息保护代理域集合</span><span class="sxs-lookup"><span data-stu-id="47e0f-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="47e0f-107">属性</span><span class="sxs-lookup"><span data-stu-id="47e0f-107">Properties</span></span>
|<span data-ttu-id="47e0f-108">属性</span><span class="sxs-lookup"><span data-stu-id="47e0f-108">Property</span></span>|<span data-ttu-id="47e0f-109">类型</span><span class="sxs-lookup"><span data-stu-id="47e0f-109">Type</span></span>|<span data-ttu-id="47e0f-110">说明</span><span class="sxs-lookup"><span data-stu-id="47e0f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47e0f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="47e0f-111">displayName</span></span>|<span data-ttu-id="47e0f-112">String</span><span class="sxs-lookup"><span data-stu-id="47e0f-112">String</span></span>|<span data-ttu-id="47e0f-113">显示名称</span><span class="sxs-lookup"><span data-stu-id="47e0f-113">Display name</span></span>|
|<span data-ttu-id="47e0f-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="47e0f-114">proxiedDomains</span></span>|<span data-ttu-id="47e0f-115">[proxiedDomain](../resources/intune-mam-proxieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="47e0f-115">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="47e0f-116">代理域集合</span><span class="sxs-lookup"><span data-stu-id="47e0f-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="47e0f-117">关系</span><span class="sxs-lookup"><span data-stu-id="47e0f-117">Relationships</span></span>
<span data-ttu-id="47e0f-118">无</span><span class="sxs-lookup"><span data-stu-id="47e0f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47e0f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47e0f-119">JSON Representation</span></span>
<span data-ttu-id="47e0f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47e0f-120">Here is a JSON representation of the resource.</span></span>
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









