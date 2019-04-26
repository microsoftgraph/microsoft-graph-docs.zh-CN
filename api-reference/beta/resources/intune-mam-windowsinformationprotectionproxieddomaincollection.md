---
title: windowsInformationProtectionProxiedDomainCollection 资源类型
description: Windows 信息保护代理域集合
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0cf20d0a0afb33732278b9c8f988b3008854b770
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558291"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="d6ac2-103">windowsInformationProtectionProxiedDomainCollection 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6ac2-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="d6ac2-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d6ac2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6ac2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6ac2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6ac2-106">Windows 信息保护代理域集合</span><span class="sxs-lookup"><span data-stu-id="d6ac2-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="d6ac2-107">属性</span><span class="sxs-lookup"><span data-stu-id="d6ac2-107">Properties</span></span>
|<span data-ttu-id="d6ac2-108">属性</span><span class="sxs-lookup"><span data-stu-id="d6ac2-108">Property</span></span>|<span data-ttu-id="d6ac2-109">类型</span><span class="sxs-lookup"><span data-stu-id="d6ac2-109">Type</span></span>|<span data-ttu-id="d6ac2-110">说明</span><span class="sxs-lookup"><span data-stu-id="d6ac2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6ac2-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d6ac2-111">displayName</span></span>|<span data-ttu-id="d6ac2-112">String</span><span class="sxs-lookup"><span data-stu-id="d6ac2-112">String</span></span>|<span data-ttu-id="d6ac2-113">显示名称</span><span class="sxs-lookup"><span data-stu-id="d6ac2-113">Display name</span></span>|
|<span data-ttu-id="d6ac2-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="d6ac2-114">proxiedDomains</span></span>|<span data-ttu-id="d6ac2-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d6ac2-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="d6ac2-116">代理域集合</span><span class="sxs-lookup"><span data-stu-id="d6ac2-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6ac2-117">关系</span><span class="sxs-lookup"><span data-stu-id="d6ac2-117">Relationships</span></span>
<span data-ttu-id="d6ac2-118">无</span><span class="sxs-lookup"><span data-stu-id="d6ac2-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6ac2-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6ac2-119">JSON Representation</span></span>
<span data-ttu-id="d6ac2-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6ac2-120">Here is a JSON representation of the resource.</span></span>
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





